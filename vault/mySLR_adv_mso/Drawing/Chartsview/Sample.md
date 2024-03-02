
## 1. Bar

```chartsview
#-----------------#
#- chart type    -#
#-----------------#
type: Bar

#-----------------#
#- chart data    -#
#-----------------#
data:
  - action: "Browse the website"
    pv: 50000
  - action: "Add to cart"
    pv: 35000
  - action: "Generate orders"
    pv: 25000
  - action: "Pay order"
    pv: 15000
  - action: "Seal the deal"
    pv: 8500

#-----------------#
#- chart options -#
#-----------------#
options:
  xField: "pv"
  yField: "action"
  conversionTag: {}
```


## 2. Pie

```chartsview
#-----------------#
#- chart type    -#
#-----------------#
type: Pie

#-----------------#
#- chart data    -#
#-----------------#
data:
  - type: "Wage income per capita (¥)"
    value: 17917
  - type: "Operating net income per capita (¥)"
    value: 5307
  - type: "Property Per Capita Net Income (¥)"
    value: 2791
  - type: "Transfer of net income per capita (¥)"
    value: 6173

#-----------------#
#- chart options -#
#-----------------#
options:
  angleField: "value"
  colorField: "type"
  radius: 0.5
  label:
    type: "spider"
    content: "{percentage}\n{name}"
  legend:
    layout: "horizontal"
    position: "bottom"
```

## 3. WordCloud

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

## 4. WordCount

```chartsview
#-----------------#
#- chart type    -#
#-----------------#
type: WordCloud

#-----------------#
#- chart data    -#
#-----------------#
data: "wordcount:Literature_collection/"

#-----------------#
#- chart options -#
#-----------------#
options:
  wordField: "word"
  weightField: "count"
  colorField: "count"
  wordStyle:
    rotation: 30
```

## 5. Treemap

```chartsview
#-----------------#
#- chart type    -#
#-----------------#
type: Treemap

#-----------------#
#- chart data    -#
#-----------------#
data:
  name: 'root'
  children:
    - name: 'Machine Learning'
      value: 560
    - name: 'Data Analysis'
      value: 500
    - name: 'NLP'
      value: 150
    - name: 'Computer Vision' 
      value: 140 
    - name: 'Deep Learning' 
      value: 115 
    - name: 'Reinforcement Learning' 
      value: 95 
    - name: 'Neural Networks' 
      value: 90
    - name: 'Big Data' 
      value: 75 
    - name: 'Cloud Computing' 
      value: 98 
    - name: 'Blockchain' 
      value: 60 
    - name: 'Internet of Things (IoT)' 
      value: 45 
    - name: 'Cybersecurity' 
      value: 40 
    - name: 'Quantum Computing' 
      value: 40 
    - name: 'Augmented Reality (AR)' 
      value: 35
      
    
#-----------------#
#- chart options -#
#-----------------#
options:
  colorField: "name"
```

## 6. DualAxes

```chartsview
#-----------------#
#- chart type    -#
#-----------------#
type: DualAxes

#-----------------#
#- chart data    -#
#-----------------#
data:
  -
    - time: "Mac 2024"
      value: 350
      count: 800
    - time: "April 2024"
      value: 900
      count: 600
    - time: "May 2024"
      value: 300
      count: 400
    - time: "Jun 2024"
      value: 450
      count: 380
    - time: "Jul 2024"
      value: 470
      count: 22
  -
    - time: "Mac 2024"
      value: 350
      count: 800
    - time: "April 2024"
      value: 900
      count: 600
    - time: "May 2024"
      value: 300
      count: 400
    - time: "Jun 2024"
      value: 450
      count: 380
    - time: "Jul 2024"
      value: 470
      count: 22

#-----------------#
#- chart options -#
#-----------------#
options:
  xField: 'time'
  yField: ['value', 'count']
  yAxis:
    value:
      min: 0
      label:
        formatter:
          function formatter(val) {
            return ''.concat(val, '个');
          }
  geometryOptions:
    - geometry: 'column'
    - geometry: 'line'
      lineStyle:
        lineWidth: 2
```

## 7. Mix

```chartsview
#-----------------#
#- chart type    -#
#-----------------#
type: Mix

#-----------------#
#- chart data    -#
#-----------------#
data.area:
  - time: 1246406400000
    temperature: [14.3, 27.7]
  - time: 1246492800000
    temperature: [14.5, 27.8]
  - time: 1246579200000
    temperature: [15.5, 29.6]
  - time: 1246665600000
    temperature: [16.7, 30.7]
  - time: 1246752000000
    temperature: [16.5, 25.0]
  - time: 1246838400000
    temperature: [17.8, 25.7]

data.line:
  - time: 1246406400000
    temperature: 21.5
  - time: 1246492800000
    temperature: 22.1
  - time: 1246579200000
    temperature: 23
  - time: 1246665600000
    temperature: 23.8
  - time: 1246752000000
    temperature: 21.4
  - time: 1246838400000
    temperature: 21.3

#-----------------#
#- chart options -#
#-----------------#
options:
  appendPadding: 8
  syncViewPadding: true
  tooltip:
    shared: true
    showMarkers: false
    showCrosshairs: true
    offsetY: -50

options.area:
  axes: {}
  meta:
    time:
      type: 'time'
      mask: 'MM-DD'
      nice: true
      tickInterval: 172800000
      range: [0, 1]
    temperature:
      nice: true
      sync: true
      alias: 'kadar suhu'
  geometries:
    - type: 'area'
      xField: 'time'
      yField: 'temperature'
      mapping: {}

options.line:
  axes: false
  meta:
    time:
      type: 'time'
      mask: 'MM-DD'
      nice: true
      tickInterval: 172800000
      range: [0, 1]
    temperature:
      sync: 'temperature'
      alias: 'suhu'
  geometries:
    - type: 'line'
      xField: 'time'
      yField: 'temperature'
      mapping: {}
    - type: 'point'
      xField: 'time'
      yField: 'temperature'
      mapping:
        shape: 'circle'
        style:
          fillOpacity: 1
```

## 8. Radar

```chartsview
#-----------------#
#- chart type    -#
#-----------------#
type: Radar

#-----------------#
#- chart data    -#
#-----------------#
data:
  - item: "Design"
    user: "a"
    score: 70
  - item: "Design"
    user: "b"
    score: 30
  - item: "Marketing"
    user: "a"
    score: 50
  - item: "Marketing"
    user: "b"
    score: 60
  - item: "Technology"
    user: "a"
    score: 50
  - item: "Technology"
    user: "b"
    score: 40
  - item: "Support"
    user: "a"
    score: 30
  - item: "Support"
    user: "b"
    score: 40
  - item: "Sales"
    user: "a"
    score: 60
  - item: "Sales"
    user: "b"
    score: 40

#-----------------#
#- chart options -#
#-----------------#
options:
  xField: "item"
  yField: "score"
  seriesField: "user"
  meta:
    score:
      alias: "Score"
      min: 0
      nice: true
  xAxis:
    line: null
    tickLine: null
  yAxis:
    label: false
    grid:
      alternateColor: "rgba(0, 0, 0, 0.04)"
  point: {}
  area: {}
```

## 9. OrganizationTreeGraph

```chartsview
#-----------------#
#- chart type    -#
#-----------------#
type: OrganizationTreeGraph

#-----------------#
#- chart data    -#
#-----------------#
data:
  id: "root"
  label: "My books"
  children:
    - id: "c1"
      label: "Chapter 1"
      children:
        - id: "c1-1"
          label: "C1-1"
          children:
            - id: "c1-1-1"
              label: "C1-1-1"
            - id: "c1-1-2"
              label: "C1-1-2"
        - id: "c1-2"
          label: "C1-2"
          children:
            - id: "c1-2-1"
              label: "C1-2-1"
            - id: "c1-2-2"
              label: "C1-2-2"
    - id: "c2"
      label: "Chapter 2"
      children:
        - id: "c2-1"
          label: "C2-1"
          children:
            - id: "c2-1-1"
              label: "C2-1-1"

#-----------------#
#- chart options -#
#-----------------#
options: {}
```