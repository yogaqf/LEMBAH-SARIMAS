---
ID                 : Mawar 06
LB                 : 
Living Room        : 
Bed Room           :
Bath Room          :
Kitchen            :
Terakhir_Perbaikan : 
---
# [[All Asset]] / [[Total Asset by Location]] / Mawar 06
Total_Asset:: `$= dv.pages('"ASSET"').where(p => p.Location == "Mawar 06").length`




```ad-Asset
title: Asset Type
collapse: open
```dataview 
TABLE length(rows) as Qty 
FROM "ASSET" 
WHERE contains(Location, "Mawar 06")
group by Type
```
```ad-Asset
title: Sub Location
collapse: open
```dataview 
TABLE length(rows) as Qty 
FROM "ASSET" 
WHERE contains(Location, "Mawar 06")
group by Sub_Location
```



# Sub Location
```ad-Sub_Location
title: Living Room
collapse: open
```dataview  
table Name, Type,Status, Condition, Last_Upd
from "ASSET"
WHERE contains(Location, "Mawar 06")
WHERE contains(Sub_Location, "Living Room")
sort Name asc
```
```ad-Sub_Location
title: Bath Room
collapse: open
```dataview  
table Name, Type,Status, Condition, Last_Upd
from "ASSET"
WHERE contains(Location, "Mawar 06")
WHERE contains(Sub_Location, "Bath Room")
sort Name asc
```
```ad-Sub_Location
title: Outer Room
collapse: open
```dataview  
table Name, Type,Status, Condition, Last_Upd
from "ASSET"
WHERE contains(Location, "Mawar 06")
WHERE contains(Sub_Location, "Outer Room")
sort Name asc
```
