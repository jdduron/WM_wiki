


### TARGETC Register Map
| PCLK # |                  |          |         |                |
|--------|------------------|----------|---------|----------------|
| 1      | Vofs1            | Ch. 1    |         |                |
| 2      | Vofs2            | Ch. 1    |         |                |
| 3      | Vofs1            | Ch. 2    |         |                |
| 4      | Vofs2            | Ch. 2    |         |                |
| 5      | Vofs1            | Ch. 3    |         |                |
| 6      | Vofs2            | Ch. 3    |         |                |
| 7      | Vofs1            | Ch. 4    |         |                |
| 8      | Vofs2            | Ch. 4    |         |                |
| 9      | Vofs1            | Ch. 5    |         |                |
| 10     | Vofs2            | Ch. 5    |         |                |
| 11     | Vofs1            | Ch. 6    |         |                |
| 12     | Vofs2            | Ch. 6    |         |                |
| 13     | Vofs1            | Ch. 7    |         |                |
| 14     | Vofs2            | Ch. 7    |         |                |
| 15     | Vofs1            | Ch. 8    |         |                |
| 16     | Vofs2            | Ch. 8    |         |                |
| 17     | Vofs1            | Ch. 9    |         |                |
| 18     | Vofs2            | Ch. 9    |         |                |
| 19     | Vofs1            | Ch. 10   |         |                |
| 20     | Vofs2            | Ch. 10   |         |                |
| 21     | Vofs1            | Ch. 11   |         |                |
| 22     | Vofs2            | Ch. 11   |         |                |
| 23     | Vofs1            | Ch. 12   |         |                |
| 24     | Vofs2            | Ch. 12   |         |                |
| 25     | Vofs1            | Ch. 13   |         |                |
| 26     | Vofs2            | Ch. 13   |         |                |
| 27     | Vofs1            | Ch. 14   |         |                |
| 28     | Vofs2            | Ch. 14   |         |                |
| 29     | Vofs1            | Ch. 15   |         |                |
| 30     | Vofs2            | Ch. 15   |         |                |
| 31     | Vofs1            | Ch. 16   |         |                |
| 32     | Vofs2            | Ch. 16   |         |                |
| 33     | TTBias           | Ch.1-4   |         |                |
| 34     | PMTref4          | Ch.1-4   | TTBias  |                |
| 35     | THResh           | Ch.1-4   | TTBias  |                |
| 36     | Wbias            | Ch.1-4   | TTBias  |                |
| 37     | TTBias           | Ch.5-8   |         |                |
| 38     | PMTref4          | Ch.5-8   | TTBias  |                |
| 39     | THResh           | Ch.5-8   | TTBias  |                |
| 40     | Wbias            | Ch.5-8   | TTBias  |                |
| 41     | TTBias           | Ch.9-12  |         |                |
| 42     | PMTref4          | Ch.9-12  | TTBias  |                |
| 43     | THResh           | Ch.9-12  | TTBias  |                |
| 44     | Wbias            | Ch.9-12  | TTBias  |                |
| 45     | TTBias           | Ch.13-16 |         |                |
| 46     | PMTref4          | Ch.13-16 | TTBias  |                |
| 47     | THResh           | Ch.13-16 | TTBias  |                |
| 48     | Wbias            | Ch.13-16 | TTBias  |                |
| 49     | Sbbias           | Vramp    | Dbbias  |                |
| 50     | Vdisch           | Vramp    | Dbbias  |                |
| 51     | Isel             | Vramp    | Dbbias  |                |
| 52     | Dbbias           | Vramp    |         |                |
| 53     | Qbias            | PLL      | Vqbuff  |                |
| 54     | Vqbuff           | PLL      |         |                |
| 55     | VtrimT           | PLL      | Vqbuff  |                |
| 56     | Misc Digital Reg |          | 12 bit  |                |
| 57     | VadjP            | Timebase | VAPbuff |                |
| 58     | VAPbuff          | Timebase |         |                |
| 59     | VadjN            | Timebase | VANbuff |                |
| 60     | VANbuff          | Timebase |         |                |
| 61     | TRGsumbias       | Trigger  | Itbias  |                |
| 62     | Vbias            | Trigger  | Itbias  |                |
| 63     | TRGGbias         | Trigger  | Itbias  |                |
| 64     | Itbias           | Trigger  | Itbias  |                |
| 65     | SSPin LE         | Timebase |         | 8 bit time     |
| 66     | SSPin TE         | Timebase |         | 8 bit time     |
| 67     | WR_ADDR_Incr1 LE | Timebase |         | 8 bit time     |
| 68     | WR_ADDR_Incr1 TE | Timebase |         | 8 bit time     |
| 69     | WR_STRB1 LE      | Timebase |         | 8 bit time     |
| 70     | WR_STRB1 TE      | Timebase |         | 8 bit time     |
| 71     | WR_ADDR_Incr2 LE | Timebase |         | 8 bit time     |
| 72     | WR_ADDR_Incr2 TE | Timebase |         | 8 bit time     |
| 73     | WR_STRB2 LE      | Timebase |         | 8 bit time     |
| 74     | WR_STRB2 TE      | Timebase |         | 8 bit time     |
| 75     | MonTiming SEL    | Timebase |         | 8 bit time     |
| 76     | SSToutFB         | Timebase |         | 8 bit time     |
| 77     | CMPbias2         | Wilk     | Sbbias  |                |
| 78     | Pubias           | Wilk     | Sbbias  |                |
| 79     | CMPbias          | Wilk     | Sbbias  |                |
| 80     | TPGreg           |          |         | 12 bit pattern |