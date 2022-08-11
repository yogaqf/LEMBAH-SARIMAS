---
ID : Melati
LB : 1200 Mtr
Terakhir_Perbaikan : 12/12/2021
---


Melati



---
## <mark style="background: #FF5582A6;">Asset Group</mark> 
```dataview 
TABLE length(rows) as Qty FROM "ASSET" group by Type
```
---
## <mark style="background: #CACFD9A6;">Balcony</mark> 
```dataview  
table Name, Type,Bungalow, Tag as Kondisi, Last_Upd
from "ASSET/TV"
WHERE contains(Ruangan, "Balcony")
```
