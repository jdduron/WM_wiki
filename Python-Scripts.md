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
