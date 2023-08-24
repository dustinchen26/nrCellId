# nrCellId_Calculator
online calculate: https://dustinchen26.github.io/nrCellId

## Description & example
```
【Description】
nrCellId has a total size of 36 bits. These 36 bits are constitute of gNBId and cellId. 
Please input gNBIdLength, gNBId, cellId, then it will calculate the nrCellId.

gNBIdLength: 22
gNBId : 5
cellId : 1

Convert and Calculate
nrCellId (Binary): 000000000000000000010100000000000001
nrCellId (Hexadecimal): 0x14001

CU xml Output:
                    <gNBId>5</gNBId>
                    <gNBIdLength>22</gNBIdLength>
                    <cellLocalId>1</cellLocalId>
DU xml Output:
                    <gNBId>5</gNBId>
                    <gNBIdLength>22</gNBIdLength>
                    <nrCellId>14001</nrCellId>
                    <pdcchDmrsScramblingID>1</pdcchDmrsScramblingID>
                    <pdschDataScramblingID>1</pdschDataScramblingID>
                    <puschDataScramblingID>1</puschDataScramblingID>
                    <cellId>1</cellId>
                    <scramblingID0Dl>1</scramblingID0Dl>
                    <scramblingID1Dl>1</scramblingID1Dl>
                    <scramblingID0>1</scramblingID0>
                    <scramblingID1>1</scramblingID1>
                    <cellId>1</cellId>
                    <nCI>14001</nCI>
                    <nRPCI>1</nRPCI>
```