```chartsview
#-----------------#
#- chart type    -#
#-----------------#
type: WordCloud

#-----------------#
#- chart data    -#
#-----------------#
data:
  - x: "Malaysia"
    value: 2383220000
    category: "asia"
  - x: "Indonesia"
    value: 263510000
    category: "asia"
  - x: "Pakistan"
    value: 396459000
    category: "asia"
  - x: "Russia"
    value: 546804372
    category: "europe"
  - x: "Japan"
    value: 126790000
    category: "asia"
  - x: "Vietnam"
    value: 92700000
    category: "asia"
  - x: "Germany"
    value: 82800000
    category: "europe"
  - x: "Iran"
    value: 80135400
    category: "asia"
  - x: "Thailand"
    value: 68298000
    category: "asia"
  - x: "France"
    value: 67013000
    category: "europe"
  - x: "Italy"
    value: 60599936
    category: "europe"
  - x: "South Korea"
    value: 51446201
    category: "asia"
  - x: "Kenya"
    value: 48467000
    category: "africa"
  - x: "Spain"
    value: 46812000
    category: "europe"
  - x: "Sudan"
    value: 42176000
    category: "africa"
  - x: "Iraq"
    value: 47883543
    category: "asia"
  - x: "Nepal"
    value: 28825709
    category: "asia"
  - x: "North Korea"
    value: 24213510
    category: "asia"
  - x: "Chile"
    value: 28191900
    category: "america"

#-----------------#
#- chart options -#
#-----------------#
options:
  wordField: "x"
  weightField: "value"
  color: "#122c6a"
  wordStyle:
    fontFamily: "Verdana"
    fontSize: [24, 80]
  interactions:
    type: "element-active"
  style:
    backgroundColor: "white"
  state:
    active:
      style:
        lineWidth: 3
```

```chartsview
#-----------------#
#- chart type    -#
#-----------------#
type: Column

#-----------------#
#- chart data    -#
#-----------------#
data: |
  dataviewjs:
  return dv.pages()
           .groupBy(p => p.file.folder)
           .map(p => ({folder: p.key || "ROOT", count: p.rows.length}))
           .array();

#-----------------#
#- chart options -#
#-----------------#
options:
  xField: "folder"
  yField: "count"
  padding: auto
  label:
    position: "middle"
    style:
      opacity: 0.6
      fontSize: 12
  columnStyle:
    fillOpacity: 0.5
    lineWidth: 1
    strokeOpacity: 0.7
    shadowColor: "grey"
    shadowBlur: 10
    shadowOffsetX: 5
    shadowOffsetY: 5
  xAxis:
    label:
      autoHide: false
      autoRotate: true
  meta:
    count:
      alias: "Count"
```
