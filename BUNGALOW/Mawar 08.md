---
ID                 : Mawar 08
LB                 : 
Living Room        : 
Bed Room           :
Bath Room          :
Kitchen            :
Terakhir_Perbaikan : 
---
# [[All Asset]] / [[Total Asset by Location]] / Mawar 08
Total_Asset:: `$= dv.pages('"ASSET"').where(p => p.Location == "Mawar 08").length`



# Type
```dataview 
TABLE length(rows) as Qty 
FROM "ASSET" 
WHERE contains(Location, "Mawar 08")
group by Type
```
```dataview 
TABLE length(rows) as Qty 
FROM "ASSET" 
WHERE contains(Location, "Mawar 08")
group by Sub_Location
```

# Sub Location

```dataview  
table Name, Type,Status, Condition, Last_Upd
from "ASSET"
WHERE contains(Location, "Mawar 08")
WHERE contains(Sub_Location, "Living Room")
sort Name asc
```


```dataview  
table Name, Type,Status, Condition, Last_Upd
from "ASSET"
WHERE contains(Location, "Mawar 08")
WHERE contains(Sub_Location, "Bath Room")
sort Name asc
```
