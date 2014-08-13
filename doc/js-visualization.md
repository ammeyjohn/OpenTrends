Visualization
=============

d3.js
-----

> [http://d3js.org/](http://d3js.org/)

	LICENSE: BSD
	BROWSER: IE6+, Firefox2+, Safari3+, Opera9.5+
	TAG: SVG

![logo](../images/logo_d3js.png)
**D3.js** is a JavaScript library for manipulating documents based on data. D3 helps you bring data to life using HTML, SVG and CSS. D3’s emphasis on web standards gives you the full capabilities of modern browsers without tying yourself to a proprietary framework, combining powerful visualization components and a data-driven approach to DOM manipulation.

#### Introduction

**D3** allows you to bind arbitrary data to a Document Object Model (DOM), and then apply data-driven transformations to the document. For example, you can use D3 to generate an HTML table from an array of numbers. Or, use the same data to create an interactive SVG bar chart with smooth transitions and interaction.

D3 is not a monolithic framework that seeks to provide every conceivable feature. Instead, D3 solves the crux of the problem: efficient manipulation of documents based on data. This avoids proprietary representation and affords extraordinary flexibility, exposing the full capabilities of web standards such as CSS3, HTML5 and SVG. With minimal overhead, D3 is extremely fast, supporting large datasets and dynamic behaviors for interaction and animation. D3’s functional style allows code reuse through a diverse collection of components and plugins.

#### Demos:
![demo](../images/demo_d3js.png)

InfoVis Toolkit
---------------
> [http://philogb.github.io/jit/index.html](http://philogb.github.io/jit/index.html)
	
	LICENSE: MIT
	BROWSER: IE6+, Firefox2+, Safari3+, Opera9.5+
	TAG: Canvas

The JavaScript **InfoVis Toolkit** provides tools for creating Interactive Data Visualizations for the Web.

#### Demos:
![demo](../images/demo_jit_1.png)
![demo](../images/demo_jit_2.png)
![demo](../images/demo_jit_3.png)
![demo](../images/demo_jit_4.png)
![demo](../images/demo_jit_5.png)
![demo](../images/demo_jit_6.png)
![demo](../images/demo_jit_7.png)
![demo](../images/demo_jit_8.png)
![demo](../images/demo_jit_9.png)
![demo](../images/demo_jit_10.png)
![demo](../images/demo_jit_11.png)

Processing.js
-------------
> [http://processingjs.org/](http://processingjs.org/)
	
	LICENSE: GPL v2
	BROWSER: Safari, Firefox, Chrome, Opera, IE
	TAG: Canvas

![logo](../images/logo_processing_js.png)
**Processing.js** is the sister project of the popular Processing visual programming language, designed for the web. Processing.js makes your data visualizations, digital art, interactive animations, educational graphs, video games, etc. work using web standards and without any plug-ins. You write code using the Processing language, include it in your web page, and Processing.js does the rest. It's not magic, but almost.

Protovis
--------
> [http://mbostock.github.io/protovis/](http://mbostock.github.io/protovis/)
		
	LICENSE: BSD
	BROWSER: Firefox 3, Chrome and Safari 4
	TAG: SVG

**Protovis** composes custom views of data with simple marks such as bars and dots. Unlike low-level graphics libraries that quickly become tedious for visualization, Protovis defines marks through dynamic properties that encode data, allowing inheritance, scales and layouts to simplify construction.

Protovis is free and open-source, provided under the BSD License. It uses JavaScript and SVG for web-native visualizations; no plugin required (though you will need a modern web browser)! Although programming experience is helpful, Protovis is mostly declarative and designed to be learned [by example](http://mbostock.github.io/protovis/ex/ "by example").

#### Getting Started
How does Protovis work? Consider this bar chart, which visually encodes an array of numbers with height:
```javascript
var vis = new pv.Panel()
    .width(150)
    .height(150);

vis.add(pv.Bar)
    .data([1, 1.2, 1.7, 1.5, .7, .3])
    .width(20)
    .height(function(d) d * 80)
    .bottom(0)
    .left(function() this.index * 25);

vis.render();
```
![logo](../images/demo_protovis_1.png)

This blue bar is rendered once per number, mapping the data to height using a little function (d * 80). Thus, a mark represents a set of graphical elements that share data and visual encodings. Although marks are simple by themselves, you can combine them in interesting ways to make rich, interactive visualizations.

To simplify construction, Protovis supports panels and inheritance. A panel is a container for replicating marks. Inheritance lets you derive new marks from existing ones, sharing some or all of the properties. For example, here we derive labels for a rule and bar:
```javascript
var vis = new pv.Panel()
    .width(150)
    .height(150);

vis.add(pv.Rule)
    .data(pv.range(0, 2, .5))
    .bottom(function(d) d * 80 + .5)
  .add(pv.Label);

vis.add(pv.Bar)
    .data([1, 1.2, 1.7, 1.5, .7])
    .width(20)
    .height(function(d) d * 80)
    .bottom(0)
    .left(function() this.index * 25 + 25)
  .anchor("bottom").add(pv.Label);

vis.render();
```
![logo](../images/demo_protovis_2.png)

The rule’s label inherits the data and bottom property, causing it to appear on the rule and render the value (datum) as text. The bar’s label uses the bottom anchor to tweak positioning, so that the label is centered at the bottom of the bar.

Raphaël
-------
> [http://raphaeljs.com/](http://raphaeljs.com/)
		
	LICENSE: MIT
	BROWSER: Firefox 3.0+, Safari 3.0+, Chrome 5.0+, Opera 9.5+ and Internet Explorer 6.0+
	TAG: SVG, VML

![logo](../images/logo_raphael.png)
**Raphaël** is a small JavaScript library that should simplify your work with vector graphics on the web. If you want to create your own specific chart or image crop and rotate widget, for example, you can achieve it simply and easily with this library.

Raphaël ['ræfeɪəl] uses the SVG W3C Recommendation and VML as a base for creating graphics. This means every graphical object you create is also a DOM object, so you can attach JavaScript event handlers or modify them later. Raphaël’s goal is to provide an adapter that will make drawing vector art compatible cross-browser and easy.

#### Examples:
```javascript
// Creates canvas 320 × 200 at 10, 50
var paper = Raphael(10, 50, 320, 200);

// Creates circle at x = 50, y = 40, with radius 10
var circle = paper.circle(50, 40, 10);
// Sets the fill attribute of the circle to red (#f00)
circle.attr("fill", "#f00");

// Sets the stroke attribute of the circle to white
circle.attr("stroke", "#fff");
```
#### Demos:
![demo](../images/demo_raphael.jpg)

vis.js
------

> [http://visjs.org/](http://visjs.org/)

	LICENSE: Apache v2.0

![logo](../images/logo_visjs.png)
**Vis.js** is a dynamic, browser based visualization library. The library is designed to be easy to use, to handle large amounts of dynamic data, and to enable manipulation of and interaction with the data. The library consists of the components DataSet, Timeline, Network, Graph2d, and Graph3d.
The vis.js library is developed by Almende B.V, as part of CHAP. Vis.js runs fine on Chrome, Firefox, Opera, Safari, IE9+, and most mobile browsers (with full touch support).

#### Examples

```javascript
// DOM element where the Timeline will be attached
var container = document.getElementById('mytimeline');

// Create a DataSet with data (enables two way data binding)
var data = new vis.DataSet([
  {id: 1, content: 'item 1', start: '2013-04-20'},
  {id: 2, content: 'item 2', start: '2013-04-14'},
  {id: 3, content: 'item 3', start: '2013-04-18'},
  {id: 4, content: 'item 4', start: '2013-04-16', end: '2013-04-19'},
  {id: 5, content: 'item 5', start: '2013-04-25'},
  {id: 6, content: 'item 6', start: '2013-04-27'}
]);

// Configuration for the Timeline
var options = {};

// Create a Timeline
var timeline = new vis.Timeline(container, data, options);
```