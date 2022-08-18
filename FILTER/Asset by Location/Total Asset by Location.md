# [[All Asset]] / Total Asset by Location
```ad-Dataview
collapse: open
```dataview 
Table ID as Bungalow, Total_Asset
from "BUNGALOW"
sort ID asc

```

```ad-Chart
collapse: open
```dataviewjs
const data = dv.pages('"ASSET"');

const TotalAsalia11 = data.where(p => p.Location == "Asalia 11").length;
const TotalMawar01 = data.where(p => p.Location == "Mawar 01").length;
const TotalMawar02 = data.where(p => p.Location == "Mawar 02").length;
const TotalMawar03 = data.where(p => p.Location == "Mawar 03").length;
const TotalMawar04 = data.where(p => p.Location == "Mawar 04").length;
const TotalMawar05 = data.where(p => p.Location == "Mawar 05").length;
const TotalMawar06 = data.where(p => p.Location == "Mawar 06").length;
const TotalMelati = data.where(p => p.Location == "Melati").length;

const DataArray = [TotalAsalia11, TotalMawar01, TotalMawar02, TotalMawar03, TotalMawar04, TotalMawar05, TotalMawar06, TotalMelati];

const chartData = {
    type: 'bar',
    data: {
        labels: ['Asalia 11', 'Mawar 01', 'Mawar 02', 'Mawar 03', 'Mawar 04', 'Mawar 05', 'Mawar 06', 'Melati'],
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

