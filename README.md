# nrCellId_Calculator
online calculate: https://dustinchen26.github.io/nrCellId

## Description & example
```
【Spec】
ref: ETSI TS 128 541 / 29 571 / 38 413 / 38 300
  (1) NR Cell Global Identifier (NCGI): used to identify NR cells globally. The NCGI is constructed from the PLMN identity the cell belongs to and the NR Cell Identity(NCI) of the cell.
  (2) NR Cell Identity (NrCellId): BIT STRING (SIZE(36))
  (3) gNB ID (gNBId): BIT STRING (SIZE(22..32))
  (4) cellLocalId (cellId): The NCI can be constructed by encoding the gNB Identifier using gNBId and cellLocalId

【Tool Description】
nrCellId(36 bits) = gNBId + cellId. 
Please enter (gNBIdLength, gNBId, cellId), then it will calculate the nrCellId. 
Fill in nrCellId(Hexadecimal) to du xml (nrCellId, nCI)

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
