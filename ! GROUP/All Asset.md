# All Asset
---
```ad-Sort
collapse: open

[[Total Asset by Status]]
[[Total Asset by Condition]]
[[Total Asset by Location]]
[[Total Asset by Category]]
[[Total Asset by Type]]

```

## <mark style="background: #FF5582A6;">Asset List</mark> 
```dataview  
table ID as No, Name, Category , Location, file.mtime as Last_Upd
from "ASSET"
sort file.mtime desc
```
