# [[All Asset]] / Total Asset by Type
Total_Asset:: $= dv.pages("ASSET").length
```ad-Dataview
collapse: open
```dataview 
TABLE length(rows) as Total_Asset
FROM "ASSET" 
Group by Type
```

```ad-Chart
collapse: open
```dataviewjs
const data = dv.pages('"ASSET"');

const TotalAsalia11 = data.where(p => p.Location == "Asalia 11").length;
const TotalMelati = data.where(p => p.Location == "Melati").length;
const TotalMawar01 = data.where(p => p.Location == "Mawar 01").length;


const DataArray = [TotalAsalia11, TotalMelati, TotalMawar01];

const chartData = {
    type: 'bar',
    data: {
        labels: ['Asalia 11', 'Melati', 'Mawar 01'],
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
- [[Dispenser]]

