# [[All Asset]] / Total Asset by Type
```ad-Dataview
collapse: open
```dataview 
TABLE length(rows) as Total_Asset
FROM "ASSET" 
Group by Type
```


## Table
| Bungalow          | Qty |
| ----------------- | --- |
| Cermin            | 1   |
| Dispenser         | 3   |
| Dispenser Keramik | 15  |
| Jam Dinding       | 5   |
| Kayu Risbang      | 9   |
| Kulkas            | 1   |
| Kursi Set         | 45  | 
| Lampu Dinding     | 6   |
| Lemari Pakaian    | 7   |
| Lukisan           | 8   |
| Meja Tempel       | 8   |
| Meja TV           | 4   |
| Nakas             | 5   |
| Pewangi Ruangan   | 5   |
| Rak Handuk        | 5   |
| Receiver          | 5   |
| Remote Rcv        | 5   |
| Telepon           | 5   |
| Tempat Gelas      | 5   |
| Tempat Sampah     | 5   |
| TV                | 5   |
| Wastafel          | 5   |
| Wifi Router       | 7   |
^table

## Chart
```chart  
type: line  
id: table  
layout: column  
width: 80%  
beginAtZero: true  
labelColors: true
```

## List
- [[Dispenser]]

