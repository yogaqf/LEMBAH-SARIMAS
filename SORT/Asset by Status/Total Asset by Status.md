# [[All Asset]] / Total Asset by Status

```ad-Dataview
collapse: open
```dataview 
TABLE length(rows) as Total_Asset
FROM "ASSET" 
Group by Status
```




## Table
| Status  | Qty |
| ------- | --- |
| IN USE  | 29  |
| New     | 3   |
| Useless | 6.7 |
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
- IN USE

