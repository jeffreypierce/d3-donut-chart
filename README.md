## D3 Donut Chart
A simple, configurable, animatable chart build with [d3.js](https://github.com/mbostock/d3/)

#### Usage

```
var donutChart = new DonutChart(selector, [settings])  
donutChart.update(dataSet) 
```

Where `selector` is a id or class of a DOM node, `settings` (optional) is an object of configuration options (see below) and `dataSet` is data values formatted as an array of arrays like this:

```
[['JavaScript', 30], ['C++', 10], ['Ruby', 15], ['Python', 20]]
```
A live example can be viewed [here](http://jeffreypierce.net/d3-donut-chart/)

#### Configuration Options

+ width (Number): The width of the chart, *450*

+ height (Number): The height of the chart, *300*

+ radius (Number): The radius of the chart, *100*

+ innerRadius (Number): How much whitespace is cut away from the middle of the chart, *70*

+ strokeColor(Color Hex): The color of the dividers between the slices,  *"#FFF"*

+ strokeWidth (Number): Width of the slice dividers, *5*

+ enableLabels (Boolean): Whether or not to show the labels, *true*

+ labelGroupOffset (Number): Offset in pixels of the labels, *20*

+ labelColor(Color Hex): Color of the labels, *"#333"*

+ labelValueText (Function): Returns the text string to show as the value label, the current slice is passed in as argument, *percentage value*

+ labelValueOffset (Number): Value label offset in pixels from the label group, *16*

+ labelNameText: (Function): Returns the text string to show as the name label, the current slice is passed in as argument, *slice name (slice value)*

+ labelNameOffset (Number): Name label offset in pixels from the label group, *0*

+ tickColor (Color Hex): Color of the tick, *"#333"*

+ tickWidth (Number): Width of the tick, *1*

+ tickOffset (Array): Offset values in pixels of the tick in the format of [x1, x2, y1, y2], *[0,0,2,8]*

+ easeFunction (String): Type of transition ease from [here](https://github.com/mbostock/d3/wiki/Transitions#wiki-d3_ease), *'cubic'*

+ animationDuration (Number): Speed, in millis, of the animation, *250*

+ colors (Array): List of color hexs for the slices, *d3.scale.category20()*

- - -

I based this chart on a tutorial I took a few years back and now forget where it was from. So thanks to the original author of that blog post, whoever you are…

- - -

The MIT License (MIT)

Copyright (c) 2014 Jeffrey Pierce

Permission is hereby granted, free of charge, to any person obtaining a copy
of this software and associated documentation files (the "Software"), to deal
in the Software without restriction, including without limitation the rights
to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
copies of the Software, and to permit persons to whom the Software is
furnished to do so, subject to the following conditions:

The above copyright notice and this permission notice shall be included in all
copies or substantial portions of the Software.

THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND, EXPRESS OR
IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY,
FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE
AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE
SOFTWARE.
