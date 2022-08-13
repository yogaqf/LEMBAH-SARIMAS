# [[All Asset]] / Total Asset by Category
```ad-Dataview
collapse: open
```dataview 
TABLE length(rows) as Total_Asset
FROM "ASSET" 
Group by Category
```


## Table
| Bungalow        | Qty |
| --------------- | --- |
| Chinaware       | 1   |
| Decoration      | 3   | 
| Electronic      | 15  |
| Furniture       | 5   |
| Other Equipment | 9   |
| Sanitaryware    | 1   |
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
- [[Electronic]]
- 