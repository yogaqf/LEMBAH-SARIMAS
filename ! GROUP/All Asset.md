# All Asset
---
## ==Total Asset by Location==
```dataview 
TABLE length(rows) as Total_Asset
FROM "ASSET" 
group by Location
```

## ==Total Asset by Group==
```dataview 
TABLE length(rows) as Total_Asset
FROM "ASSET" 
group by Group
```

## ==Total Asset by Type==
```dataview 
TABLE length(rows) as Total_Asset
FROM "ASSET" 
group by Type
```


---

## <mark style="background: #FF5582A6;">Asset List</mark> 
```dataview  
table ID as No, Name, Type, Group , Location
from "ASSET"
sort ID asc
```
