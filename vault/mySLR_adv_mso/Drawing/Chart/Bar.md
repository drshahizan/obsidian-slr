
```chart
type: bar
labels: [IEEE, WOS, Scopus, ACM, TEST, TEST, Sunday, "Next Week", "Next Month"]
series:
  - title: Articles Read
    data: [12, 4, 7, 5, 8, 10, 9, 15, 20]
  - title: Articles Written
    data: [1, 0, 3, 2, 1, 0, 1, 2, 3]
```

## DataviewJS

[DataviewJS](https://blacksmithgu.github.io/obsidian-dataview/queries/dql-js-inline/) is a JavaScript API provided by Dataview. It allows you to query your vault using JavaScript, which gives you a _ton_ of power and flexibility. If you know JavaScript, then this should be pretty easy to pick up.

```dataviewjs
const labels = ['Machine Learning', 'Data Analysis', 'Natural Language Processing'];
const data = [12, 4, 7];

const chartData = {  
    type: 'bar',
    data: {
        labels: labels,
        datasets: [{
            label: 'Articles Read',
            data: data
        }]
    }
}
window.renderChart(chartData, this.container);
```
