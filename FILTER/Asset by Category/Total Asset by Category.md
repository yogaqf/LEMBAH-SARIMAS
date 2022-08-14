# [[All Asset]] / Total Asset by Category
Total_Asset:: `$= dv.pages('"ASSET"').length`
```ad-Dataview
collapse: open
```dataview 
TABLE length(rows) as Total_Asset
FROM "ASSET" 
Group by Category
```

```ad-Chart
collapse: open
```dataviewjs
const data = dv.pages('"ASSET"');

const TotalChinaware = data.where(p => p.Category == "Chinaware").length;
const TotalDecoration = data.where(p => p.Category == "Decoration").length;
const TotalElectronic = data.where(p => p.Category == "Electronic").length;
const TotalFurniture = data.where(p => p.Category == "Furniture").length;
const TotalGlassware = data.where(p => p.Category == "Glassware").length;
const TotalOtherEquipment = data.where(p => p.Category == "Other Equipment").length;
const TotalSanitaryware = data.where(p => p.Category == "Sanitaryware").length;

const DataArray = [TotalChinaware, TotalDecoration, TotalElectronic, TotalFurniture, TotalGlassware, TotalOtherEquipment, TotalSanitaryware];

const chartData = {
    type: 'bar',
    data: {
        labels: ['Chinaware', 'Decoration', 'Electronic','Furniture', 'Glassware', 'Other Equipment', 'Sanitaryware'],
        datasets: [{
            label: 'Total',
            data: DataArray,
            backgroundColor: [
                'rgba(255, 99, 132, 0.2)'
            ],
            borderColor: [
                'rgba(255, 99, 132, 1)'
            ],
            borderWidth: 1
        }]
    }
}

window.renderChart(chartData, this.container);
```


## List
- [[Electronic]]

