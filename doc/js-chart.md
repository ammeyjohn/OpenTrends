Chart
=====

dygraphs
--------
> [http://dygraphs.com](http://dygraphs.com/)
	
	LICENSE: MIT

**dygraphs** is a fast, flexible open source JavaScript charting library.It allows users to explore and interpret dense data sets. 

#### Features
- Handles huge data sets: dygraphs plots millions of points without getting bogged down.
- Interactive out of the box: zoom, pan and mouseover are on by default.
- Strong support for error bars / confidence intervals.
- Highly customizable: using options and custom callbacks, you can make dygraphs do almost anything.
- dygraphs is highly compatible: it works in all major browsers (including IE8). You can even pinch to zoom on mobile/tablet devices!
- There's an active community developing and supporting dygraphs.

#### Examples:

```javascript
new Dygraph(div, "ny-vs-sf.txt", {
  legend: 'always',
  title: 'NYC vs. SF',
  showRoller: true,
  rollPeriod: 14,
  customBars: true,
  ylabel: 'Temperature (F)',
});
```
![demo](../images/demo_dygraphs.png)

ECharts
-------

> [http://echarts.baidu.com](http://echarts.baidu.com/)
	
	LICENSE: 
	BROWSER: IE6/7/8/9+，chrome、firefox、safari、opera 

![logo](../images/logo_echarts.png)
基于Canvas，纯Javascript图表库，提供直观，生动，可交互，可个性化定制的数据可视化图表。创新的拖拽重计算、数据视图、值域漫游等特性大大增强了用户体验，赋予了用户对数据进行挖掘、整合的能力。

Highcharts
----------

> [http://www.highcharts.com/](http://www.highcharts.com/)

	LICENSE: FREE FOR NON-COMMERCIAL

**Highcharts** is a JavaScript charting library with a huge range of chart options available. The output is rendered using SVG in modern browsers and VML in Internet Explorer. The charts are beautifully animated into view automatically, and the framework also supports live data streams. It's free to download and use non-commercially (and licensable for commercial use). You can also play with the extensive demos using JSFiddle.

tangle
------

> [http://worrydream.com/Tangle/](http://worrydream.com/Tangle/)

	LICENSE: 

Tangle is a JavaScript library for creating reactive documents. Your readers can interactively explore possibilities, play with parameters, and see the document update immediately. Tangle is super-simple and easy to learn.