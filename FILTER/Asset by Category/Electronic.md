# [[All Asset]] / [[Total Asset by Category]] / Electronic
Total_Asset:: #PR

```dataview  
table ID as No, Name, Type, Group , Location
from "ASSET"
WHERE contains(Category, "Electronic")
sort ID asc
```
