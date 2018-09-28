Return to [WATCHMAN Wiki home](https://github.com/WMidlab/WATCHMAN/wiki)

### Data Packet Format

The packet structure consists of a string of char. The first 4 char make up the header “head”. Every data packet ends the last 4 char “end”. The word after “head” states how many words are in the packet after #words (Length of packet -2). The body of the packet depends on what commands or data are being sent. A delimiter “/” is being used to separate each word, command, number, in the string. The maximum length depends on the length of the UDP packet and the IPv4 protocol, 65,507 bytes.

Example: `head/4/body1/body2/body3/end`


|    Word      |    Bits 31:0       |  Notes/Description                                | 
|--------------|--------------------|---------------------------------------------------|
|    0         |    0x68656164      |    header word ->   "head" in ASCII               |  
|    1         |    packet size     |    number of words   following this one (N-2)     |
|    2:N-1     |    body            |    (specific identifiers   enumerated below)      |
|    N-2       |   "end"            |    end                                            |


### Commands

There are 4 commands implemented right now, ping, read register, write register and read all registers.

# Ping
PC sends string “ping” that requests a “pong” from the zynq. 

Example:

> C:\Users\Public\Documents\WATCHMAN\Python_Scripts>send.py                                      
> UDP target IP: 192.168.1.10                                                               
> UDP target port: 7                                     
> Enter a command: ping              
> Enter a command: send                                      
> head/2/ping/end/                    
> received "head/3/pong/end"

# Read Register
PC must send “read/register_address” to ZYNQ. ZYNQ will echo back “read/register_address/register_value”.

Example:
> C:\Users\Public\Documents\WATCHMAN\Python_Scripts>send.py      
> UDP target IP: 192.168.1.10     
> UDP target port: 7    
> Enter a command: read  
> Enter reg address: 6  
> Enter a command: send  
> head/3/read/6/end/  
> received "head/5/read/6/16/end"   

# Write Register
PC must send “rite/register_address/register_value” to ZYNQ. ZYNQ will echo back “rite/register_address/register_value”.

Example:
> C:\Users\Public\Documents\WATCHMAN\Python_Scripts>send.py
> UDP target IP: 192.168.1.10
> UDP target port: 7
> Enter a command: rite
> Enter reg address: 2
> Enter reg value:10
> Enter a command: send
> head/4/rite/2/10/end/
> received "head/5/rite/2/10/end"

# Read all Registers
PC must send “rall” to ZYNQ. ZYNQ will echo back “rall/register_address/register_value/register_address/register_value/register_address/register_value”.
The length of the return packet depends on the number of registers instantiated. (Right now there are 10).

Example:
> C:\Users\Public\Documents\WATCHMAN\Python_Scripts>send.py   
> UDP target IP: 192.168.1.10    
> UDP target port: 7   
> Enter a command: rall   
> Enter a command: send   
> head/2/rall/end/      
> received "head/13/rall/10/11/10/13/14/15/16/17/18/19/end"

Send multiple commands in a single packet:

Example:
> C:\Users\Public\Documents\WATCHMAN\Python_Scripts>send.py    
> UDP target IP: 192.168.1.10   
> UDP target port: 7    
> Enter a command: ping   
> Enter a command: read   
> Enter reg address: 2  
> Enter a command: read   
> Enter reg address: 3    
> Enter a command: rite   
> Enter reg address: 2   
> Enter reg value:1111   
> Enter a command: rite   
> Enter reg address: 3  
> Enter reg value:2222    
> Enter a command: rall    
> Enter a command: ping    
> Enter a command: ping    
> Enter a command: send    
> head/22/ping/read/2/read/3/rite/2/1111/rite/3/2222/rall/ping/ping/end/    
> received "head/27/pong/read/2/10/read/3/13/rite/2/1111/rite/3/2222/rall/10/11/1111/2222/14/15/16/17/18/19/pong/end"
 
# DATA format
ZYNQ creates a packet by converting int values to char strings with “head” and delimiter “/”. The second word was set to be “test” to show what is the source of the data. The last word is “end”.In this case it is a random test pattern for a 4 channel, 16 samples. This is sent to UDP port 8

Example:
> C:\Users\Public\Documents\WATCHMAN\Python_Scripts>plot_data.py   
> UDP target IP: 192.168.1.10    
> UDP target port: 8   
> received "head/test/1028/540/1364/3094/674/4000/2671/1780/1596/3353/893/2774/2987/3230/21/3455/2837/3145/1240/2448/2415/1281/3256/3312/330/36/701/1327/2084/710/2356/2777/1931/3880/3627/3684/108/360/2476/752/2981/2227/1673/1779/75/670/1071/2070/3705/1952/1222/100/2069/3885/113/1740/19/2923/723/1502/1934/2523/3213/291/end"

