 # owf-lib-viz-canvasjs
Open Water Foundation visualization library based on CanvasJS

## Getting Started

A standard development folder structure is recommended. The website development files can be set up as follows (Windows is assumed, but Linux would be similar):

```
> C:
> cd \Users\user
> mkdir Canvas-JS
> cd Canvas-JS
> mkdir git-repos
> cd git-repos
> git clone https://github.com/OpenWaterFoundation/owf-lib-viz-canvasjs-js
``` 
The repository contains multiple folders that include time series examples using different sets of data.
## Additional Documentation

See also:
* [CanvasJS Documentation](http://canvasjs.com/docs/charts/basics-of-creating-html5-chart/)
* [CanvasJS How To Examples](http://canvasjs.com/docs/charts/how-to/creating-dynamic-charts)
* [CanvasJS Options Reference](http://canvasjs.com/docs/charts/chart-options/)

## Data Format RCC-ACIS Precipitation Time Series
|Date   |StationID 1   |StationID 2   |StationID 3   |StationID X   |
|:-:|---|---|---|---|
|1/01/2000   |0.0   |1.0   |0.0   |precipitation amount   |
|1/02/2000   |0.5   |1.73   |0.2   |precipitation amount   |
|1/03/2000   |0.26   |0.84   |0.64   |precipitation amount   |

** **Note** the data below each station is the amount of precipitation that occured that day. 

## NOTES

* Requires a decent understanding of javascript and JQuery
* Requires small amount of code to implement 
* When graphing multiple series, there must be multiple specifications in the data option. For example, when graphing 3 series the code would look as follows:
```
data: [
{
    type: "line",
    dataPoints: getDataPointsFromCSV(data,1),
    legendText: '53005',
    showInLegend: true,
},
{
    type: "line",
    dataPoints: getDataPointsFromCSV(data,2),
    legendText: '58839',
    showInLegend: true,
},
{
    type: "line",
    dataPoints: getDataPointsFromCSV(data,3),
    legendText: '052759',
    showInLegend: true,
}
]
```
* Provides examples and documentation
* Open Source
* Free
* Has a good release history
* Actively developed

## What is a Timeseries Graph

Timeseries, also known as Line Graphs, are used to display quantitative value over a continuous interval or time span. It is most frequently used to show trends and relationships (when grouped with other lines). Line Graphs also help to give a "big picture" over an interval, to see how it has developed over that period.

Line Graphs are drawn by first plotting data points on a Cartesian coordinate grid, then connecting a line between these points. Typically, the y-axis has a quantitative value, while the x-axis has either a category or sequenced scale. Negative values can be displayed below the x-axis.

For more information refer to the links below:

* [Timeseries Graph](http://www.datavizcatalogue.com/methods/line_graph.html)
* [Timeseries Documenation](https://developers.google.com/chart/interactive/docs/gallery/linechart)