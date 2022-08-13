# [[All Asset]] / Total Asset by Location
```ad-Dataview
collapse: open
```dataview 
TABLE length(rows) as Total_Asset
FROM "ASSET" 
Group by Location
```




## Table
| Bungalow  | Qty |
| --------- | --- |
| Asalia 11 | 16  |
| Mawar 01  | 6   |
| Melati    | 7   |
^table

## Chart
```chart  
type: bar  
id: table  
layout: rows  
width: 80%  
beginAtZero: true  
```

## List
- [[Melati]]
- 