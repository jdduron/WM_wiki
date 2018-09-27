Return to [TARGETC ASIC page](https://github.com/WMidlab/WATCHMAN/wiki/TARGETC-ASIC-Documentation)

### TARGETX Register map					
					
| Register # | Name             | Description                  | recommended value (DEC) | Reg Address (HEX) | recommended value (HEX) |
|------------|------------------|------------------------------|-------------------------|-------------------|-------------------------|
| 0          | Trig Ch1         | set DAC for trigger hreshold | 1450                    | 00000000          | 000005AA                |
| 1          | Wbias Ch1        | width of comparator pulse    | 985                     | 00000002          | 000003D9                |
| 2          | Trig Ch2         | set DAC for trigger hreshold | 1450                    | 00000004          | 000005AA                |
| 3          | Wbias Ch2        | width of comparator pulse    | 985                     | 00000006          | 000003D9                |
| 4          | Trig Ch3         | set DAC for trigger hreshold | 1450                    | 00000008          | 000005AA                |
| 5          | Wbias Ch3        | width of comparator pulse    | 985                     | 0000000A          | 000003D9                |
| 6          | Trig Ch4         | set DAC for trigger hreshold | 1450                    | 0000000C          | 000005AA                |
| 7          | Wbias Ch4        | width of comparator pulse    | 985                     | 0000000E          | 000003D9                |
| 8          | Trig Ch5         | set DAC for trigger hreshold | 1450                    | 00000010          | 000005AA                |
| 9          | Wbias Ch5        | width of comparator pulse    | 985                     | 00000012          | 000003D9                |
| 10         | Trig Ch6         | set DAC for trigger hreshold | 1450                    | 00000014          | 000005AA                |
| 11         | Wbias Ch6        | width of comparator pulse    | 985                     | 00000016          | 000003D9                |
| 12         | Trig Ch7         | set DAC for trigger hreshold | 1450                    | 00000018          | 000005AA                |
| 13         | Wbias Ch7        | width of comparator pulse    | 985                     | 0000001A          | 000003D9                |
| 14         | Trig Ch8         | set DAC for trigger hreshold | 1450                    | 0000001C          | 000005AA                |
| 15         | Wbias Ch8        | width of comparator pulse    | 985                     | 0000001E          | 000003D9                |
| 16         | Trig Ch9         | set DAC for trigger hreshold | 1450                    | 00000020          | 000005AA                |
| 17         | Wbias Ch9        | width of comparator pulse    | 985                     | 00000022          | 000003D9                |
| 18         | Trig Ch10        | set DAC for trigger hreshold | 1450                    | 00000024          | 000005AA                |
| 19         | Wbias Ch10       | width of comparator pulse    | 985                     | 00000026          | 000003D9                |
| 20         | Trig Ch11        | set DAC for trigger hreshold | 1450                    | 00000028          | 000005AA                |
| 21         | Wbias Ch11       | width of comparator pulse    | 985                     | 0000002A          | 000003D9                |
| 22         | Trig Ch12        | set DAC for trigger hreshold | 1450                    | 0000002C          | 000005AA                |
| 23         | Wbias Ch12       | width of comparator pulse    | 985                     | 0000002E          | 000003D9                |
| 24         | Trig Ch13        | set DAC for trigger hreshold | 1450                    | 00000030          | 000005AA                |
| 25         | Wbias Ch13       | width of comparator pulse    | 985                     | 00000032          | 000003D9                |
| 26         | Trig Ch14        | set DAC for trigger hreshold | 1450                    | 00000034          | 000005AA                |
| 27         | Wbias Ch14       | width of comparator pulse    | 985                     | 00000036          | 000003D9                |
| 28         | Trig Ch15        | set DAC for trigger hreshold | 1450                    | 00000038          | 000005AA                |
| 29         | Wbias Ch15       | width of comparator pulse    | 985                     | 0000003A          | 000003D9                |
| 30         | Trig Ch16        | set DAC for trigger hreshold | 1450                    | 0000003C          | 000005AA                |
| 31         | Wbias Ch16       | width of comparator pulse    | 985                     | 0000003E          | 000003D9                |
| 32         | unused           | -                            |                         | 00000040          | 00000000                |
| 33         | unused           | -                            |                         | 00000042          | 00000000                |
| 34         | unused           | -                            |                         | 00000044          | 00000000                |
| 35         | unused           | -                            |                         | 00000046          | 00000000                |
| 36         | unused           | -                            |                         | 00000048          | 00000000                |
| 37         | unused           | -                            |                         | 0000004A          | 00000000                |
| 38         | unused           | -                            |                         | 0000004C          | 00000000                |
| 39         | unused           | -                            |                         | 0000004E          | 00000000                |
| 40         | unused           | -                            |                         | 00000050          | 00000000                |
| 41         | unused           | -                            |                         | 00000052          | 00000000                |
| 42         | unused           | -                            |                         | 00000054          | 00000000                |
| 43         | unused           | -                            |                         | 00000056          | 00000000                |
| 44         | unused           | -                            |                         | 00000058          | 00000000                |
| 45         | unused           | -                            |                         | 0000005A          | 00000000                |
| 46         | unused           | -                            |                         | 0000005C          | 00000000                |
| 47         | unused           | -                            |                         | 0000005E          | 00000000                |
| 48         | Sbbias           | Vramp                        | 1300                    | 00000060          | 00000514                |
| 49         | Vdisch           | Vramp                        | 0                       | 00000062          | 00000000                |
| 50         | Isel             | Vramp                        | 2650                    | 00000064          | 00000A5A                |
| 51         | Dbbias           | Vramp                        | 1100                    | 00000066          | 0000044C                |
| 52         | Qbias            | PLL                          | 1244                    | 00000068          | 000004DC                |
| 53         | Vqbuff           | PLL                          | 1062                    | 0000006A          | 00000426                |
| 54         | VtrimT           | PLL                          | 1209                    | 0000006C          | 000004B9                |
| 55         | Misc Digital Reg |                              | 0                       | 0000006E          | 00000000                |
| 56         | VadjP            | Timebase                     | 1152                    | 00000070          | 00000480                |
| 57         | VAPbuff          | Timebase                     | 0                       | 00000072          | 00000000                |
| 58         | VadjN            | Timebase                     | 2235                    | 00000074          | 000008BB                |
| 59         | VANbuff          | Timebase                     | 0                       | 00000076          | 00000000                |
| 60         | unused           |                              | 1130                    | 00000078          | 0000046A                |
| 61         | Vbias            | Trigger                      | 1100                    | 0000007A          | 0000044C                |
| 62         | TRGGbias         | Trigger                      | 1100                    | 0000007C          | 0000044C                |
| 63         | Itbias           | Trigger                      | 1100                    | 0000007E          | 0000044C                |
| 64         | SSPin LE         | Timebase                     | 143                     | 00000080          | 0000008F                |
| 65         | SSPin TE         | Timebase                     | 163                     | 00000082          | 000000A3                |
| 66         | WR_ADDR_Inc1 LE  | Timebase                     | 5                       | 00000084          | 00000005                |
| 67         | WR_ADDR_Inc1 TE  | Timebase                     | 25                      | 00000086          | 00000019                |
| 68         | WR_STRB1 LE      | Timebase                     | 20                      | 00000088          | 00000014                |
| 69         | WR_STRB1 TE      | Timebase                     | 40                      | 0000008A          | 00000028                |
| 70         | WR_ADDR_Inc2 LE  | Timebase                     | 33                      | 0000008C          | 00000021                |
| 71         | WR_ADDR_Inc2 TE  | Timebase                     | 53                      | 0000008E          | 00000035                |
| 72         | WR_STRB2 LE      | Timebase                     | 56                      | 00000090          | 00000038                |
| 73         | WR_STRB2 TE      | Timebase                     | 12                      | 00000092          | 0000000C                |
| 74         | MonTiming SEL    | Timebase                     | 40                      | 00000094          | 00000028                |
| 75         | SSToutFB         | Timebase                     | 58                      | 00000096          | 0000003A                |
| 76         | CMPbias2         | Wilk                         | 737                     | 00000098          | 000002E1                |
| 77         | Pubias           | Wilk                         | 3112                    | 0000009A          | 00000C28                |
| 78         | CMPbias2         | Wilk                         | 1152                    | 0000009C          | 00000480                |
| 79         | TPGreg           | Test pattern generator       | 2730                    | 0000009E          | 00000AAA                |

