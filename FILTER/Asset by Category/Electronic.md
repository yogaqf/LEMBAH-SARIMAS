# [[All Asset]] / [[Total Asset by Category]] / Electronic
Total_Asset:: `$= dv.pages('"ASSET"').where(p => p.Category == "Electronic").length`
```dataview  
table ID as No, Name, Type, Status, Condition, Location
from "ASSET"
WHERE contains(Category, "Electronic")
sort Category asc
```
