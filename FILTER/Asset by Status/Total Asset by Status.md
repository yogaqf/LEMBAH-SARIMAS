# [[All Asset]] / Total Asset by Status
Total_Asset:: `$= dv.pages('"ASSET"').length`
```ad-Dataview
collapse: open
```dataview 
TABLE length(rows) as Total_Asset
FROM "ASSET" 
Group by Status
```

```ad-Chart
collapse: open
```dataviewjs
const data = dv.pages('"ASSET"');

const TotalINUSE = data.where(p => p.Status == "IN USE").length;

const DataArray = [TotalINUSE];

const chartData = {
    type: 'bar',
    data: {
        labels: ['IN USE'],
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
- IN USE
