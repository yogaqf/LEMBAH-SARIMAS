# [[All Asset]] / [[Total Asset by Type]] / Dispenser
Total_Asset:: `$= dv.pages('"ASSET"').where(p => p.Type == "Dispenser").length`
```dataview  
table ID as No, Name, Type, Status, Condition, Location
from "ASSET"
WHERE contains(Type, "Dispenser")
sort ID asc
```
