# nrCellId_Calculator
online calculate: https://dustinchen26.github.io/nrCellId

## Description & example
```
【Description】
nrCellId has a total size of 36 bits. These 36 bits are constitute of gNBId and cellId. 
Please input gNBIdLength, gNBId, cellId, then it will calculate the nrCellId.

【example】
gNBIdLength: 22
gNBId : 5
cellId : 1
Convert and Calculate

nrCellId (Binary): 000000000000000000010100000000000001
nrCellId (Hexadecimal)●: 0x14001

CU xml Output:
  <GNBCUFunction>
      <gNBId>5</gNBId>
      <gNBIdLength>22</gNBIdLength>

      <NRCellCU>
        <cellLocalId>1</cellLocalId>
		
DU xml Output:
      <gNBId>5</gNBId>
      <gNBIdLength>22</gNBIdLength>

                 <nRCGI>
                    <nrCellId>14001</nrCellId>
                 </nRCGI>

                    <cellAccessInfo>
                       <pLMNIdentityList>
                          <cellId>1</cellId>
                       </pLMNIdentityList>
                    </cellAccessInfo>

        <nCI>14001</nCI>	  
```