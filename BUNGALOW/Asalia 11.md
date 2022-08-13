---
ID                 : Asalia 11
LB                 : 
Living Room        : 
Bed Room           :
Bath Room          :
Kitchen            :
Terakhir_Perbaikan : 
---
# [[All Asset]] / [[Total Asset by Location]] / Asalia 11

## History Perbaikan
- None









---
## <mark style="background: #FF5582A6;">Asset Type</mark> 
```dataview 
TABLE length(rows) as Qty 
FROM "ASSET" 
WHERE contains(Location, "Asalia 11")
group by Type
```

## <mark style="background: #FF5582A6;">Sub Location</mark> 
```dataview 
TABLE length(rows) as Qty 
FROM "ASSET" 
WHERE contains(Location, "Asalia 11")
group by Sub_Location
```
---




# Sub Location

## <mark style="background: #CACFD9A6;">Balcony</mark> 

## <mark style="background: #ADCCFFA6;">Living Room</mark> 
```dataview  
table Name, Type,Status, Tag as Condition, Last_Upd
from "ASSET"
WHERE contains(Location, "Asalia 11")
WHERE contains(Sub_Location, "Living Room")
```
## <mark style="background: #FFB86CA6;">Bed Room 1</mark> 

## <mark style="background: #FFB86CA6;">Bed Room 2</mark> 

## <mark style="background: #D2B3FFA6;">Bath Room 1</mark> 

## <mark style="background: #D2B3FFA6;">Bath Room 2</mark> 
