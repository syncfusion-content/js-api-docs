---
layout: post
title: API reference for ejChart
description: What are the options, methods and events available in Essential JavaScript Chart.
documentation: API
platform: js-api
keywords: ejChart, API, Essential JS Chart, Chart
metaname: 
metacontent: 
---

# ejChart
<ts root="datavisualization" />

Essential chart can be easily configured to the DOM element, such as div. You can create a Chart with highly customizable look and feel.


#### Syntax

{% highlight js %}

$(element).ejChart();

{% endhighlight %}


#### Example


{% highlight html %}
 
<div id="container"></div> 
 
<script>
// Create Chart
$('#container').ejChart();      
</script>

{% endhighlight %}




#### Requires

* module:jQuery.js

* module:ej.core.js

* module:ej.data.js

* module:ej.chart.js

* module:jQuery.globalize.js


## Members




### annotations `array`
{:#members:annotations}




Options for adding and customizing annotations in Chart.



N> Annotations are not supported in 3D chart types.


### annotations.angle `number`
{:#members:annotations-angle}




Angle to rotate the annotation in degrees.


#### Default Value

* '0'




#### Example


{% highlight js %}
 
$("#container").ejChart({

   annotations :[{ angle : 45}]                    

});


{% endhighlight %}


Try it: [Annotation angle](http://jsplayground.syncfusion.com/rgl4uwkj)




### annotations.content `string`
{:#members:annotations-content}




Text content or id of a HTML element to be displayed as annotation.


#### Default Value

* ""




#### Example


{% highlight js %}
 
$("#container").ejChart({

   annotations :[{ content :"Template"}]
                       
});


{% endhighlight %}


Try it: [Annotation Content](http://jsplayground.syncfusion.com/plihjtm3)




### annotations.coordinateUnit `enum`
{:#members:annotations-coordinateunit}

<ts name="ej.datavisualization.Chart.CoordinateUnit"/>
Specifies how annotations have to be placed in Chart.

<table class="props">
<thead>
<tr>
<th>Name</th>
<th>Type</th>
<th class="last">Description</th>
</tr>
</thead>
<tbody>
<tr>
<td class="name">
None</td>
<td class="type">string</td>
<td class="description">Place the annotation to the center of the chart.</td>
</tr>
<tr>
<td class="name">
Pixels</td>
<td class="type">string</td>
<td class="description">To place the annotation based on the pixel.</td>
</tr>
<tr>
<td class="name">
Points</td>
<td class="type">string</td>
<td class="description">To place the annotation based on the points</td>
</tr>
</tbody>
</table>

#### Default Value

* "none". See <a href="ejchart.html#members:annotations-coordinateunit">CoordinateUnit</a>




#### Example


{% highlight js %}
 
$("#container").ejChart({

   annotations :[{ coordinateUnit :"pixels"}]
                    
});

{% endhighlight %}




### annotations.horizontalAlignment `enum`
{:#members:annotations-horizontalalignment}

<ts name="ej.datavisualization.Chart.HorizontalAlignment"/>
Specifies the horizontal alignment of the annotation.

<table class="props">
<thead>
<tr>
<th>Name</th>
<th>Type</th>
<th class="last">Description</th>
</tr>
</thead>
<tbody>
<tr>
<td class="name">
Left</td>
<td class="type">string</td> 
<td class="description">To place the annotation on left side .</td>
</tr>
<tr>
<td class="name">
Right</td>
<td class="type">string</td>
<td class="description">To place the annotation on right side.</td>
</tr>
<tr>
<td class="name">
Middle</td>
<td class="type">string</td>
<td class="description">To place the annotation to the middle of the chart.</td>
</tr>
</tbody>
</table>


#### Default Value

* "middle". See <a href="ejchart.html#members:annotations-horizontalalignment">HorizontalAlignment</a>




#### Example


{% highlight js %}
 
$("#container").ejChart({

   annotations :[{ horizontalAlignment :"left"}]
                    
});

{% endhighlight %}


Try it: [Horizontal Alignment](http://jsplayground.syncfusion.com/n5zfhoir)




### annotations.margin `object`
{:#members:annotations-margin}




Options to customize the margin of annotation.


Try it: [Margin](http://jsplayground.syncfusion.com/n5zfhoir)






### annotations.margin.bottom `number`
{:#members:annotations-margin-bottom}




Annotation is placed at the specified value above its original position.


#### Default Value

* 0




#### Example


{% highlight js %}
 
$("#container").ejChart({

   annotations :[{ margin :{ bottom:10}}]                    

});

{% endhighlight %}




### annotations.margin.left `number`
{:#members:annotations-margin-left}




Annotation is placed at the specified value from left side of its original position.


#### Default Value

* 0




#### Example


{% highlight js %}
 
$("#container").ejChart({

   annotations :[{ margin :{ left:10}}]                    

});

{% endhighlight %}




### annotations.margin.right `number`
{:#members:annotations-margin-right}




Annotation is placed at the specified value from the right side of its original position.


#### Default Value

* 0




#### Example


{% highlight js %}
 
$("#container").ejChart({

   annotations :[{ margin :{ right:10}}]                    

});

{% endhighlight %}




### annotations.margin.top `number`
{:#members:annotations-margin-top}




Annotation is placed at the specified value under its original position.


#### Default Value

* 0




#### Example


{% highlight js %}
 
$("#container").ejChart({

   annotations :[{ margin :{ top:10}}]                    

});

{% endhighlight %}




### annotations.opacity `number`
{:#members:annotations-opacity}




Controls the opacity of the annotation.


#### Default Value

* 1




#### Example


{% highlight js %}
 
$("#container").ejChart({

   annotations :[{ opacity : 0.5}]                    

});

{% endhighlight %}


Try it: [Annotation Opacity](http://jsplayground.syncfusion.com/rgl4uwkj)




### annotations.region `enum`
{:#members:annotations-region}

<ts name="ej.datavisualization.Chart.Region"/>
Specifies whether annotation has to be placed with respect to chart or series.


<table class="props">
<thead>
<tr>
<th>Name</th>
<th>Type</th> 
<th class="last">Description</th>
</tr>
</thead>
<tbody>
<tr>
<td class="name">
Chart</td>
<td class="type">string</td> 
<td class="description">Place the annotation with respect to chart.</td>
</tr>
<tr>
<td class="name">
Series</td>
<td class="type">string</td>
<td class="description">Place the annotation with respect to series.</td>
</tr> 
</tbody>
</table>


#### Default Value

* "chart". See <a href="ejchart.html#members:annotations-region">Region</a>




#### Example


{% highlight js %}
 
$("#container").ejChart({

   annotations :[{ region :"series"}]                    

});

{% endhighlight %}


Try it: [Annotation Region](http://jsplayground.syncfusion.com/yfxghhut)




### annotations.verticalAlignment `enum`
{:#members:annotations-verticalalignment}

<ts name="ej.datavisualization.Chart.VerticalAlignment"/>
Specifies the vertical alignment of the annotation.

<table class="props">
<thead>
<tr>
<th>Name</th>
<th>Type</th> 
<th class="last">Description</th>
</tr>
</thead>
<tbody>
<tr>
<td class="name">
Top</td>
<td class="type">string</td> 
<td class="description">Place the annotation to the top of the chart.</td>
</tr>
<tr>
<td class="name">
Bottom</td>
<td class="type">string</td>
<td class="description">Place the annotation to the bottom of the chart.</td>
</tr> 
<tr>
<td class="name">
Middle</td>
<td class="type">string</td>
<td class="description">Place the annotation to the middle of the chart.</td>
</tr> 
</tbody>
</table>


#### Default Value

* "middle". See <a href="ejchart.html#members:annotations-verticalalignment">VerticalAlignment</a>




#### Example


{% highlight js %}
 
$("#container").ejChart({

   annotations :[{ verticalAlignment :"top"}]                    

});

{% endhighlight %}


Try it: [Vertical Alignment](http://jsplayground.syncfusion.com/frjpm2um)




### annotations.visible `boolean`
{:#members:annotations-visible}




Controls the visibility of the annotation.


#### Default Value

* false




#### Example


{% highlight js %}
 
$("#container").ejChart({

   annotations :[{ visible :true}]                    

});

{% endhighlight %}


Try it: [Annotation Visibility](http://jsplayground.syncfusion.com/plihjtm3)




### annotations.x `number`
{:#members:annotations-x}




Represents the horizontal offset when coordinateUnit is pixels. 
when coordinateUnit is points, it represents the x-coordinate of axis bounded with xAxisName property or primary X axis when xAxisName is not provided. 
This property is not applicable when coordinateUnit is none.


#### Default Value

* 0




#### Example


{% highlight js %}
 
$("#container").ejChart({

   annotations :[{ x : 100}]                    

});

{% endhighlight %}


Try it: [Annotation Positioning](http://jsplayground.syncfusion.com/frjpm2um)




### annotations.xAxisName `string`
{:#members:annotations-xaxisname}




Name of the horizontal axis to be used for positioning the annotation. This property is applicable only when coordinateUnit is points.


#### Default Value

* ""




#### Example


{% highlight js %}
 
$("#container").ejChart({

   annotations :[{ xAxisName : "xAxis1"}]                    

});

{% endhighlight %}


Try it: [JS Playground Sample](http://jsplayground.syncfusion.com/h23k4jcy)




### annotations.y `number`
{:#members:annotations-y}




Represents the vertical offset when coordinateUnit is pixels. 
When coordinateUnit is points, it represents the y-coordinate of axis bounded with yAxisName property or primary Y axis when yAxisName is not provided. 
This property is not applicable when coordinateUnit is none.


#### Default Value

* 0




#### Example


{% highlight js %}
 

$("#container").ejChart({
annotations :[{ y : 100}]                    
});

{% endhighlight %}


Try it: [JS Playground Sample](http://jsplayground.syncfusion.com/1nq2ss4v)




### annotations.yAxisName `string`
{:#members:annotations-yaxisname}




Name of the vertical axis to be used for positioning the annotation. 
This property is applicable only when coordinateUnit is points.


#### Default Value

* ""




#### Example


{% highlight js %}
 
$("#container").ejChart({

   annotations :[{ yAxisName : "yAxis1"}]                    

});

{% endhighlight %}


Try it: [JS Playground Sample](http://jsplayground.syncfusion.com/2nqhtn0y)

### background `string`
{:#members:background}




Sets the background color of the  chart.


#### Default Value

* transparent




#### Example


{% highlight js %}
 
$("#container").ejChart({

   background: "skyblue"                      

});

{% endhighlight %}


Try it: [JS playground Sample](http://jsplayground.syncfusion.com/fqyoilqm)





### backGroundImageUrl `string`
{:#members:backgroundimageurl}




URL of the image to be used as chart background.


#### Default Value

* null




#### Example


{% highlight js %}
 
$("#container").ejChart({

   backGroundImageUrl: "../images/chart/wheat.png"                      

});

{% endhighlight %}


Try it: [JS playground Sample](http://jsplayground.syncfusion.com/i1bys43l)




### border `object`
{:#members:border}




Options for customizing the color, opacity and width of the chart border.


Try it: [JS Playground Sample](http://jsplayground.syncfusion.com/wxxv2rq1)





### border.color `string`
{:#members:border-color}




Border color of the chart.


#### Default Value

* null




#### Example


{% highlight js %}
                             
$("#container").ejChart({

   border: { color: "green" }                      

});

{% endhighlight %}




### border.opacity `number`
{:#members:border-opacity}




Opacity of the chart border.


#### Default Value

* 0.3




#### Example


{% highlight js %}
 
$("#container").ejChart({

   border: { opacity: 0.5 }                      

});

{% endhighlight %}




### border.width `number`
{:#members:border-width}




Width of the Chart border.


#### Default Value

* 0




#### Example


{% highlight js %}
 
$("#container").ejChart({

   border: { width: 2 }                      

});

{% endhighlight %}




### exportSettings `object`
{:#members:exportsettings}

This provides options for customizing export settings


### exportSettings.filename `string`
{:#members:exportsettings-filename}




Specifies the downloading filename


#### Default Value



* "chart"




#### Example


{% highlight js %}
 
$("#container").ejChart({

     exportSettings: { filename : "myChart" }
                          
});

{% endhighlight %}


### exportSettings.action `string`
{:#members:exportsettings-action}




Specifies the name of the action URL


#### Default Value



* ""




#### Example


{% highlight js %}
 
$("#container").ejChart({

     exportSettings: { action : "http://js.syncfusion.com/ExportingServices/api/JSChartExport/Export" }
                          
});

{% endhighlight %}

### exportSettings.angle `number`
{:#members:exportsettings-angle}




Specifies the angle for rotation


#### Default Value



* 0




#### Example


{% highlight js %}
 
$("#container").ejChart({

     exportSettings: { angle : 90}
                          
});

{% endhighlight %}


### exportSettings.type `enum`
{:#members:exportsettings-type}


<ts name="ej.datavisualization.Chart.ExportingType"/>
Specifies the format of the file to export

<table class="props">
<thead>
<tr>
<th>Name</th>
<th>Type</th> 
<th class="last">Description</th>
</tr>
</thead>
<tbody>
<tr>
<td class="name">
PNG</td>
<td class="type">string</td> 
<td class="description last">The chart will be exported in .png format</td>
</tr>
<tr>
<td class="name">
JPG</td>
<td class="type">string</td>
<td class="description last">The chart will be exported in .jpg format</td>
</tr> 
<tr>
<td class="name">
PDF</td>
<td class="type">string</td>
<td class="description last">The chart will be exported in .pdf format</td>
</tr> 
<tr>
<td class="name">
DOCX</td>
<td class="type">string</td>
<td class="description last">The chart will be exported in .doc format</td>
</tr> 
<tr>
<td class="name">
XLSX</td>
<td class="type">string</td>
<td class="description last">The chart will be exported in .xlsx format</td>
</tr> 
<tr>
<td class="name">
SVG</td>
<td class="type">string</td>
<td class="description last">The chart will be exported in .svg format</td>
</tr> 
</tbody>
</table>

#### Default Value



* "png"




#### Example


{% highlight js %}
 
$("#container").ejChart({

     exportSettings: { type : "jpg"}
                          
});

{% endhighlight %}


### exportSettings.orientation `enum`
{:#members:exportsettings-orientation}


<ts name="ej.datavisualization.Chart.ExportingOrientation"/>
Specifies the orientation of the document

<table class="props">
<thead>
<tr>
<th>Name</th>
<th>Type</th> 
<th class="last">Description</th>
</tr>
</thead>
<tbody>
<tr>
<td class="name">
Portrait</td>
<td class="type">string</td> 
<td class="description last">The Chart is exported in portrait for .doc type</td>
</tr>
<tr>
<td class="name">
Landscape</td>
<td class="type">string</td>
<td class="description last">The Chart is exported in landscape for .doc type</td>
</tr> 
</tbody>
</table>


#### Default Value



* "portrait"




#### Example


{% highlight js %}
 
$("#container").ejChart({

     exportSettings: { orientation : "landscape"}
                          
});

{% endhighlight %}


### exportSettings.mode `enum`
{:#members:exportsettings-mode}

<ts name="ej.datavisualization.Chart.ExportingMode"/>
Specifies the mode of exporting

<table class="props">
<thead>
<tr>
<th>Name</th>
<th>Type</th> 
<th class="last">Description</th>
</tr>
</thead>
<tbody>
<tr>
<td class="name">
Server Side</td>
<td class="type">string</td> 
<td class="description last">The Chart is exported at server side</td>
</tr>
<tr>
<td class="name">
Client Side</td>
<td class="type">string</td>
<td class="description last">The Chart is exported at client side</td>
</tr> 
</tbody>
</table>


#### Default Value



* "client"




#### Example


{% highlight js %}
 
$("#container").ejChart({

     exportSettings: { mode : "server"}
                          
});

{% endhighlight %}


### exportSettings.multipleExport `boolean`
{:#members:exportsettings-multipleexport}




Enable/ disable the multiple excel exporting


#### Default Value



* false




#### Example


{% highlight js %}
 
$("#container").ejChart({

     exportSettings: { multipleExport : true }
                          
});

{% endhighlight %}


### chartArea `object`
{:#members:chartarea}




Options for configuring the border and background of the plot area.




### chartArea.background `string`
{:#members:chartarea-background}




Background color of the plot area.


#### Default Value



* transparent




#### Example


{% highlight js %}
 
$("#container").ejChart({

     chartArea: { background : "white" }
                          
});

{% endhighlight %}


Try it: [JS Playground Sample](http://jsplayground.syncfusion.com/picztz23)


### chartArea.border `object`
{:#members:chartarea-border}




Options for customizing the border of the plot area.


Try it: [JS Playground Sample](http://jsplayground.syncfusion.com/kzy21bwx)




### chartArea.border.color `string`
{:#members:chartarea-border-color}




Border color of the plot area.


#### Default Value



* Gray




#### Example


{% highlight js %}
 
$("#container").ejChart({

    chartArea: { border: { color :"green"} }
                         
});

{% endhighlight %}


### chartArea.border.opacity `number`
{:#members:chartarea-border-opacity}




Opacity of the plot area border.


#### Default Value



* 0.3




#### Example


{% highlight js %}
 
$("#container").ejChart({

    chartArea: { border: { opacity : 0.5} }
                          
});

{% endhighlight %}


### chartArea.border.width `number`
{:#members:chartarea-border-width}




Border width of the plot area.


#### Default Value



* 0.5




#### Example


{% highlight js %}
 
$("#container").ejChart({

    chartArea: { border: { width : 0.2} }
                          
});

{% endhighlight %}




### columnDefinitions `array`
{:#members:columndefinitions}




Options to split Chart into multiple plotting areas vertically. Each object in the collection represents a plotting area in Chart.


Try it: [JS Playground Sample](http://jsplayground.syncfusion.com/zdfd1sai)




### columnDefinitions.unit `enum`
{:#members:columndefinitions-unit}

<ts name="ej.datavisualization.Chart.Unit"/>
Specifies the unit to measure the width of the column in plotting area.


<table class="props">
<thead>
<tr>
<th>Name</th>
<th>Type</th> 
<th class="last">Description</th>
</tr>
</thead>
<tbody>
<tr>
<td class="name">
Percentage</td>
<td class="type">string</td> 
<td class="description">Specifies the width of the column in percentage.</td>
</tr>
<tr>
<td class="name">
Pixel</td>
<td class="type">string</td>
<td class="description">Specifies the width of the column in pixel.</td>
</tr>  
</tbody>
</table>


#### Default Value

* 'pixel'. See <a href="ejchart.html#members:columnDefinitions">Unit</a>




#### Example


{% highlight js %}
 
$("#container").ejChart({

    columnDefinitions :[{unit : "percentage"}]                     

});

{% endhighlight %}




### columnDefinitions.columnWidth `number`
{:#members:columndefinitions-columnwidth}




Width of the column in plotting area. Width is measured in either pixel or percentage based on the value of unit property.


#### Default Value

* 50




#### Example


{% highlight js %}
 
$("#container").ejChart({

   columnDefinitions :[{ columnWidth : 50 }]                     

});

{% endhighlight %}




### columnDefinitions.lineColor `string`
{:#members:columndefinitions-linecolor}




Color of the line that indicates the starting point of the column in plotting area.


#### Default Value

* "transparent"




#### Example


{% highlight js %}
 
$("#container").ejChart({

   columnDefinitions :[{ lineColor : "green" }]                     

});

{% endhighlight %}




### columnDefinitions.lineWidth `number`
{:#members:columndefinitions-linewidth}




Width of the line that indicates the starting point of the column in plot area.


#### Default Value

* 1




#### Example


{% highlight js %}
 
$("#container").ejChart({

   columnDefinitions :[{ lineWidth : 2 }]                     

});

{% endhighlight %}




### commonSeriesOptions `object`
{:#members:commonseriesoptions}




Options for configuring the properties of all the series. You can also override the options for specific series by using series collection.


### commonSeriesOptions.animationDuration `string`
{:#members:commonseriesoptions-animationduration}

Specifies animation duration for series rendering

#### Default Value

 * null

#### Example

{% highlight js %}

$("#container").ejChart({
commonSeriesOptions : [{
            animationDuration : 2000 
        }]                   
});
{% endhighlight %}



### commonSeriesOptions.border `object`
{:#members:commonseriesoptions-border}




Options to customize the border of all the series.






### commonSeriesOptions.border.color `string`
{:#members:commonseriesoptions-border-color}




Border color of all series.


#### Default Value



* "transparent"




#### Example


{% highlight js %}
 

$("#container").ejChart({
commonSeriesOptions :{border :{ color : "green" } }                  
});
{% endhighlight %}


### commonSeriesOptions.border.dashArray `string`
{:#members:commonseriesoptions-border-dasharray}




DashArray for border of the series.



#### Default Value



 * null




#### Example


{% highlight js %}
 
 
$("#container").ejChart({
   commonSeriesOptions : {
      border: {
           dashArray: "5,3"
       } 
    }                   
});
 {% endhighlight %}


### commonSeriesOptions.border.width `number`
{:#members:commonseriesoptions-border-width}




Border width of all series.


#### Default Value



* 1




#### Example


{% highlight js %}
 
 
$("#container").ejChart({
commonSeriesOptions :{border :{ width : 2 } }                  
});
{% endhighlight %}



### commonSeriesOptions.columnFacet `enum`
{:#members:commonseriesoptions-columnfacet}

<ts name="ej.datavisualization.Chart.ColumnFacet"/>
To render the column and bar type series in rectangle/cylinder shape. See <a href="global.html#ColumnFacet">ColumnFacet</a>


<table class="props">
<thead>
<tr>
<th>Name</th>
<th>Type</th> 
<th class="last">Description</th>
</tr>
</thead>
<tbody>
<tr>
<td class="name">
Rectangle</td>
<td class="type">string</td> 
<td class="description">Draw column and bar series in rectangle shape</td>
</tr>
<tr>
<td class="name">
Cylinder</td>
<td class="type">string</td>
<td class="description">Draw column and bar series in cylinder shape</td>
</tr> 
</tbody>
</table>



#### Default Value



 * "rectangle"




#### Example


{% highlight js %}
 

$('#container').ejChart({

    commonSeriesOptions: {
    
        //change to cylinder chart
		columnFacet: "cylinder"

    },

    //...

});

{% endhighlight %}


### commonSeriesOptions.columnWidth `number`
{:#members:commonseriesoptions-columnwidth}




Relative width of the columns in column type series. Value ranges from 0 to 1. Width also depends upon **columnSpacing** property.



#### Default Value



 * 0.7




#### Example


{% highlight js %}
 

$('#container').ejChart({

    commonSeriesOptions: {
    
        //Width of columns in column type series
		columnWidth: 0.8

        //... 
    },

    //...

});

{% endhighlight %}




### commonSeriesOptions.columnSpacing `number`
{:#members:commonseriesoptions-columnspacing}




Spacing between columns of different series. Value ranges from 0 to 1



#### Default Value



 * 0




#### Example


{% highlight js %}
 

$('#container').ejChart({

    commonSeriesOptions: {
    
        //20% Spacing between columns
		columnWidth: 0.2

    },

    //...

});

{% endhighlight %}




### commonSeriesOptions.visibleOnLegend `string`
{:#members:commonseriesoptions-visibleonlegend}




Enables or disables the visibility of legend item.



#### Default Value



 * "visible"




#### Example


{% highlight js %}
 

$("#container").ejChart({
commonSeriesOptions : {visibleOnLegend: "hidden" }                   
});
{% endhighlight %}


### commonSeriesOptions.stackingGroup `string`
{:#members:commonseriesoptions-stackinggroup}


Group of the stacking collection series.


#### Default Value



 * ""




#### Example


{% highlight js %}
 

$("#container").ejChart({
commonSeriesOptions :{stackingGroup : " "}                  
});
 {% endhighlight %}


### commonSeriesOptions.dashArray `string`
{:#members:commonseriesoptions-dasharray}




Pattern of dashes and gaps used to stroke all the line type series.


#### Default Value



 * ""




#### Example


{% highlight js %}
 

$("#container").ejChart({
commonSeriesOptions :{dashArray : "2,3"}                  
});
 {% endhighlight %}




### commonSeriesOptions.dataSource `object`
{:#members:commonseriesoptions-datasource}




Set the dataSource for all series. It can be an array of JSON objects or an instance of ej.DataManager.


#### Default Value



* null




#### Example


{% highlight js %}
 

$("#container").ejChart({
commonSeriesOptions : {dataSource: data }                   
});

 {% endhighlight %}
 
 
 Try it: [JS Playground Sample](http://jsplayground.syncfusion.com/ubbu5ukf)

### commonSeriesOptions.cardinalSplineTension `number`
{:#members:commonseriesoptions-cardinalsplinetension} 

Specifies spline tension value for cardinal spline type. Value ranges from 0 to 1.

#### Default Value

* 0.5

#### Example

{% highlight js %} 
$("#container").ejChart({
commonSeriesOptions :{ cardinalSplineTension : 0.5}                  
});
{% endhighlight %}


### commonSeriesOptions.doughnutCoefficient `number`
{:#members:commonseriesoptions-doughnutcoefficient}




Controls the size of the hole in doughnut series. Value ranges from 0 to 1


#### Default Value



* 0.4




#### Example


{% highlight js %}
 
 
$("#container").ejChart({
commonSeriesOptions :{ doughnutCoefficient : 0.5}                  
});
{% endhighlight %}


Try it: [JS Playground Sample](http://jsplayground.syncfusion.com/15exlbqk)



### commonSeriesOptions.doughnutSize `number`
{:#members:commonseriesoptions-doughnutsize}




Controls the size of the doughnut series. Value ranges from 0 to 1.


#### Default Value



* 0.8




#### Example


{% highlight js %}
 
 
$("#container").ejChart({
commonSeriesOptions :{ doughnutSize : 0.9}                  
});
 {% endhighlight %}
 
 
 Try it: [JS Playground Sample](http://jsplayground.syncfusion.com/ywbzcwhh)



### commonSeriesOptions.drawType `enum`
{:#members:commonseriesoptions-drawtype}


<ts name="ej.datavisualization.Chart.DrawType"/>
Specifies the type of series to be drawn in radar or polar series. 


<table class="props">
<thead>
<tr>
<th>Name</th>
<th>Type</th> 
<th class="last">Description</th>
</tr>
</thead>
<tbody>
<tr>
<td class="name">
Line</td>
<td class="type">string</td> 
<td class="description">Line type series will be drawn.</td>
</tr>
<tr>
<td class="name">
Area</td>
<td class="type">string</td>
<td class="description">Area type series will be drawn.</td>
</tr> 
<tr>
<td class="name">
Column</td>
<td class="type">string</td>
<td class="description">Column type series will be drawn.</td>
</tr> 
</tbody>
</table>


#### Default Value



* "line". See <a href="ejchart.html#members:commonseriesoptions-drawtype">DrawType</a>

#### Example


{% highlight js %}
 

$("#container").ejChart({
commonSeriesOptions :{ drawType : "area"}                  
});
 {% endhighlight %}


Try it: [JS Playground Sample](http://jsplayground.syncfusion.com/woedp3qa)



### commonSeriesOptions.enableAnimation `boolean`
{:#members:commonseriesoptions-enableanimation}




Enable/disable the animation for all the series.


#### Default Value



* true




#### Example


{% highlight js %}
 
 
$("#container").ejChart({
commonSeriesOptions :{ enableAnimation : false}                  
});
 {% endhighlight %}




### commonSeriesOptions.enableSmartLabels `boolean`
{:#members:commonseriesoptions-enablesmartlabels}




To avoid overlapping of data labels smartly. 


#### Default Value



* true




#### Example


{% highlight js %}
 
 
$("#container").ejChart({
commonSeriesOptions :{ enableSmartLabels : false}                  
});
  {% endhighlight %}


Try it: [JS Playground Sample](http://jsplayground.syncfusion.com/ojz1vbr4)



### commonSeriesOptions.endAngle `number`
{:#members:commonseriesoptions-endangle}




Start angle of pie/doughnut series.


#### Default Value



* null




#### Example


{% highlight js %}
 
 
$("#container").ejChart({
commonSeriesOptions :{ endAngle : 270}                  
});
 {% endhighlight %}


Try it: [JS Playground Sample](http://jsplayground.syncfusion.com/52kkuy5d)


### commonSeriesOptions.explode `boolean`
{:#members:commonseriesoptions-explode}




Explodes the pie/doughnut slices on mouse move.


#### Default Value



* false




#### Example


{% highlight js %}
 
 
$("#container").ejChart({
commonSeriesOptions :{ explode : true}                  
});
{% endhighlight %}


Try it: [JS Playground Sample](http://jsplayground.syncfusion.com/cletijkr)



### commonSeriesOptions.explodeAll `boolean`
{:#members:commonseriesoptions-explodeall}




Explodes all the slice of pie/doughnut on render.


#### Default Value



* false




#### Example


{% highlight js %}
 
 
$("#container").ejChart({
commonSeriesOptions :{ explodeAll : true}                  
});
 {% endhighlight %}
 
 
 Try it: [JS Playground Sample](http://jsplayground.syncfusion.com/2btbqicb)



### commonSeriesOptions.explodeIndex `number`
{:#members:commonseriesoptions-explodeindex}




Index of the point to be exploded from pie/doughnut/pyramid/funnel.


#### Default Value



* null




#### Example


{% highlight js %}
 
 
$("#container").ejChart({
commonSeriesOptions :{ explodeIndex : 2}                  
});
 {% endhighlight %}
 
 
 
 Try it: [JS Playground Sample](http://jsplayground.syncfusion.com/lypx2awm)




### commonSeriesOptions.explodeOffset `number`
{:#members:commonseriesoptions-explodeoffset}




Specifies the distance of the slice from the center, when it is exploded.


#### Default Value



* 0.4




#### Example


{% highlight js %}
 
 
$("#container").ejChart({
commonSeriesOptions :{ explodeOffset : 20}                  
});
 {% endhighlight %}
 
 
 Try it: [JS Playground Sample](http://jsplayground.syncfusion.com/t2ysyshe)



### commonSeriesOptions.fill `string`
{:#members:commonseriesoptions-fill}




Fill color for all the series.


#### Default Value



* null




#### Example


{% highlight js %}
 
 
$("#container").ejChart({
commonSeriesOptions :{fill : "green"}                  
});
{% endhighlight %}



Try it: [JS Playground](http://jsplayground.syncfusion.com/wdgfh0f1)



### commonSeriesOptions.font `object`
{:#members:commonseriesoptions-font}




Options for customizing the font of all the series.






### commonSeriesOptions.font.color `string`
{:#members:commonseriesoptions-font-color}




Font color of the text in all series.


#### Default Value



* "#707070"




#### Example


{% highlight js %}
 
 
$("#container").ejChart({
commonSeriesOptions :{font :{color : "green"}}                 
});
{% endhighlight %}




### commonSeriesOptions.font.fontFamily `string`
{:#members:commonseriesoptions-font-fontfamily}




Font Family for all the series.


#### Default Value



* "Segoe UI"




#### Example


{% highlight js %}
 

$("#container").ejChart({
commonSeriesOptions :{ font : { fontFamily : "Algerian"}}                 
});
 {% endhighlight %}




### commonSeriesOptions.font.fontStyle `enum`
{:#members:commonseriesoptions-font-fontstyle}


<ts name="ej.datavisualization.Chart.FontStyle"/>
Specifies the font Style for all the series.


<table class="props">
<thead>
<tr>
<th>Name</th>
<th>Type</th> 
<th class="last">Description</th>
</tr>
</thead>
<tbody>
<tr>
<td class="name">
Normal</td>
<td class="type">string</td> 
<td class="description">Specifies the fontStyle as normal.</td>
</tr>
<tr>
<td class="name">
Italic</td>
<td class="type">string</td>
<td class="description">Specifies the fontStyle as italic.</td>
</tr> 
</tbody>
</table>


#### Default Value



* "normal"




#### Example


{% highlight js %}
 

$("#container").ejChart({
commonSeriesOptions : {font :{fontStyle : "italic"}}                 
});
{% endhighlight %}




### commonSeriesOptions.font.fontWeight `enum`
{:#members:commonseriesoptions-font-fontweight}


<ts name="ej.datavisualization.Chart.FontWeight"/>
Specifies the font weight for all the series.


<table class="props">
<thead>
<tr>
<th>Name</th>
<th>Type</th> 
<th class="last">Description</th>
</tr>
</thead>
<tbody>
<tr>
<td class="name">
Regular</td>
<td class="type">string</td> 
<td class="description">Specifies the font weight as regular.</td>
</tr>
<tr>
<td class="name">
Bold</td>
<td class="type">string</td>
<td class="description">Specifies the font weight as bold.</td>
</tr> 
<tr>
<td class="name">
Lighter</td>
<td class="type">string</td>
<td class="description">Specifies the font weight as lighter.</td>
</tr> 
</tbody>
</table>


#### Default Value



* "regular"




#### Example


{% highlight js %}
 

$("#container").ejChart({
commonSeriesOptions :{font :{fontWeight : "lighter"}}                 
});
{% endhighlight %}




### commonSeriesOptions.font.opacity `number`
{:#members:commonseriesoptions-font-opacity}




Opacity for text in all the series.


#### Default Value



* 1




#### Example


{% highlight js %}
 

$("#container").ejChart({
commonSeriesOptions :{font :{opacity : 0.5}}                 
});
{% endhighlight %}




### commonSeriesOptions.font.size `string`
{:#members:commonseriesoptions-font-size}




Font size for text in all the series.

#### Default Value



 * "12px"




#### Example


{% highlight js %}
 
 
$("#container").ejChart({
commonSeriesOptions :{font :{size : "14px"}}                 
});
{% endhighlight %}



Try it: [JS Playground Sample](http://jsplayground.syncfusion.com/gmjlryrg)



### commonSeriesOptions.funnelHeight `string`
{:#members:commonseriesoptions-funnelheight}




Sets the height of the funnel in funnel series. Values can be either pixel or percentage.


#### Default Value



 * "32.7%"




#### Example


{% highlight js %}
 
<div id="container"></div> 
<script>
$("#container").ejChart({
commonSeriesOptions : {funnelHeight : '40%' }                 
});
</script> {% endhighlight %}


Try it: [JS Playground Sample](http://jsplayground.syncfusion.com/cnku50hw)




### commonSeriesOptions.funnelWidth `string`
{:#members:commonseriesoptions-funnelwidth}




Sets the width of the funnel in funnel series. Values can be either pixel or percentage.

#### Default Value



 * "11.6%"




#### Example


{% highlight js %}
 

$("#container").ejChart({
commonSeriesOptions : {funnelWidth : '40%' }                  
});
 {% endhighlight %}
 
 
 
 Try it: [JS Playground Sample](http://jsplayground.syncfusion.com/aj4pwnrm)




### commonSeriesOptions.gapRatio `number`
{:#members:commonseriesoptions-gapratio}




Gap between the slices in pyramid and funnel series.


#### Default Value



 * 0




#### Example


{% highlight js %}
 
 
$("#container").ejChart({
commonSeriesOptions :{ gapRatio : 0.5}                  
});
  {% endhighlight %}
  
  
Try it: [JS Playground](http://jsplayground.syncfusion.com/om3zazbd)




### commonSeriesOptions.isClosed `boolean`
{:#members:commonseriesoptions-isclosed}




Specifies whether to join start and end point of a line/area series used in polar/radar chart to form a closed path.


#### Default Value



 * true




#### Example


{% highlight js %}
 
 
$("#container").ejChart({
commonSeriesOptions :{ isClosed : false}                  
});
{% endhighlight %}


Try it: [JS Playground Sample](http://jsplayground.syncfusion.com/d41kmmwt)




### commonSeriesOptions.isStacking `boolean`
{:#members:commonseriesoptions-isstacking}




Specifies whether to stack the column series in polar/radar charts.


#### Default Value



 * false




#### Example


{% highlight js %}
 
 
$("#container").ejChart({
commonSeriesOptions :{ isStacking : "true"}                  
});
 {% endhighlight %}


Try it: [JS Playground Sample](http://jsplayground.syncfusion.com/g40hdrpl)




### commonSeriesOptions.isTransposed `boolean`
{:#members:commonseriesoptions-istransposed}




Renders the chart vertically. This is applicable only for Cartesian type series.


#### Default Value



* false




#### Example


{% highlight js %}
 
 
$("#container").ejChart({
commonSeriesOptions : {isTransposed : false }                   
});
{% endhighlight %}


### commonSeriesOptions.showMedian `boolean`
{:#members:commonseriesoptions-showmedian}




Render the x mark in the center of the box and whisker series type.x represents the average value of the box and whisker series.


#### Default Value



* true




#### Example


{% highlight js %}
 
 
$("#container").ejChart({
commonSeriesOptions : {showMedian : true }                   
});
{% endhighlight %}




### commonSeriesOptions.labelPosition `enum`
{:#members:commonseriesoptions-labelposition}


<ts name="ej.datavisualization.Chart.LabelPosition"/>
Position of the data label in pie/doughnut/pyramid/funnel series. OutsideExtended position is not applicable for pyramid/funnel.


<table class="props">
<thead>
<tr>
<th>Name</th>
<th>Type</th> 
<th class="last">Description</th>
</tr>
</thead>
<tbody>
<tr>
<td class="name">
Inside</td>
<td class="type">string</td> 
<td class="description">To place the datalabel inside the chart.</td>
</tr>
<tr>
<td class="name">
Outside</td>
<td class="type">string</td>
<td class="description">To place the datalabel outside the chart.</td>
</tr> 
<tr>
<td class="name">
OutsideExtended</td>
<td class="type">string</td>
<td class="description">To place the datalabel at the extend of the chart.</td>
</tr> 
</tbody>
</table>


#### Default Value



* "inside". See <a href="ejchart.html#members:commonseriesoptions-labelposition">LabelPosition</a>



#### Example


{% highlight js %}
 

$("#container").ejChart({
commonSeriesOptions :{ labelPosition : "outside"}                  
});
 {% endhighlight %}
 

Try it: [JS Playground Sample](http://jsplayground.syncfusion.com/w5q1jt5k)


### commonSeriesOptions.splitMode `enum`
{:#members:commonseriesoptions-splitmode}


<ts name="ej.datavisualization.Chart.SplitMode"/>
Specifies the mode for splitting the data points in pieOfPie series.


<table class="props">
<thead>
<tr>
<th>Name</th>
<th>Type</th> 
<th class="last">Description</th>
</tr>
</thead>
<tbody>
<tr>
<td class="name">
Position</td>
<td class="type">string</td> 
<td class="description">Splitting the data points based on the specified position value.</td>
</tr>
<tr>
<td class="name">
Value</td>
<td class="type">string</td>
<td class="description">Splitting the data points based on the specified Y value.</td>
</tr> 
<tr>
<td class="name">
Percentage</td>
<td class="type">string</td>
<td class="description">Splitting the data points based on the specified percentage value.</td>
</tr> 
<tr>
<td class="name">
Indexes</td>
<td class="type">string</td>
<td class="description">The data points with the specified indexes are get splitted.</td>
</tr> 
</tbody>
</table>


#### Default Value



* "value". See <a href="ejchart.html#members:commonseriesoptions-splitmode">SplitMode</a>



#### Example


{% highlight js %}
 

$("#container").ejChart({
commonSeriesOptions :{ splitMode : "position"}               
});
 {% endhighlight %}


### commonSeriesOptions.boxPlotMode `enum`
{:#members:commonseriesoptions-boxplotmode}


<ts name="ej.datavisualization.Chart.boxPlotMode"/>
Quartile calculation has been performed in three different formulas to render the box and whisker series.


<table class="props">
<thead>
<tr>
<th>Name</th>
<th>Type</th> 
<th class="last">Description</th>
</tr>
</thead>
<tbody>
<tr>
<td class="name">
Exclusive</td>
<td class="type">string</td> 
<td class="description">To render the series with exclusive calculations</td>
</tr>
<tr>
<td class="name">
Inclusive</td>
<td class="type">string</td>
<td class="description">To render the series with inclusive calculations</td>
</tr> 
<tr>
<td class="name">
Normal</td>
<td class="type">string</td>
<td class="description">To render the series with normal calculations</td>
</tr> 
</tbody>
</table>


#### Default Value



* "exclusive"



#### Example


{% highlight js %}
 

$("#container").ejChart({
commonSeriesOptions :{ boxPlotMode : "inclusive"}                  
});
 {% endhighlight %}
 


### commonSeriesOptions.bubbleOptions `object`
{:#members:commonseriesoptions-bubbleoptions}

Options for customizing the bubble options of the Bubble series 

### commonSeriesOptions.bubbleOptions.radiusMode `enum`
{:#members:commonseriesoptions-bubbleoptions-radiusmode}



<ts name="ej.datavisualization.Chart.RadiusMode"/>
Used for the calculation of the bubble radius based on the mode selected 


<table class="props">
<thead>
<tr>
<th>Name</th>
<th>Type</th> 
<th class="last">Description</th>
</tr>
</thead>
<tbody>
<tr>
<td class="name">
MinMax</td>
<td class="type">string</td> 
<td class="description">To render the bubble based on the Minimum and Maximum radius </td>
</tr>
<tr>
<td class="name">
Auto</td>
<td class="type">string</td>
<td class="description">To render the bubble based on the Range and Size of the Chart</td>
</tr> 
</tbody>
</table>


#### Default Value



* "minMax"



#### Example


{% highlight js %}
 

$("#container").ejChart({
commonSeriesOptions :{ bubbleOptions: { radiusMode: "minMax" }}                  
});

 {% endhighlight %}
 
### commonSeriesOptions.bubbleOptions.minRadius `number`
{:#members:commonseriesoptions-bubbleoptions-minradius}



Used for the setting the minimum radius of the bubble 


#### Default Value



* 1



#### Example


{% highlight js %}
 

$("#container").ejChart({
commonSeriesOptions :{ bubbleOptions: { minRadius: 3 }}                  
});

 {% endhighlight %}


### commonSeriesOptions.bubbleOptions.maxRadius `number`
{:#members:commonseriesoptions-bubbleoptions-maxradius}



Used for setting the maximum radius of the bubble 


#### Default Value



* 3



#### Example


{% highlight js %}
 

$("#container").ejChart({
commonSeriesOptions :{ bubbleOptions: { maxRadius: 7 }}                  
});

 {% endhighlight %}

Try it: [JS Playground Sample](http://jsplayground.syncfusion.com/zdnbwech)



### commonSeriesOptions.splineType `enum`
{:#members:commonseriesoptions-splinetype}


<ts name="ej.datavisualization.Chart.SplineType"/>
To render the spline series curve in different forms. 



<table class="props">
<thead>
<tr>
<th>Name</th>
<th>Type</th> 
<th class="last">Description</th>
</tr>
</thead>
<tbody>
<tr>
<td class="name">
Natural</td>
<td class="type">string</td> 
<td class="description">To render the series with natural curve</td>
</tr>
<tr>
<td class="name">
Monotonic</td>
<td class="type">string</td>
<td class="description">To render the series with monotonic curve</td>
</tr> 
<tr>
<td class="name">
Cardinal</td>
<td class="type">string</td>
<td class="description">To render the series with cardinal curve</td>
</tr> 
<tr>
<td class="name">
Clamped</td>
<td class="type">string</td>
<td class="description">To render the series with clamped curve</td>
</tr> 
</tbody>
</table>


#### Default Value



* "natural". See <a href="ejchart.html#members:splinetype">SplineType</a>

#### Example

{% highlight js %} 

$("#container").ejChart({
commonSeriesOptions :{ splineType : "cardinal"}                  
});
{% endhighlight %}



### commonSeriesOptions.lineCap `enum`
{:#members:commonseriesoptions-linecap}


<ts name="ej.datavisualization.Chart.LineCap"/>
Specifies the line cap of the series. 



<table class="props">
<thead>
<tr>
<th>Name</th>
<th>Type</th> 
<th class="last">Description</th>
</tr>
</thead>
<tbody>
<tr>
<td class="name">
Butt</td>
<td class="type">string</td> 
<td class="description">Specifies the line cap of the series to butt.</td>
</tr>
<tr>
<td class="name">
Round</td>
<td class="type">string</td>
<td class="description">Specifies the line cap of the series to round.</td>
</tr> 
<tr>
<td class="name">
Square</td>
<td class="type">string</td>
<td class="description">Specifies the line cap of the series to square.</td>
</tr> 
</tbody>
</table>


#### Default Value



* "butt". See <a href="ejchart.html#members:commonseriesoptions-linecap">LineCap</a>


#### Example


{% highlight js %}
 
 
$("#container").ejChart({
commonSeriesOptions :{lineCap : "butt"}                  
});
{% endhighlight %}




### commonSeriesOptions.lineJoin `enum`
{:#members:commonseriesoptions-linejoin}


<ts name="ej.datavisualization.Chart.LineJoin"/>
Specifies the type of shape to be used where two lines meet.


<table class="props">
<thead>
<tr>
<th>Name</th>
<th>Type</th> 
<th class="last">Description</th>
</tr>
</thead>
<tbody>
<tr>
<td class="name">
Round</td>
<td class="type">string</td> 
<td class="description">Line join will be round.</td>
</tr>
<tr>
<td class="name">
Bevel</td>
<td class="type">string</td>
<td class="description">Line join will be bevel.</td>
</tr> 
<tr>
<td class="name">
Miter</td>
<td class="type">string</td>
<td class="description">Line join will be miter.</td>
</tr> 
</tbody>
</table>


#### Default Value



* "round". See <a href="ejchart.html#members:commonseriesoptions-linejoin">LineJoin</a>


#### Example


{% highlight js %}
 
 
$("#container").ejChart({
commonSeriesOptions :{lineCap : "round"}                  
});
{% endhighlight %}




### commonSeriesOptions.marker `object`
{:#members:commonseriesoptions-marker}




Options for displaying and customizing marker for individual point in a series. Marker contains shapes and/or data labels.






### commonSeriesOptions.marker.border `object`
{:#members:commonseriesoptions-marker-border}




Options for customizing the border of the marker shape.






### commonSeriesOptions.marker.border.color `string`
{:#members:commonseriesoptions-marker-border-color}




Border color of the marker shape. 


#### Default Value



* "white"




#### Example


{% highlight js %}
 
 
$("#container").ejChart({
commonSeriesOptions :{color : "green"}                  
});
 {% endhighlight %}




### commonSeriesOptions.marker.border.width `number`
{:#members:commonseriesoptions-marker-border-width}




Border width of the marker shape. 


#### Default Value



* 3




#### Example


{% highlight js %}
 
 
$("#container").ejChart({
commonSeriesOptions :{marker :{border :{width : 2}}}                  
});
{% endhighlight %}




### commonSeriesOptions.marker.dataLabel `object`
{:#members:commonseriesoptions-marker-datalabel}




Options for displaying and customizing data labels.






### commonSeriesOptions.marker.dataLabel.angle `number`
{:#members:commonseriesoptions-marker-datalabel-angle}




Angle of the data label in degrees. Only the text gets rotated, whereas the background and border does not rotate. 


#### Default Value



 * null




#### Example


{% highlight js %}
 
 
$("#container").ejChart({
commonSeriesOptions :{marker :{dataLabel :{angle : 90}}}                  
});
 {% endhighlight %}



Try it: [JS Playground Sample](http://jsplayground.syncfusion.com/rbw3xizf)



### commonSeriesOptions.marker.dataLabel.maximumLabelWidth `number`
{:#members:commonseriesoptions-marker-datalabel-maximumlabelwidth}


Maximum label width of the data label. 


#### Default Value

 * null


#### Example


{% highlight js %}
 
 
$("#container").ejChart({
commonSeriesOptions :{marker :{dataLabel :{maximumLabelWidth : 90}}}                  
});
 {% endhighlight %}


Try it: [JS Playground Sample](http://jsplayground.syncfusion.com/klibjzkp)



### commonSeriesOptions.marker.dataLabel.enableWrap `boolean`
{:#members:commonseriesoptions-marker-datalabel-enablewrap}

Enable the wrap option to the data label. 

#### Default Value

 * false

#### Example

{% highlight js %}
 
 
$("#container").ejChart({
commonSeriesOptions :{marker :{dataLabel :{enableWrap : false}}}                  
});
 {% endhighlight %}


Try it: [JS Playground Sample](http://jsplayground.syncfusion.com/klibjzkp)

### commonSeriesOptions.marker.dataLabel.enableContrastColor `boolean`
{:#members:commonseriesoptions-marker-datalabel-enablecontrastcolor}

Enables saturation to the data label. 

#### Default Value

 * false

#### Example

{% highlight js %}
$("#container").ejChart({
commonSeriesOptions :{marker :{dataLabel :{enableContrastColor : false}}}                  
});
 {% endhighlight %}


### commonSeriesOptions.marker.dataLabel.showEdgeLabels `boolean`
{:#members:commonseriesoptions-marker-datalabel-showedgelabels}

Displays the partially visible labels inside the chart Area 

#### Default Value

 * false

#### Example

{% highlight js %}
$("#container").ejChart({
commonSeriesOptions :{marker :{dataLabel :{showEdgeLabels : false}}}                  
});
 {% endhighlight %}



### commonSeriesOptions.marker.dataLabel.border `object`
{:#members:commonseriesoptions-marker-datalabel-border}




Options for customizing the border of the data label.






### commonSeriesOptions.marker.dataLabel.border.color `string`
{:#members:commonseriesoptions-marker-datalabel-border-color}




Border color of the data label. 


#### Default Value



* null




#### Example


{% highlight js %}
 
 
$("#container").ejChart({
commonSeriesOptions :{marker :{dataLabel :{border : {color : "green"}}}}                 
});
{% endhighlight %}




### commonSeriesOptions.marker.dataLabel.border.width `number`
{:#members:commonseriesoptions-marker-datalabel-border-width}




Border width of the data label. 


#### Default Value



* 0.1




#### Example


{% highlight js %}
 
 
$("#container").ejChart({
commonSeriesOptions :{marker :{dataLabel :{border :{ width :2 }}}}                 
});
 {% endhighlight %}
 
 
 Try it: [JS Playground Sample](http://jsplayground.syncfusion.com/f4b4p32r)



### commonSeriesOptions.marker.dataLabel.connectorLine `object`
{:#members:commonseriesoptions-marker-datalabel-connectorline}




Options for displaying and customizing the line that connects point and data label.






### commonSeriesOptions.marker.dataLabel.connectorLine.type `enum`
{:#members:commonseriesoptions-marker-datalabel-connectorline-type}


<ts name="ej.datavisualization.Chart.ConnectorLineType"/>
Specifies when the connector has to be drawn as Bezier curve or straight line. This is applicable only for Pie and Doughnut chart types.


<table class="props">
<thead>
<tr>
<th>Name</th>
<th>Type</th> 
<th class="last">Description</th>
</tr>
</thead>
<tbody>
<tr>
<td class="name">
Line</td>
<td class="type">string</td> 
<td class="description">ConnectorLine type is line.</td>
</tr>
<tr>
<td class="name">
Bezier</td>
<td class="type">string</td>
<td class="description">ConnectorLine type is Bezier.</td>
</tr> 
 
</tbody>
</table>


#### Default Value



* "line". See <a href="ejchart.html#members:commonseriesoptions-marker-datalabel-connectorline-type">ConnectorLineType</a>


#### Example


{% highlight js %}
 

$("#container").ejChart({
commonSeriesOptions :{marker :{dataLabel :{connectorLine :{ type : "bezier" }}}}                 
});
{% endhighlight %}



Try it: [JS Playground Sample](http://jsplayground.syncfusion.com/pmnp5qjl)



### commonSeriesOptions.marker.dataLabel.connectorLine.width `number`
{:#members:commonseriesoptions-marker-datalabel-connectorline-width}




Width of the connector.


#### Default Value



* 0.5




#### Example


{% highlight js %}
 
 
$("#container").ejChart({
commonSeriesOptions :{marker :{dataLabel :{connectorLine :{ width : 2 }}}}                 
});
 {% endhighlight %}
 

Try it: [JS Playground Sample](http://jsplayground.syncfusion.com/pmnp5qjl)



### commonSeriesOptions.marker.dataLabel.connectorLine.color `string`
{:#members:commonseriesoptions.marker.datalabel.connectorline.color}




Color of the connector line.



#### Default Value



 * "#565656"




#### Example


{% highlight js %}
 
 
$("#container").ejChart({
commonSeriesOptions :{marker :{dataLabel :{connectorLine :{ color : "red" }}}}                 
});
 {% endhighlight %} 
 
 
 
 ### commonSeriesOptions.marker.dataLabel.connectorLine.height `string`
{:#members:commonseriesoptions.marker.datalabel.connectorline.height}




Height of the connector line.



#### Default Value



 * null




#### Example


{% highlight js %}
 
 
$("#container").ejChart({
commonSeriesOptions :{marker :{dataLabel :{connectorLine :{ height : 20 }}}}                 
});
 {% endhighlight %} 
 


### commonSeriesOptions.marker.dataLabel.fill `string`
{:#members:commonseriesoptions-marker-datalabel-fill}




Background color of the data label. 


#### Default Value



* null




#### Example


{% highlight js %}
 
 
$("#container").ejChart({
commonSeriesOptions :{marker :{dataLabel :{fill : "green"}}}                 
});
{% endhighlight %}




### commonSeriesOptions.marker.dataLabel.font `object`
{:#members:commonseriesoptions-marker-datalabel-font}




Options for customizing the data label font.






### commonSeriesOptions.marker.dataLabel.font.fontFamily `string`
{:#members:commonseriesoptions-marker-datalabel-font-fontfamily}




Font family of the data label. 


#### Default Value



* "Segoe UI"




#### Example


{% highlight js %}
 
 
$("#container").ejChart({
commonSeriesOptions :{marker :{dataLabel :{ font :{fontFamily : "Algerian"}}}}                 
});
{% endhighlight %}




### commonSeriesOptions.marker.dataLabel.font.fontStyle `enum`
{:#members:commonseriesoptions-marker-datalabel-font-fontstyle}

<ts ref="ej.datavisualization.Chart.FontStyle"/>


Font style of the data label.   


#### Default Value



* "normal". See <a href="ejchart.html#members:commonseriesoptions-marker-datalabel-font-fontstyle">FontStyle</a>


#### Example


{% highlight js %}
 
 
$("#container").ejChart({
commonSeriesOptions :{marker :{dataLabel :{font :{ fontStyle : "italic" }}}}                 
});
 {% endhighlight %}




### commonSeriesOptions.marker.dataLabel.font.fontWeight `enum`
{:#members:commonseriesoptions-marker-datalabel-font-fontweight}


<ts ref="ej.datavisualization.Chart.FontWeight"/>


Font weight of the data label.  


#### Default Value



* "regular". See <a href="ejchart.html#members:commonseriesoptions-marker-datalabel-font-fontweight">FontWeight</a>



#### Example


{% highlight js %}
 
 
$("#container").ejChart({
commonSeriesOptions :{marker :{dataLabel :{font : { fontWeight : "lighter" }}}}                 
});
{% endhighlight %}




### commonSeriesOptions.marker.dataLabel.font.opacity `number`
{:#members:commonseriesoptions-marker-datalabel-font-opacity}




Opacity of the text. 


#### Default Value



 * 1




#### Example


{% highlight js %}
 
 
$("#container").ejChart({
commonSeriesOptions :{marker :{dataLabel :{font :{ opacity : 0.5 }}}}                 
});
{% endhighlight %}

### commonSeriesOptions.marker.dataLabel.font.color `string`
{:#members:commonseriesoptions-marker-datalabel-font-color}

Font color of the data label text. 

#### Default Value

 * null

#### Example

{% highlight js %}

 
$("#container").ejChart({
commonSeriesOptions :{marker :{dataLabel :{font :{ color : "red" }}}}                 
});
{% endhighlight %}


### commonSeriesOptions.marker.dataLabel.font.size `string`
{:#members:commonseriesoptions-marker-datalabel-font-size}




Font size of the data label. 


#### Default Value



* "12px"




#### Example


{% highlight js %}
 

$("#container").ejChart({
commonSeriesOptions :{marker :{dataLabel :{font : { size : "14px" }}}}                 
});
{% endhighlight %}




### commonSeriesOptions.marker.dataLabel.horizontalTextAlignment `enum`
{:#members:commonseriesoptions-marker-datalabel-horizontaltextalignment}


<ts name="ej.datavisualization.Chart.HorizontalTextAlignment"/>
Horizontal alignment of the data label. 



<table class="props">
<thead>
<tr>
<th>Name</th>
<th>Type</th> 
<th class="last">Description</th>
</tr>
</thead>
<tbody>
<tr>
<td class="name">
Center</td>
<td class="type">string</td> 
<td class="description">Place the series to the center of the point.</td>
</tr>
<tr>
<td class="name">
Near</td>
<td class="type">string</td>
<td class="description">Place the series to the left of the point.</td>
</tr> 
<tr>
<td class="name">
Far</td>
<td class="type">string</td>
<td class="description">Place the annotation to the right of the point.</td>
</tr> 
</tbody>
</table>


#### Default Value



* "center"




#### Example


{% highlight js %}
 

$("#container").ejChart({
commonSeriesOptions :{marker :{dataLabel :{horizontalTextAlignment : "far"}}}                  
});
{% endhighlight %}


Try it: [JS Playground Sample](http://jsplayground.syncfusion.com/c3i3lxpg)



### commonSeriesOptions.marker.dataLabel.margin `object`
{:#members:commonseriesoptions-marker-datalabel-margin}




Margin of the text to its background shape. The size of the background shape increases based on the margin applied to its text.






### commonSeriesOptions.marker.dataLabel.margin.bottom `number`
{:#members:commonseriesoptions-marker-datalabel-margin-bottom}




Bottom margin of the text. 


#### Default Value



* 5




#### Example


{% highlight js %}
 
 
$("#container").ejChart({
commonSeriesOptions :{marker :{dataLabel :{margin :{ bottom :10 }}}}                 
});
{% endhighlight %}




### commonSeriesOptions.marker.dataLabel.margin.left `number`
{:#members:commonseriesoptions-marker-datalabel-margin-left}



Left margin of the text. 


#### Default Value



 * 5




#### Example


{% highlight js %}
 
 
$("#container").ejChart({
commonSeriesOptions :{marker :{dataLabel :{margin :{ left : 10}}}}                 
});
{% endhighlight %}




### commonSeriesOptions.marker.dataLabel.margin.right `number`
{:#members:commonseriesoptions-marker-datalabel-margin-right}




Right margin of the text. 


#### Default Value



* 5




#### Example


{% highlight js %}
 
 
$("#container").ejChart({
commonSeriesOptions :{marker :{dataLabel :{margin :{ right :10 }}}}                 
});
{% endhighlight %}




### commonSeriesOptions.marker.dataLabel.margin.top `number`
{:#members:commonseriesoptions-marker-datalabel-margin-top}




Top margin of the text. 


#### Default Value



* 5




#### Example


{% highlight js %}
 

$("#container").ejChart({
commonSeriesOptions :{marker :{dataLabel :{margin :{ top :10 } }}}                 
});
{% endhighlight %}


Try it: [JS Playground Sample](http://jsplayground.syncfusion.com/dff0lfpg)



### commonSeriesOptions.marker.dataLabel.opacity `number`
{:#members:commonseriesoptions-marker-datalabel-opacity}




Opacity of the data label. 


#### Default Value



* 1




#### Example


{% highlight js %}
 
 
$("#container").ejChart({
commonSeriesOptions :{marker :{dataLabel :{opacity : 0.5}}}                 
});
{% endhighlight %}

### commonSeriesOptions.marker.dataLabel.offset `object|number`
{:#members:commonseriesoptions-marker-datalabel-offset}

Options for customizing the datalabel positions 

### commonSeriesOptions.marker.dataLabel.offset.x `number`
{:#members:commonseriesoptions-marker-datalabel-offset-x}




X value or horizontal offset to position the labels in chart.


#### Default Value

* 0




#### Example


{% highlight js %}
 
$("#container").ejChart({

   commonSeriesOptions :[{  marker :{dataLabel :{offset : { x:10 }}} }]                    

});

{% endhighlight %}




### commonSeriesOptions.marker.dataLabel.offset.y `number`
{:#members:commonseriesoptions-marker-datalabel-offset-y}




Y value or vertical offset to position the labels.


#### Default Value

* 0




#### Example


{% highlight js %}
 
$("#container").ejChart({

   commonSeriesOptions :[{  marker :{dataLabel :{offset : { y:10 }}} }]                  

});

{% endhighlight %}



### commonSeriesOptions.marker.dataLabel.shape `enum`
{:#members:commonseriesoptions-marker-datalabel-shape}


<ts name="ej.datavisualization.Chart.Shape"/>
Background shape of the data label. 




<table class="props">
<thead>
<tr>
<th>Name</th>
<th>Type</th> 
<th class="last">Description</th>
</tr>
</thead>
<tbody>
<tr>
<td class="name">
None</td>
<td class="type">string</td> 
<td class="description">No shape for the datalabel.</td>
</tr>
<tr>
<td class="name">
LeftArrow</td>
<td class="type">string</td>
<td class="description">Shape of the datalabel will be leftarrow.</td>
</tr> 
<tr>
<td class="name">
RightArrow</td>
<td class="type">string</td>
<td class="description">Shape of the datalabel will be rightarrow.</td>
</tr> 
<tr>
<td class="name">
Circle</td>
<td class="type">string</td>
<td class="description">Shape of the datalabel will be circle.</td>
</tr> 
<tr>
<td class="name">
Cross</td>
<td class="type">string</td>
<td class="description">Shape of the datalabel will be cross.</td>
</tr> 
<tr>
<td class="name">
HorizLine</td>
<td class="type">string</td>
<td class="description">Shape of the datalabel will be horizline.</td>
</tr> 
<tr>
<td class="name">
VertLine</td>
<td class="type">string</td>
<td class="description">Shape of the datalabel will be vertline.</td>
</tr> 
<tr>
<td class="name">
Diamond</td>
<td class="type">string</td>
<td class="description">Shape of the datalabel will be diamond.</td>
</tr> 
<tr>
<td class="name">
Rectangle</td>
<td class="type">string</td>
<td class="description">Shape of the datalabel will be rectangle.</td>
</tr> 
<tr>
<td class="name">
Triangle</td>
<td class="type">string</td>
<td class="description">Shape of the datalabel will be triangle.</td>
</tr> 
<tr>
<td class="name">
Hexagon</td>
<td class="type">string</td>
<td class="description">Shape of the datalabel will be hexagon.</td>
</tr> 
<tr>
<td class="name">
Pentagon</td>
<td class="type">string</td>
<td class="description">Shape of the datalabel will be pentagon.</td>
</tr> 
<tr>
<td class="name">
Star</td>
<td class="type">string</td>
<td class="description">Shape of the datalabel will be star.</td>
</tr> 
<tr>
<td class="name">
Ellipse</td>
<td class="type">string</td>
<td class="description">Shape of the datalabel will be ellipse.</td>
</tr> 
<tr>
<td class="name">
Trapezoid</td>
<td class="type">string</td>
<td class="description">Shape of the datalabel will be trapezoid.</td>
</tr> 
<tr>
<td class="name">
UpArrow</td>
<td class="type">string</td>
<td class="description">Shape of the datalabel will be uparrow.</td>
</tr> 
<tr>
<td class="name">
DownArrow</td>
<td class="type">string</td>
<td class="description">Shape of the datalabel will be downarrow.</td>
</tr> 
<tr>
<td class="name">
Image</td>
<td class="type">string</td>
<td class="description">Shape of the datalabel will be image.</td>
</tr> 
<tr>
<td class="name">
SeriesType</td>
<td class="type">string</td>
<td class="description">Shape of the datalabel will be SeriesType.</td>
</tr> 

</tbody>
</table>


#### Default Value



* "none". See <a href="ejchart.html#members:commonseriesoptions-marker-datalabel-shape">Shape</a>




#### Example


{% highlight js %}
 
 
$("#container").ejChart({
commonSeriesOptions :{marker :{dataLabel :{shape : "circle"}}}                 
});
{% endhighlight %}


### commonSeriesOptions.marker.dataLabel.template `string`
{:#members:commonseriesoptions-marker-datalabel-template}




Custom template to format the data label content. Use “point.x” and “point.y” as a placeholder text to display the corresponding data point’s x and y value.


#### Default Value



* ""


#### Example


{% highlight js %}
 
 
$("#container").ejChart({
commonSeriesOptions : { marker : { dataLabel : { template : "LabelTemplateID" }}}                 
});

{% endhighlight %}


### commonSeriesOptions.marker.dataLabel.textMappingName `string`
{:#members:commonseriesoptions-marker-datalabel-textmappingname}




Name of a field in data source, where datalabel text is displayed.  


#### Default Value



* ""


#### Example


{% highlight js %}
 
 
$("#container").ejChart({
commonSeriesOptions : { marker : { dataLabel : { textMappingName : "TextFieldName" }}}                 
});

{% endhighlight %}




### commonSeriesOptions.marker.dataLabel.textPosition `enum`
{:#members:commonseriesoptions-marker-datalabel-textposition}


<ts name="ej.datavisualization.Chart.TextPosition"/>
Specifies the position of the data label. This property can be used only for the series such as column, bar, stacked column, stacked bar, 100% stacked column, 100% stacked bar, candle and OHLC.




<table class="props">
<thead>
<tr>
<th>Name</th>
<th>Type</th> 
<th class="last">Description</th>
</tr>
</thead>
<tbody>
<tr>
<td class="name">
Top</td>
<td class="type">string</td> 
<td class="description">Place the datalabel to the top of the point.</td>
</tr>
<tr>
<td class="name">
Bottom</td>
<td class="type">string</td>
<td class="description">Place the datalabel to the bottom of the point.</td>
</tr> 
<tr>
<td class="name">
Middle</td>
<td class="type">string</td>
<td class="description">Place the datalabel on the point.</td>
</tr> 
</tbody>
</table>


#### Default Value



* "top". See <a href="ejchart.html#members:series-marker-datalabel-textposition">TextPosition</a>




#### Example


{% highlight js %}
 
 
$("#container").ejChart({
commonSeriesOptions :{marker :{dataLabel :{textPosition : "bottom"}}}                 
});
{% endhighlight %}


Try it: [JS Playground  Sample](http://jsplayground.syncfusion.com/tzmb3o0y)



### commonSeriesOptions.marker.dataLabel.verticalTextAlignment `enum`
{:#members:commonseriesoptions-marker-datalabel-verticaltextalignment}


<ts name="ej.datavisualization.Chart.VerticalTextAlignment"/>
Vertical alignment of the data label. 



<table class="props">
<thead>
<tr>
<th>Name</th>
<th>Type</th> 
<th class="last">Description</th>
</tr>
</thead>
<tbody>
<tr>
<td class="name">
Center</td>
<td class="type">string</td> 
<td class="description">Place the datalabel on the point.</td>
</tr>
<tr>
<td class="name">
Near</td>
<td class="type">string</td>
<td class="description">Place the datalabel below the point.</td>
</tr> 
<tr>
<td class="name">
Far</td>
<td class="type">string</td>
<td class="description">Place the datalabel away from the point.</td>
</tr> 
</tbody>
</table>


#### Default Value



* "center"




#### Example


{% highlight js %}
 
 
$("#container").ejChart({
commonSeriesOptions :{marker :{dataLabel :{verticalTextAlignment : "far"}}}                  
});
{% endhighlight %}


Try it: [JS Playground  Sample](http://jsplayground.syncfusion.com/zro5pbw2)



### commonSeriesOptions.marker.dataLabel.visible `boolean`
{:#members:commonseriesoptions-marker-datalabel-visible}




Controls the visibility of the data labels. 


#### Default Value



* false




#### Example


{% highlight js %}
 
 
$("#container").ejChart({
commonSeriesOptions :{marker :{dataLabel :{visible : true}}                  
});
 {% endhighlight %}




### commonSeriesOptions.marker.fill `string`
{:#members:commonseriesoptions-marker-fill}




Color of the marker shape. 


#### Default Value



* null




#### Example


{% highlight js %}
 

$("#container").ejChart({
commonSeriesOptions :{marker : { fill : "green" } }                  
});
{% endhighlight %}


Try it: [JS Playground Sample](http://jsplayground.syncfusion.com/wh0gldoo)



### commonSeriesOptions.marker.imageUrl `string`
{:#members:commonseriesoptions-marker-imageurl}




The URL for the Image to be displayed as marker. In order to display image as marker, set series.marker.shape as ‘image’.


#### Default Value



* ""




#### Example


{% highlight js %}
 
 
$("#container").ejChart({
commonSeriesOptions :{marker :{ imageUrl: "../images/sample.png"}}                  
});
{% endhighlight %}


Try it: [JS Playground Sample](http://jsplayground.syncfusion.com/251niupi)



### commonSeriesOptions.marker.opacity `number`
{:#members:commonseriesoptions-marker-opacity}




Opacity of the marker. 


#### Default Value



 * 1




#### Example


{% highlight js %}
 
 
$("#container").ejChart({
commonSeriesOptions :{marker :{ opacity : 0.5 }}                  
});
{% endhighlight %}




### commonSeriesOptions.marker.shape `enum`
{:#members:commonseriesoptions-marker-shape}


<ts ref="ej.datavisualization.Chart.Shape"/>


Specifies the shape of the marker. 


#### Default Value



* "circle". See <a href="ejchart.html#members:shape">Shape</a>




#### Example


{% highlight js %}
 
 
$("#container").ejChart({
commonSeriesOptions :{marker :{ shape: "rectangle"}                  
});
{% endhighlight %}


Try it: [JS Playground Sample](http://jsplayground.syncfusion.com/wh0gldoo)



### commonSeriesOptions.marker.size `object`
{:#members:commonseriesoptions-marker-size}




Options for customizing the size of the marker shape.






### commonSeriesOptions.marker.size.height `number`
{:#members:commonseriesoptions-marker-size-height}




Height of the marker. 


#### Default Value



* 6




#### Example


{% highlight js %}
 
 
$("#container").ejChart({
commonSeriesOptions :{marker :{size :{height : 5}}}                  
});
{% endhighlight %}




### commonSeriesOptions.marker.size.width `number`
{:#members:commonseriesoptions-marker-size-width}




Width of the marker. 


#### Default Value



* 6




#### Example


{% highlight js %}
 
 
$("#container").ejChart({
commonSeriesOptions :{marker :{ size :{ width : 2 } } }                  
});
{% endhighlight %}


Try it: [JS Playground Sample](http://jsplayground.syncfusion.com/fbrqexxu)


### commonSeriesOptions.marker.visible `boolean`
{:#members:commonseriesoptions-marker-visible}




Controls the visibility of the marker shape. 


#### Default Value



* false




#### Example


{% highlight js %}
 

$("#container").ejChart({
commonSeriesOptions :{marker :{ visible : true}}                  
});
 {% endhighlight %}


Try it: [JS Playground Sample](http://jsplayground.syncfusion.com/f2qfyfbt)



### commonSeriesOptions.opacity `number`
{:#members:commonseriesoptions-opacity}




Opacity of the series.


#### Default Value



* 1




#### Example


{% highlight js %}
 
 
$("#container").ejChart({
commonSeriesOptions :{opacity : 0.5}                  
});
 {% endhighlight %}



### commonSeriesOptions.outlierSettings `object`
{:#members:commonseriesoptions-outliersettings}




Options for customizing the outlier of the series.




### commonSeriesOptions.outlierSettings.shape `enum`
{:#members:commonseriesoptions-outliersettings-shape}


<ts ref="ej.datavisualization.Chart.Shape"/>


Specifies the shape of the outlier. 


#### Default Value



* "circle". See <a href="ejchart.html#members:commonseriesoptions-outliersettings-shape">Shape</a>




#### Example


{% highlight js %}
 
 
$("#container").ejChart({
commonSeriesOptions :{outlier :{ shape: "rectangle"}                  
});
{% endhighlight %}



### commonSeriesOptions.outlierSettings.size `object`
{:#members:commonseriesoptions-outliersettings-size}




Options for customizing the size of the outlier shape.






### commonSeriesOptions.outlierSettings.size.height `number`
{:#members:commonseriesoptions-outliersettings-size-height}




Height of the outlier shape. 


#### Default Value



* 6




#### Example


{% highlight js %}
 
 
$("#container").ejChart({
commonSeriesOptions :{outlierSettings :{size :{height : 5}}}                  
});
{% endhighlight %}




### commonSeriesOptions.outlierSettings.size.width `number`
{:#members:commonseriesoptions-outliersettings-size-width}




Width of the outlier shape. 


#### Default Value



* 6




#### Example


{% highlight js %}
 
 
$("#container").ejChart({
commonSeriesOptions :{outlierSettings :{ size :{ width : 2 } } }                  
});
{% endhighlight %}




 




### commonSeriesOptions.palette `string`
{:#members:commonseriesoptions-palette}




Name of a field in data source, where the fill color for all the data points is generated.


#### Default Value



* ""




#### Example


{% highlight js %}
 
 
$("#container").ejChart({
commonSeriesOptions : { palette : "ColorFieldName" }                  
});
{% endhighlight %}




### commonSeriesOptions.pieCoefficient `number`
{:#members:commonseriesoptions-piecoefficient}




Controls the size of pie series. Value ranges from 0 to 1.


#### Default Value



* 0.8




#### Example


{% highlight js %}
 
 
$("#container").ejChart({
commonSeriesOptions :{ pieCoefficient : 1}                  
});
 {% endhighlight %}



Try it: [JS Playground Sample](http://jsplayground.syncfusion.com/yzleny3o)

### commonSeriesOptions.pieOfPieCoefficient `number`
{:#members:commonseriesoptions-pieofpiecoefficient}




Controls the size of the second pie in pieOfPie series. Value ranges from 0 to 1.


#### Default Value



* 0.6




#### Example


{% highlight js %}
 
 
$("#container").ejChart({
commonSeriesOptions :{ pieOfPieCoefficient : 1}                  
});
 {% endhighlight %}

 
### commonSeriesOptions.splitValue `string`
{:#members:commonseriesoptions-splitvalue}




Split Value of pieOfPie series.


#### Default Value



 * null



#### Example


{% highlight js %}
 
 
$("#container").ejChart({
commonSeriesOptions : [{splitValue: "40" }]                   
});
{% endhighlight %}
 
### commonSeriesOptions.gapWidth `number`
{:#members:commonseriesoptions-gapwidth}




Distance between the two pie's in pieOfPie series.


#### Default Value



 * 50




#### Example


{% highlight js %}
 
 
$("#container").ejChart({
commonSeriesOptions :{ gapWidth : 300}                  
});
  {% endhighlight %}

### commonSeriesOptions.pointColorMappingName `string`
{:#members:commonseriesoptions-pointcolormappingname}




Name of the property in the datasource that contains fill color for the series.


#### Default Value



* null




#### Example


{% highlight js %}
 
 
$("#container").ejChart({
commonSeriesOptions : {pointColorMappingName: "color" }                   
});
 {% endhighlight %}
 
 



### commonSeriesOptions.pyramidMode `enum`
{:#members:commonseriesoptions-pyramidmode}


<ts name="ej.datavisualization.Chart.PyramidMode"/>
Specifies the mode of the pyramid series. 



<table class="props">
<thead>
<tr>
<th>Name</th>
<th>Type</th> 
<th class="last">Description</th>
</tr>
</thead>
<tbody>
<tr>
<td class="name">
Linear</td>
<td class="type">string</td> 
<td class="description">Specifies the pyramid mode to linear.</td>
</tr>
<tr>
<td class="name">
Surface</td>
<td class="type">string</td>
<td class="description">Specifies the pyramid mode to surface.</td>
</tr>
</tbody>
</table>


#### Default Value



* "linear". See <a href="ejchart.html#members:commonseriesoptions-pyramidmode">PyramidMode</a>

#### Example


{% highlight js %}
 
 
$("#container").ejChart({
commonSeriesOptions :{ pyramidMode : "linear"}                  
});
 {% endhighlight %}


Try it: [JS Playground Sample](http://jsplayground.syncfusion.com/maeo3b3s)



### commonSeriesOptions.startAngle `number`
{:#members:commonseriesoptions-startangle}




Start angle from where the pie/doughnut series renders. By default it starts from 0.


#### Default Value



* null




#### Example


{% highlight js %}
 
 
$("#container").ejChart({
commonSeriesOptions :{ startAngle : 150}                  
});
 {% endhighlight %}
 

Try it: [JS Playground Sample](http://jsplayground.syncfusion.com/gposb4vh)


### commonSeriesOptions.cornerRadius `object`
{:#members:commonseriesoptions-cornerradius}




Options for customizing the corner radius. cornerRadius property also takes the numeric input and applies it for all the four corners of the column.


#### Example


{% highlight js %}
 
 
$("#container").ejChart({
commonSeriesOptions : {
             cornerRadius: 10 
    }                   
});
 {% endhighlight %} 



### commonSeriesOptions.cornerRadius.topLeft `number`
{:#members:commonseriesoptions-cornerradius-topleft}




Specifies the radius for the top left corner.



#### Default Value



 * 0




#### Example


{% highlight js %}
 
 
$("#container").ejChart({
commonSeriesOptions : {
             cornerRadius: {topLeft : 10 }
    }                   
});
 {% endhighlight %} 


### commonSeriesOptions.cornerRadius.topRight `number`
{:#members:commonseriesoptions-cornerradius-topright}




Specifies the radius for the top right corner.



#### Default Value



 * 0




#### Example


{% highlight js %}
 
 
$("#container").ejChart({
commonSeriesOptions : {
             cornerRadius: {topRight : 10 }
    }                   
});
 {% endhighlight %} 



### commonSeriesOptions.cornerRadius.bottomLeft `number`
{:#members:commonseriesoptions-cornerradius-bottomleft}




Specifies the radius for the bottom left corner.



#### Default Value



 * 0




#### Example


{% highlight js %}
 
 
$("#container").ejChart({
commonSeriesOptions : {
             cornerRadius: {bottomLeft : 10 }
    }                   
});
 {% endhighlight %} 


### commonSeriesOptions.cornerRadius.bottomRight `number`
{:#members:commonseriesoptions-cornerradius-bottomright}




Specifies the radius for the bottom right corner.



#### Default Value



 * 0




#### Example


{% highlight js %}
 
 
$("#container").ejChart({
commonSeriesOptions : {
             cornerRadius: {bottomRight : 10 }
    }                   
});
 {% endhighlight %} 



### commonSeriesOptions.tooltip `object`
{:#members:commonseriesoptions-tooltip}




Options for customizing the tooltip of chart.



### commonSeriesOptions.tooltip.border `object`
{:#members:commonseriesoptions-tooltip-border}




Options for customizing the border of the tooltip.






### commonSeriesOptions.tooltip.border.color `string`
{:#members:commonseriesoptions-tooltip-border-color}




Border color of the tooltip.


#### Default Value



* null




#### Example


{% highlight js %}
 
 
$("#container").ejChart({
commonSeriesOptions :{tooltip :{border:{ color : "green" }}}                  
});
 {% endhighlight %}




### commonSeriesOptions.tooltip.border.width `number`
{:#members:commonseriesoptions-tooltip-border-width}




Border width of the tooltip.


#### Default Value



* 1




#### Example


{% highlight js %}
 
 
$("#container").ejChart({
commonSeriesOptions :{tooltip :{border :{ width : 2}}}                  
});
  {% endhighlight %}



Try it: [JS Playground Sample](http://jsplayground.syncfusion.com/dmvqb51g)

### commonSeriesOptions.tooltip.rx `number`
{:#members:commonseriesoptions-tooltip-rx}




Customize the corner radius of the tooltip rectangle.


#### Default Value



0




#### Example


{% highlight js %}
 
 
$("#container").ejChart({
commonSeriesOptions :{tooltip :{rx: 10}}                  
});
  {% endhighlight %}



Try it: [JS Playground Sample](http://jsplayground.syncfusion.com/y4bnt0gl)


### commonSeriesOptions.tooltip.ry `number`
{:#members:commonseriesoptions-tooltip-ry}




Customize the corner radius of the tooltip rectangle.


#### Default Value



0




#### Example


{% highlight js %}
 
 
$("#container").ejChart({
commonSeriesOptions :{tooltip :{ry: 10}}                  
});
  {% endhighlight %}



Try it: [JS Playground Sample](http://jsplayground.syncfusion.com/y4bnt0gl)


### commonSeriesOptions.tooltip.duration `string`
{:#members:commonseriesoptions-tooltip-duration}




Specifies the duration, the tooltip has to be displayed.


#### Default Value



* "500ms"




#### Example


{% highlight js %}
 
 
$("#container").ejChart({
commonSeriesOptions :{tooltip :{duration : "300ms"}}                  
});
  {% endhighlight %}




### commonSeriesOptions.tooltip.enableAnimation `boolean`
{:#members:commonseriesoptions-tooltip-enableanimation}




Enables/disables the animation of the tooltip when moving from one point to other.


#### Default Value



* true




#### Example


{% highlight js %}
 
 
$("#container").ejChart({
commonSeriesOptions :{tooltip :{enableAnimation : false}}                  
});
{% endhighlight %}




### commonSeriesOptions.tooltip.fill `string`
{:#members:commonseriesoptions-tooltip-fill}




Background color of the tooltip.


#### Default Value



* null




#### Example


{% highlight js %}
 
 
$("#container").ejChart({
commonSeriesOptions :{tooltip :{fill : "green"}}                  
});
 {% endhighlight %}




### commonSeriesOptions.tooltip.format `string`
{:#members:commonseriesoptions-tooltip-format}




Format of the tooltip content.


#### Default Value



* "#point.x# : #point.y#"




#### Example


{% highlight js %}
 
 
$("#container").ejChart({
commonSeriesOptions :{ tooltip : { format : "#point.x# : #point.y#%" } }                  
});
 {% endhighlight %}



Try it: [JS Playground Sample](http://jsplayground.syncfusion.com/rzxmpi0c)



### commonSeriesOptions.tooltip.opacity `number`
{:#members:commonseriesoptions-tooltip-opacity}




Opacity of the tooltip.


#### Default Value



* 0.5




#### Example


{% highlight js %}
 
 
$("#container").ejChart({
commonSeriesOptions :{tooltip :{opacity : 0.5}}                  
});
{% endhighlight %}



Try it: [JS Playground Sample](http://jsplayground.syncfusion.com/jih5jejk)



### commonSeriesOptions.tooltip.template `string`
{:#members:commonseriesoptions-tooltip-template}




Custom template to format the tooltip content. Use “point.x” and “point.y” as a placeholder text to display the corresponding data point’s x and y value.


#### Default Value



* null




#### Example


{% highlight js %}
 <div id="item" style="display: none;"> 
    <div>
       <div>#point.x#</div>
        <div>#point.y#</div>
       </div>       
 </div>
 
$("#container").ejChart({
commonSeriesOptions :{ tooltip: { template : "item" }}                  
});
{% endhighlight %}


Try it: [JS Playground Sample](http://jsplayground.syncfusion.com/rmunfu1b)



### commonSeriesOptions.tooltip.visible `boolean`
{:#members:commonseriesoptions-tooltip-visible}




Controls the visibility of the tooltip.


#### Default Value



* false




#### Example


{% highlight js %}
 

$("#container").ejChart({
commonSeriesOptions :{ tooltip :{visible : true} }                  
});
 {% endhighlight %}


Try it: [JS Playground Sample](http://jsplayground.syncfusion.com/tpizvdt0)


### commonSeriesOptions.type `enum`
{:#members:commonseriesoptions-type}


<ts name="ej.datavisualization.Chart.Type"/>
Specifies the type of the series to render in chart. 





<table class="props">
<thead>
<tr>
<th>Name</th>
<th>Type</th> 
<th class="last">Description</th>
</tr>
</thead>
<tbody>
<tr>
<td class="name">
Area</td>
<td class="type">string</td> 
<td class="description">Specifies the series type as area.</td>
</tr>
<tr>
<td class="name">
Line</td>
<td class="type">string</td>
<td class="description">Specifies the series type as line.</td>
</tr> 
<tr>
<td class="name">
Spline</td>
<td class="type">string</td>
<td class="description">Specifies the series type as spline.</td>
</tr> 
<tr>
<td class="name">
Column</td>
<td class="type">string</td> 
<td class="description">Specifies the series type as column.</td>
</tr>
<tr>
<td class="name">
Scatter</td>
<td class="type">string</td>
<td class="description">Specifies the series type as scatter.</td>
</tr> 
<tr>
<td class="name">
Bubble</td>
<td class="type">string</td>
<td class="description">Specifies the series type as bubble.</td>
</tr> 
<tr>
<td class="name">
SplineArea</td>
<td class="type">string</td> 
<td class="description">Specifies the series type as splinearea.</td>
</tr>
<tr>
<td class="name">
StepArea</td>
<td class="type">string</td>
<td class="description">Specifies the series type as steparea.</td>
</tr> 
<tr>
<td class="name">
StepLine</td>
<td class="type">string</td>
<td class="description">Specifies the series type as stepline.</td>
</tr> 
<tr>
<td class="name">
Pie</td>
<td class="type">string</td> 
<td class="description">PSpecifies the series type as pie.</td>
</tr>
<tr>
<td class="name">
HiLo</td>
<td class="type">string</td>
<td class="description">Specifies the series type as HiLo.</td>
</tr> 
<tr>
<td class="name">
HiLoOpenClose</td>
<td class="type">string</td>
<td class="description">Specifies the series type as HiLoOpenClose.</td>
</tr> 
<tr>
<td class="name">
Candle</td>
<td class="type">string</td> 
<td class="description">Specifies the series type as candle.</td>
</tr>
<tr>
<td class="name">
Bar</td>
<td class="type">string</td>
<td class="description">Specifies the series type as bar.</td>
</tr> 
<tr>
<td class="name">
StackingArea</td>
<td class="type">string</td>
<td class="description">Specifies the series type as stackingarea.</td>
</tr> 
<tr>
<td class="name">
StackingArea100</td>
<td class="type">string</td> 
<td class="description">Specifies the series type as stackingarea100.</td>
</tr>
<tr>
<td class="name">
RangeColumn</td>
<td class="type">string</td>
<td class="description">Specifies the series type as rangecolumn.</td>
</tr> 
<tr>
<td class="name">
StackingColumn</td>
<td class="type">string</td>
<td class="description">Specifies the series type as stackingcolumn.</td>
</tr> 
<tr>
<td class="name">
StackingColumn100</td>
<td class="type">string</td> 
<td class="description">Specifies the series type as stackingcolumn100.</td>
</tr>
<tr>
<td class="name">
StackingBar</td>
<td class="type">string</td>
<td class="description">Specifies the series type as stackingbar.</td>
</tr> 
<tr>
<td class="name">
StackingBar100</td>
<td class="type">string</td>
<td class="description">Specifies the series type as stackingbar100.</td>
</tr> 
<tr>
<td class="name">
StackingSplineArea</td>
<td class="type">string</td>
<td class="description">sets the seriesType of chart to stackingSplineArea</td>
</tr>
<tr>
<td class="name">
StackingSplineArea100</td>
<td class="type">string</td>
<td class="description">sets the seriesType of chart to stackingsplinearea100</td>
</tr> 
<tr>
<td class="name">
Pyramid</td>
<td class="type">string</td> 
<td class="description">Specifies the series type as pyramid.</td>
</tr>
<tr>
<td class="name">
Funnel</td>
<td class="type">string</td>
<td class="description">Specifies the series type as funnel.</td>
</tr> 
<tr>
<td class="name">
Doughnut</td>
<td class="type">string</td>
<td class="description">Specifies the series type as doughnut.</td>
</tr> 
<tr>
<td class="name">
Polar</td>
<td class="type">string</td> 
<td class="description">Specifies the series type as polar.</td>
</tr>
<tr>
<td class="name">
Radar</td>
<td class="type">string</td>
<td class="description">Specifies the series type as radar.</td>
</tr> 
<tr>
<td class="name">
RangeArea</td>
<td class="type">string</td>
<td class="description">Specifies the series type as rangearea.</td>
</tr> 
</tbody>
</table>


#### Default Value



* "column". See <a href="ejchart.html#members:commonseriesoptions-type">Type</a>


#### Example


{% highlight js %}
 
 
$("#container").ejChart({
commonSeriesOptions :{ type : "spline"}                  
});
 {% endhighlight %}


Try it: [JS Playground Sample](http://jsplayground.syncfusion.com/iyglee55)



### commonSeriesOptions.xAxisName `string`
{:#members:commonseriesoptions-xaxisname}




Specifies the name of the x-axis that has to be associated with this series. Add an axis instance with this name to axes collection.


#### Default Value



* null




#### Example


{% highlight js %}
 
 
$("#container").ejChart({
commonSeriesOptions :{ xAxisName : "xAxis"}                  
});
 {% endhighlight %}


Try it: [JS Playground Sample](http://jsplayground.syncfusion.com/p1t424pc)


### commonSeriesOptions.xName `string`
{:#members:commonseriesoptions-xname}




Name of the property in the datasource that contains x value for the series.


#### Default Value



* null




#### Example


{% highlight js %}
 
 
$("#container").ejChart({
commonSeriesOptions : {xName: "XValue" }                   
});
 {% endhighlight %}
 
 
 Try it: [JS Playground Sample](http://jsplayground.syncfusion.com/ubbu5ukf)




### commonSeriesOptions.yAxisName `string`
{:#members:commonseriesoptions-yaxisname}




Specifies the name of the y-axis that has to be associated with this series. Add an axis instance with this name to axes collection.


#### Default Value



* null




#### Example


{% highlight js %}
 

$("#container").ejChart({
commonSeriesOptions :{ yAxisName : "yAxis"}                  
});
 {% endhighlight %}
 
 
 Try it: [JS Playground Sample](http://jsplayground.syncfusion.com/kac2fcth)



### commonSeriesOptions.yName `string`
{:#members:commonseriesoptions-yname}




Name of the property in the datasource that contains y value for the series.


#### Default Value



* null




#### Example


{% highlight js %}
 
 
$("#container").ejChart({
commonSeriesOptions :{yName: "yValue" }               
});
 {% endhighlight %}
 
 
 Try it: [JS Playground Sample](http://jsplayground.syncfusion.com/ubbu5ukf)
 
 

 
### commonSeriesOptions.high `string`
{:#members:commonseriesoptions-high}




Name of the property in the datasource that contains high value for the series.


#### Default Value



 * null




#### Example


{% highlight js %}
 
 
$("#container").ejChart({
commonSeriesOptions : {high: "high" }                  
});
{% endhighlight %}




### commonSeriesOptions.low `string`
{:#members:commonseriesoptions-low}




Name of the property in the datasource that contains low value for the series.


#### Default Value



 * null




#### Example


{% highlight js %}
 
 
$("#container").ejChart({
commonSeriesOptions : {low: "low" }                 
});
{% endhighlight %}


Try it: [JS Playground Sample](http://jsplayground.syncfusion.com/fqxo0isj)



### commonSeriesOptions.open `string`
{:#members:commonseriesoptions-open}




Name of the property in the datasource that contains open value for the series.


#### Default Value



 * null




#### Example


{% highlight js %}
 
 
$("#container").ejChart({
commonSeriesOptions : {open: "open" }                   
});
{% endhighlight %}



### commonSeriesOptions.close `string`
{:#members:commonseriesoptions-close}


Name of the property in the datasource that contains close value for the series.


#### Default Value



 * null




#### Example


{% highlight js %}
 
 
$("#container").ejChart({
commonSeriesOptions : {close: "close" }                   
});
{% endhighlight %}


Try it: [JS Playground Sample](http://jsplayground.syncfusion.com/fqxo0isj)



### commonSeriesOptions.zOrder `number`
{:#members:commonseriesoptions-zOrder}




Z-order of the series.


#### Default Value



* 0




#### Example


{% highlight js %}
 
 
$("#container").ejChart({
commonSeriesOptions :{zOrder : 1}                  
});

 {% endhighlight %}
 
 


### commonSeriesOptions.size `string`
{:#members:commonseriesoptions-size}




Name of the property in the datasource that contains the size value for the bubble series.


#### Default Value



 * null




#### Example


{% highlight js %}
 
 
$("#container").ejChart({
commonSeriesOptions : [{size: "size" }]                   
});
{% endhighlight %}


Try it: [JS Playground Sample](http://jsplayground.syncfusion.com/kf0d05wi)


### commonSeriesOptions.emptyPointSettings `object`
{:#members:commonseriesoptions-emptypointsettings}




Options for customizing the empty point in the series.


### commonSeriesOptions.emptyPointSettings.visible `boolean`
{:#members:commonseriesoptions-emptypointsettings-visible}




Controls the visibility of the empty point.



#### Default Value



 * true




#### Example


{% highlight js %}
 
 
$("#container").ejChart({
commonSeriesOptions : {
      emptyPointSettings: {

           visible : false,
       } 
    }                   
});
 {% endhighlight %}



Try it: [JS Playground Sample](http://jsplayground.syncfusion.com/hpl0ffff)


### commonSeriesOptions.emptyPointSettings.displayMode `enum`
{:#members:commonseriesoptions-emptypointsettings-displaymode}


<ts name="ej.datavisualization.Chart.EmptyPointMode"/>
Specifies the mode of empty point.



<table class="props">
<thead>
<tr>
<th>Name</th>
<th>Type</th> 
<th class="last">Description</th>
</tr>
</thead>
<tbody>
<tr>
<td class="name">
Gap</td>
<td class="type">string</td> 
<td class="description">Display the gap for empty point.</td>
</tr>
<tr>
<td class="name">
Zero</td>
<td class="type">string</td>
<td class="description">Set zero has empty point value.</td>
</tr> 
<tr>
<td class="name">
Average</td>
<td class="type">string</td>
<td class="description">Set the average of the adjacent point to empty point.</td>
</tr> 
</tbody>
</table>



#### Default Value



 * "gap"




#### Example


{% highlight js %}
 
 
$("#container").ejChart({
commonSeriesOptions : {
      emptyPointSettings: {

           displayMode : "gap",
       } 
    }                   
});
 {% endhighlight %}
 
See [Mode](https://help.syncfusion.com/api/js/global#members:mode). 

 
### commonSeriesOptions.emptyPointSettings.style `object`
{:#members:commonseriesoptions-emptypointsettings-style}




Options for customizing the color and border of the empty point in the series.


### commonSeriesOptions.emptyPointSettings.style.color `string`
{:#members:commonseriesoptions-emptypointsettings-style-color}




Color of the empty point.



#### Default Value



 * ""




#### Example


{% highlight js %}
 
 
$("#container").ejChart({
commonSeriesOptions : {
      emptyPointSettings: {

           style: { color : "red" }
       } 
    }                   
});
 {% endhighlight %}
 
 
### commonSeriesOptions.emptyPointSettings.style.border `object`
{:#members:commonseriesoptions-emptypointsettings-style-border}




Options for customizing border of the empty point in the series.
 

### commonSeriesOptions.emptyPointSettings.style.border.color `string`
{:#members:commonseriesoptions-emptypointsettings-style-border-color}




Border color of the empty point.



#### Default Value



 * ""




#### Example


{% highlight js %}
 
 
$("#container").ejChart({
commonSeriesOptions : {
      emptyPointSettings: {

           style: { border: { color : "red" } }
       } 
    }                   
});
 {% endhighlight %}
 

### commonSeriesOptions.emptyPointSettings.style.border.width `number`
{:#members:commonseriesoptions-emptypointsettings-style-border-color}




Border width of the empty point.



#### Default Value



 * 1




#### Example


{% highlight js %}
 
 
$("#container").ejChart({
commonSeriesOptions : {
      emptyPointSettings: {

           style: { border: { width : 1.2 } }
       } 
    }                   
});
 {% endhighlight %}
 

 
### commonSeriesOptions.positiveFill `string`
{:#members:commonseriesoptions-positivefill}




Fill color for the positive column of the waterfall.



#### Default Value



 * null




#### Example


{% highlight js %}
 
 
$("#container").ejChart({
      commonSeriesOptions : {
                positiveFill : “Red”
    }                   
});
 {% endhighlight %}     
 
 Try it: [JS Playground Sample](http://jsplayground.syncfusion.com/t5dhe5d0)
 
 
### commonSeriesOptions.connectorLine `object`
{:#members:commonseriesoptions-connectorline}




Options for customizing the waterfall connector line.

Try it: [JS Playground Sample](http://jsplayground.syncfusion.com/t5dhe5d0)


### commonSeriesOptions.connectorLine.width `number`
{:#members:commonseriesoptions-connectorline-width}




Width of the connector line.



#### Default Value



 * 1




#### Example


{% highlight js %}
 
 
$("#container").ejChart({
commonSeriesOptions : {
             connectorLine: {width : 1 }
    }                   
});
 {% endhighlight %} 
 

### commonSeriesOptions.connectorLine.color `string`
{:#members:commonseriesoptions-connectorline-color}




Color of the connector line.



#### Default Value



 * "#565656"




#### Example


{% highlight js %}
 
 
$("#container").ejChart({
    commonSeriesOptions : {
             connectorLine: {color : "grey" }
    }                   
});
 {% endhighlight %} 
 
 

### commonSeriesOptions.connectorLine.dashArray `string`
{:#members:commonseriesoptions-connectorline-dasharray}




DashArray of the connector line.



#### Default Value



 * null




#### Example


{% highlight js %}
 
 
$("#container").ejChart({
    commonSeriesOptions : {
             connectorLine: {dashArray : "2,3" }
    }                   
});
 {% endhighlight %} 
 



### commonSeriesOptions.connectorLine.opacity `number`
{:#members:commonseriesoptions-connectorline-opacity}




DashArray of the connector line.



#### Default Value



 * 1




#### Example


{% highlight js %}
 
 
$("#container").ejChart({
    commonSeriesOptions : {
             connectorLine: {opacity : 0.5 }
    }                   
});
 {% endhighlight %} 


### commonSeriesOptions.dragSettings `object`
{:#members:commonseriesoptions-dragsettings}

Options to customize the drag and drop in series.

### commonSeriesOptions.dragSettings.enable `boolean`
{:#members:commonseriesoptions-dragsettings-enable}

drag/drop the series

#### Default Value

* "false"

#### Example


{% highlight js %}
 
 
$("#container").ejChart({
    commonSeriesOptions : {
          dragSettings:{enable: true}
    }                   
});

 {% endhighlight %} 

### commonSeriesOptions.dragSettings.type `string`
{:#members:commonseriesoptions-dragsettings-type}


Specifies the type of drag settings.


#### Default Value


* "xy"

#### Example


{% highlight js %}
 
 
$("#container").ejChart({
    commonSeriesOptions : {
          dragSettings:{type: "x"}
    }                   
});
 {% endhighlight %} 
 


### commonSeriesOptions.errorBar `object`
{:#members:commonseriesoptions-errorbar}


Options to customize the error bar in series.


### commonSeriesOptions.errorBar.visibility `boolean`
{:#members:commonseriesoptions-errorbar-visibility}


Show/hides the error bar

#### Default Value



 * "visible"




#### Example


{% highlight js %}
 
 
$("#container").ejChart({
    commonSeriesOptions : {
          errorBar:{visibility: "hidden"}
    }                   
});
 {% endhighlight %} 
 
 
 Try it: [JS Playground Sample](http://jsplayground.syncfusion.com/t5dhe5d0) 
   
### commonSeriesOptions.errorBar.type `enum`
{:#members:commonseriesoptions-errorbar-type}

<ts name="ej.datavisualization.Chart.ErrorBarType"/>
Specifies the type of error bar.



<table class="props">
<thead>
<tr>
<th>Name</th>
<th>Type</th> 
<th class="last">Description</th>
</tr>
</thead>
<tbody>
<tr>
<td class="name">
FixedValue</td>
<td class="type">string</td> 
<td class="description">Set the type of the error bar as FixedValue.</td>
</tr>
<tr>
<td class="name">
Percentage</td>
<td class="type">string</td>
<td class="description">Set the type of the error bar as Percentage.</td>
</tr> 
<tr>
<td class="name">
StandardDeviation</td>
<td class="type">string</td>
<td class="description">Set the type of the error bar as StandardDeviation.</td>
</tr> 
<tr>
<td class="name">
StandardError</td>
<td class="type">string</td>
<td class="description">Set the type of the error bar as StandardError.</td>
</tr> 
</tbody>
</table>

#### Default Value



 * "FixedValue"




#### Example


{% highlight js %}
 
 
$("#container").ejChart({
    commonSeriesOptions : {
          errorBar:{type: "Percentage"}
    }                   
});
 {% endhighlight %} 
 
 Try it: [JS Playground Sample](http://jsplayground.syncfusion.com/t5dhe5d0) 
 
### commonSeriesOptions.errorBar.mode `enum`
{:#members:commonseriesoptions-errorbar-mode}
 
<ts name="ej.datavisualization.Chart.ErrorBarMode"/>
Specifies the mode of error bar.



<table class="props">
<thead>
<tr>
<th>Name</th>
<th>Type</th> 
<th class="last">Description</th>
</tr>
</thead>
<tbody>
<tr>
<td class="name">
Both</td>
<td class="type">string</td> 
<td class="description">Place the annotation to the top of the chart.</td>
</tr>
<tr>
<td class="name">
Vertical</td>
<td class="type">string</td>
<td class="description">Place the annotation to the bottom of the chart.</td>
</tr> 
<tr>
<td class="name">
Horizontal</td>
<td class="type">string</td>
<td class="description">Place the annotation to the middle of the chart.</td>
</tr> 
</tbody>
</table>

#### Default Value



 * "vertical"




#### Example


{% highlight js %}
 
 
$("#container").ejChart({
    commonSeriesOptions : {
          errorBar:{mode: "Horizontal"}
    }                   
});
 {% endhighlight %} 
 
 Try it: [JS Playground Sample](http://jsplayground.syncfusion.com/t5dhe5d0) 
 

### commonSeriesOptions.errorBar.direction `enum`
{:#members:commonseriesoptions-errorbar-direction}


<ts name="ej.datavisualization.Chart.ErrorBarDirection"/>
Specifies the direction of error bar.




<table class="props">
<thead>
<tr>
<th>Name</th>
<th>Type</th> 
<th class="last">Description</th>
</tr>
</thead>
<tbody>
<tr>
<td class="name">
Both</td>
<td class="type">string</td> 
<td class="description">Set the direction to both.</td>
</tr>
<tr>
<td class="name">
Plus</td>
<td class="type">string</td>
<td class="description">Set the direction to plus.</td>
</tr> 
<tr>
<td class="name">
Minus</td>
<td class="type">string</td>
<td class="description">Set the direction to minus.</td>
</tr> 
</tbody>
</table>

#### Default Value



 * "both"




#### Example


{% highlight js %}
 
 
$("#container").ejChart({
    commonSeriesOptions : {
          errorBar:{direction: "plus"}
    }                   
});
 {% endhighlight %} 
 
 Try it: [JS Playground Sample](http://jsplayground.syncfusion.com/t5dhe5d0) 
 

### commonSeriesOptions.errorBar.verticalErrorValue `number`
{:#members:commonseriesoptions-errorbar-verticalerrorvalue}


Value of vertical error bar.

#### Default Value



 * 3




#### Example


{% highlight js %}
 
 
$("#container").ejChart({
    commonSeriesOptions : {
          errorBar:{verticalErrorValue: 1}
    }                   
});
 {% endhighlight %} 
 
Try it: [JS Playground Sample](http://jsplayground.syncfusion.com/t5dhe5d0) 

### commonSeriesOptions.errorBar.horizontalErrorValue `number`
{:#members:commonseriesoptions-errorbar-horizontalerrorvalue}


Value of horizontal  error bar.

#### Default Value



 * 1




#### Example


{% highlight js %}
 
 
$("#container").ejChart({
    commonSeriesOptions : {
          errorBar:{horizontalErrorValue: 1}
    }                   
});
 {% endhighlight %} 
 
Try it: [JS Playground Sample](http://jsplayground.syncfusion.com/t5dhe5d0) 


### commonSeriesOptions.errorBar.horizontalPositiveErrorValue `number`
{:#members:commonseriesoptions-errorbar-horizontalpositiveerrorvalue}


Value of positive horizontal error bar.

#### Default Value



 * 1




#### Example


{% highlight js %}
 
 
$("#container").ejChart({
    commonSeriesOptions : {
          errorBar:{horizontalPositiveErrorValue: 1}
    }                   
});
 {% endhighlight %} 
 
Try it: [JS Playground Sample](http://jsplayground.syncfusion.com/t5dhe5d0) 



### commonSeriesOptions.errorBar.horizontalNegativeErrorValue `number`
{:#members:commonseriesoptions-errorbar-horizontalnegativeerrorvalue}


Value of negative horizontal error bar.

#### Default Value



 * 1




#### Example


{% highlight js %}
 
 
$("#container").ejChart({
    commonSeriesOptions : {
          errorBar:{horizontalNegativeErrorValue: 1}
    }                   
});
 {% endhighlight %} 
 
Try it: [JS Playground Sample](http://jsplayground.syncfusion.com/t5dhe5d0) 


### commonSeriesOptions.errorBar.verticalPositiveErrorValue `number`
{:#members:commonseriesoptions-errorbar-verticalpositiveerrorvalue}


Value of positive vertical error bar.

#### Default Value



 * 5




#### Example


{% highlight js %}
 
 
$("#container").ejChart({
    commonSeriesOptions : {
          errorBar:{verticalPositiveErrorValue: 1}
    }                   
});
 {% endhighlight %} 
 
Try it: [JS Playground Sample](http://jsplayground.syncfusion.com/t5dhe5d0) 



### commonSeriesOptions.errorBar.verticalNegativeErrorValue `number`
{:#members:commonseriesoptions-errorbar-verticalnegativeerrorvalue}


Value of negative vertical error bar.

#### Default Value



 * 5




#### Example


{% highlight js %}
 
 
$("#container").ejChart({
    commonSeriesOptions : {
          errorBar:{verticalNegativeErrorValue: 1}
    }                   
});
 {% endhighlight %} 
 
Try it: [JS Playground Sample](http://jsplayground.syncfusion.com/t5dhe5d0) 


### commonSeriesOptions.errorBar.fill `string`
{:#members:commonseriesoptions-errorbar-fill}


Fill color of the error bar.

#### Default Value



 * "#000000"




#### Example


{% highlight js %}
 
 
$("#container").ejChart({
    commonSeriesOptions : {
        errorBar:{       
           fill:”red”
        }

    }                   
});
 {% endhighlight %} 
 
Try it: [JS Playground Sample](http://jsplayground.syncfusion.com/t5dhe5d0) 
    

### commonSeriesOptions.errorBar.width `number`
{:#members:commonseriesoptions-errorbar-width}


Width of the error bar.

#### Default Value



 * 1




#### Example


{% highlight js %}
 
 
$("#container").ejChart({
    commonSeriesOptions : {
        errorBar:{       
           width: 1
        }

    }                   
});
 {% endhighlight %} 



### commonSeriesOptions.errorBar.cap `object`
{:#members:commonseriesoptions-errorbar-cap}


Options for customizing the error bar cap.

Try it: [JS Playground Sample](http://jsplayground.syncfusion.com/t5dhe5d0) 


### commonSeriesOptions.errorBar.cap.visible `boolean`
{:#members:commonseriesoptions-errorbar-cap-visible}

Show/Hides the error bar cap.

#### Default Value



 * true




#### Example


{% highlight js %}
 
 
$("#container").ejChart({
    commonSeriesOptions : {
       errorBar:{       
         cap:{visible:false}
        }
    }s                   
});
 {% endhighlight %} 
 

### commonSeriesOptions.errorBar.cap.width `number`
{:#members:commonseriesoptions-errorbar-cap-width}

Width of the error bar cap.

#### Default Value



 * 1




#### Example


{% highlight js %}
 
 
$("#container").ejChart({
    commonSeriesOptions : {
       errorBar:{       
         cap:{width:1}
        }
    }                   
});
 {% endhighlight %} 
 
 
 
### commonSeriesOptions.errorBar.cap.length `number`
{:#members:commonseriesoptions-errorbar-cap-length}

Length of the error bar cap.

#### Default Value



 * 1




#### Example


{% highlight js %}
 
 
$("#container").ejChart({
    commonSeriesOptions : {
       errorBar:{       
         cap:{length: 10}
        }
    }                   
});
 {% endhighlight %} 
 

### commonSeriesOptions.errorBar.cap.fill `string`
{:#members:commonseriesoptions-errorbar-cap-fill}

Color of the error bar cap.

#### Default Value



 *  “#000000”




#### Example


{% highlight js %}
 
 
$("#container").ejChart({
    commonSeriesOptions :{
       errorBar:{       
         cap:{fill: “red”}
        }
    }                   
});
 {% endhighlight %} 


### commonSeriesOptions.trendlines `array`
{:#members:commonseriesoptions-trendlines}




Option to add the trendlines to chart.




### commonSeriesOptions.trendlines.visibility `boolean`
{:#members:commonseriesoptions-trendlines-visibility}




Show/hides the trendline.


#### Default Value



* ""




#### Example


{% highlight js %}
 
 
$("#container").ejChart({
commonSeriesOptions :{trendlines:[{ visibility:'visible' }]}                 
});
{% endhighlight %}



### commonSeriesOptions.trendlines.visibleOnLegend `string`
{:#members:commonseriesoptions-trendlines-visibleonlegend}


Show/hides the trendline legend.


#### Default Value



* visible




#### Example


{% highlight js %}
 
 
$("#container").ejChart({
commonSeriesOptions :[{trendlines:[{ visibleOnLegend:'hidden' }]}]                  
});
{% endhighlight %}



### commonSeriesOptions.trendlines.type `enum`
{:#members:commonseriesoptions-trendlines-type}


<ts name="ej.datavisualization.Chart.TrendlinesType"/>

Specifies the type of the trendline for the series.

<table class="props">
<thead>
<tr>
<th>Name</th>
<th>Type</th> 
<th class="last">Description</th>
</tr>
</thead>
<tbody>
<tr>
<td class="name">
Linear</td>
<td class="type">string</td> 
<td class="description">Specifies the trendline type as linear.</td>
</tr>
<tr>
<td class="name">
Exponential</td>
<td class="type">string</td>
<td class="description">Specifies the trendline type as exponential.</td>
</tr> 
<tr>
<td class="name">
Logarithmic</td>
<td class="type">string</td>
<td class="description">Specifies the trendline type as logarithmic.</td>
</tr> 
<tr>
<td class="name">
Power</td>
<td class="type">string</td>
<td class="description">Specifies the trendline type as power.</td>
</tr>
<tr>
<td class="name">
Polynomial</td>
<td class="type">string</td>
<td class="description">Specifies the trendline type as polynomial.</td>
</tr>
</tbody>
</table>


#### Default Value



* "linear". See <a href="ejchart.html#members:commonseriesoptions-trendlines-type">TrendlinesType</a>




#### Example


{% highlight js %}
 
 
$("#container").ejChart({
commonSeriesOptions :{trendlines:[{ type:'linear' }]}                 
});
{% endhighlight %}



### commonSeriesOptions.trendlines.name `string`
{:#members:commonseriesoptions-trendlines-name}




Name for the trendlines that is to be displayed in the legend text.


#### Default Value



* "trendline"



#### Example


{% highlight js %}
 
 
$("#container").ejChart({
commonSeriesOptions :{trendlines:[{ name:'Trendline' }]}                  
});
{% endhighlight %}




### commonSeriesOptions.trendlines.fill `string`
{:#members:commonseriesoptions-trendlines-fill}




Fill color of the trendlines.


#### Default Value



* "#0000FF"



#### Example


{% highlight js %}
 
 
$("#container").ejChart({
commonSeriesOptions :{trendlines:[{ fill:'#0000FF' }]}                 
});
{% endhighlight %}




### commonSeriesOptions.trendlines.width `number`
{:#members:commonseriesoptions-trendlines-width}




Width of the trendlines.


#### Default Value



* 1



#### Example


{% highlight js %}
 
 
$("#container").ejChart({
commonSeriesOptions :{trendlines:[{ width:1 }]}                
});
{% endhighlight %}



### commonSeriesOptions.trendlines.opacity `number`
{:#members:commonseriesoptions-trendlines-opacity}




Opacity of the trendline.


#### Default Value



* 1



#### Example


{% highlight js %}
 
 
$("#container").ejChart({
commonSeriesOptions :{trendlines:[{ opacity:1 }]}                 
});
{% endhighlight %}




### commonSeriesOptions.trendlines.dashArray `string`
{:#members:commonseriesoptions-trendlines-dasharray}




Pattern of dashes and gaps used to stroke the trendline.


#### Default Value



* ""



#### Example


{% highlight js %}
 
 
$("#container").ejChart({
commonSeriesOptions :{trendlines:[{ dashArray:"" }]}                 
});
{% endhighlight %}



### commonSeriesOptions.trendlines.forwardForecast `number`
{:#members:commonseriesoptions-trendlines-forwardforecast}




Future trends of the current series.


#### Default Value



* 0



#### Example


{% highlight js %}
 
 
$("#container").ejChart({
commonSeriesOptions :{trendlines:[{ forwardForeCast:2 }]}                 
});
{% endhighlight %}



### commonSeriesOptions.trendlines.backwardForecast `number`
{:#members:commonseriesoptions-trendlines-backwardforecast}




Past trends of the current series.


#### Default Value



* 0



#### Example


{% highlight js %}
 
 
$("#container").ejChart({
commonSeriesOptions :{trendlines:[{ backwardForeCast:2 }]}                
});
{% endhighlight %}

Try it: [JS Playground Sample](http://jsplayground.syncfusion.com/d5o0dk1l)



### commonSeriesOptions.trendlines.polynomialOrder `number`
{:#members:commonseriesoptions-trendlines-polynomialorder}




Specifies the order of the polynomial trendlines.


#### Default Value



* 0



#### Example


{% highlight js %}
 
 
$("#container").ejChart({
commonSeriesOptions :{trendlines:[{ polynomialOrder:2 }]}             
});
{% endhighlight %}

Try it: [JS Playground Sample](http://jsplayground.syncfusion.com/opxwgddc)


### commonSeriesOptions.trendlines.period `number`
{:#members:commonseriesoptions-trendlines-period}




Specifies the moving average starting period value.


#### Default Value



* 2



#### Example


{% highlight js %}
 
 
$("#container").ejChart({
commonSeriesOptions :{trendlines:[{ period: 3 }]}             
});
{% endhighlight %}

Try it: [JS Playground Sample](http://jsplayground.syncfusion.com/opxwgddc)


### commonSeriesOptions.trendlines.tooltip `object`
{:#members:commonseriesoptions-trendlines-tooltip}




Options for customizing the tooltip of the trendlines in the chart.


### commonSeriesOptions.trendlines.tooltip.border `object`
{:#members:commonseriesoptions-trendlines-tooltip-border}




Options for customizing the border of the  trendline tooltip.




### commonSeriesOptions.trendlines.tooltip.border.color `string`
{:#members:commonseriesoptions-trendlines-tooltip-border-color}




Border color of the trendline tooltip.


#### Default Value



* null




#### Example


{% highlight js %}
 
 
$("#container").ejChart({        
commonSeriesOptions :[{ trendlines:[{ tooltip :{border:{ color : "green" }} }]}]                  
});
 {% endhighlight %}




### commonSeriesOptions.trendlines.tooltip.border.width `number`
{:#members:commonseriesoptions-trendlines-tooltip-border-width}




Border width of the trendline tooltip.


#### Default Value



* 1




#### Example


{% highlight js %}
 
 
$("#container").ejChart({
commonSeriesOptions :[{ trendlines:[{ tooltip :{border:{  width : 2 }} }]}]                   
});
  {% endhighlight %}



Try it: [JS Playground Sample](http://jsplayground.syncfusion.com/dmvqb51g)



### commonSeriesOptions.trendlines.tooltip.rx `number`
{:#members:commonseriesoptions-trendlines-tooltip-rx}




Customize the corner radius of the trendline tooltip rectangle.


#### Default Value



0




#### Example


{% highlight js %}
 
 
$("#container").ejChart({
commonSeriesOptions :[{ trendlines:[{ tooltip :{rx: 10} }]}]                  
});
  {% endhighlight %}



Try it: [JS Playground Sample](http://jsplayground.syncfusion.com/y4bnt0gl)


### commonSeriesOptions.trendlines.tooltip.ry `number`
{:#members:commonseriesoptions-trendlines-tooltip-ry}




Customize the corner radius of the trendline tooltip rectangle.


#### Default Value



0




#### Example


{% highlight js %}
 
 
$("#container").ejChart({
commonSeriesOptions :[{ trendlines:[{ tooltip :{ry: 10} }]}]                  
});
  {% endhighlight %}



Try it: [JS Playground Sample](http://jsplayground.syncfusion.com/y4bnt0gl)



### commonSeriesOptions.trendlines.tooltip.duration `string`
{:#members:commonseriesoptions-trendlines-tooltip-duration}




Specifies the duration, the tooltip has to be displayed.


#### Default Value



* "500ms"




#### Example


{% highlight js %}
 
 
$("#container").ejChart({
commonSeriesOptions :[{ trendlines:[{ tooltip :{duration : "300ms"} }]}]                   
});
  {% endhighlight %}



### commonSeriesOptions.trendlines.tooltip.enableAnimation `boolean`
{:#members:commonseriesoptions-trendlines-tooltip-enableanimation}




Enables/disables the animation of the trendline tooltip when moving from one point to other.


#### Default Value



* true




#### Example


{% highlight js %}
 
 
$("#container").ejChart({
commonSeriesOptions :[{ trendlines:[{ tooltip :{enableAnimation : false} }]}]                   
});
{% endhighlight %}



### commonSeriesOptions.trendlines.tooltip.fill `string`
{:#members:commonseriesoptions-trendlines-tooltip-fill}




Background color of the trendline tooltip.


#### Default Value



* null




#### Example


{% highlight js %}
 
 
$("#container").ejChart({
commonSeriesOptions :[{ trendlines:[{ tooltip :{fill : "green"} }]}]                   
});
 {% endhighlight %}



### commonSeriesOptions.trendlines.tooltip.format `string`
{:#members:commonseriesoptions-trendlines-tooltip-format}




Format of the tooltip content displayed in the trendlines.


#### Default Value



* "#point.x# : #point.y#"




#### Example


{% highlight js %}
 
 
$("#container").ejChart({
commonSeriesOptions :[{ trendlines:[{ tooltip :{format : "#point.x# : #point.y#%"} }]}]                  
});
 {% endhighlight %}



Try it: [JS Playground Sample](http://jsplayground.syncfusion.com/rzxmpi0c)



### commonSeriesOptions.trendlines.tooltip.opacity `number`
{:#members:commonseriesoptions-trendlines-tooltip-opacity}





Opacity of the trendline tooltip.


#### Default Value



* 0.5




#### Example


{% highlight js %}
 
 
$("#container").ejChart({
commonSeriesOptions :[{ trendlines:[{ tooltip :{opacity : 0.5} }]}]                 
});
{% endhighlight %}


### commonSeriesOptions.trendlines.intercept `number`
{:#members:commonseriesoptions-trendlines-intercept}





Specifies the intercept value of the trendlines.


#### Default Value



* null




#### Example


{% highlight js %}
 
 
$("#container").ejChart({
commonSeriesOptions :{ trendlines:[{ intercept : 10 }]}                 
});
{% endhighlight %}



### commonSeriesOptions.highlightSettings `object`
{:#members:commonseriesoptions-highlightsettings}




Options for customizing the appearance of the series or data point while highlighting.




### commonSeriesOptions.highlightSettings.enable `boolean`
{:#members:commonseriesoptions-highlightsettings-enable}




Enables/disables the ability to highlight the series or data point interactively.


#### Default Value



* false




#### Example


{% highlight js %}
 
 
$("#container").ejChart({
commonSeriesOptions :{highlightSettings:{enable:true}}                  
});
{% endhighlight %}



### commonSeriesOptions.highlightSettings.mode `enum`
{:#members:commonseriesoptions-highlightsettings-mode}


<ts name="ej.datavisualization.Chart.Mode"/>
Specifies whether the series or data point has to be highlighted.


<table class="props">
<thead>
<tr>
<th>Name</th>
<th>Type</th> 
<th class="last">Description</th>
</tr>
</thead>
<tbody>
<tr>
<td class="name">
Series</td>
<td class="type">string</td> 
<td class="description">Highlight/Select the series of the chart.</td>
</tr>
<tr>
<td class="name">
Point</td>
<td class="type">string</td>
<td class="description">Highlight/Select the point in the series.</td>
</tr> 
<tr>
<td class="name">
Cluster</td>
<td class="type">string</td>
<td class="description">Highlight/Select the points all series of same index.</td>
</tr> 
<tr>
<td class="name">
Range</td>
<td class="type">string</td>
<td class="description">Select the data points by mouse dragging in the chart area.</td>
</tr> 
</tbody>
</table>


#### Default Value



* "series". See <a href="ejchart.html#members:commonseriesoptions-highlightsettings-mode">Mode</a>




#### Example


{% highlight js %}
 
 
$("#container").ejChart({
commonSeriesOptions :{highlightSettings:{mode:"point"}}                  
});
{% endhighlight %}



### commonSeriesOptions.highlightSettings.color `string`
{:#members:commonseriesoptions-highlightsettings-color}




Color of the series/point on highlight.


#### Default Value



* ""

 

#### Example


{% highlight js %}
 
 
$("#container").ejChart({
commonSeriesOptions :{highlightSettings:{color:"red"}}                  
});
{% endhighlight %}



### commonSeriesOptions.highlightSettings.opacity `number`
{:#members:commonseriesoptions-highlightsettings-opacity}




Opacity of the series/point on highlight.


#### Default Value



* 0.6

 

#### Example


{% highlight js %}
 
 
$("#container").ejChart({
commonSeriesOptions :{highlightSettings:{opacity:1}}               
});
{% endhighlight %}



### commonSeriesOptions.highlightSettings.border `object`
{:#members:commonseriesoptions-highlightsettings-border}



Options for customizing the border of series on highlight.



### commonSeriesOptions.highlightSettings.border.color `string`
{:#members:commonseriesoptions-highlightsettings-border-color}



Border color of the series/point on highlight.


#### Default Value



* ""

 

#### Example


{% highlight js %}
 
 
$("#container").ejChart({
commonSeriesOptions :{highlightSettings:{border:{color:"black"}}}                 
});
{% endhighlight %}



### commonSeriesOptions.highlightSettings.border.width `string`
{:#members:commonseriesoptions-highlightsettings-border-width}



Border width of the series/point on highlight.


#### Default Value



* 2

 

#### Example


{% highlight js %}
 
 
$("#container").ejChart({
commonSeriesOptions :{highlightSettings:{border:{width:1}}}                  
});
{% endhighlight %}


Try it: [JS Playground Sample](http://jsplayground.syncfusion.com/rppilz5a)


### commonSeriesOptions.highlightSettings.pattern `string`
{:#members:commonseriesoptions-highlightsettings-pattern}




Specifies the pattern for the series/point on highlight.

#### Default Value



* "none". See <a href="global.html#members:pattern">Pattern</a>

 

#### Example


{% highlight js %}
 
 
$("#container").ejChart({
commonSeriesOptions :{highlightSettings:{pattern:"chessboard"}}                  
});
{% endhighlight %}


Try it: [JS Playground Sample](http://jsplayground.syncfusion.com/e31yyof2)



### commonSeriesOptions.highlightSettings.customPattern `string`
{:#members:commonseriesoptions-highlightsettings-custompattern}




Custom pattern for the series on highlight.

#### Default Value



* ""

 

#### Example


{% highlight js %}
 
 
$("#container").ejChart({
commonSeriesOptions :{highlightSettings:{customPattern:""}}                  
});
{% endhighlight %}


Try it: [JS Playground Sample](http://jsplayground.syncfusion.com/ecgabpa5)



### commonSeriesOptions.selectionSettings `object`
{:#members:commonseriesoptions.selectionsettings}




Options for customizing the appearance of the series/data point on selection.



### commonSeriesOptions.selectionSettings.enable `boolean`
{:#members:commonseriesoptions-selectionsettings-enable}




Enables/disables the ability to select a series/data point interactively.


#### Default Value



* false




#### Example


{% highlight js %}
 
 
$("#container").ejChart({
commonSeriesOptions :{selectionSettings:{enable:true}}                  
});
{% endhighlight %}


### commonSeriesOptions.selectionSettings.type `enum`
{:#members:commonseriesoptions-selectionsettings-type}

<ts name="ej.datavisualization.Chart.SelectionType"/>
Specifies the type of selection.


<table class="props">
<thead>
<tr>
<th>Name</th>
<th>Type</th>
<th class="last">Description</th>
</tr>
</thead>
<tbody>
<tr>
<td class="name">
Single</td>
<td class="type">string</td>
<td class="description">It will be select the single series / point of the chart.</td>
</tr>
<tr>
<td class="name">
Multiple</td>
<td class="type">string</td>
<td class="description">It will be select the multiple series / point of the chart.</td>
</tr>
</tbody>
</table>

#### Default Value


* "single"

See. [Type](https://help.syncfusion.com/api/js/global.html#LabelPosition)
 

#### Example


{% highlight js %}
 
 
$("#container").ejChart({ 
commonSeriesOptions:{
  selectionSettings:{
              type : 'multiple'
             }
	}
  }); 

{% endhighlight %}


### commonSeriesOptions.selectionSettings.mode `enum`
{:#members:commonseriesoptions-selectionsettings-mode}



<ts ref="ej.datavisualization.Chart.Mode"/>


Specifies whether the series or data point has to be selected.


#### Default Value



* "series". See <a href="ejchart.html#members:commonseriesoptions-highlightsettings-mode">Mode</a>




#### Example


{% highlight js %}
 
 
$("#container").ejChart({
commonSeriesOptions :{selectionSettings:{mode:"point"}}                  
});
{% endhighlight %}

Try it: [JS Playground Sample](http://jsplayground.syncfusion.com/yghrxu21)




### commonSeriesOptions.selectionSettings.rangeType `enum`
{:#members:commonseriesoptions-selectionsettings-rangetype}

<ts name="ej.datavisualization.Chart.RangeType"/>
Specifies the drawn rectangle type.


<table class="props">
<thead>
<tr>
<th>Name</th>
<th>Type</th>
<th class="last">Description</th>
</tr>
</thead>
<tbody>
<tr>
<td class="name">
XY</td>
<td class="type">string</td>
<td class="description">It will be draw a range rectangle in both horizontal and vertically.</td>
</tr>
<tr>
<td class="name">
X</td>
<td class="type">string</td>
<td class="description">It will be draw a range rectangle in horizontally.</td>
</tr>
<tr>
<td class="name">
Y</td>
<td class="type">string</td>
<td class="description">It will be draw a range rectangle in vertically.</td>
</tr>
</tbody>
</table>

#### Default Value



* "xy" 

#### Example


{% highlight js %}
 
 
$("#container").ejChart({
     commonSeriesOptions: [{
      selectionSettings:{
              rangeType : 'x'
             }
	  }]
  }); 

{% endhighlight %}


### commonSeriesOptions.selectionSettings.color `string`
{:#members:commonseriesoptions-selectionsettings-color}




Color of the series/point on selection.


#### Default Value



* ""

 

#### Example


{% highlight js %}
 
 
$("#container").ejChart({
commonSeriesOptions :{selectionSettings:{color:"red"}}                  
});
{% endhighlight %}



### commonSeriesOptions.selectionSettings.opacity `number`
{:#members:commonseriesoptions-selectionsettings-opacity}




Opacity of the series/point on selection.


#### Default Value



* 0.6

 

#### Example


{% highlight js %}
 
 
$("#container").ejChart({
commonSeriesOptions:{selectionSettings:{opacity:1}}                  
});
{% endhighlight %}


### commonSeriesOptions.selectionSettings.border `object`
{:#members:commonseriesoptions-selectionsettings-border}



Options for customizing the border of the series on selection.



### commonSeriesOptions.selectionSettings.border.color `string`
{:#members:commonseriesoptions-selectionsettings-border-color}



Border color of the series/point on selection.


#### Default Value



* ""

 

#### Example


{% highlight js %}
 
 
$("#container").ejChart({
commonSeriesOptions :{selectionSettings:{border:{color:"black"}}}                 
});
{% endhighlight %}



### commonSeriesOptions.selectionSettings.border.width `string`
{:#members:commonseriesoptions-selectionsettings-border-width}



Border width of the series/point on selection.


#### Default Value



* 2

 

#### Example


{% highlight js %}
 
 
$("#container").ejChart({
commonSeriesOptions :{selectionSettings:{border:{width:1}}}                  
});
{% endhighlight %}



### commonSeriesOptions.selectionSettings.pattern `string`
{:#members:commonseriesoptions-selectionsettings-pattern}




Specifies the pattern for the series/point on selection.

#### Default Value



* "none". See <a href="global.html#members:pattern">Pattern</a>

 

#### Example


{% highlight js %}
 
 
$("#container").ejChart({
commonSeriesOptions :{selectionSettings:{pattern:"chessboard"}}                  
});
{% endhighlight %}


Try it: [JS Playground Sample](http://jsplayground.syncfusion.com/zbipilg5)


### commonSeriesOptions.selectionSettings.customPattern `string`
{:#members:commonseriesoptions-selectionsettings-custompattern}



Custom pattern for the series on selection.

#### Default Value



* ""

 

#### Example


{% highlight js %}
 
 
$("#container").ejChart({
commonSeriesOptions :{selectionSettings:{customPattern:""}}                  
});
{% endhighlight %}


Try it: [JS Playground Sample](http://jsplayground.syncfusion.com/ne1iit3s)


### selectedDataPointIndexes `array`
{:#members:selecteddatapointindexes}

Options for displaying the chart along with selected points while loading 

#### Default Value

* [ ]

#### Example

{% highlight js %}
 
$("#container").ejChart({

  selectedDataPointIndexes: [
               { seriesIndex:0 , pointIndex:2 },
               { seriesIndex:1 , pointIndex:4 }
           ],     

});

{% endhighlight %}


Try it: [JS Playground Sample](http://jsplayground.syncfusion.com/b3oj1nlt)

### crosshair `object`
{:#members:crosshair}




Options for displaying and customizing the crosshair.



### crosshair.trackballTooltipSettings `object`
{:#members:crosshair-trackballtooltipsettings}

Options for customizing the trackball tooltip.

### crosshair.trackballTooltipSettings.border `object`
{:#members:crosshair-trackballtooltipsettings-border}

Options for customizing the trackball tooltip border.


### crosshair.trackballTooltipSettings.border.width `number`
{:#members:crosshair-trackballtooltipsettings-border-width}

Border width of the trackball tooltip.

#### Default Value

* null

#### Example

{% highlight js %}
 
$("#container").ejChart({

   crosshair : { trackballTooltipSettings : { border : { width :2 } } }              

});

{% endhighlight %}


### crosshair.trackballTooltipSettings.border.color `string`
{:#members:crosshair-trackballtooltipsettings-border-color}

Border color of the trackball tooltip.

#### Default Value

* null

#### Example

{% highlight js %}
 
$("#container").ejChart({

   crosshair : { trackballTooltipSettings : { border : { color :"red" } } }              

});

{% endhighlight %}



### crosshair.trackballTooltipSettings.fill `string`
{:#members:crosshair-trackballtooltipsettings-fill}

Background color of the trackball tooltip.

#### Default Value

* null

#### Example

{% highlight js %}
 
$("#container").ejChart({

   crosshair : { trackballTooltipSettings : { fill :"red"  } }              

});

{% endhighlight %}



### crosshair.trackballTooltipSettings.rx `number`
{:#members:crosshair-trackballtooltipsettings-rx}

Rounded corner x value of the trackball tooltip.

#### Default Value

* 3

#### Example

{% highlight js %}
 
$("#container").ejChart({

   crosshair : { trackballTooltipSettings : { rx : 5  } }              

});

{% endhighlight %}


### crosshair.trackballTooltipSettings.ry `number`
{:#members:crosshair-trackballtooltipsettings-ry}

Rounded corner y value of the trackball tooltip.

#### Default Value

* 3

#### Example

{% highlight js %}
 
$("#container").ejChart({

   crosshair : { trackballTooltipSettings : { ry : 5  } }              

});

{% endhighlight %}


### crosshair.trackballTooltipSettings.opacity `number`
{:#members:crosshair-trackballtooltipsettings-opacity}

Opacity value of the trackball tooltip.

#### Default Value

* 1

#### Example

{% highlight js %}
 
$("#container").ejChart({

   crosshair : { trackballTooltipSettings : { opacity : 0.5  } }              

});

{% endhighlight %}


### crosshair.trackballTooltipSettings.mode `enum`
{:#members:crosshair-trackballtooltipsettings-mode}

<ts name="ej.datavisualization.Chart.CrosshairMode"/>
Specifies the mode of the trackball tooltip.


<table class="props">
<thead>
<tr>
<th>Name</th>
<th>Type</th> 
<th class="last">Description</th>
</tr>
</thead>
<tbody>
<tr>
<td class="name">
Float</td>
<td class="type">string</td> 
<td class="description">Shown the trackball tooltip as float mode.</td>
</tr>
<tr>
<td class="name">
Grouping</td>
<td class="type">string</td>
<td class="description">Shown the trackball tooltip as grouping mode.</td>
</tr> 
</tbody>
</table>


#### Default Value

* "float". See <a href="ejchart.html#members:crosshair-trackballtooltipsettings-mode">CrosshairMode</a>

#### Example


{% highlight js %}
 
$("#container").ejChart({

   crosshair : { trackballTooltipSettings : { mode : 'grouping'  } }              

});

{% endhighlight %}




### crosshair.marker `object`
{:#members:crosshair-marker}




Options for customizing the marker in crosshair.






### crosshair.marker.border `object`
{:#members:crosshair-marker-border}




Options for customizing the border.






### crosshair.marker.border.width `number`
{:#members:crosshair-marker-border-width}




Border width of the marker.


#### Default Value

* 3




#### Example


{% highlight js %}
 
$("#container").ejChart({

   crosshair : { marker : { border : { width :2 } } }              

});

{% endhighlight %}




### crosshair.marker.opacity `boolean`
{:#members:crosshair-marker-opacity}




Opacity of the marker.


#### Default Value

* true




#### Example


{% highlight js %}
 
$("#container").ejChart({

   crosshair :{marker :{opacity :2}}              

});

{% endhighlight %}




### crosshair.marker.size `object`
{:#members:crosshair-marker-size}




Options for customizing the size of the marker.






### crosshair.marker.size.height `number`
{:#members:crosshair-marker-size-height}




Height of the marker.


#### Default Value

* 10




#### Example


{% highlight js %}
 
$("#container").ejChart({

   crosshair :{marker :{size :{ height :15 }}}              

});

{% endhighlight %}




### crosshair.marker.size.width `number`
{:#members:crosshair-marker-size-width}




Width of the marker.


#### Default Value

* 10




#### Example


{% highlight js %}
 
$("#container").ejChart({

   crosshair :{marker :{size : {width :15}}}              

});

{% endhighlight %}




### crosshair.marker.visible `boolean`
{:#members:crosshair-marker-visible}




Show/hides the marker.


#### Default Value

* true




#### Example


{% highlight js %}
 
$("#container").ejChart({

   crosshair :{marker :{visible :false}}              

});

{% endhighlight %}


Try it: [JS Playground Sample](http://jsplayground.syncfusion.com/hfja2bta)




### crosshair.line `object`
{:#members:crosshair-line}




Options for customizing the crosshair line.






### crosshair.line.color `string`
{:#members:crosshair-line-color}




Color of the crosshair line.
 


#### Default Value

* "transparent"




#### Example


{% highlight js %}
 
$("#container").ejChart({

   crosshair : { line : { color "red" } }              

});

{% endhighlight %}


### crosshair.line.width `number`
{:#members:crosshair-line-width}




Width of the crosshair line.
 


#### Default Value

* 1




#### Example


{% highlight js %}
 
$("#container").ejChart({

   crosshair : { line : { width: 2 } }              

});

{% endhighlight %}





 



### crosshair.type `enum`
{:#members:crosshair-type}

<ts name="ej.datavisualization.Chart.CrosshairType"/>
Specifies the type of the crosshair. It can be trackball or crosshair

<table class="props">
<thead>
<tr>
<th>Name</th>
<th>Type</th> 
<th class="last">Description</th>
</tr>
</thead>
<tbody>
<tr>
<td class="name">
Crosshair</td>
<td class="type">string</td> 
<td class="description">View the value of an axis at mouse position.</td>
</tr>
<tr>
<td class="name">
Trackball</td>
<td class="type">string</td>
<td class="description">Track a data point close to the mouse position.</td>
</tr> 
</tbody>
</table>


#### Default Value

* "crosshair". See <a href="ejchart.html#members:crosshair-type">CrosshairType</a>




#### Example


{% highlight js %}
 
$("#container").ejChart({

   crosshair :{type : "trackball"}              

});

{% endhighlight %}




### crosshair.visible `boolean`
{:#members:crosshair-visible}




Show/hides the crosshair/trackball visibility.


#### Default Value

* false




#### Example


{% highlight js %}
 
$("#container").ejChart({

   crosshair :{visible :true}              

});

{% endhighlight %}


Try it: [JS Playground Sample](http://jsplayground.syncfusion.com/31w3q03j)




### depth `number`
{:#members:depth}




Depth of the 3D Chart from front view of series to background wall. This property is applicable only for 3D view.


#### Default Value



* 100




#### Example

{% highlight js %}


$("#container").ejChart({

    depth : 100
                
});

{% endhighlight %}

Try it: [JS Playground Sample](http://jsplayground.syncfusion.com/mfcep44t)

### enable3D `boolean`
{:#members:enable3d}




Controls whether 3D view has to be enabled or not. 3D view is supported only for column, bar. Stacking column, stacking bar, pie and doughnut series types.


#### Default Value



* false




#### Example

{% highlight js %}


$("#container").ejChart({

        enable3D : true
                     
});

{% endhighlight %}

Try it: [JS Playground Sample](http://jsplayground.syncfusion.com/dx0nj11k)




### enableCanvasRendering `boolean`
{:#members:enablecanvasrendering}




Controls whether Chart has to be rendered as Canvas or SVG. Canvas rendering supports all functionalities in SVG rendering except 3D Charts.


#### Default Value

* false




#### Example


{% highlight js %}
 
$("#container").ejChart({

   enableCanvasRendering : true             

});

{% endhighlight %}


Try it: [JS Playground Sample](http://jsplayground.syncfusion.com/2nvdn2ml)



### initSeriesRender `boolean`
{:#members:initseriesrender}




Controls whether the series has to be rendered at initial loading of chart, this will be useful in scenarios where chart is placed at the bottom of the web page and we need to render the series only when the chart is visible while scrolling to the top.


#### Default Value



* true




#### Example


{% highlight js %}
 

$("#container").ejChart({

     initSeriesRender : false
                  
});

{% endhighlight %}


### enableRotation `boolean`
{:#members:enablerotation}




Controls whether 3D view has to be rotated on dragging. This property is applicable only for 3D view.


#### Default Value



* false




#### Example


{% highlight js %}
 

$("#container").ejChart({

     enableRotation : true
                  
});

{% endhighlight %}


Try it: [JS Playground Sample](http://jsplayground.syncfusion.com/hf5wopxp)


### indicators `array`
{:#members:indicators}




Options to customize the technical indicators.






### indicators.dPeriod `number`
{:#members:indicators-dperiod}




The dPeriod value for stochastic indicator.


#### Default Value



* 3




#### Example


{% highlight js %}
 
$("#container").ejChart({

      indicators :[{ dPeriod : 4}]
                    
});

{% endhighlight %}


Try it: [JS Playground Sample](http://jsplayground.syncfusion.com/hnfnqsqd)


### indicators.enableAnimation `boolean`
{:#members:indicators-enableanimation}




Enables/disables the animation.


#### Default Value



* false




#### Example


{% highlight js %}
 
$("#container").ejChart({

     indicators :[{ enableAnimation :  true}]
                    
});

{% endhighlight %}

Try it: [JS Playground Sample](http://jsplayground.syncfusion.com/p443wnjd)

### indicators.animationDuration `boolean`
{:#members:indicators-animationduration}

Specifies animation duration for indicator rendering.

#### Default Value

* null

#### Example


{% highlight js %}
$("#container").ejChart({

     indicators :[{ animationDuration:2000}]
});

{% endhighlight %}

### indicators.fill `string`
{:#members:indicators-fill}




Color of the technical indicator.


#### Default Value



* "#00008B"




#### Example


{% highlight js %}
 
$("#container").ejChart({

    indicators :[{ fill : "#ff0000"}]
                    
});

{% endhighlight %}

Try it: [JS Playground Sample](http://jsplayground.syncfusion.com/vrm2umdf)


### indicators.histogram `object`
{:#members:indicators-histogram}




Options to customize the histogram in MACD indicator.






### indicators.histogram.border `object`
{:#members:indicators-histogram-border}




Options to customize the histogram border in MACD indicator.


Try it: [JS Playground Sample](http://jsplayground.syncfusion.com/stbnoy0x)



### indicators.histogram.border.color `string`
{:#members:indicators-histogram-border-color}




Color of the histogram border in MACD indicator.


#### Default Value


* "#9999ff"



#### Example


{% highlight js %}

$("#container").ejChart({

    indicators :[{ histogram : {border: {color: "#ff0000"}}}]
                        
});

{% endhighlight %}




### indicators.histogram.border.width `number`
{:#members:indicators-histogram-border-width}




Controls the width of histogram border line in MACD indicator.


#### Default Value



* 1




#### Example


{% highlight js %}

$("#container").ejChart({
 
    indicators :[{ histogram : {border: {width: 2}}}]
                        
});

{% endhighlight %}




### indicators.histogram.fill `string`
{:#members:indicators-histogram-fill}




Color of histogram columns in MACD indicator.


#### Default Value



* "#ccccff"




#### Example


{% highlight js %}

$("#container").ejChart({

    indicators :[{ histogram : {fill: "#ff0000"}}]
                        
});

{% endhighlight %}

Try it: [JS Playground Sample](http://jsplayground.syncfusion.com/2rvadgmd)


### indicators.histogram.opacity `number`
{:#members:indicators-histogram-opacity}




Opacity of histogram columns in MACD indicator.


#### Default Value



* 1




#### Example


{% highlight js %}

$("#container").ejChart({

    indicators :[{ histogram : {opacity: 0.5}}]
                        
});

{% endhighlight %}




### indicators.kPeriod `number`
{:#members:indicators-kperiod}




Specifies the k period in stochastic indicator.


#### Default Value



* 3




#### Example


{% highlight js %}

$("#container").ejChart({

    indicators :[{ kPeriod : 4}]
                        
});

{% endhighlight %}




### indicators.longPeriod `number`
{:#members:indicators-longperiod}




Specifies the long period in MACD indicator.


#### Default Value



* 26




#### Example


{% highlight js %}

$("#container").ejChart({

    indicators :[{ longPeriod :  14"}]
                        
});

{% endhighlight %}




### indicators.lowerLine `object`
{:#members:indicators-lowerline}




Options to customize the lower line in indicators.






### indicators.lowerLine.fill `string`
{:#members:indicators-lowerline-fill}




Color of lower line.


#### Default Value



* "#008000"




#### Example


{% highlight js %}

$("#container").ejChart({

     indicators :[{ lowerLine : {fill: "#ff0000"}}]
                         
});

{% endhighlight %}




### indicators.lowerLine.width `number`
{:#members:indicators-lowerline-width}




Width of the lower line.


#### Default Value



* 2




#### Example


{% highlight js %}

$("#container").ejChart({

     indicators :[{ lowerLine : {width: 3}}]
                         
});

{% endhighlight %}




### indicators.macdLine `object`
{:#members:indicators-macdline}




Options to customize the MACD line.

Try it: [JS Playground Sample](http://jsplayground.syncfusion.com/oarmpbow)




### indicators.macdLine.fill `string`
{:#members:indicators-macdline-fill}




Color of MACD line.


#### Default Value



* "#ff9933"




#### Example


{% highlight js %}

$("#container").ejChart({

    indicators :[{ macdLine : {fill: "#ff0000"}}]
                        
});

{% endhighlight %}




### indicators.macdLine.width `number`
{:#members:indicators-macdline-width}




Width of the MACD line.


#### Default Value



* 2




#### Example


{% highlight js %}

$("#container").ejChart({

     indicators :[{ macdLine : {width: 3}}]
                         
});

{% endhighlight %}




### indicators.macdType `string`
{:#members:indicators-macdtype}




Specifies the type of the MACD indicator. 


#### Default Value



* "line". See <a href="global.html#members:macdtype">MACDType</a>




#### Example


{% highlight js %}

$("#container").ejChart({

    indicators :[{ macdType :  "both"}]
                        
});

{% endhighlight %}




### indicators.period `number`
{:#members:indicators-period}




Specifies period value in indicator.


#### Default Value



* 14




#### Example


{% highlight js %}

$("#container").ejChart({

    indicators :[{ period : 20}]
                        
});

{% endhighlight %}

Try it: [JS Playground Sample](http://jsplayground.syncfusion.com/yk3njhr1)


### indicators.periodLine `object`
{:#members:indicators-periodline}




Options to customize the period line in indicators.

Try it: [JS Playground Sample](http://jsplayground.syncfusion.com/20dlmyxk)




### indicators.periodLine.fill `string`
{:#members:indicators-periodline-fill}




Color of period line in indicator.


#### Default Value



* "blue"




#### Example


{% highlight js %}

$("#container").ejChart({

    indicators :[{ periodLine : {fill: "#ff0000"}}]
                        
});

{% endhighlight %}




### indicators.periodLine.width `number`
{:#members:indicators-periodline-width}




Width of the period line in indicators.


#### Default Value



* 2




#### Example


{% highlight js %}

$("#container").ejChart({

    indicators :[{ periodLine : {width: 3}}]
                        
});

{% endhighlight %}




### indicators.seriesName `string`
{:#members:indicators-seriesname}




Name of the series for which indicator has to be drawn.


#### Default Value



* ""




#### Example


{% highlight js %}

$("#container").ejChart({

    indicators :[{ seriesName : "rsi"}]
                        
});

{% endhighlight %}

Try it: [JS Playground Sample](http://jsplayground.syncfusion.com/yk3njhr1)


### indicators.shortPeriod `number`
{:#members:indicators-shortperiod}




Specifies the short period in MACD indicator.


#### Default Value



* 13




#### Example


{% highlight js %}

$("#container").ejChart({

     indicators :[{ shortPeriod :  14"}]
                         
});

{% endhighlight %}

Try it: [JS Playground Sample](http://jsplayground.syncfusion.com/2hpibxjj)


### indicators.standardDeviations `number`
{:#members:indicators-standarddeviations}




Specifies the standard deviation value for Bollinger band indicator.


#### Default Value



* 2




#### Example


{% highlight js %}

$("#container").ejChart({
    
     indicators :[{ standardDeviations : 3}]
                         
});

{% endhighlight %}

Try it: [JS Playground Sample](http://jsplayground.syncfusion.com/0b04ckwl)


### indicators.tooltip `object`
{:#members:indicators-tooltip}




Options to customize the tooltip.

Try it: [JS Playground Sample](http://jsplayground.syncfusion.com/ritlgl5w)




### indicators.tooltip.border `object`
{:#members:indicators-tooltip-border}




Option to customize the border of indicator tooltip.






### indicators.tooltip.border.color `string`
{:#members:indicators-tooltip-border-color}




Border color of indicator tooltip.


#### Default Value



* null




#### Example


{% highlight js %}

$("#container").ejChart({

       indicators :[{ tooltip :{border : { color :"#0000ff"}} }]
                             
});

{% endhighlight %}




### indicators.tooltip.border.width `number`
{:#members:indicators-tooltip-border-width}




Border width of indicator tooltip.


#### Default Value



* 1




#### Example


{% highlight js %}

$("#container").ejChart({

     indicators :[{ tooltip :{border : { width :2}} }]
                         
});

{% endhighlight %}




### indicators.tooltip.duration `string`
{:#members:indicators-tooltip-duration}




Specifies the animation duration of indicator tooltip.


#### Default Value



* "500ms"




#### Example


{% highlight js %}

$("#container").ejChart({

    indicators :[{ tooltip :{duration : "300ms"}}]
                        
});

{% endhighlight %}




### indicators.tooltip.enableAnimation `boolean`
{:#members:indicators-tooltip-enableanimation}




Enables/disables the tooltip animation.


#### Default Value



* true




#### Example


{% highlight js %}

$("#container").ejChart({
 
        indicators :[{ tooltip :{enableAnimation : false}}]
                            
});

{% endhighlight %}




### indicators.tooltip.format `string`
{:#members:indicators-tooltip-format}




Format of indicator tooltip. Use “point.x” and “point.y” as a placeholder text to display the corresponding data point’s x and y value.


#### Default Value



* "#point.x# : #point.y#"




#### Example


{% highlight js %}

$("#container").ejChart({

     indicators :[{ tooltip :{format : "#point.x#"}}]
                         
});

{% endhighlight %}




### indicators.tooltip.fill `string`
{:#members:indicators-tooltip-fill}




Background color of indicator tooltip.


#### Default Value



* null




#### Example


{% highlight js %}

$("#container").ejChart({

    indicators :[{ tooltip :{fill : "#FFF000"}}]
                        
});

{% endhighlight %}




### indicators.tooltip.opacity `number`
{:#members:indicators-tooltip-opacity}




Opacity of indicator tooltip.


#### Default Value



* 0.95




#### Example


{% highlight js %}

$("#container").ejChart({

    indicators :[{ tooltip :{opacity : 0.5}}]
                        
});

{% endhighlight %}




### indicators.tooltip.visible `boolean`
{:#members:indicators-tooltip-visible}




Controls the visibility of indicator tooltip.


#### Default Value



* false




#### Example


{% highlight js %}

$("#container").ejChart({

    indicators :[{ tooltip :{visible : true}}]
                        
});

{% endhighlight %}




### indicators.trigger `number`
{:#members:indicators-trigger}




Trigger value of MACD indicator.


#### Default Value



* 9




#### Example


{% highlight js %}

$("#container").ejChart({

    indicators :[{ trigger :  14}]
                        
});

{% endhighlight %}

Try it: [JS Playground Sample](http://jsplayground.syncfusion.com/nrh5tk4z)


### indicators.visibility `string`
{:#members:indicators-trigger}




Specifies the visibility of indicator.


#### Default Value



* "visible"




#### Example


{% highlight js %}

$("#container").ejChart({

     indicators :[{ visibility :  "visible"}]
                         
});

{% endhighlight %}

Try it: [JS Playground Sample](http://jsplayground.syncfusion.com/gshculgi)


### indicators.type `string`
{:#members:indicators-type}




Specifies the type of indicator that has to be rendered.


#### Default Value



* "sma". See <a href="global.html#members:indicatorstype">IndicatorsType</a>




#### Example


{% highlight js %}

$("#container").ejChart({

     indicators :[{ type : "momentum"}]
                         
});

{% endhighlight %}

Try it: [JS Playground Sample](http://jsplayground.syncfusion.com/mr4ykv5i)


### indicators.upperLine `object`
{:#members:indicators-upperline}




Options to customize the upper line in indicators

Try it: [JS Playground Sample](http://jsplayground.syncfusion.com/duskfkix)




### indicators.upperLine.fill `string`
{:#members:indicators-upperline-fill}




Fill color of the upper line in indicators


#### Default Value



* "#ff9933"




#### Example


{% highlight js %}

$("#container").ejChart({

     indicators :[{ upperLine : {fill: "#ff0000"}}]
                         
});

{% endhighlight %}




### indicators.upperLine.width `number`
{:#members:indicators-upperline-width}




Width of the upper line in indicators.


#### Default Value



* 2




#### Example


{% highlight js %}

$("#container").ejChart({

     indicators :[{ upperLine : {width: 3}}]
                         
});

{% endhighlight %}




### indicators.width `number`
{:#members:indicators-width}




Width of the indicator line.


#### Default Value



* 2




#### Example


{% highlight js %}

$("#container").ejChart({

     indicators :[{ width :  3}]
                         
});

{% endhighlight %}

Try it: [JS Playground Sample](http://jsplayground.syncfusion.com/r23e0yrp)


### indicators.xAxisName `string`
{:#members:indicators-xaxisname}




Name of the horizontal axis used for indicator. Primary X axis is used when x axis name is not specified.


#### Default Value



* ""




#### Example


{% highlight js %}

$("#container").ejChart({
    
      indicators :[{ xAxisName :  "xAxis"}]
                          
});

{% endhighlight %}

Try it: [JS Playground Sample](http://jsplayground.syncfusion.com/kksyu40s)


### indicators.yAxisName `string`
{:#members:indicators-yaxisname}




Name of the vertical axis used for indicator. Primary Y axis is used when y axis name is not specified


#### Default Value



* ""




#### Example


{% highlight js %}

$("#container").ejChart({
 
    indicators :[{ yAxisName :  "yAxis"}]
                        
});

{% endhighlight %}

### isResponsive `boolean`
{:#members:isresponsive}




Controls whether Chart has to be responsive while resizing.


#### Default Value

* false




#### Example


{% highlight js %}
 
$("#container").ejChart({

   isResponsive : true             

});

{% endhighlight %}


Try it: [JS Playground Sample](http://jsplayground.syncfusion.com/1dkyopq5)


### legend `object`
{:#members:legend}




Options to customize the legend items and legend title.






### legend.alignment `enum`
{:#members:legend-alignment}

<ts name="ej.datavisualization.Chart.Alignment"/>
Horizontal alignment of the legend.


<table class="props">
<thead>
<tr>
<th>Name</th>
<th>Type</th> 
<th class="last">Description</th>
</tr>
</thead>
<tbody>
<tr>
<td class="name">
Center</td>
<td class="type">string</td> 
<td class="description"> Align the legend as center to the chart</td>
</tr>
<tr>
<td class="name">
Near</td>
<td class="type">string</td>
<td class="description"> Align the legend as near to the chart</td>
</tr> 
<tr>
<td class="name">
Far</td>
<td class="type">string</td>
<td class="description"> Align the legend as far to the chart</td>
</tr> 
</tbody>
</table>

#### Default Value

* "Center". See <a href="ejchart.html#members:legend-alignment">Alignment</a>




#### Example


{% highlight js %}
 
$("#container").ejChart({

   legend :{alignment : "far"}                    

});

{% endhighlight %}


Try it: [JS Playground Sample](http://jsplayground.syncfusion.com/jpcc441l)




### legend.background `string`
{:#members:legend-background}




Background for the legend. Use this property to add a background image or background color for the legend.


#### Default Value

* ""




#### Example


{% highlight js %}
 
$("#container").ejChart({

   legend :{ background : "green url('flower.png')"}                    

});

{% endhighlight %}


Try it: [JS Playground Sample](http://jsplayground.syncfusion.com/yesrbzgh)




### legend.border `object`
{:#members:legend-border}




Options for customizing the legend border.


Try it: [JS Playground Sample](http://jsplayground.syncfusion.com/zob1c5er)




### legend.border.color `string`
{:#members:legend-border-color}




Border color of the legend.


#### Default Value

* "transparent"




#### Example


{% highlight js %}
 
$("#container").ejChart({

   legend : {border :{ color :"green"}}                     

});

{% endhighlight %}




### legend.border.width `number`
{:#members:legend-border-width}




Border width of the legend.


#### Default Value

* 1




#### Example


{% highlight js %}
 
$("#container").ejChart({

   legend :{ border :{width :2}}                     

});

{% endhighlight %}




### legend.columnCount `number`
{:#members:legend-columncount}




Number of columns to arrange the legend items.


#### Default Value

* null




#### Example


{% highlight js %}
 
$("#container").ejChart({

   legend :{ columnCount : 2}                    

});

{% endhighlight %}


Try it: [JS Playground Sample](http://jsplayground.syncfusion.com/g3p1ocgh)




### legend.enableScrollbar `boolean`
{:#members:legend-enablescrollbar}




Controls whether legend has to use scrollbar or not. When enabled, scroll bar appears depending upon size and position properties of legend.


#### Default Value

* true




#### Example


{% highlight js %}
 
$("#container").ejChart({

   legend :{ enableScrollbar : false}                    

});

{% endhighlight %}


Try it: [JS Playground Sample](http://jsplayground.syncfusion.com/3budcknt)




### legend.fill `string`
{:#members:legend-fill}




Fill color for the legend items. By using this property, it displays all legend item shapes in same color. 
Legend items representing invisible series is displayed in gray color.


#### Default Value

* null




#### Example


{% highlight js %}
 
$("#container").ejChart({

   legend :{ fill : "green"}                    

});

{% endhighlight %}


Try it: [JS Playground Sample](http://jsplayground.syncfusion.com/3alytf20)




### legend.font `object`
{:#members:legend-font}




Options to customize the font used for legend item text.


Try it: [JS Playground Sample](http://jsplayground.syncfusion.com/jo5t2d4u)




### legend.font.fontFamily `string`
{:#members:legend-font-fontfamily}




Font family for legend item text.


#### Default Value

* "Segoe UI"




#### Example


{% highlight js %}
 
$("#container").ejChart({

   legend :{ font :{fontFamily : "Algerian"}}                    

});

{% endhighlight %}




### legend.font.fontStyle `enum`
{:#members:legend-font-fontstyle}

<ts ref="ej.datavisualization.Chart.FontStyle"/>


Font style for legend item text.


#### Default Value

* "Normal". See <a href="global.html#enum:fontstyle">FontStyle</a>




#### Example


{% highlight js %}
 
$("#container").ejChart({

   legend :{ font :{fontStyle : "italic"}}                    

});

{% endhighlight %}




### legend.font.fontWeight `enum`
{:#members:legend-font-fontweight}

<ts ref="ej.datavisualization.Chart.FontWeight"/>


Font weight for legend item text.


#### Default Value

* "Regular". See <a href="global.html#enum:fontweight">FontWeight</a>




#### Example


{% highlight js %}
 
$("#container").ejChart({

   legend :{ font :{fontWeight : "lighter"}}                    

});

{% endhighlight %}




### legend.font.size `string`
{:#members:legend-font-size}




Font size for legend item text.


#### Default Value

* "12px"




#### Example


{% highlight js %}
 
$("#container").ejChart({

   legend :{ font :{size : "14px"}}                    

});

{% endhighlight %}




### legend.itemPadding `number`
{:#members:legend-itempadding}




Gap or padding between the legend items.


#### Default Value

* 10




#### Example


{% highlight js %}
 
$("#container").ejChart({

   legend :{itemPadding : 5}                     

});

{% endhighlight %}


Try it: [JS Playground Sample](http://jsplayground.syncfusion.com/tozzsrit)




### legend.itemStyle `object`
{:#members:legend-itemstyle}




Options to customize the style of legend items.






### legend.itemStyle.border `object`
{:#members:legend-itemstyle-border}




Options for customizing the border of legend items.


Try it: [JS Playground Sample](http://jsplayground.syncfusion.com/hplwwoll)




### legend.itemStyle.border.color `string`
{:#members:legend-itemstyle-border-color}




Border color of the legend items.


#### Default Value

* "transparent"




#### Example


{% highlight js %}
 
$("#container").ejChart({

   legend :{ itemStyle :{border : { color : "green' }}}                    

});

{% endhighlight %}




### legend.itemStyle.border.width `number`
{:#members:legend-itemstyle-border-width}




Border width of the legend items.


#### Default Value

* 1




#### Example


{% highlight js %}
 
$("#container").ejChart({

   legend :{ itemStyle :{border :{ width : 2 }}}                    

});

{% endhighlight %}




### legend.itemStyle.height `number`
{:#members:legend-itemstyle-height}




Height of the shape in legend items.


#### Default Value

* 10




#### Example


{% highlight js %}
 
$("#container").ejChart({

   legend :{ itemStyle :{height : 20}}                    

});

{% endhighlight %}




### legend.itemStyle.width `number`
{:#members:legend-itemstyle-width}




Width of the shape in legend items.


#### Default Value

* 10




#### Example


{% highlight js %}
 
$("#container").ejChart({

   legend :{ itemStyle :{width : 15}}                    

});

{% endhighlight %}




### legend.location `object`
{:#members:legend-location}




Options to customize the location of chart legend. Legend is placed in provided location only when value of **position** property is **custom**


Try it: [JS Playground Sample](http://jsplayground.syncfusion.com/xurqtijv)




### legend.location.x `number`
{:#members:legend-location-x}




X value or horizontal offset to position the legend in chart.


#### Default Value

* 0




#### Example


{% highlight js %}
 
$("#container").ejChart({

   legend :{location :{x :20}}                    

});

{% endhighlight %}




### legend.location.y `number`
{:#members:legend-location-y}




Y value or vertical offset to position the legend.


#### Default Value

* 0




#### Example


{% highlight js %}
 
$("#container").ejChart({

   legend :{location : {y : 100}}                  

});

{% endhighlight %}




### legend.opacity `number`
{:#members:legend-opacity}




Opacity of the legend.


#### Default Value

* 1




#### Example


{% highlight js %}
 
$("#container").ejChart({

   legend :{ opacity : 0.5}                    

});

{% endhighlight %}


Try it: [JS Playground Sample](http://jsplayground.syncfusion.com/nlewhk5r)




### legend.position `enum`
{:#members:legend-position}

<ts name="ej.datavisualization.Chart.Position"/>
Places the legend at specified position. Legend can be placed at **left**, **right**, **top** or **bottom** of the chart area. 
To manually specify the location of legend, set **custom** as value to this property.


<table class="props">
<thead>
<tr>
<th>Name</th>
<th>Type</th> 
<th class="last">Description</th>
</tr>
</thead>
<tbody>
<tr>
<td class="name">
Left</td>
<td class="type">string</td> 
<td class="description">Legend will be placed left side of the chart area</td>
</tr>
<tr>
<td class="name">
Right</td>
<td class="type">string</td>
<td class="description">Legend will be placed right side of the chart area</td>
</tr> 
<tr>
<td class="name">
Top</td>
<td class="type">string</td>
<td class="description">Legend will be placed top of the chart area</td>
</tr> 
<tr>
<td class="name">
Bottom</td>
<td class="type">string</td>
<td class="description">Legend will be placed bottom of the chart area</td>
</tr> 
</tbody>
</table>


#### Default Value

* "Bottom". See <a href="ejchart.html#members:legend-position">Position</a>




#### Example


{% highlight js %}
 
$("#container").ejChart({

   legend :{ position : "top"}                    

});

{% endhighlight %}


Try it: [JS Playground Sample](http://jsplayground.syncfusion.com/dwcvfzuv)




### legend.rowCount `number`
{:#members:legend-rowcount}




Number of rows to arrange the legend items.


#### Default Value

* null




#### Example


{% highlight js %}
 
$("#container").ejChart({

   legend :{ rowCount :2}                    

});

{% endhighlight %}


Try it: [JS Playground Sample](http://jsplayground.syncfusion.com/tovkgqw5)




### legend.shape `enum`
{:#members:legend-shape}

<ts ref="ej.datavisualization.Chart.Shape"/>



Shape of the legend items. Default shape for pie and doughnut series is circle and all other series uses rectangle.


#### Default Value

* "None". See <a href="ejchart.html#members:legend-shape">Shape</a>




#### Example


{% highlight js %}
 
$("#container").ejChart({

   legend :{ shape : "circle" }                      

});

{% endhighlight %}


Try it: [JS Playground Sample](http://jsplayground.syncfusion.com/uq3eho3v)




### legend.size `object`
{:#members:legend-size}




Options to customize the size of the legend.


Try it: [JS Playground Sample](http://jsplayground.syncfusion.com/tovkgqw5)




### legend.size.height `string`
{:#members:legend-size-height}




Height of the legend. Height can be specified in either pixel or percentage.


#### Default Value

* null




#### Example


{% highlight js %}
 
$("#container").ejChart({

   legend :{ size :{height : "20%"}}                    

});

{% endhighlight %}




### legend.size.width `string`
{:#members:legend-size-width}




Width of the legend. Width can be specified in either pixel or percentage.


#### Default Value

* null




#### Example


{% highlight js %}
 
$("#container").ejChart({

   legend :{ size :{width : "20%"}}                    

});

{% endhighlight %}




### legend.title `object`
{:#members:legend-title}




Options to customize the legend title.






### legend.title.font `object`
{:#members:legend-title-font}




Options to customize the font used for legend title


Try it: [JS Playground Sample](http://jsplayground.syncfusion.com/bkgyatau)




### legend.title.font.fontFamily `string`
{:#members:legend-title-font-fontfamily}




Font family for the text in legend title.


#### Default Value

* "Segoe UI"




#### Example


{% highlight js %}
 
$("#container").ejChart({

   legend: { title: { font :{fontFamily: "Algerian" } } }                      

});

{% endhighlight %}




### legend.title.font.fontStyle `enum`
{:#members:legend-title-font-fontstyle}

<ts ref="ej.datavisualization.Chart.FontStyle"/>


Font style for legend title.


#### Default Value

* "normal". See <a href="global.html#enum:fontstyle">FontStyle</a>




#### Example


{% highlight js %}
 
$("#container").ejChart({

   legend: { title: { font :{fontStyle: "normal" } } }                      

});

{% endhighlight %}




### legend.title.font.fontWeight `enum`
{:#members:legend-title-font-fontweight}

<ts ref="ej.datavisualization.Chart.FontWeight"/>


Font weight for legend title.


#### Default Value

* "normal". See <a href="global.html#enum:fontweight">FontWeight</a>




#### Example


{% highlight js %}
 
$("#container").ejChart({

   legend: { title: { font :{fontWeight: "normal" } } }                      

});

{% endhighlight %}




### legend.title.font.size `string`
{:#members:legend-title-font-size}




Font size for legend title.


#### Default Value

* "12px"




#### Example


{% highlight js %}
 
$("#container").ejChart({

   legend: { title: { font :{size: "14px" } } }                      

});

{% endhighlight %}




### legend.title.text `string`
{:#members:legend-title-text}




Text to be displayed in legend title.


#### Default Value

* ""




#### Example


{% highlight js %}
 
$("#container").ejChart({

   legend: { title: { text : "Countries" } }                      

});

{% endhighlight %}


Try it: [JS Playground Sample](http://jsplayground.syncfusion.com/ux1xb3j4)




### legend.title.textAlignment `enum`
{:#members:legend-title-textalignment}

<ts name="ej.datavisualization.Chart.Alignment"/>
Alignment of the legend title.


<table class="props">
<thead>
<tr>
<th>Name</th>
<th>Type</th> 
<th class="last">Description</th>
</tr>
</thead>
<tbody>
<tr>
<td class="name">
Center</td>
<td class="type">string</td> 
<td class="description">Legend Title will be aligned as center of the legends</td>
</tr>
<tr>
<td class="name">
Near</td>
<td class="type">string</td>
<td class="description">Legend Title will be aligned as near</td>
</tr> 
<tr>
<td class="name">
Far</td>
<td class="type">string</td>
<td class="description">Legend Title will be aligned as far</td>
</tr> 
</tbody>
</table>





#### Default Value

* "center". See <a href="ejchart.html#members:legend-title-textalignment">Alignment</a>




#### Example


{% highlight js %}
 
$("#container").ejChart({

   legend: { title: { textAlignment : "near" } }                      

});

{% endhighlight %}


Try it: [JS Playground Sample](http://jsplayground.syncfusion.com/hnrnl1o1)


### legend.textOverflow `enum`
{:#members:legend-textoverflow}

<ts name="ej.datavisualization.Chart.TextOverflow"/>
Specifies the action taken when the legend width is more than the textWidth.


<table class="props">
<thead>
<tr>
<th>Name</th>
<th>Type</th> 
<th class="last">Description</th>
</tr>
</thead>
<tbody>
<tr>
<td class="name">
None</td>
<td class="type">string</td> 
<td class="description">No action will be performed</td>
</tr>
<tr>
<td class="name">
Trim</td>
<td class="type">string</td>
<td class="description">Legend text will be Trimmed</td>
</tr> 
<tr>
<td class="name">
Wrap</td>
<td class="type">string</td>
<td class="description">Legend text will be Wrap by word</td>
</tr> 
<tr>
<td class="name">
WrapAndTrim</td>
<td class="type">string</td>
<td class="description">Legend text will be wrap with trim action</td>
</tr> 
</tbody>
</table>




#### Default Value

* "none". See <a href="ejchart.html#members:legend-textoverflow">textOverflow</a>




#### Example


{% highlight js %}
 
$("#container").ejChart({ 
  legend :{
              textOverflow : "trim"
             }
  }); 

{% endhighlight %}


Try it: [JS Playground Sample](http://jsplayground.syncfusion.com/hnrnl1o1)


### legend.textWidth `number`
{:#members:legend-textwidth}




Text width for legend item.


#### Default Value

* 34




#### Example


{% highlight js %}
 
$("#container").ejChart({ 
  legend :{
              textWidth : 50
             }
  }); 

{% endhighlight %}


Try it: [JS Playground Sample](http://jsplayground.syncfusion.com/hnrnl1o1)



### legend.visible `boolean`
{:#members:legend-visible}




Controls the visibility of the legend.


#### Default Value

* true




#### Example


{% highlight js %}
 
$("#container").ejChart({

   legend : {visible : false}                     

});

{% endhighlight %}


Try it: [JS Playground Sample](http://jsplayground.syncfusion.com/dwcvfzuv)


### legend.toggleSeriesVisibility `boolean`
{:#members:legend-toggleseriesvisibility}




Controls the selection through the legend.


#### Default Value

* true




#### Example


{% highlight js %}
 
$("#container").ejChart({

   legend : {toggleSeriesVisibility : false}                     

});

{% endhighlight %}


Try it: [JS Playground Sample](http://jsplayground.syncfusion.com/f1oocjec)



### locale `string`
{:#members:locale}




Name of the culture based on which chart should be localized. Number and date time values are localized with respect to the culture name. 
String type properties like title text are not localized automatically. Provide localized text as value to string type properties.


#### Default Value

* "en-US"




#### Example


{% highlight js %}
 
$("#container").ejChart({

   locale : "en-US"            

});

{% endhighlight %}


Try it: [JS Playground Sample](http://jsplayground.syncfusion.com/g3q30pdl)



### palette `array`
{:#members:palette}




Palette is used to store the series fill color in array and apply the color to series collection in the order of series index.


#### Default value

* null




#### Example


{% highlight js %}
 
$("#container").ejChart({

   palette: ["#34e2d3", "#36fe3a", "#dede3d"]          

});

{% endhighlight %}


Try it: [JS Playground Sample](http://jsplayground.syncfusion.com/0vka45gc)

### margin `object`
{:#members:margin}




Options to customize the left, right, top and bottom margins of chart area.


Try it: [JS Playground Sample](http://jsplayground.syncfusion.com/5rlvd0ri)




### margin.left `number`
{:#members:margin-left}




Spacing for the left margin of chart area. Setting positive value decreases the width of the chart area from left side.


#### Default Value

* 10




#### Example


{% highlight js %}
 
$("#container").ejChart({

   margin : { left: 15 }             

});

{% endhighlight %}




### margin.right `number`
{:#members:margin-right}




Spacing for the right margin of chart area. Setting positive value decreases the width of the chart area from right side.


#### Default Value

* 10




#### Example


{% highlight js %}
 
$("#container").ejChart({

   margin : { right: 10 }             

});

{% endhighlight %}




### margin.top `number`
{:#members:margin-top}




Spacing for the top margin of chart area. Setting positive value decreases the height of the chart area from the top.


#### Default Value

* 10




#### Example


{% highlight js %}
 
$("#container").ejChart({

   margin : { top: 10 }             

});

{% endhighlight %}




### margin.bottom `number`
{:#members:margin-bottom}




Spacing for the bottom margin of the chart area. Setting positive value decreases the height of the chart area from the bottom.


#### Default Value

* 10




#### Example


{% highlight js %}
 
$("#container").ejChart({

   margin : { bottom: 10 }             

});

{% endhighlight %}




### perspectiveAngle `number`
{:#members:perspectiveangle}




Perspective angle of the 3D view. Chart appears closer when perspective angle is decreased, and distant when perspective angle is increased. 
This property is applicable only when 3D view is enabled


#### Default Value



* 90




#### Example


{% highlight js %}

$("#container").ejChart({

     perspectiveAngle : 60
                  
});

{% endhighlight %}


Try it: [JS Playground Sample](http://jsplayground.syncfusion.com/ofpxunlm)




### primaryXAxis `object`
{:#members:primaryxaxis}




This is a horizontal axis that contains options to configure axis and it is the primary x axis for all the series in series array. To override x axis for particular series, create an axis object by providing unique name by using name property and add it to axes array. Then, assign the name to the series&rsquo;s xAxisName property to link both axis and series.






### primaryXAxis.alternateGridBand `object`
{:#members:primaryxaxis-alternategridband}




Options for customizing horizontal axis alternate grid band.






### primaryXAxis.alternateGridBand.even `object`
{:#members:primaryxaxis-alternategridband-even}




Options for customizing even grid band.






### primaryXAxis.alternateGridBand.even.fill `string`
{:#members:primaryxaxis-alternategridband-even-fill}




Fill color for the even grid bands.


#### Default Value



* transparent




#### Example


{% highlight js %}

$("#container").ejChart({

    primaryXAxis: { alternateGridBand: { even :{ fill : "green" } } }
                        
});

{% endhighlight %}




### primaryXAxis.alternateGridBand.even.opacity `number`
{:#members:primaryxaxis-alternategridband-even-opacity}




Opacity of the even grid band.


#### Default Value



* 1




#### Example


{% highlight js %}

$("#container").ejChart({

    primaryXAxis: { alternateGridBand: { even :{ opacity : 0.5 } } }
                       
});

{% endhighlight %}

Try it: [JS Playground Sample](http://jsplayground.syncfusion.com/vanuvupl)


### primaryXAxis.alternateGridBand.odd `object`
{:#members:primaryxaxis-alternategridband-odd}




Options for customizing odd grid band.






### primaryXAxis.alternateGridBand.odd.fill `string`
{:#members:primaryxaxis-alternategridband-odd-fill}




Fill color of the odd grid bands


#### Default Value



* transparent




#### Example


{% highlight js %}
 
$("#container").ejChart({

    primaryXAxis: { alternateGridBand: { odd :{ fill : "red" } } }
                          
});

{% endhighlight %}




### primaryXAxis.alternateGridBand.odd.opacity `number`
{:#members:primaryxaxis-alternategridband-odd-opacity}




Opacity of odd grid band


#### Default Value



* 1




#### Example


{% highlight js %}

$("#container").ejChart({

    primaryXAxis: { alternateGridBand: { odd :{ opacity : 0.5 } } }
                          
});

{% endhighlight %}

Try it: [JS Playground Sample](http://jsplayground.syncfusion.com/n23ku03f)




### primaryXAxis.crossesAt `number`
{:#members:primaryxaxis-crossesat}




Specifies where horizontal axis should intersect the vertical axis or vice versa. Value should be provided in axis co-ordinates. If provided value is greater than the maximum value of crossing axis, then axis will be placed at the opposite side.


#### Default Value



* null




#### Example


{% highlight js %}

	$("#container").ejChart({

		primaryXAxis:
		{
			//Crosses primary Y axis at 0
			crossesAt: 0,

			//...
		},	
	});

{% endhighlight %}




### primaryXAxis.crossesInAxis `string`
{:#members:primaryxaxis-crossesinaxis}




Name of the axis used for crossing. Vertical axis name should be provided for horizontal axis and vice versa. If the provided name does not belongs to a valid axis, then primary X axis or primary Y axis will be used for crossing


#### Default Value



* null




#### Example


{% highlight js %}

	$("#container").ejChart({

		primaryXAxis:
		{
			//Crosses vertical axis at -0.2
			crossesAt: -0.2,

			//Crosses in secondary Y axis
			crossesInAxis: 'secondaryYAxis',

			//...
		},
	});

{% endhighlight %}




### primaryXAxis.isIndexed `boolean`
{:#members:primaryxaxis-isindexed}




Category axis can also plot points based on index value of data points. Index based plotting can be enabled by setting ‘isIndexed’ property to true.


#### Default Value



* false




#### Example


{% highlight js %}

$("#container").ejChart({

    primaryXAxis: { isIndexed: true }
                          
});

{% endhighlight %}


### primaryXAxis.enableAutoIntervalOnZooming`boolean`
{:#members:primaryxaxis-enableautointervalonzooming}



Specifies the interval of the axis according to the zoomed data of the chart. 

#### Default Value



* true




#### Example


{% highlight js %}

$("#container").ejChart({

    primaryXAxis: { enableAutoIntervalOnZooming: true }
                          
});

{% endhighlight %}





### primaryXAxis.axisLine `object`
{:#members:primaryxaxis-axisline}




Options for customizing the axis line.  






### primaryXAxis.axisLine.dashArray `string`
{:#members:primaryxaxis-axisline-dasharray}




Pattern of dashes and gaps to be applied to the axis line.


#### Default Value



* null




#### Example


{% highlight js %}

$("#container").ejChart({

    primaryXAxis: { axisLine : { dashArray : "2,3" } }
                          
});

{% endhighlight %}

Try it: [JS Playground Sample](http://jsplayground.syncfusion.com/gx3dji4o)


### primaryXAxis.axisLine.offset `number`
{:#members:primaryxaxis-axisline-offset}




Padding for axis line. Normally, it is used along with plotOffset to pad the plot area.


#### Default Value



* null




#### Example


{% highlight js %}

$("#container").ejChart({

    primaryXAxis: { axisLine : { offset : 5 } }
                          
});

{% endhighlight %}

Try it: [JS Playground Sample](http://jsplayground.syncfusion.com/fmchh3yz)


### primaryXAxis.axisLine.visible `boolean`
{:#members:primaryxaxis-axisline-visible}




Show/hides the axis line.


#### Default Value



* true




#### Example


{% highlight js %}

$("#container").ejChart({

    primaryXAxis: { axisLine : { visible : false } }
                          
});

{% endhighlight %}


### primaryXAxis.axisLine.color `string`
{:#members:primaryxaxis-axisline-color}


#### Default Value



* ""




#### Example


{% highlight js %}

$("#container").ejChart({

    primaryXAxis: { axisLine : { color : "red" } }
                          
});

{% endhighlight %}



### primaryXAxis.axisLine.width `number`
{:#members:primaryxaxis-axisline-width}




Width of axis line.


#### Default Value



* 1




#### Example


{% highlight js %}

$("#container").ejChart({

    primaryXAxis: { axisLine : { width : 2 } }
                          
});

{% endhighlight %}

Try it: [JS Playground Sample](http://jsplayground.syncfusion.com/0chmy5rg)


### primaryXAxis.columnIndex `number`
{:#members:primaryxaxis-columnindex}




Specifies the index of the column where the axis is associated, when the chart area is divided into multiple plot areas by using columnDefinitions.


#### Default Value



* null




#### Example


{% highlight js %}

$("#container").ejChart({

     primaryXAxis: { columnIndex: 2 }
                           
});

{% endhighlight %}




### primaryXAxis.columnSpan `number`
{:#members:primaryxaxis-columnspan}




Specifies the number of columns or plot areas an axis has to span horizontally.


#### Default Value



* null




#### Example


{% highlight js %}

$("#container").ejChart({

    primaryXAxis: { columnSpan: 2 }
                          
});

{% endhighlight %}

Try it: [JS Playground Sample](http://jsplayground.syncfusion.com/zqgvpx1v)


### primaryXAxis.crosshairLabel `object`
{:#members:primaryxaxis-crosshairlabel}




Options to customize the crosshair label.






### primaryXAxis.crosshairLabel.visible `boolean`
{:#members:primaryxaxis-crosshairlabel-visible}




Show/hides the crosshair label associated with this axis.


#### Default Value



* false




#### Example


{% highlight js %}

$("#container").ejChart({

    primaryXAxis: { crosshairLabel : { visible : true} }
                          
});

{% endhighlight %}




### primaryXAxis.desiredIntervals `number`
{:#members:primaryxaxis-desiredintervals}




With this setting, you can request axis to calculate intervals approximately equal to your desired interval.


#### Default Value



* null




#### Example


{% highlight js %}

$("#container").ejChart({

     primaryXAxis: { desiredIntervals: 5 }
                           
});

{% endhighlight %}


### primaryXAxis.labelPlacement `enum`
{:#members:primaryxaxis-labelplacement}

<ts name="ej.datavisualization.Chart.LabelPlacement"/>
Specifies the placement of labels. 


<table class="props">
<thead>
<tr>
<th>Name</th>
<th>Type</th> 
<th class="last">Description</th>
</tr>
</thead>
<tbody>
<tr>
<td class="name">
OnTicks</td>
<td class="type">string</td> 
<td class="description">Labels will be placed on tick</td>
</tr>
<tr>
<td class="name">
BetweenTicks</td>
<td class="type">string</td>
<td class="description">Labels will be placed between ticks</td>
</tr> 
</tbody>
</table>



#### Default Value



* ej.datavisualization.Chart.LabelPlacement.BetweenTicks. See <a href="ejchart.html#members:primaryxaxis-labelplacement">LabelPlacement</a>


#### Example


{% highlight js %}

$("#container").ejChart({

    primaryXAxis: { labelPlacement : "onTicks" }
                          
});

{% endhighlight %}



### primaryXAxis.edgeLabelPlacement `enum`
{:#members:primaryxaxis-edgelabelplacement}

<ts name="ej.datavisualization.Chart.EdgeLabelPlacement"/>
Specifies the position of labels at the edge of the axis. 


<table class="props">
<thead>
<tr>
<th>Name</th>
<th>Type</th> 
<th class="last">Description</th>
</tr>
</thead>
<tbody>
<tr>
<td class="name">
None</td>
<td class="type">string</td> 
<td class="description">no action will be perform</td>
</tr>
<tr>
<td class="name">
Shift</td>
<td class="type">string</td>
<td class="description">Perform shift action to the edge labels</td>
</tr> 
<tr>
<td class="name">
Hide</td>
<td class="type">string</td>
<td class="description">The edge label will be hidden</td>
</tr> 
</tbody>
</table>





#### Default Value



* ej.datavisualization.Chart.EdgeLabelPlacement.None. See <a href="ejchart.html#members:primaryxaxis-edgelabelplacement">EdgeLabelPlacement</a>




#### Example


{% highlight js %}

$("#container").ejChart({

    primaryXAxis: { edgeLabelPlacement : "shift" }
                          
});

{% endhighlight %}

Try it: [JS Playground Sample](http://jsplayground.syncfusion.com/ff44lp52)


### primaryXAxis.enableTrim `boolean`
{:#members:primaryxaxis-enabletrim}




Specifies whether to trim the axis label when the width of the label exceeds the maximumLabelWidth.


#### Default Value



* false




#### Example


{% highlight js %}

$("#container").ejChart({

    primaryXAxis: { enableTrim : true }
                          
});

{% endhighlight %}

Try it: [JS Playground Sample](http://jsplayground.syncfusion.com/qt3th50v)


### primaryXAxis.font `object`
{:#members:primaryxaxis-font}




Options for customizing the font of the axis Labels.






### primaryXAxis.font.fontFamily `string`
{:#members:primaryxaxis-font-fontfamily}




Font family of labels.


#### Default Value



* "Segoe UI"




#### Example


{% highlight js %}

$("#container").ejChart({

     primaryXAxis: { font : { fontFamily : "Algerian"} }
                           
});

{% endhighlight %}




### primaryXAxis.font.fontStyle `enum`
{:#members:primaryxaxis-font-fontstyle}

<ts ref="ej.datavisualization.Chart.FontStyle"/>



Font style of labels.


#### Default Value




* ej.datavisualization.Chart.FontStyle.Normal. See <a href="global.html#enum:fontstyle">FontStyle</a>




#### Example


{% highlight js %}

$("#container").ejChart({

    primaryXAxis: { font : { fontStyle : "Italic"} }
                          
});

{% endhighlight %}




### primaryXAxis.font.fontWeight `enum`
{:#members:primaryxaxis-font-fontweight}

<ts ref="ej.datavisualization.Chart.FontWeight"/>


Font weight of the label.


#### Default Value



* ej.datavisualization.Chart.FontWeight.Regular. See <a href="global.html#enum:fontweight">FontWeight</a>




#### Example


{% highlight js %}

$("#container").ejChart({

     primaryXAxis: { font : { fontWeight : "lighter"} }
                           
});

{% endhighlight %}




### primaryXAxis.font.opacity `number`
{:#members:primaryxaxis-font-opacity}




Opacity of the axis labels.


#### Default Value



* 1




#### Example


{% highlight js %}

$("#container").ejChart({

    primaryXAxis: { font : { opacity : 0.5} }
                          
});

{% endhighlight %}




### primaryXAxis.font.size `string`
{:#members:primaryxaxis-font-size}




Font size of the axis labels.


#### Default Value



* "13px"




#### Example


{% highlight js %}

$("#container").ejChart({

     primaryXAxis: { font : { size : "12px"} }
                           
});

{% endhighlight %}

Try it: [JS Playground Sample](http://jsplayground.syncfusion.com/xm2ur0jj)


### primaryXAxis.intervalType `enum`
{:#members:primaryxaxis-intervaltype}

<ts name="ej.datavisualization.Chart.IntervalType"/>
Specifies the type of interval in date time axis.


<table class="props">
<thead>
<tr>
<th>Name</th>
<th>Type</th> 
<th class="last">Description</th>
</tr>
</thead>
<tbody>
<tr>
<td class="name">
Days</td>
<td class="type">string</td> 
<td class="description">Specify the interval type as days</td>
</tr>
<tr>
<td class="name">
Hours</td>
<td class="type">string</td>
<td class="description">Specify the interval type as hours</td>
</tr> 
<tr>
<td class="name">
Seconds</td>
<td class="type">string</td>
<td class="description">Specify the interval type as seconds</td>
</tr> 
<tr>
<td class="name">
Milliseconds</td>
<td class="type">string</td>
<td class="description">Specify the interval type as milliseconds</td>
</tr> 
<tr>
<td class="name">
Minutes</td>
<td class="type">string</td>
<td class="description">Specify the interval type as minutes</td>
</tr> 
<tr>
<td class="name">
Months</td>
<td class="type">string</td>
<td class="description">Specify the interval type as months</td>
</tr> 
<tr>
<td class="name">
Years</td>
<td class="type">string</td>
<td class="description">Specify the interval type as years</td>
</tr> 
</tbody>
</table>





#### Default Value




* null. See <a href="ejchart.html#members:primaryxaxis-intervaltype">IntervalType</a>




#### Example


{% highlight js %}

$("#container").ejChart({

     primaryXAxis: { intervalType: "days" }
                           
});

{% endhighlight %}

Try it: [JS Playground Sample](http://jsplayground.syncfusion.com/qccdazta)


### primaryXAxis.isInversed `boolean`
{:#members:primaryxaxis-isinversed}




Specifies whether to inverse the axis.


#### Default Value



* false




#### Example


{% highlight js %}

$("#container").ejChart({

     primaryXAxis: { isInversed : true}
                           
});

{% endhighlight %}

Try it: [JS Playground Sample](http://jsplayground.syncfusion.com/xp1frbzw)


### primaryXAxis.labelFormat `string`
{:#members:primaryxaxis-labelformat}




Custom formatting for axis label and supports all standard formatting type of numerical and date time values.


#### Default Value



* null




#### Example


{% highlight js %}

$("#container").ejChart({

    primaryXAxis: { labelFormat: "{value}%" }
                          
});

{% endhighlight %}

Try it: [JS Playground Sample](http://jsplayground.syncfusion.com/x22gftws)


### primaryXAxis.labelIntersectAction `enum`
{:#members:primaryxaxis-labelintersectaction}

<ts name="ej.datavisualization.Chart.LabelIntersectAction"/>
Specifies the action to take when the axis labels are overlapping with each other. 


<table class="props">
<thead>
<tr>
<th>Name</th>
<th>Type</th> 
<th class="last">Description</th>
</tr>
</thead>
<tbody>
<tr>
<td class="name">
None</td>
<td class="type">string</td> 
<td class="description">no action will be perform in axis labels</td>
</tr>
<tr>
<td class="name">
Rotate90</td>
<td class="type">string</td>
<td class="description">Displays axis labels with 90 degree</td>
</tr> 
<tr>
<td class="name">
Rotate45</td>
<td class="type">string</td>
<td class="description">Displays axis labels with 45 degree</td>
</tr> 
<tr>
<td class="name">
Wrap</td>
<td class="type">string</td>
<td class="description">Axis labels will be Wrap</td>
</tr> 
<tr>
<td class="name">
WrapByword</td>
<td class="type">string</td>
<td class="description">Axis labels will be Wrap by word</td>
</tr> 
<tr>
<td class="name">
Trim</td>
<td class="type">string</td>
<td class="description">Axis labels will be trimmed</td>
</tr> 
<tr>
<td class="name">
Hide</td>
<td class="type">string</td>
<td class="description">Axis labels will be hide when overlap to others</td>
</tr> 
<tr>
<td class="name">
MultipleRows</td>
<td class="type">string</td>
<td class="description">Axis labels will display the next line when overlap to others</td>
</tr> 
</tbody>
</table>





#### Default Value



* ej.datavisualization.Chart.LabelIntersectAction.None. See <a href="ejchart.html#members:primaryxaxis-labelintersectaction">LabelIntersectAction</a>




#### Example


{% highlight js %}

$("#container").ejChart({

    primaryXAxis: { labelIntersectAction : "multipleRows" }
                          
});

{% endhighlight %}

Try it: [JS Playground Sample](http://jsplayground.syncfusion.com/sedhp2ek)


### primaryXAxis.labelPosition `enum`
{:#members:primaryxaxis-labelposition}

<ts name="ej.datavisualization.Chart.LabelPosition"/>
Specifies the position of the axis labels.


<table class="props">
<thead>
<tr>
<th>Name</th>
<th>Type</th> 
<th class="last">Description</th>
</tr>
</thead>
<tbody>
<tr>
<td class="name">
Inside</td>
<td class="type">string</td> 
<td class="description">The axis labels area visible inside the axis line</td>
</tr>
<tr>
<td class="name">
OutSide</td>
<td class="type">string</td>
<td class="description">The axis labels area visible outside the axis line</td>
</tr> 
</tbody>
</table>






#### Default Value



* "outside". See <a href="ejchart.html#members:primaryxaxis-labelposition">LabelPosition</a>




#### Example


{% highlight js %}

$("#container").ejChart({

    primaryXAxis: { labelPosition : "inside" }
                       
});

{% endhighlight %}

Try it: [JS Playground Sample](http://jsplayground.syncfusion.com/u0s1y0dg)



### primaryXAxis.alignment `enum`
{:#members:primaryxaxis-alignment}

<ts name="ej.datavisualization.Chart.LabelAlignment"/>
Specifies the position of the axis labels.


<table class="props">
<thead>
<tr>
<th>Name</th>
<th>Type</th> 
<th class="last">Description</th>
</tr>
</thead>
<tbody>
<tr>
<td class="name">
Near</td>
<td class="type">string</td> 
<td class="description">The axis labels placed as near</td>
</tr>
<tr>
<td class="name">
Far</td>
<td class="type">string</td>
<td class="description">The axis labels placed as far</td>
</tr> 
<tr>
<td class="name">
Center</td>
<td class="type">string</td>
<td class="description">The axis labels placed as center</td>
</tr> 
</tbody>
</table>


#### Default Value



* "center". See <a href="ejchart.html#members:primaryxaxis-alignment">Alignment</a>




#### Example


{% highlight js %}

$("#container").ejChart({

    primaryXAxis: { alignment : "far" }
                       
});

{% endhighlight %}

Try it: [JS Playground Sample](http://jsplayground.syncfusion.com/vfgwipz1)



### primaryXAxis.labelRotation `number`
{:#members:primaryxaxis-labelrotation}




Angle in degrees to rotate the axis labels.


#### Default Value



* null




#### Example


{% highlight js %}

$("#container").ejChart({

    primaryXAxis: { labelRotation: 90 }
                          
});

{% endhighlight %}

Try it: [JS Playground Sample](http://jsplayground.syncfusion.com/gl5iwbsh)


### primaryXAxis.logBase `number`
{:#members:primaryxaxis-logbase}




Logarithmic base value. This is applicable only for logarithmic axis.


#### Default Value



* 10




#### Example


{% highlight js %}

$("#container").ejChart({

    primaryXAxis: { logBase: 5 }
                          
});

  {% endhighlight %}




### primaryXAxis.majorGridLines `object`
{:#members:primaryxaxis-majorgridlines}




Options for customizing major gird lines.






### primaryXAxis.majorGridLines.dashArray `string`
{:#members:primaryxaxis-majorgridlines-dasharray}




Pattern of dashes and gaps used to stroke the major grid lines.


#### Default Value



* null




#### Example


{% highlight js %}

$("#container").ejChart({

    primaryXAxis: { majorGridLines: { dashArray : "2,3"} }
                          
});

{% endhighlight %}



### primaryXAxis.majorGridLines.color `string`
{:#members:primaryxaxis-majorgridlines-color}




Color of the major grid line.


#### Default Value



* null




#### Example


{% highlight js %}

$("#container").ejChart({

    primaryXAxis: { majorGridLines: { color : "red"} }
                          
});

{% endhighlight %}




### primaryXAxis.majorGridLines.opacity `number`
{:#members:primaryxaxis-majorgridlines-opacity}




Opacity of major grid lines.


#### Default Value



* 1




#### Example


{% highlight js %}

$("#container").ejChart({

    primaryXAxis: { majorGridLines: { opacity: 0.5 } }
                          
});

{% endhighlight %}




### primaryXAxis.majorGridLines.visible `boolean`
{:#members:primaryxaxis-majorgridlines-visible}




Show/hides the major grid lines.


#### Default Value



* true




#### Example


{% highlight js %}

$("#container").ejChart({

    primaryXAxis: { majorGridLines: { visible: false } }
                          
});

{% endhighlight %}




### primaryXAxis.majorGridLines.width `number`
{:#members:primaryxaxis-majorgridlines-width}




Width of the major grid lines.


#### Default Value



* 1




#### Example


{% highlight js %}

$("#container").ejChart({

    primaryXAxis: { majorGridLines: { width : 0.5} }
                          
});

{% endhighlight %}

Try it: [JS Playground Sample](http://jsplayground.syncfusion.com/1tjezqc0)


### primaryXAxis.majorTickLines `object`
{:#members:primaryxaxis-majorticklines}




Options for customizing the major tick lines.






### primaryXAxis.majorTickLines.size `number`
{:#members:primaryxaxis-majorticklines-size}




Length of the major tick lines.


#### Default Value



* 5




#### Example


{% highlight js %}

$("#container").ejChart({

    primaryXAxis: { majorTickLines: { size: 2 } }
                          
});

{% endhighlight %}




### primaryXAxis.majorTickLines.visible `boolean`
{:#members:primaryxaxis-majorticklines-visible}




Show/hides the major tick lines.


#### Default Value



* true




#### Example


{% highlight js %}

$("#container").ejChart({

    primaryXAxis: { majorTickLines: { visible: false } }
                          
});

{% endhighlight %}




### primaryXAxis.majorTickLines.width `number`
{:#members:primaryxaxis-majorticklines-width}




Width of the major tick lines.


#### Default Value



* 1




#### Example


{% highlight js %}

$("#container").ejChart({

    primaryXAxis: { majorTickLines: { width: 2 } }
                          
});

{% endhighlight %}

Try it: [JS Playground Sample](http://jsplayground.syncfusion.com/30i5qgrm)


### primaryXAxis.maximumLabels `number`
{:#members:primaryxaxis-maximumlabels}




Maximum number of labels to be displayed in every 100 pixels.


#### Default Value



* 3




#### Example


{% highlight js %}

$("#container").ejChart({

    primaryXAxis: { maximumLabels : 5 }
                          
});

{% endhighlight %}

Try it: [JS Playground Sample](http://jsplayground.syncfusion.com/a4gcmpzx)


### primaryXAxis.maximumLabelWidth `number`
{:#members:primaryxaxis-maximumlabelwidth}




Maximum width of the axis label. When the label exceeds the width, the label gets trimmed when the enableTrim is set to true.


#### Default Value



* 34




#### Example


{% highlight js %}

$("#container").ejChart({

     primaryXAxis: { maximumLabelWidth :34.5 }
                           
});

{% endhighlight %}




### primaryXAxis.minorGridLines `object`
{:#members:primaryxaxis-minorgridlines}




Options for customizing the minor grid lines.






### primaryXAxis.minorGridLines.dashArray `string`
{:#members:primaryxaxis-minorgridlines-dasharray}




Patterns of dashes and gaps used to stroke the minor grid lines.


#### Default Value



* null




#### Example


{% highlight js %}

$("#container").ejChart({

    primaryXAxis: { minorGridLines: { dashArray: "2,3" } }
                          
});

{% endhighlight %}




### primaryXAxis.minorGridLines.visible `boolean`
{:#members:primaryxaxis-minorgridlines-visible}




Show/hides the minor grid lines.


#### Default Value



* true




#### Example


{% highlight js %}

$("#container").ejChart({

    primaryXAxis: { minorGridLines: { visible: true } }
                          
});

{% endhighlight %}




### primaryXAxis.minorGridLines.width `number`
{:#members:primaryxaxis-minorgridlines-width}




Width of the minorGridLines.


#### Default Value



* 1




#### Example


{% highlight js %}

$("#container").ejChart({

    primaryXAxis: { minorGridLines: { width: 2 } }
                          
});

{% endhighlight %}

Try it: [JS Playground Sample](http://jsplayground.syncfusion.com/xlobmfvj)


### primaryXAxis.minorTickLines `object`
{:#members:primaryxaxis-minorticklines}




Options for customizing the minor tick lines.






### primaryXAxis.minorTickLines.size `number`
{:#members:primaryxaxis-minorticklines-size}




Length of the minor tick lines.


#### Default Value



* 5




#### Example


{% highlight js %}

$("#container").ejChart({

    primaryXAxis: { minorTickLines: { size: 2 } }
                          
});

{% endhighlight %}




### primaryXAxis.minorTickLines.visible `boolean`
{:#members:primaryxaxis-minorticklines-visible}




Show/hides the minor tick lines.


#### Default Value



* true




#### Example


{% highlight js %}

$("#container").ejChart({

    primaryXAxis: { minorTickLines: { visible: true } }
                          
});
Width of the minor tick line.
{% endhighlight %}




### primaryXAxis.minorTickLines.width `number`
{:#members:primaryxaxis-minorticklines-width}




Width of the minor tick line.


#### Default Value



* 1




#### Example


{% highlight js %}

$("#container").ejChart({
 
    primaryXAxis: { minorTickLines: { width: 2 } }
                          
});

{% endhighlight %}




### primaryXAxis.minorTicksPerInterval `number`
{:#members:primaryxaxis-minorticksperinterval}




Specifies the number of minor ticks per interval.


#### Default Value



* null




#### Example


{% highlight js %}

$("#container").ejChart({
 
    primaryXAxis: { minorTicksPerInterval: 5 }
                          
});

{% endhighlight %}


### primaryXAxis.name `string`
{:#members:primaryxaxis-name}




Unique name of the axis. To associate an axis with the series, you have to set this name to the xAxisName/yAxisName property of the series.


#### Default Value



* null




#### Example


{% highlight js %}

$("#container").ejChart({

    primaryXAxis: { name: "xAxis" }
                          
});

{% endhighlight %}




### primaryXAxis.opposedPosition `boolean`
{:#members:primaryxaxis-opposedposition}




Specifies whether to render the axis at the opposite side of its default position.


#### Default Value



* false




#### Example


{% highlight js %}

$("#container").ejChart({

    primaryXAxis: { opposedPosition : true }
                          
});

{% endhighlight %}



### primaryXAxis.orientation `enum`
{:#members:primaryxaxis-orientation}

<ts name="ej.datavisualization.Chart.AxisOrientation"/>
Specifies the orientation of the axis line

<table class="props">
<thead>
<tr>
<th>Name</th>
<th>Type</th> 
<th class="last">Description</th>
</tr>
</thead>
<tbody>
<tr>
<td class="name">
Horizontal</td>
<td class="type">string</td> 
<td class="description last">The axis line is displayed in horizontal direction </td>
</tr>
<tr>
<td class="name">
Vertical</td>
<td class="type">string</td>
<td class="description last">The axis line is displayed in vertical direction</td>
</tr> 
</tbody>
</table>


#### Default Value



* Horizontal




#### Example


{% highlight js %}

$("#container").ejChart({

    primaryXAxis: { orientation : 'Vertical' }
                          
});

{% endhighlight %}




### primaryXAxis.plotOffset `number`
{:#members:primaryxaxis-plotoffset}




Specifies the padding for the plot area.


#### Default Value



* 10




#### Example


{% highlight js %}

$("#container").ejChart({

    primaryXAxis: { plotOffset: 0 }
                          
});

{% endhighlight %}

Try it: [JS Playground Sample](http://jsplayground.syncfusion.com/yo4ek2ci)


### primaryXAxis.range `object`
{:#members:primaryxaxis-range}




Options to customize the range of the axis.

Try it: [JS Playground Sample](http://jsplayground.syncfusion.com/Sync_jhhilggd)


### primaryXAxis.range.min `number`
{:#members:primaryxaxis-range-min}




Minimum value of the axis range.


#### Default Value

* null




#### Example


{% highlight js %}

$("#container").ejChart({

    primaryXAxis: { range : { min: 10 } }
                          
});

{% endhighlight %}


### primaryXAxis.range.max `number`
{:#members:primaryxaxis-range-max}




Maximum value of the axis range.


#### Default Value

* null




#### Example


{% highlight js %}

$("#container").ejChart({

    primaryXAxis: { range : { max: 100 } }
                          
});

{% endhighlight %}


### primaryXAxis.range.interval `number`
{:#members:primaryxaxis-range-interval}




Interval of the axis range.


#### Default Value

* null




#### Example


{% highlight js %}

$("#container").ejChart({

    primaryXAxis: { range : { interval: 10 } }
                          
});

{% endhighlight %}


### primaryXAxis.rangePadding `enum`
{:#members:primaryxaxis-rangepadding}

<ts name="ej.datavisualization.Chart.RangePadding"/>
Specifies the padding for the axis range.


<table class="props">
<thead>
<tr>
<th>Name</th>
<th>Type</th> 
<th class="last">Description</th>
</tr>
</thead>
<tbody>
<tr>
<td class="name">
Additional</td>
<td class="type">string</td> 
<td class="description">Interval of the axis is added as padding to the minimum and maximum values of the range</td>
</tr>
<tr>
<td class="name">
Normal</td>
<td class="type">string</td>
<td class="description">Padding is applied to the axis based on the range calculation</td>
</tr> 
<tr>
<td class="name">
None</td>
<td class="type">string</td>
<td class="description"> Padding cannot be applied to the axis</td>
</tr> 
<tr>
<td class="name">
Round</td>
<td class="type">string</td>
<td class="description">Axis range is rounded to the nearest possible value divided by the interval</td>
</tr> 
</tbody>
</table>



#### Default Value


* "None". See <a href="ejchart.html#members:primaryxaxis-rangepadding">RangePadding</a>




#### Example


{% highlight js %}

$("#container").ejChart({

    primaryXAxis: { rangePadding : "normal" }
                          
});

{% endhighlight %}




### primaryXAxis.roundingPlaces `number`
{:#members:primaryxaxis-roundingplaces}




Rounds the number to the given number of decimals.


#### Default Value



* null




#### Example


{% highlight js %}

$("#container").ejChart({

    primaryXAxis: { roundingPlaces: 3 }
                          
});

{% endhighlight %}


Try it: [JS Playground Sample](http://jsplayground.syncfusion.com/hgqmxm50)


### primaryXAxis.multiLevelLabels `array`
{:#members:primaryxaxis-multilevellabels}


Options for customizing the multi level labels.


#### Default Value



* [ ]







### primaryXAxis.multiLevelLabels.visible `boolean`
{:#members:primaryxaxis-multilevellabels-visible}




Visibility of the multi level labels.


#### Default Value



* false




#### Example


{% highlight js %}

$("#container").ejChart({
 
    primaryXAxis: { multiLevelLabels:[{ visible: true }]}
                          
});

{% endhighlight %}


### primaryXAxis.multiLevelLabels.text `string`
{:#members:primaryxaxis-multilevellabels-text}




Text of the multi level labels.


#### Default Value



* ""




#### Example


{% highlight js %}

$("#container").ejChart({
 
    primaryXAxis: { multiLevelLabels:[{ text: "2016" }]}
                          
});

{% endhighlight %}


### primaryXAxis.multiLevelLabels.start `object`
{:#members:primaryxaxis-multilevellabels-start}




Starting value of the multi level labels.


#### Default Value



* null




#### Example


{% highlight js %}

$("#container").ejChart({
 
    primaryXAxis: { multiLevelLabels:[{ start: 1 }]}
                          
});

{% endhighlight %}

### primaryXAxis.multiLevelLabels.end `object`
{:#members:primaryxaxis-multilevellabels-end}




Ending value of the multi level labels.


#### Default Value



* null




#### Example


{% highlight js %}

$("#container").ejChart({
 
    primaryXAxis: { multiLevelLabels:[{ end: 4 }]}
                          
});

{% endhighlight %}


### primaryXAxis.multiLevelLabels.level `number`
{:#members:primaryxaxis-multilevellabels-level}




Specifies the level of multi level labels.


#### Default Value



* 0




#### Example


{% highlight js %}

$("#container").ejChart({
 
    primaryXAxis: { multiLevelLabels:[{ level: 2 }]}
                          
});

{% endhighlight %}


### primaryXAxis.multiLevelLabels.maximumTextWidth `number`
{:#members:primaryxaxis-multilevellabels-maximumtextwidth}




Specifies the maximum width of the text in multi level labels.


#### Default Value



* null




#### Example


{% highlight js %}

$("#container").ejChart({
 
    primaryXAxis: { multiLevelLabels:[{ maximumTextWidth: 30 }]}
                          
});

{% endhighlight %}



### primaryXAxis.multiLevelLabels.textAlignment `enum`
{:#members:primaryxaxis-multilevellabels-textalignment}

<ts ref="ej.datavisualization.Chart.TextAlignment"/>


Specifies the alignment of the text in multi level labels.


#### Default Value



* "center". See <a href="global.html#enum:textalignment">TextAlignment</a>




#### Example


{% highlight js %}

$("#container").ejChart({
 
    primaryXAxis: { multiLevelLabels:[{ textAlignment: "near" }]}
                          
});

{% endhighlight %}


### primaryXAxis.multiLevelLabels.textOverflow `enum`
{:#members:primaryxaxis-multilevellabels-textoverflow}

<ts ref="ej.datavisualization.Chart.TextOverflow"/>


Specifies the handling of text over flow in multi level labels.


#### Default Value



* "center". See <a href="ejchart.html#members:legend-textoverflow">TextOverflow</a>




#### Example


{% highlight js %}

$("#container").ejChart({
 
    primaryXAxis: { multiLevelLabels:[{ textOverflow: "trim" }]}
                          
});

{% endhighlight %}



### primaryXAxis.multiLevelLabels.font `object`
{:#members:primaryxaxis-multilevellabels-font}




Options for customizing the font of the text.






### primaryXAxis.multiLevelLabels.font.color `string`
{:#members:primaryxaxis-multilevellabels-font-color}




Font color of the multi level labels text.


#### Default Value



* null




#### Example


{% highlight js %}

$("#container").ejChart({

     primaryXAxis: { multiLevelLabels:[{ font : { color: "green"} }]}
                           
});

{% endhighlight %}




### primaryXAxis.multiLevelLabels.font.fontFamily `string`
{:#members:primaryxaxis-multilevellabels-font-fontfamily}




Font family of the multi level labels text.


#### Default Value



* "Segoe UI"




#### Example


{% highlight js %}

$("#container").ejChart({

    primaryXAxis: { multiLevelLabels:[{ font : { fontFamily : "Algerian"} }]}
                          
});

{% endhighlight %}




### primaryXAxis.multiLevelLabels.font.fontStyle `enum`
{:#members:primaryxaxis-multilevellabels-font-fontstyle}

<ts ref="ej.datavisualization.Chart.FontStyle"/>


Font style of the multi level labels text.


#### Default Value



* "Normal"




#### Example


{% highlight js %}

$("#container").ejChart({ 

    primaryXAxis: { multiLevelLabels:[{ font : { fontStyle: "Bold"} }]}
                          
});

{% endhighlight %}




### primaryXAxis.multiLevelLabels.font.fontWeight `string`
{:#members:primaryxaxis-multilevellabels-font-fontweight}




Font weight of the multi level label text.


#### Default Value



* "regular"




#### Example


{% highlight js %}

$("#container").ejChart({

      primaryXAxis: { multiLevelLabels:[{ font : { fontWeight: "lighter"} }]}
                            
});

{% endhighlight %}




### primaryXAxis.multiLevelLabels.font.opacity `number`
{:#members:primaryxaxis-multilevellabels-font-opacity}




Opacity of the multi level label text.


#### Default Value



* 1




#### Example


{% highlight js %}

$("#container").ejChart({

primaryXAxis: { multiLevelLabels:[{ font : { opacity: 0.5} }]}
                      
});

{% endhighlight %}




### primaryXAxis.multiLevelLabels.font.size `string`
{:#members:primaryxaxis-multilevellabels-font-size}




Font size of the multi level label text.


#### Default Value



* "12px"




#### Example


{% highlight js %}

$("#container").ejChart({

        primaryXAxis: { multiLevelLabels:[{ font : { size: "15px"} }]}
                              
});

{% endhighlight %}


### primaryXAxis.multiLevelLabels.border `object`
{:#members:primaryxaxis-multilevellabels-border}




Options for customizing the border of the series.






### primaryXAxis.multiLevelLabels.border.color `string`
{:#members:primaryxaxis-multilevellabels-border-color}




Border color of the multi level labels.


#### Default Value



*  null




#### Example


{% highlight js %}
 
 
$("#container").ejChart({
        primaryXAxis: { multiLevelLabels:[{border :{ color : "green" } }]}                  
});
{% endhighlight %}




### primaryXAxis.multiLevelLabels.border.width `number`
{:#members:primaryxaxis-multilevellabels-border-width}




Border width of the multi level labels.


#### Default Value



* 1




#### Example


{% highlight js %}
 

$("#container").ejChart({
        primaryXAxis: { multiLevelLabels:[{border :{ width : 2 } }]}                  
});
{% endhighlight %}


### primaryXAxis.multiLevelLabels.border.type `enum`
{:#members:primaryxaxis-multilevellabels-border-type}


<ts name="ej.datavisualization.Chart.MultiLevelLabelsBorderType"/>
Border type of the multi level labels.


<table class="props">
<thead>
<tr>
<th>Name</th>
<th>Type</th>
<th class="last">Description</th>
</tr>
</thead>
<tbody>
<tr>
<td class="name">
Rectangle</td>
<td class="type">string</td>
<td class="description">To render rectangle border.</td>
</tr>
<tr>
<td class="name">
None</td>
<td class="type">string</td>
<td class="description">No border will be rendered.</td>
</tr>
<tr>
<td class="name">
WithoutTopAndBottom</td>
<td class="type">string</td>
<td class="description">Border will be rendered only on left and right side of the labels.</td>
</tr>
<tr>
<td class="name">
Brace</td>
<td class="type">string</td>
<td class="description">To render brace border style.</td>
</tr>
<tr>
<td class="name">
CurlyBrace</td>
<td class="type">string</td>
<td class="description">To render curly brace border style.</td>
</tr>
</tbody>
</table>

#### Default Value



* "rectangle". See <a href="ejchart.html#members:primaryxaxis-multilevellabels-border-type">Type</a>




#### Example


{% highlight js %}
 

$("#container").ejChart({
        primaryXAxis: { multiLevelLabels:[{border :{ type : "brace" } }]}                  
});
{% endhighlight %}


### primaryXAxis.showNextToAxisLine `boolean`
{:#members:primaryxaxis-shownexttoaxisline}



Specifies whether the axis elements need to be placed nearby the axis line, while crossing.



#### Default Value



* true




#### Example


{% highlight js %}

$("#container").ejChart({

    primaryXAxis: { showNextToAxisLine : false }
                          
});

{% endhighlight %}



### primaryXAxis.stripLine `array`
{:#members:primaryxaxis-stripline}


Options for customizing the strip lines.


#### Default Value



* [ ]







### primaryXAxis.stripLine.borderColor `string`
{:#members:primaryxaxis-stripline-bordercolor}




Border color of the strip line.


#### Default Value



* "gray"




#### Example


{% highlight js %}

$("#container").ejChart({
 
    primaryXAxis: { stripLine:[{ borderColor: "green" }]}
                          
});

{% endhighlight %}




### primaryXAxis.stripLine.color `string`
{:#members:primaryxaxis-stripline-color}




Background color of the strip line.


#### Default Value



* "gray"




#### Example


{% highlight js %}

$("#container").ejChart({

    primaryXAxis: { stripLine:[{ color: "green" }]}
                          
});

{% endhighlight %}




### primaryXAxis.stripLine.end `number`
{:#members:primaryxaxis-stripline-end}




End value of the strip line.


#### Default Value



* null




#### Example


{% highlight js %}

$("#container").ejChart({

     primaryXAxis: { stripLine:[{ end: 5 }]}
                           
});

{% endhighlight %}




### primaryXAxis.stripLine.font `object`
{:#members:primaryxaxis-stripline-font}




Options for customizing the font of the text.






### primaryXAxis.stripLine.font.color `string`
{:#members:primaryxaxis-stripline-font-color}




Font color of the strip line text.


#### Default Value



* "black"




#### Example


{% highlight js %}

$("#container").ejChart({

     primaryXAxis: { stripLine:[{ font : { color: "green"} }]}
                           
});

{% endhighlight %}




### primaryXAxis.stripLine.font.fontFamily `string`
{:#members:primaryxaxis-stripline-font-fontfamily}




Font family of the strip line text.


#### Default Value



* "Segoe UI"




#### Example


{% highlight js %}

$("#container").ejChart({

    primaryXAxis: { stripLine:[{ font : { fontFamily : "Algerian"} }]}
                          
});

{% endhighlight %}




### primaryXAxis.stripLine.font.fontStyle `enum`
{:#members:primaryxaxis-stripline-font-fontstyle}

<ts ref="ej.datavisualization.Chart.FontStyle"/>


Font style of the strip line text.


#### Default Value



* "Normal"




#### Example


{% highlight js %}

$("#container").ejChart({ 

    primaryXAxis: { stripLine:[{ font : { fontStyle: "Bold"} }]}
                          
});

{% endhighlight %}




### primaryXAxis.stripLine.font.fontWeight `string`
{:#members:primaryxaxis-stripline-font-fontweight}




Font weight of the strip line text.


#### Default Value



* "regular"




#### Example


{% highlight js %}

$("#container").ejChart({

      primaryXAxis: { stripLine:[{ font : { fontWeight: "lighter"} }]}
                            
});

{% endhighlight %}




### primaryXAxis.stripLine.font.opacity `number`
{:#members:primaryxaxis-stripline-font-opacity}




Opacity of the strip line text.


#### Default Value



* 1




#### Example


{% highlight js %}

$("#container").ejChart({

primaryXAxis: { stripLine:[{ font : { opacity: 0.5} }]}
                      
});

{% endhighlight %}




### primaryXAxis.stripLine.font.size `string`
{:#members:primaryxaxis-stripline-font-size}




Font size of the strip line text.


#### Default Value



* "12px"




#### Example


{% highlight js %}

$("#container").ejChart({

        primaryXAxis: { stripLine:[{ font : { size: "15px"} }]}
                              
});

{% endhighlight %}




### primaryXAxis.stripLine.start `number`
{:#members:primaryxaxis-stripline-start}




Start value of the strip line.


#### Default Value



* null




#### Example


{% highlight js %}

$("#container").ejChart({

     primaryXAxis: { stripLine:[{ start: 2 }]}
                           
});

{% endhighlight %}




### primaryXAxis.stripLine.startFromAxis `boolean`
{:#members:primaryxaxis-stripline-startfromaxis}




Indicates whether to render the strip line from the minimum/start value of the axis. This property does not work when start property is set.


#### Default Value



* false




#### Example


{% highlight js %}

$("#container").ejChart({

    primaryXAxis: { stripLine:[{ startFromAxis : true }]}
                          
});

{% endhighlight %}




### primaryXAxis.stripLine.text `string`
{:#members:primaryxaxis-stripline-text}




Specifies text to be displayed inside the strip line.


#### Default Value



* "stripLine"




#### Example


{% highlight js %}

$("#container").ejChart({
 
    primaryXAxis: { stripLine:[{ text : "Empty Point" }]}
                           
});

{% endhighlight %}




### primaryXAxis.stripLine.textAlignment `enum`
{:#members:primaryxaxis-stripline-textalignment}

<ts name="ej.datavisualization.Chart.TextAlignment"/>
Specifies the alignment of the text inside the strip line.


<table class="props">
<thead>
<tr>
<th>Name</th>
<th>Type</th> 
<th class="last">Description</th>
</tr>
</thead>
<tbody>
<tr>
<td class="name">
MiddleTop</td>
<td class="type">string</td> 
<td class="description">The text has been aligned top of the stripline</td>
</tr>
<tr>
<td class="name">
MiddleCenter</td>
<td class="type">string</td>
<td class="description">The text has been aligned in center of the stripline</td>
</tr> 
<tr>
<td class="name">
MiddleBottom</td>
<td class="type">string</td>
<td class="description">The text has been aligned bottom of the stripline</td>
</tr> 
</tbody>
</table>





#### Default Value



* "middlecenter". See <a href="ejchart.html#members:primaryxaxis-stripline-textalignment">TextAlignment</a>




#### Example


{% highlight js %}

$("#container").ejChart({

     primaryXAxis: { stripLine:[{ textAlignment : "middletop" }]}
                           
});

{% endhighlight %}




### primaryXAxis.stripLine.visible `boolean`
{:#members:primaryxaxis-stripline-visible}




Show/hides the strip line.


#### Default Value



* false




#### Example


{% highlight js %}

$("#container").ejChart({

    primaryXAxis: { stripLine:[{ visible : true }]}
                          
});

{% endhighlight %}




### primaryXAxis.stripLine.width `number`
{:#members:primaryxaxis-stripline-width}




Width of the strip line.


#### Default Value



* 0




#### Example


{% highlight js %}

$("#container").ejChart({

      primaryXAxis: { stripLine:[{ width : 0 }]}
                            
});

{% endhighlight %}




### primaryXAxis.stripLine.zIndex `enum`
{:#members:primaryxaxis-stripline-zindex}

<ts name="ej.datavisualization.Chart.ZIndex"/>
Specifies the order where the strip line and the series have to be rendered. When Z-order is “behind”, strip line is rendered under the series and when it is “over”, it is rendered above the series.


<table class="props">
<thead>
<tr>
<th>Name</th>
<th>Type</th> 
<th class="last">Description</th>
</tr>
</thead>
<tbody>
<tr>
<td class="name">
Inside</td>
<td class="type">string</td> 
<td class="description">Displays the stripline inside the series</td>
</tr>
<tr>
<td class="name">
Over</td>
<td class="type">string</td>
<td class="description">Displays the stripline over the series</td>
</tr> 

</tbody>
</table>


#### Default Value



* "over". See <a href="ejchart.html#members:primaryxaxis-stripline-zindex">ZIndex</a>




#### Example


{% highlight js %}

$("#container").ejChart({

    primaryXAxis: { stripLine:[{ zIndex: "behind" }]}
                          
});

{% endhighlight %}

Try it: [JS Playground Sample](http://jsplayground.syncfusion.com/1at44wzi)


### primaryXAxis.tickLinesPosition `enum`
{:#members:primaryxaxis-ticklinesposition}

<ts name="ej.datavisualization.Chart.TickLinesPosition"/>
Specifies the position of the axis tick lines.


<table class="props">
<thead>
<tr>
<th>Name</th>
<th>Type</th> 
<th class="last">Description</th>
</tr>
</thead>
<tbody>
<tr>
<td class="name">
Inside</td>
<td class="type">string</td> 
<td class="description">The tick lines are placed inside of the axis line</td>
</tr>
<tr>
<td class="name">
Outside</td>
<td class="type">string</td>
<td class="description">The tick lines are placed outside of the axis line</td>
</tr>
</tbody>
</table>






#### Default Value




* "outside". See <a href="ejchart.html#members:primaryxaxis-ticklinesposition">TickLinesPosition</a>




#### Example


{% highlight js %}

$("#container").ejChart({

    primaryXAxis: { tickLinesPosition : "inside" }
                           
});

{% endhighlight %}


### primaryXAxis.labelBorder `object`
{:#members:primaryxaxis-labelborder}




Options for customizing the border of the labels.






### primaryXAxis.labelBorder.color `string`
{:#members:primaryxaxis-labelborder-color}




Specifies the color of the label border.


#### Default Value



* null




#### Example


{% highlight js %}

$("#container").ejChart({

    primaryXAxis: { labelBorder:{color: "green"} }
                      
});

{% endhighlight %}



### primaryXAxis.labelBorder.width `number`
{:#members:primaryxaxis-labelborder-width}




Specifies the width of the label border.


#### Default Value



* 1




#### Example


{% highlight js %}

$("#container").ejChart({

    primaryXAxis: { labelBorder:{width: 2} }
                      
});

{% endhighlight %}



### primaryXAxis.title `object`
{:#members:primaryxaxis-title}




Options for customizing the axis title.






### primaryXAxis.title.enableTrim `boolean`
{:#members:primaryxaxis-title-enabletrim}




Specifies whether to trim the axis title when it exceeds the chart area or the maximum width of the title.


#### Default Value



* false




#### Example


{% highlight js %}

$("#container").ejChart({

    primaryXAxis: { title:{enableTrim:true} }
                      
});

{% endhighlight %}




### primaryXAxis.title.font `object`
{:#members:primaryxaxis-title-font}




Options for customizing the title font.






### primaryXAxis.title.font.fontFamily `string`
{:#members:primaryxaxis-title-font-fontfamily}




Font family of the title text.


#### Default Value



* "Segoe UI"




#### Example


{% highlight js %}

$("#container").ejChart({

    primaryXAxis: { title: { font : { fontFamily : "Algerian"} } }
                      
});

{% endhighlight %}




### primaryXAxis.title.font.fontStyle `enum`
{:#members:primaryxaxis-title-font-fontstyle}

<ts ref="ej.datavisualization.Chart.FontStyle"/>


Font style of the title text.


#### Default Value



* ej.datavisualization.Chart.FontStyle.Normal




#### Example


{% highlight js %}


$("#container").ejChart({

     primaryXAxis: { title: { font : { fontStyle : "Italic"} } }
                      
});

{% endhighlight %}




### primaryXAxis.title.font.fontWeight `enum`
{:#members:primaryxaxis-title-font-fontweight}

<ts ref="ej.datavisualization.Chart.FontWeight"/>


Font weight of the title text.


#### Default Value



* ej.datavisualization.Chart.FontWeight.Regular. See <a href="global.html#enum:fontweight">FontWeight</a>




#### Example


{% highlight js %}

$("#container").ejChart({

     primaryXAxis: { title: { font : { fontWeight : "lighter"} } }
                      
});

{% endhighlight %}




### primaryXAxis.title.font.opacity `number`
{:#members:primaryxaxis-title-font-opacity}




Opacity of the axis title text.


#### Default Value



* 1




#### Example


{% highlight js %}

$("#container").ejChart({

     primaryXAxis: { title: { font : { opacity : 0.8} } }
                           
});

{% endhighlight %}




### primaryXAxis.title.font.size `string`
{:#members:primaryxaxis-title-font-size}




Font size of the axis title.


#### Default Value



* "16px"




#### Example


{% highlight js %}

$("#container").ejChart({

    primaryXAxis: { title: { font : { size : "14px"} } }
                          
});

{% endhighlight %}




### primaryXAxis.title.maximumTitleWidth `number`
{:#members:primaryxaxis-title-maximumtitlewidth}




Maximum width of the title, when the title exceeds this width, the title gets trimmed, when enableTrim is true. 


#### Default Value



* 34




#### Example


{% highlight js %}

$("#container").ejChart({

      primaryYAxis: { title:{maximumTitleWidth: null} }
                            
});

{% endhighlight %}




### primaryXAxis.title.text `string`
{:#members:primaryxaxis-title-text}




Title for the axis.


#### Default Value



* ""




#### Example


{% highlight js %}

$("#container").ejChart({

primaryXAxis: { title: { text: "Year" } }
                      
});

{% endhighlight %}




### primaryXAxis.title.visible `boolean`
{:#members:primaryxaxis-title-visible}




Controls the visibility of axis title.


#### Default Value



* true




#### Example


{% highlight js %}

$("#container").ejChart({

    primaryXAxis: { title: { visible: false } }
                          
});

{% endhighlight %}


### primaryXAxis.title.offset `number`
{:#members:primaryxaxis-title-offset}




offset value for axis title.


#### Default Value



* 0




#### Example


{% highlight js %}

$("#container").ejChart({

    primaryXAxis: { title: { offset: 0 } }
                          
});

{% endhighlight %}

### primaryXAxis.title.position `enum`
{:#members:primaryxaxis-title-position}

<ts ref="ej.datavisualization.Chart.LabelPosition"/>

Specifies the position of the axis title.


#### Default Value



* "outside". See <a href="ejchart.html#members:primaryxaxis-title-position">Position</a>




#### Example


{% highlight js %}

$("#container").ejChart({

    primaryXAxis: { title: { position : "inside" }}
                           
});

{% endhighlight %}

### primaryXAxis.title.alignment `enum`
{:#members:primaryxaxis-title-alignment}

<ts ref="ej.datavisualization.Chart.TextAlignment"/>

Specifies the position of the axis title.


#### Default Value



* "center". See <a href="ejchart.html#members:primaryxaxis-alignment">Alignment</a>




#### Example


{% highlight js %}

$("#container").ejChart({

    primaryXAxis: { title: { alignment : "near" }}
                           
});

{% endhighlight %}



### primaryXAxis.valueType `enum`
{:#members:primaryxaxis-valuetype}

<ts name="ej.datavisualization.Chart.ValueType"/>
Specifies the type of data the axis is handling.


<table class="props">
<thead>
<tr>
<th>Name</th>
<th>Type</th> 
<th class="last">Description</th>
</tr>
</thead>
<tbody>
<tr>
<td class="name">
Double</td>
<td class="type">string</td> 
<td class="description">Specify the numeric axis</td>
</tr>
<tr>
<td class="name">
Category</td>
<td class="type">string</td>
<td class="description">Specify the category axis</td>
</tr> 
<tr>
<td class="name">
DateTime</td>
<td class="type">string</td>
<td class="description">Specify the datetime axis</td>
</tr> 
<tr>
<td class="name">
Logarithmic</td>
<td class="type">string</td>
<td class="description">Specify the logarithmic axis</td>
</tr> 
</tbody>
</table>





#### Default Value




* null. See <a href="ejchart.html#members:primaryxaxis-valuetype">ValueType</a>




#### Example


{% highlight js %}

$("#container").ejChart({

     primaryXAxis: { valueType: "double" }
                           
});

{% endhighlight %}




### primaryXAxis.visible `boolean`
{:#members:primaryxaxis-visible}




Show/hides the axis.


#### Default Value



* true




#### Example


{% highlight js %}

$("#container").ejChart({

    primaryXAxis: { visible: false }
                          
});

{% endhighlight %}




### primaryXAxis.zoomFactor `number`
{:#members:primaryxaxis-zoomfactor}




The axis is scaled by this factor. When zoomFactor is 0.5, the chart is scaled by 200% along this axis. Value ranges from 0 to 1.


#### Default Value



* 1




#### Example


{% highlight js %}

$("#container").ejChart({

    primaryXAxis: { zoomFactor : 0.5 }
                          
});

{% endhighlight %}




### primaryXAxis.zoomPosition `number`
{:#members:primaryxaxis-zoomposition}




Position of the zoomed axis. Value ranges from 0 to 1.



#### Default Value



* 0




#### Example


{% highlight js %}

$("#container").ejChart({

    primaryXAxis: { zoomPosition :0.5 }
                          
});

{% endhighlight %}


### primaryXAxis.scrollbarSettings `object`
{:#members:primaryxaxis-scrollbarsettings}




Options for customizing the axis scrollbar 


### primaryXAxis.scrollbarSettings.visible `boolean`
{:#members:primaryxaxis-scrollbarsettings-visible}




Specifies to enables or disables the scroll bar.


#### Default Value



* false




#### Example


{% highlight js %}

$("#container").ejChart({

    primaryXAxis: { scrollbarSettings:{visible:true} }
                      
});

{% endhighlight %}


### primaryXAxis.scrollbarSettings.canResize `boolean`
{:#members:primaryxaxis-scrollbarsettings-canresize}




Controls whether scrollbar has to be responsive in the chart.


#### Default Value



* false




#### Example


{% highlight js %}

$("#container").ejChart({

    primaryXAxis: { scrollbarSettings:{canResize:true} }
                      
});

{% endhighlight %}



### primaryXAxis.scrollbarSettings.range `object`
{:#members:primaryxaxis-scrollbarsettings-range}


Options to customize the range for the scrollbar in the axis.

 


### primaryXAxis.scrollbarSettings.range.min `number`
{:#members:primaryxaxis-scrollbarsettings-range-min}




Minimum value of the scrollbar range.


#### Default Value

* null




#### Example


{% highlight js %}

$("#container").ejChart({

    primaryXAxis: { scrollbarSettings : { range : { min: 10 } } }
                          
});

{% endhighlight %}


### primaryXAxis.scrollbarSettings.range.max `number`
{:#members:primaryxaxis-scrollbarsettings-range-max}




Maximum value for the scrollbar range .


#### Default Value

* null




#### Example


{% highlight js %}

$("#container").ejChart({

    primaryXAxis: { scrollbarSettings : { range : { max: 100 } } } 
                          
});

{% endhighlight %}


### primaryXAxis.scrollbarSettings.pointsLength `number`
{:#members:primaryxaxis-scrollbarsettings-pointslength}




The maximum number of points to be displayed in the scrollbar. 


#### Default Value

* null




#### Example


{% highlight js %}

$("#container").ejChart({

    primaryXAxis: { scrollbarSettings : { pointsLength : 50 } } 
                          
});

{% endhighlight %}



### axes `array`
{:#members:axes}

To override x axis for particular series, create an axis object by providing unique name by using name property and add it to axes array. Then, assign the name to the series&rsquo;s xAxisName property to link both axis and series.


### axes.alternateGridBand `object`
{:#members:axes-alternategridband}




Options for customizing axis alternate grid band.






### axes.alternateGridBand.even `object`
{:#members:axes-alternategridband-even}




Options for customizing even grid band.






### axes.alternateGridBand.even.fill `string`
{:#members:axes-alternategridband-even-fill}




Fill color for the even grid bands.


#### Default Value



* transparent




#### Example


{% highlight js %}

$("#container").ejChart({

    axes: [{ alternateGridBand: { even :{ fill : "green" } } }]
                        
});

{% endhighlight %}




### axes.alternateGridBand.even.opacity `number`
{:#members:axes-alternategridband-even-opacity}




Opacity of the even grid band.


#### Default Value



* 1




#### Example


{% highlight js %}

$("#container").ejChart({

    axes: [ { alternateGridBand: { even :{ opacity : 0.5 } } } ]
                       
});

{% endhighlight %}

Try it: [JS Playground Sample](http://jsplayground.syncfusion.com/l3nds5td)


### axes.alternateGridBand.odd `object`
{:#members:axes-alternategridband-odd}




Options for customizing odd grid band.






### axes.alternateGridBand.odd.fill `string`
{:#members:axes-alternategridband-odd-fill}




Fill color of the odd grid bands


#### Default Value



* transparent




#### Example


{% highlight js %}
 
$("#container").ejChart({

    axes: [ { alternateGridBand: { odd :{ fill : "red" } } } ]
                          
});

{% endhighlight %}




### axes.alternateGridBand.odd.opacity `number`
{:#members:axes-alternategridband-odd-opacity}




Opacity of odd grid band


#### Default Value



* 1




#### Example


{% highlight js %}

$("#container").ejChart({

    axes: [ { alternateGridBand: { odd :{ opacity : 0.5 } } } ]
                          
});

{% endhighlight %}

Try it: [JS Playground Sample](http://jsplayground.syncfusion.com/0dhpptec)


### axes.crossesAt `number`
{:#members:axes-crossesat}




Specifies where axis should intersect the vertical axis or vice versa. Value should be provided in axis co-ordinates. If provided value is greater than the maximum value of crossing axis, then axis will be placed at the opposite side.


#### Default Value



* null




#### Example


{% highlight js %}

	$("#container").ejChart({

		axes:
		[{
			//Crosses axis at 0
			crossesAt: 0,

			//...
        }],	
	});

{% endhighlight %}



{:#members:axes-crossesinaxis}




Name of the axis used for crossing. Vertical axis name should be provided for horizontal axis and vice versa. If the provided name does not belongs to a valid axis, then primary X axis or primary Y axis will be used for crossing


#### Default Value



* null




#### Example


{% highlight js %}

	$("#container").ejChart({

		axes:
		[ {
			//Crosses axis at -0.2
			crossesAt: -0.2,

			//Crosses in an axis
			crossesInAxis: 'secondaryYAxis',

			//...
        }],
	});

{% endhighlight %}




### axes.isIndexed `boolean`
{:#members:axes-isindexed}




Category axis can also plot points based on index value of data points. Index based plotting can be enabled by setting ‘isIndexed’ property to true.


#### Default Value



* false




#### Example


{% highlight js %}

$("#container").ejChart({

    axes: [ { isIndexed: true }]
                          
});

{% endhighlight %}


### axes.axisLine `object`
{:#members:axes-axisline}




Options for customizing the axis line.  







### axes.axisLine.dashArray `string`
{:#members:axes-axisline-dasharray}




Pattern of dashes and gaps to be applied to the axis line.


#### Default Value



* null




#### Example


{% highlight js %}

$("#container").ejChart({

    axes:[ { axisLine : { dashArray : "2,3" } } ]
                          
});

{% endhighlight %}

Try it: [JS Playground Sample](http://jsplayground.syncfusion.com/3pqlrwwx)


### axes.axisLine.offset `number`
{:#members:axes-axisline-offset}




Padding for axis line. Normally, it is used along with plotOffset to pad the plot area.


#### Default Value



* null




#### Example


{% highlight js %}

$("#container").ejChart({

    axes: [ { axisLine : { offset : 5 } } ]
                          
});

{% endhighlight %}

Try it: [JS Playground Sample](http://jsplayground.syncfusion.com/sokh4rez)


### axes.axisLine.visible `boolean`
{:#members:axes-axisline-visible}




Show/hides the axis line.


#### Default Value



* true




#### Example


{% highlight js %}

$("#container").ejChart({

    axes: [ { axisLine : { visible : false } } ]
                          
});

{% endhighlight %}


### axes.axisLine.color `string`
{:#members:axes-axisline-color}




Color of axis line.


#### Default Value



* ""




#### Example


{% highlight js %}

$("#container").ejChart({

    axes: [ { axisLine : { color : "red" } } ]
                          
});

{% endhighlight %}




### axes.axisLine.width `number`
{:#members:axes-axisline-width}




Width of axis line.


#### Default Value



* 1




#### Example


{% highlight js %}

$("#container").ejChart({

    axes: [ { axisLine : { width : 2 } } ]
                          
});

{% endhighlight %}

Try it: [JS Playground Sample](http://jsplayground.syncfusion.com/nqumidfr)


### axes.columnIndex `number`
{:#members:axes-columnindex}




Specifies the index of the column where the axis is associated, when the chart area is divided into multiple plot areas by using columnDefinitions.


#### Default Value



* null




#### Example


{% highlight js %}

$("#container").ejChart({

     axes: [ { columnIndex: 2 } ]
                           
});

{% endhighlight %}




### axes.columnSpan `number`
{:#members:axes-columnspan}




Specifies the number of columns or plot areas an axis has to span horizontally.


#### Default Value



* null




#### Example


{% highlight js %}

$("#container").ejChart({

    axes: [ { columnSpan: 2 } ]
                          
});

{% endhighlight %}

### axes.crosshairLabel `object`
{:#members:axes-crosshairlabel}




Options to customize the crosshair label.






### axes.crosshairLabel.visible `boolean`
{:#members:axes-crosshairlabel-visible}




Show/hides the crosshair label associated with this axis.


#### Default Value



* false




#### Example


{% highlight js %}

$("#container").ejChart({

    axes: [ { crosshairLabel : { visible : true} } ]
                          
});

{% endhighlight %}

### axes.desiredIntervals `number`
{:#members:axes-desiredintervals}




With this setting, you can request axis to calculate intervals approximately equal to your desired interval.


#### Default Value



* null




#### Example


{% highlight js %}

$("#container").ejChart({

     axes: [{ desiredIntervals: 5 }]
                           
});

{% endhighlight %}


### axes.labelPlacement `enum`
{:#members:axes-labelplacement}

<ts ref="ej.datavisualization.Chart.LabelPlacement"/>

Specifies the placement of labels. 


#### Default Value



* ej.datavisualization.Chart.LabelPlacement.BetweenTicks. See <a href="ejchart.html#members:primaryxaxis-labelplacement">LabelPlacement</a>


#### Example


{% highlight js %}

$("#container").ejChart({

    axes:[ { labelPlacement : "onTicks" } ]
                          
});

{% endhighlight %}



### axes.edgeLabelPlacement `enum`
{:#members:axes-edgelabelplacement}

<ts ref="ej.datavisualization.Chart.EdgeLabelPlacement"/>

Specifies the position of labels at the edge of the axis. 

#### Default Value



* ej.datavisualization.Chart.EdgeLabelPlacement.None. See <a href="ejchart.html#members:primaryxaxis-edgelabelplacement">EdgeLabelPlacement</a>




#### Example


{% highlight js %}

$("#container").ejChart({

    axes: [ { edgeLabelPlacement : "shift" } ]
                          
});

{% endhighlight %}

Try it: [JS Playground Sample](http://jsplayground.syncfusion.com/zff5idq4)


### axes.enableTrim `boolean`
{:#members:axes-enabletrim}




Specifies whether to trim the axis label when the width of the label exceeds the maximumLabelWidth.


#### Default Value



* false




#### Example


{% highlight js %}

$("#container").ejChart({

    axes:[ { enableTrim : true } ]
                          
});

{% endhighlight %}



### axes.enableAutoIntervalOnZooming `boolean`
{:#members:axes-enableautointervalonzooming}


Specifies the interval of the axis according to the zoomed data of the chart. 


#### Default Value



* true




#### Example


{% highlight js %}

$("#container").ejChart({

    axes:[ { enableAutoIntervalOnZooming : true } ]   
                          
});

{% endhighlight %}



### axes.font `object`
{:#members:axes-font}




Options for customizing the font of the axis Labels.






### axes.font.fontFamily `string`
{:#members:axes-font-fontfamily}




Font family of labels.


#### Default Value



* "Segoe UI"




#### Example


{% highlight js %}

$("#container").ejChart({

     axes: [ { font : { fontFamily : "Algerian"} } ]
                           
});

{% endhighlight %}




### axes.font.fontStyle `enum`
{:#members:axes-font-fontstyle}

<ts ref="ej.datavisualization.Chart.FontStyle"/>



Font style of labels.


#### Default Value




* ej.datavisualization.Chart.FontStyle.Normal. See <a href="global.html#enum:fontstyle">FontStyle</a>




#### Example


{% highlight js %}

$("#container").ejChart({

    axes:[ { font : { fontStyle : "Italic"} } ]
                          
});

{% endhighlight %}




### axes.font.fontWeight `enum`
{:#members:axes-font-fontweight}

<ts ref="ej.datavisualization.Chart.FontWeight"/>


Font weight of the label.


#### Default Value



* ej.datavisualization.Chart.FontWeight.Regular. See <a href="global.html#enum:fontweight">FontWeight</a>




#### Example


{% highlight js %}

$("#container").ejChart({

     axes: [{ font : { fontWeight : "lighter"} }]
                           
});

{% endhighlight %}




### axes.font.opacity `number`
{:#members:axes-font-opacity}




Opacity of the axis labels.


#### Default Value



* 1




#### Example


{% highlight js %}

$("#container").ejChart({

    axes: [{ font : { opacity : 0.5} }]
                          
});

{% endhighlight %}




### axes.font.size `string`
{:#members:axes-font-size}




Font size of the axis labels.


#### Default Value



* "13px"




#### Example


{% highlight js %}

$("#container").ejChart({

     axes:[ { font : { size : "12px"} } ]
                           
});

{% endhighlight %}

Try it: [JS Playground Sample](http://jsplayground.syncfusion.com/5x5zgpnf)


### axes.intervalType `enum`
{:#members:axes-intervaltype}

<ts ref="ej.datavisualization.Chart.IntervalType"/>

Specifies the type of interval in date time axis.


#### Default Value


* null. See <a href="ejchart.html#members:primaryxaxis-intervaltype">IntervalType</a>


#### Example


{% highlight js %}

$("#container").ejChart({

     axes: [{ intervalType: "days" }]
                           
});

{% endhighlight %}


### axes.isInversed `boolean`
{:#members:axes-isinversed}




Specifies whether to inverse the axis.


#### Default Value



* false




#### Example


{% highlight js %}

$("#container").ejChart({

     axes:[{ isInversed : true}]
                           
});

{% endhighlight %}

Try it: [JS Playground Sample](http://jsplayground.syncfusion.com/izzaexfa)


### axes.labelFormat `string`
{:#members:axes-labelformat}




Custom formatting for axis label and supports all standard formatting type of numerical and date time values.


#### Default Value



* null




#### Example


{% highlight js %}

$("#container").ejChart({

    axes:[ { labelFormat: "{value}%" } ]
                          
});

{% endhighlight %}

Try it: [JS Playground Sample](http://jsplayground.syncfusion.com/wurgvm33)


### axes.labelIntersectAction `enum`
{:#members:axes-labelintersectaction}

<ts ref="ej.datavisualization.Chart.LabelIntersectAction"/>

Specifies the action to take when the axis labels are overlapping with each other. 


#### Default Value



* ej.datavisualization.Chart.LabelIntersectAction.None. See <a href="ejchart.html#members:primaryxaxis-labelintersectaction">LabelIntersectAction</a>




#### Example


{% highlight js %}

$("#container").ejChart({

    axes:[{ labelIntersectAction : "multipleRows" }]
                          
});

{% endhighlight %}


### axes.labelPosition `enum`
{:#members:axes-labelposition}

<ts ref="ej.datavisualization.Chart.LabelPosition"/>

Specifies the position of the axis labels.


#### Default Value



* "outside". See <a href="ejchart.html#members:primaryxaxis-labelposition">LabelPosition</a>




#### Example


{% highlight js %}

$("#container").ejChart({

    axes:[{ labelPosition : "inside" }]
                       
});

{% endhighlight %}

Try it: [JS Playground Sample](http://jsplayground.syncfusion.com/4qljgc5m)



### axes.alignment `enum`
{:#members:axes-alignment}

<ts ref="ej.datavisualization.Chart.LabelAlignment"/>

Specifies the position of the axis labels.



#### Default Value



* "center". See <a href="ejchart.html#members:primaryxaxis-alignment">Alignment</a>




#### Example


{% highlight js %}

$("#container").ejChart({

    axes:[{ alignment : "far" }]
                       
});

{% endhighlight %}



### axes.labelRotation `number`
{:#members:axes-labelrotation}




Angle in degrees to rotate the axis labels.


#### Default Value



* null




#### Example


{% highlight js %}

$("#container").ejChart({

    axes: [{ labelRotation: 90 }]
                          
});

{% endhighlight %}



### axes.logBase `number`
{:#members:axes-logbase}




Logarithmic base value. This is applicable only for logarithmic axis.


#### Default Value



* 10




#### Example


{% highlight js %}

$("#container").ejChart({

    axes: [{ logBase: 5 }]
                          
});

  {% endhighlight %}




### axes.majorGridLines `object`
{:#members:axes-majorgridlines}




Options for customizing major gird lines.






### axes.majorGridLines.dashArray `string`
{:#members:axes-majorgridlines-dasharray}




Pattern of dashes and gaps used to stroke the major grid lines.


#### Default Value



* null




#### Example


{% highlight js %}

$("#container").ejChart({

    axes: [{ majorGridLines: { dashArray : "2,3"} }]
                          
});

{% endhighlight %}



### axes.majorGridLines.color `string`
{:#members:axes-majorgridlines-color}




Color of the major grid line.


#### Default Value



* null




#### Example


{% highlight js %}

$("#container").ejChart({

    axes:[{ majorGridLines: { color : "red"} }]
                          
});

{% endhighlight %}




### axes.majorGridLines.opacity `number`
{:#members:axes-majorgridlines-opacity}




Opacity of major grid lines.


#### Default Value



* 1




#### Example


{% highlight js %}

$("#container").ejChart({

    axes: [{ majorGridLines: { opacity: 0.5 } }]
                          
});

{% endhighlight %}




### axes.majorGridLines.visible `boolean`
{:#members:axes-majorgridlines-visible}




Show/hides the major grid lines.


#### Default Value



* true




#### Example


{% highlight js %}

$("#container").ejChart({

    axes:[{ majorGridLines: { visible: false } }]
                          
});

{% endhighlight %}




### axes.majorGridLines.width `number`
{:#members:axes-majorgridlines-width}




Width of the major grid lines.


#### Default Value



* 1




#### Example


{% highlight js %}

$("#container").ejChart({

    axes: [{ majorGridLines: { width : 0.5} }]
                          
});

{% endhighlight %}

Try it: [JS Playground Sample](http://jsplayground.syncfusion.com/53i5levx)


### axes.majorTickLines `object`
{:#members:axes-majorticklines}




Options for customizing the major tick lines.






### axes.majorTickLines.size `number`
{:#members:axes-majorticklines-size}




Length of the major tick lines.


#### Default Value



* 5




#### Example


{% highlight js %}

$("#container").ejChart({

    axes: [{ majorTickLines: { size: 2 } }]
                          
});

{% endhighlight %}




### axes.majorTickLines.visible `boolean`
{:#members:axes-majorticklines-visible}




Show/hides the major tick lines.


#### Default Value



* true




#### Example


{% highlight js %}

$("#container").ejChart({

    axes: [{ majorTickLines: { visible: false } }]
                          
});

{% endhighlight %}




### axes.majorTickLines.width `number`
{:#members:axes-majorticklines-width}




Width of the major tick lines.


#### Default Value



* 1




#### Example


{% highlight js %}

$("#container").ejChart({

    axes: [{ majorTickLines: { width: 2 } }]
                          
});

{% endhighlight %}

Try it: [JS Playground Sample](http://jsplayground.syncfusion.com/w1ii251s)


### axes.maximumLabels `number`
{:#members:axes-maximumlabels}




Maximum number of labels to be displayed in every 100 pixels.


#### Default Value



* 3




#### Example


{% highlight js %}

$("#container").ejChart({

    axes:[{ maximumLabels : 5 }]
                          
});

{% endhighlight %}



### axes.maximumLabelWidth `number`
{:#members:axes-maximumlabelwidth}




Maximum width of the axis label. When the label exceeds the width, the label gets trimmed when the enableTrim is set to true.


#### Default Value



* 34




#### Example


{% highlight js %}

$("#container").ejChart({

     axes: [{ maximumLabelWidth :34.5 }]
                           
});

{% endhighlight %}




### axes.minorGridLines `object`
{:#members:axes-minorgridlines}




Options for customizing the minor grid lines.






### axes.minorGridLines.dashArray `string`
{:#members:axes-minorgridlines-dasharray}




Patterns of dashes and gaps used to stroke the minor grid lines.


#### Default Value



* null




#### Example


{% highlight js %}

$("#container").ejChart({

    axes: [{ minorGridLines: { dashArray: "2,3" } }]
                          
});

{% endhighlight %}




### axes.minorGridLines.visible `boolean`
{:#members:axes-minorgridlines-visible}




Show/hides the minor grid lines.


#### Default Value



* true




#### Example


{% highlight js %}

$("#container").ejChart({

    axes: [{ minorGridLines: { visible: true } }]
                          
});

{% endhighlight %}




### axes.minorGridLines.width `number`
{:#members:axes-minorgridlines-width}




Width of the minorGridLines.


#### Default Value



* 1




#### Example


{% highlight js %}

$("#container").ejChart({

    axes: [{ minorGridLines: { width: 2 } }]
                          
});

{% endhighlight %}

Try it: [JS Playground Sample](http://jsplayground.syncfusion.com/uuofmzcq)


### axes.minorTickLines `object`
{:#members:axes-minorticklines}




Options for customizing the minor tick lines.






### axes.minorTickLines.size `number`
{:#members:axes-minorticklines-size}




Length of the minor tick lines.


#### Default Value



* 5




#### Example


{% highlight js %}

$("#container").ejChart({

    axes: [{ minorTickLines: { size: 2 } }]
                          
});

{% endhighlight %}




### axes.minorTickLines.visible `boolean`
{:#members:axes-minorticklines-visible}




Show/hides the minor tick lines.


#### Default Value



* true




#### Example


{% highlight js %}

$("#container").ejChart({

    axes: [{ minorTickLines: { visible: true } }]
                          
});

{% endhighlight %}




### axes.minorTickLines.width `number`
{:#members:axes-minorticklines-width}




Width of the minor tick line.


#### Default Value



* 1




#### Example


{% highlight js %}

$("#container").ejChart({
 
    axes: [{ minorTickLines: { width: 2 } }]
                          
});

{% endhighlight %}




### axes.minorTicksPerInterval `number`
{:#members:axes-minorticksperinterval}




Specifies the number of minor ticks per interval.


#### Default Value



* null




#### Example


{% highlight js %}

$("#container").ejChart({
 
    axes: [{ minorTicksPerInterval: 5 }]
                          
});

{% endhighlight %}


### axes.name `string`
{:#members:axes-name}




Unique name of the axis. To associate an axis with the series, you have to set this name to the xAxisName/yAxisName property of the series.


#### Default Value



* null




#### Example


{% highlight js %}

$("#container").ejChart({

    axes: [{ name: "xAxis" }]
                          
});

{% endhighlight %}




### axes.opposedPosition `boolean`
{:#members:axes-opposedposition}




Specifies whether to render the axis at the opposite side of its default position.


#### Default Value



* false




#### Example


{% highlight js %}

$("#container").ejChart({

    axes: [{ opposedPosition : true }]
                          
});

{% endhighlight %}



### axes.orientation `enum`
{:#members:axes-orientation}


<ts ref="ej.datavisualization.Chart.AxisOrientation"/>

Specifies the orientation of the axis line in the chart.


#### Default Value



* 'horizontal'




#### Example


{% highlight js %}

$("#container").ejChart({

    axes: [{ orientation : 'vertical' }]
                          
});

{% endhighlight %}




### axes.plotOffset `number`
{:#members:axes-plotoffset}




Specifies the padding for the plot area.


#### Default Value



* 10




#### Example


{% highlight js %}

$("#container").ejChart({

    axes: [{ plotOffset: 0 }]
                          
});

{% endhighlight %}

Try it: [JS Playground Sample](http://jsplayground.syncfusion.com/mqb1dwpy)


### axes.range `object`
{:#members:axes-range}




Options to customize the range of the axis.

Try it: [JS Playground Sample](http://jsplayground.syncfusion.com/t2ogn4fa)


### axes.range.min `number`
{:#members:axes-range-min}




Minimum value of the axis range.


#### Default Value

* null




#### Example


{% highlight js %}

$("#container").ejChart({

    axes: [{ range : { min: 10 } }]
                          
});

{% endhighlight %}


### axes.range.max `number`
{:#members:axes-range-max}




Maximum value of the axis range.


#### Default Value

* null




#### Example


{% highlight js %}

$("#container").ejChart({

    axes: [{ range : { max: 100 } }]
                          
});

{% endhighlight %}


### axes.range.interval `number`
{:#members:axes-range-interval}




Interval of the axis range.


#### Default Value

* null




#### Example


{% highlight js %}

$("#container").ejChart({

    axes: [{ range : { interval: 10 } }]
                          
});

{% endhighlight %}


### axes.rangePadding `enum`
{:#members:axes-rangepadding}

<ts ref="ej.datavisualization.Chart.RangePadding"/>

Specifies the padding for the axis range.
#### Default Value


* "None". See <a href="ejchart.html#members::primaryxaxis-rangepadding">RangePadding</a>




#### Example


{% highlight js %}

$("#container").ejChart({

    axes: [{ rangePadding : "normal" }]
                          
});

{% endhighlight %}




### axes.roundingPlaces `number`
{:#members:axes-roundingplaces}




Rounds the number to the given number of decimals.


#### Default Value



* null




#### Example


{% highlight js %}

$("#container").ejChart({

    axes: [{ roundingPlaces: 3 }]
                          
});

{% endhighlight %}


Try it: [JS Playground Sample](http://jsplayground.syncfusion.com/ccisbode)


### axes.multiLevelLabels `array`
{:#members:axes-multilevellabels}


Options for customizing the multi level labels.


#### Default Value



* [ ]







### axes.multiLevelLabels.visible `boolean`
{:#members:axes-multilevellabels-visible}




Visibility of the multi level labels.


#### Default Value



* false




#### Example


{% highlight js %}

$("#container").ejChart({
 
    axes: [{ multiLevelLabels:[{ visible: true }]}]
                          
});

{% endhighlight %}


### axes.multiLevelLabels.text `string`
{:#members:axes-multilevellabels-text}




Text of the multi level labels.


#### Default Value



* ""




#### Example


{% highlight js %}

$("#container").ejChart({
 
    axes: [{ multiLevelLabels:[{ text: "2016" }]}]
                          
});

{% endhighlight %}


### axes.multiLevelLabels.start `object`
{:#members:axes-multilevellabels-start}




Starting value of the multi level labels.


#### Default Value



* null




#### Example


{% highlight js %}

$("#container").ejChart({
 
    axes: [{ multiLevelLabels:[{ start: 1 }]}]
                          
});

{% endhighlight %}

### axes.multiLevelLabels.end `object`
{:#members:axes-multilevellabels-end}




Ending value of the multi level labels.


#### Default Value



* null




#### Example


{% highlight js %}

$("#container").ejChart({
 
    axes: [{ multiLevelLabels:[{ end: 4 }]}]
                          
});

{% endhighlight %}


### axes.multiLevelLabels.level `number`
{:#members:axes-multilevellabels-level}




Specifies the level of multi level labels.


#### Default Value



* 0




#### Example


{% highlight js %}

$("#container").ejChart({
 
    axes: [{ multiLevelLabels:[{ level: 2 }]}]
                          
});

{% endhighlight %}


### axes.multiLevelLabels.maximumTextWidth `number`
{:#members:axes-multilevellabels-maximumtextwidth}




Specifies the maximum width of the text in multi level labels.


#### Default Value



* null




#### Example


{% highlight js %}

$("#container").ejChart({
 
    axes: [{ multiLevelLabels:[{ maximumTextWidth: 30 }]}]
                          
});

{% endhighlight %}



### axes.multiLevelLabels.textAlignment `enum`
{:#members:axes-multilevellabels-textalignment}

<ts ref="ej.datavisualization.Chart.TextAlignment"/>


Specifies the alignment of the text in multi level labels.


#### Default Value



* "center". See <a href="ejchart.html#members:primaryxaxis-stripline-textalignment">TextAlignment</a>




#### Example


{% highlight js %}

$("#container").ejChart({
 
    axes: [{ multiLevelLabels:[{ textAlignment: "near" }]}]
                          
});

{% endhighlight %}


### axes.multiLevelLabels.textOverflow `enum`
{:#members:axes-multilevellabels-textoverflow}

<ts ref="ej.datavisualization.Chart.TextOverflow"/>


Specifies the handling of text over flow in multi level labels.


#### Default Value



* "center". See <a href="ejchart.html#members:legend-textoverflow">TextOverflow</a>




#### Example


{% highlight js %}

$("#container").ejChart({
 
    axes: [{ multiLevelLabels:[{ textOverflow: "trim" }]}]
                          
});

{% endhighlight %}



### axes.multiLevelLabels.font `object`
{:#members:axes-multilevellabels-font}




Options for customizing the font of the text.






### axes.multiLevelLabels.font.color `string`
{:#members:axes-multilevellabels-font-color}




Font color of the multi level labels text.


#### Default Value



* null




#### Example


{% highlight js %}

$("#container").ejChart({

     axes: [{ multiLevelLabels:[{ font : { color: "green"} }]}]
                           
});

{% endhighlight %}




### axes.multiLevelLabels.font.fontFamily `string`
{:#members:axes-multilevellabels-font-fontfamily}




Font family of the multi level labels text.


#### Default Value



* "Segoe UI"




#### Example


{% highlight js %}

$("#container").ejChart({

    axes: [{ multiLevelLabels:[{ font : { fontFamily : "Algerian"} }]}]
                          
});

{% endhighlight %}




### axes.multiLevelLabels.font.fontStyle `enum`
{:#members:axes-multilevellabels-font-fontstyle}

<ts ref="ej.datavisualization.Chart.FontStyle"/>


Font style of the multi level labels text.


#### Default Value



* "Normal"




#### Example


{% highlight js %}

$("#container").ejChart({ 

    axes: [{ multiLevelLabels:[{ font : { fontStyle: "Bold"} }]}]
                          
});

{% endhighlight %}




### axes.multiLevelLabels.font.fontWeight `string`
{:#members:axes-multilevellabels-font-fontweight}




Font weight of the multi level label text.


#### Default Value



* "regular"




#### Example


{% highlight js %}

$("#container").ejChart({

      axes: [{ multiLevelLabels:[{ font : { fontWeight: "lighter"} }]}]
                            
});

{% endhighlight %}




### axes.multiLevelLabels.font.opacity `number`
{:#members:axes-multilevellabels-font-opacity}




Opacity of the multi level label text.


#### Default Value



* 1




#### Example


{% highlight js %}

$("#container").ejChart({

axes: [{ multiLevelLabels:[{ font : { opacity: 0.5} }]}]
                      
});

{% endhighlight %}




### axes.multiLevelLabels.font.size `string`
{:#members:axes-multilevellabels-font-size}




Font size of the multi level label text.


#### Default Value



* "12px"




#### Example


{% highlight js %}

$("#container").ejChart({

        axes: [{ multiLevelLabels:[{ font : { size: "15px"} }]}]
                              
});

{% endhighlight %}


### axes.multiLevelLabels.border `object`
{:#members:axes-multilevellabels-border}




Options for customizing the border of the series.






### axes.multiLevelLabels.border.color `string`
{:#members:axes-multilevellabels-border-color}




Border color of the multi level labels.


#### Default Value



*  null




#### Example


{% highlight js %}
 
 
$("#container").ejChart({
        axes: [{ multiLevelLabels:[{border :{ color : "green" } }]}]                 
});
{% endhighlight %}




### axes.multiLevelLabels.border.width `number`
{:#members:axes-multilevellabels-border-width}




Border width of the multi level labels.


#### Default Value



* 1




#### Example


{% highlight js %}
 

$("#container").ejChart({
        axes: [{ multiLevelLabels:[{border :{ width : 2 } }]}]                  
});
{% endhighlight %}


### axes.multiLevelLabels.border.type `enum`
{:#members:axes-multilevellabels-border-type}


<ts ref="ej.datavisualization.Chart.MultiLevelLabelsBorderType"/>


Border type of the multi level labels.

#### Default Value



* "rectangle". See <a href="ejchart.html#members:primaryxaxis-multilevellabels-border-type">Type</a>




#### Example


{% highlight js %}
 

$("#container").ejChart({
        axes: [{ multiLevelLabels:[{border :{ type : "brace" } }]}]                  
});
{% endhighlight %}


### axes.showNextToAxisLine `boolean`
{:#members:axes-shownexttoaxisline}



Specifies whether the axis elements need to be placed nearby the axis line, while crossing.



#### Default Value



* true




#### Example


{% highlight js %}

$("#container").ejChart({

    axes: [{ showNextToAxisLine : false }]
                          
});

{% endhighlight %}





### axes.stripLine `array`
{:#members:axes-stripline}


Options for customizing the strip lines.


#### Default Value



* [ ]







### axes.stripLine.borderColor `string`
{:#members:axes-stripline-bordercolor}




Border color of the strip line.


#### Default Value



* "gray"




#### Example


{% highlight js %}

$("#container").ejChart({
 
    axes: [{ stripLine:[{ borderColor: "green" }]}]
                          
});

{% endhighlight %}




### axes.stripLine.color `string`
{:#members:axes-stripline-color}




Background color of the strip line.


#### Default Value



* "gray"




#### Example


{% highlight js %}

$("#container").ejChart({

    axes: [{ stripLine:[{ color: "green" }]}]
                          
});

{% endhighlight %}




### axes.stripLine.end `number`
{:#members:axes-stripline-end}




End value of the strip line.


#### Default Value



* null




#### Example


{% highlight js %}

$("#container").ejChart({

     axes: [{ stripLine:[{ end: 5 }]}]
                           
});

{% endhighlight %}




### axes.stripLine.font `object`
{:#members:axes-stripline-font}




Options for customizing the font of the text.






### axes.stripLine.font.color `string`
{:#members:axes-stripline-font-color}




Font color of the strip line text.


#### Default Value



* "black"




#### Example


{% highlight js %}

$("#container").ejChart({

     axes: [{ stripLine:[{ font : { color: "green"} }]}]
                           
});

{% endhighlight %}




### axes.stripLine.font.fontFamily `string`
{:#members:axes-stripline-font-fontfamily}




Font family of the strip line text.


#### Default Value



* "Segoe UI"




#### Example


{% highlight js %}

$("#container").ejChart({

    axes: [{ stripLine:[{ font : { fontFamily : "Algerian"} }]}]
                          
});

{% endhighlight %}




### axes.stripLine.font.fontStyle `enum`
{:#members:axes-stripline-font-fontstyle}

<ts ref="ej.datavisualization.Chart.FontStyle"/>


Font style of the strip line text.


#### Default Value



* "Normal"




#### Example


{% highlight js %}

$("#container").ejChart({ 

    axes: [{ stripLine:[{ font : { fontStyle: "Bold"} }]}]
                          
});

{% endhighlight %}




### axes.stripLine.font.fontWeight `string`
{:#members:axes-stripline-font-fontweight}




Font weight of the strip line text.


#### Default Value



* "regular"




#### Example


{% highlight js %}

$("#container").ejChart({

      axes: [{ stripLine:[{ font : { fontWeight: "lighter"} }]}]
                            
});

{% endhighlight %}




### axes.stripLine.font.opacity `number`
{:#members:axes-stripline-font-opacity}




Opacity of the strip line text.


#### Default Value



* 1




#### Example


{% highlight js %}

$("#container").ejChart({

axes: [{ stripLine:[{ font : { opacity: 0.5} }]}]
                      
});

{% endhighlight %}




### axes.stripLine.font.size `string`
{:#members:axes-stripline-font-size}




Font size of the strip line text.


#### Default Value



* "12px"




#### Example


{% highlight js %}

$("#container").ejChart({

        axes: [{ stripLine:[{ font : { size: "15px"} }]}]
                              
});

{% endhighlight %}




### axes.stripLine.start `number`
{:#members:axes-stripline-start}




Start value of the strip line.


#### Default Value



* null




#### Example


{% highlight js %}

$("#container").ejChart({

     axes: [{ stripLine:[{ start: 2 }]}]
                           
});

{% endhighlight %}




### axes.stripLine.startFromAxis `boolean`
{:#members:axes-stripline-startfromaxis}




Indicates whether to render the strip line from the minimum/start value of the axis. This property does not work when start property is set.


#### Default Value



* false




#### Example


{% highlight js %}

$("#container").ejChart({

    axes: [{ stripLine:[{ startFromAxis : true }]}]
                          
});

{% endhighlight %}




### axes.stripLine.text `string`
{:#members:axes-stripline-text}




Specifies text to be displayed inside the strip line.


#### Default Value



* "stripLine"




#### Example


{% highlight js %}

$("#container").ejChart({
 
    axes: [{ stripLine:[{ text : "Empty Point" }]}]
                           
});

{% endhighlight %}




### axes.stripLine.textAlignment `enum`
{:#members:axes-stripline-textalignment}

<ts ref="ej.datavisualization.Chart.TextAlignment"/>

Specifies the alignment of the text inside the strip line.




#### Default Value



* "middlecenter". See <a href="ejchart.html#members:legend-title-textalignment">TextAlignment</a>




#### Example


{% highlight js %}

$("#container").ejChart({

     axes: [{ stripLine:[{ textAlignment : "middletop" }]}]
                           
});

{% endhighlight %}




### axes.stripLine.visible `boolean`
{:#members:axes-stripline-visible}




Show/hides the strip line.


#### Default Value



* false




#### Example


{% highlight js %}

$("#container").ejChart({

    axes: [{ stripLine:[{ visible : true }]}]
                          
});

{% endhighlight %}




### axes.stripLine.width `number`
{:#members:axes-stripline-width}




Width of the strip line.


#### Default Value



* 0




#### Example


{% highlight js %}

$("#container").ejChart({

      axes: [{ stripLine:[{ width : 0 }]}]
                            
});

{% endhighlight %}




### axes.stripLine.zIndex `enum`
{:#members:axes-stripline-zindex}

<ts ref="ej.datavisualization.Chart.ZIndex"/>

Specifies the order where the strip line and the series have to be rendered. When Z-order is “behind”, strip line is rendered under the series and when it is “over”, it is rendered above the series.


#### Default Value



* "over". See <a href="ejchart.html#members:primaryxaxis-stripline-zindex">ZIndex</a>




#### Example


{% highlight js %}

$("#container").ejChart({

    axes: [{ stripLine:[{ zIndex: "behind" }]}]
                          
});

{% endhighlight %}

Try it: [JS Playground Sample](http://jsplayground.syncfusion.com/vuduvnu1)


### axes.tickLinesPosition `enum`
{:#members:axes-ticklinesposition}

<ts ref="ej.datavisualization.Chart.TickLinesPosition"/>

Specifies the position of the axis tick lines.



#### Default Value




* "outside". See <a href="ejchart.html#members:primaryxaxis-ticklinesposition">TickLinesPosition</a>




#### Example


{% highlight js %}

$("#container").ejChart({

    axes: [{ tickLinesPosition : "inside" }]
                           
});

{% endhighlight %}


### axes.labelBorder `object`
{:#members:axes-labelborder}




Options for customizing the border of the labels.






### axes.labelBorder.color `string`
{:#members:axes-labelborder-color}




Specifies the color of the label border.


#### Default Value



* null




#### Example


{% highlight js %}

$("#container").ejChart({

    axes: [{ labelBorder:{color: "green"} }]
                      
});

{% endhighlight %}



### axes.labelBorder.width `number`
{:#members:axes-labelborder-width}




Specifies the width of the label border.


#### Default Value



* 1




#### Example


{% highlight js %}

$("#container").ejChart({

    axes: [{ labelBorder:{width: 2} }]
                      
});

{% endhighlight %}



### axes.title `object`
{:#members:axes-title}




Options for customizing the axis title.






### axes.title.enableTrim `boolean`
{:#members:axes-title-enabletrim}




Specifies whether to trim the axis title when it exceeds the chart area or the maximum width of the title.


#### Default Value



* false




#### Example


{% highlight js %}

$("#container").ejChart({

    axes:[{ title:{enableTrim:true} }]
                      
});

{% endhighlight %}




### axes.title.font `object`
{:#members:axes-title-font}




Options for customizing the title font.






### axes.title.font.fontFamily `string`
{:#members:axes-title-font-fontfamily}




Font family of the title text.


#### Default Value



* "Segoe UI"




#### Example


{% highlight js %}

$("#container").ejChart({

    axes:[ { title: { font : { fontFamily : "Algerain"} } } ]
                      
});

{% endhighlight %}




### axes.title.font.fontStyle `enum`
{:#members:axes-title-font-fontstyle}

<ts ref="ej.datavisualization.Chart.FontStyle"/>


Font style of the title text.


#### Default Value



* ej.datavisualization.Chart.FontStyle.Normal




#### Example


{% highlight js %}


$("#container").ejChart({

     axes: [{ title: { font : { fontStyle : "Italic"} } }]
                      
});

{% endhighlight %}




### axes.title.font.fontWeight `enum`
{:#members:axes-title-font-fontweight}

<ts ref="ej.datavisualization.Chart.FontWeight"/>


Font weight of the title text.


#### Default Value



* ej.datavisualization.Chart.FontWeight.Regular. See <a href="global.html#enum:fontweight">FontWeight</a>




#### Example


{% highlight js %}

$("#container").ejChart({

     axes: [{ title: { font : { fontWeight : "lighter"} } }]
                      
});

{% endhighlight %}




### axes.title.font.opacity `number`
{:#members:axes-title-font-opacity}




Opacity of the axis title text.


#### Default Value



* 1




#### Example


{% highlight js %}

$("#container").ejChart({

     axes: [{ title: { font : { opacity : 0.8} } }]
                           
});

{% endhighlight %}




### axes.title.font.size `string`
{:#members:axes-title-font-size}




Font size of the axis title.


#### Default Value



* "16px"




#### Example


{% highlight js %}

$("#container").ejChart({

    axes: [{ title: { font : { size : "14px"} } }]
                          
});

{% endhighlight %}




### axes.title.maximumTitleWidth `number`
{:#members:axes-title-maximumtitlewidth}




Maximum width of the title, when the title exceeds this width, the title gets trimmed, when enableTrim is true. 


#### Default Value



* 34




#### Example


{% highlight js %}

$("#container").ejChart({

      axes: [{ title:{maximumTitleWidth: null} }]
                            
});

{% endhighlight %}




### axes.title.text `string`
{:#members:axes-title-text}




Title for the axis.


#### Default Value



* ""




#### Example


{% highlight js %}

$("#container").ejChart({

axes: [{ title: { text: "Year" } }]
                      
});

{% endhighlight %}




### axes.title.visible `boolean`
{:#members:axes-title-visible}




Controls the visibility of axis title.


#### Default Value



* true




#### Example


{% highlight js %}

$("#container").ejChart({

    axes:[{ title: { visible: false } }]
                          
});

{% endhighlight %}


### axes.title.offset `number`
{:#members:axes-title-offset}




offset value for axis title.


#### Default Value



* 0




#### Example


{% highlight js %}

$("#container").ejChart({

    axes: [{ title: { offset: 0 } }]
                          
});

{% endhighlight %}

### axes.title.position `enum`
{:#members:axes-title-position}

<ts ref="ej.datavisualization.Chart.LabelPosition"/>

Specifies the position of the axis title.


#### Default Value



* "outside". See <a href="ejchart.html#members:axes-title-position">Position</a>




#### Example


{% highlight js %}

$("#container").ejChart({

    axes: [{ title: { position : "inside" }}]
                           
});

{% endhighlight %}

### axes.title.alignment `enum`
{:#members:axes-title-alignment}

<ts ref="ej.datavisualization.Chart.TextAlignment"/>

Specifies the position of the axis title.


#### Default Value



* "center". See <a href="ejchart.html#members:axes-title-alignment">Alignment</a>




#### Example


{% highlight js %}

$("#container").ejChart({

    axes: [{ title: { alignment : "near" }}]
                           
});

{% endhighlight %}



### axes.valueType `enum`
{:#members:axes-valuetype}

<ts ref="ej.datavisualization.Chart.ValueType"/>

Specifies the type of data the axis is handling.




#### Default Value




* null. See <a href="ejchart.html#members:primaryxaxis-valuetype">ValueType</a>




#### Example


{% highlight js %}

$("#container").ejChart({

     axes: [{ valueType: "double" }]
                           
});

{% endhighlight %}




### axes.visible `boolean`
{:#members:axes-visible}




Show/hides the axis.


#### Default Value



* true




#### Example


{% highlight js %}

$("#container").ejChart({

    axes: [{ visible: false }]
                          
});

{% endhighlight %}




### axes.zoomFactor `number`
{:#members:axes-zoomfactor}




The axis is scaled by this factor. When zoomFactor is 0.5, the chart is scaled by 200% along this axis. Value ranges from 0 to 1.


#### Default Value



* 1




#### Example


{% highlight js %}

$("#container").ejChart({

    axes: [{ zoomFactor : 0.5 }]
                          
});

{% endhighlight %}




### axes.zoomPosition `number`
{:#members:axes-zoomposition}




Position of the zoomed axis. Value ranges from 0 to 1.



#### Default Value



* 0




#### Example


{% highlight js %}

$("#container").ejChart({

    axes: [{ zoomPosition :0.5 }]
                          
});

{% endhighlight %}

### axes.scrollbarSettings `object`
{:#members:axes-scrollbarsettings}




Options for customizing the axis scrollbar.


### axes.scrollbarSettings.visible `boolean`
{:#members:axes-scrollbarsettings-visible}




Specifies to enable or disable the scrollbar.


#### Default Value



* false




#### Example


{% highlight js %}

$("#container").ejChart({

    axes: [{ scrollbarSettings:{visible:true} }]
                      
});

{% endhighlight %}


### axes.scrollbarSettings.canResize `boolean`
{:#members:axes-scrollbarsettings-canresize}




Controls whether scrollbar has to be responsive in the chart.


#### Default Value



* false




#### Example


{% highlight js %}

$("#container").ejChart({

    axes:[{ scrollbarSettings:{canResize:true} }]
                      
});

{% endhighlight %}



### axes.scrollbarSettings.range `object`
{:#members:axes-scrollbarsettings-range}


Options to customize the range for the scrollbar in the axis.

 


### axes.scrollbarSettings.range.min `number`
{:#members:axes-scrollbarsettings-range-min}




Minimum value of the scrollbar range.


#### Default Value

* null




#### Example


{% highlight js %}

$("#container").ejChart({

    axes:[ { scrollbarSettings : { range : { min: 10 } } }]
                          
});

{% endhighlight %}


### axes.scrollbarSettings.range.max `number`
{:#members:axes-scrollbarsettings-range-max}




Maximum value for the scrollbar range .


#### Default Value

* null




#### Example


{% highlight js %}

$("#container").ejChart({

    axes:[{ scrollbarSettings : { range : { max: 100 } } } ]
                          
});

{% endhighlight %}


### axes.scrollbarSettings.pointsLength `number`
{:#members:axes-scrollbarsettings-pointslength}




The maximum number of points to be displayed in the scrollbar. 


#### Default Value

* null




#### Example


{% highlight js %}

$("#container").ejChart({

    axes: [{ scrollbarSettings : { pointsLength : 50 } } ]
                          
});

{% endhighlight %}




### primaryYAxis `object`
{:#members:primaryyaxis}




This is a vertical axis that contains options to configure axis. This is the primary y axis for all the series in series array. To override y axis for particular series, create an axis object by providing unique name by using name property and add it to axes array. Then, assign the name to the series&rsquo;s yAxisName property to link both axis and series.






### primaryYAxis.alternateGridBand `object`
{:#members:primaryyaxis-alternategridband}




Options for customizing vertical axis alternate grid band.






### primaryYAxis.alternateGridBand.even `object`
{:#members:primaryyaxis-alternategridband-even}




Options for customizing even grid band.






### primaryYAxis.alternateGridBand.even.fill `string`
{:#members:primaryyaxis-alternategridband-even-fill}




Fill color for the even grid bands.


#### Default Value



* transparent




#### Example


{% highlight js %}

$("#container").ejChart({

    primaryYAxis: { alternateGridBand: { even : {fill : "red" } } }
                          
});

{% endhighlight %}




### primaryYAxis.alternateGridBand.even.opacity `number`
{:#members:primaryyaxis-alternategridband-even-opacity}




Opacity of the even grid band.


#### Default Value



* 1




#### Example


{% highlight js %}

$("#container").ejChart({

    primaryYAxis: { alternateGridBand: { even : {opacity : 0.5 } } }
                          
});

{% endhighlight %}

Try it: [JS Playground Sample](http://jsplayground.syncfusion.com/12z4yd2l)


### primaryYAxis.alternateGridBand.odd `object`
{:#members:primaryyaxis-alternategridband-odd}




Options for customizing odd grid band.






### primaryYAxis.alternateGridBand.odd.fill `string`
{:#members:primaryyaxis-alternategridband-odd-fill}




Fill color of the odd grid bands.


#### Default Value



* "transparent"




#### Example


{% highlight js %}

$("#container").ejChart({

    primaryYAxis: { alternateGridBand: { odd : { fill :"red" }  } }
                          
});

{% endhighlight %}




### primaryYAxis.alternateGridBand.odd.opacity `number`
{:#members:primaryyaxis-alternategridband-odd-opacity}




Opacity of odd grid band.


#### Default Value



* 1




#### Example


{% highlight js %}

$("#container").ejChart({

    primaryYAxis: { alternateGridBand: { odd : { opacity :0.5 }  } }
                           
});

{% endhighlight %}

Try it: [JS Playground Sample](http://jsplayground.syncfusion.com/hyakwb3m)


### primaryYAxis.enableAutoIntervalOnZooming`boolean`
{:#members:primaryyaxis-enableautointervalonzooming}



Specifies the interval of the axis according to the zoomed data of the chart. 


#### Default Value



* true




#### Example


{% highlight js %}

$("#container").ejChart({

    primaryYAxis: { enableAutoIntervalOnZooming: true }
                          
});

{% endhighlight %}




### primaryYAxis.axisLine `object`
{:#members:primaryyaxis-axisline}




Options for customizing the axis line.






### primaryYAxis.axisLine.dashArray `string`
{:#members:primaryyaxis-axisline-dasharray}




Pattern of dashes and gaps to be applied to the axis line.


#### Default Value



* null




#### Example


{% highlight js %}

$("#container").ejChart({

    primaryYAxis: {  axisLine :{ dashArray : "2,3" } }
                          
});

{% endhighlight %}




### primaryYAxis.axisLine.offset `number`
{:#members:primaryyaxis-axisline-offset}




Padding for axis line. Normally, it is used along with plotOffset to pad the plot area.


#### Default Value



* null




#### Example


{% highlight js %}

$("#container").ejChart({

    primaryYAxis: { axisLine: { offset : 5 } }
                          
});

{% endhighlight %}

Try it: [JS Playground Sample](http://jsplayground.syncfusion.com/3drq4c1j)


### primaryYAxis.axisLine.visible `boolean`
{:#members:primaryyaxis-axisline-visible}




Show/hides the axis line.


#### Default Value



* true




#### Example


{% highlight js %}

$("#container").ejChart({

    primaryYAxis: { axisLine: { visible : false } }
                          
});

{% endhighlight %}


### primaryYAxis.axisLine.color `string`
{:#members:primaryyaxis-axisline-color}




Color of axis line.


#### Default Value



* ""




#### Example


{% highlight js %}

$("#container").ejChart({

    primaryYAxis: { axisLine: { color : "" } }
                          
});

{% endhighlight %}




### primaryYAxis.axisLine.width `number`
{:#members:primaryyaxis-axisline-width}




Width of axis line.


#### Default Value



* 1




#### Example


{% highlight js %}

$("#container").ejChart({

    primaryYAxis: { axisLine: { width : 2 } }
                          
});

{% endhighlight %}

Try it: [JS Playground Sample](http://jsplayground.syncfusion.com/zz4cubdn)


### primaryYAxis.crossesAt `number`
{:#members:primaryyaxis-crossesat}




Specifies where horizontal axis should intersect the vertical axis or vice versa. Value should be provided in axis co-ordinates. If provided value is greater than the maximum value of crossing axis, then axis will be placed at the opposite side.


#### Default Value



* null




#### Example


{% highlight js %}

	$("#container").ejChart({

		primaryYAxis:
		{
			//Crosses primary Y axis at 0
			crossesAt: 0,

			//...
		},	
	});

{% endhighlight %}




### primaryYAxis.crossesInAxis `string`
{:#members:primaryyaxis-crossesinaxis}




Name of the axis used for crossing. Vertical axis name should be provided for horizontal axis and vice versa. If the provided name does not belongs to a valid axis, then primary X axis or primary Y axis will be used for crossing


#### Default Value



* null




#### Example


{% highlight js %}

	$("#container").ejChart({

		primaryYAxis:
		{
			//Crosses vertical axis at -0.2
			crossesAt: -0.2,

			//Crosses in secondary Y axis
			crossesInAxis: 'secondaryYAxis',

			//...
		},
	});

{% endhighlight %}


### primaryYAxis.crosshairLabel `object`
{:#members:primaryyaxis-crosshairlabel}




Options to customize the crosshair label.






### primaryYAxis.crosshairLabel.visible `boolean`
{:#members:primaryyaxis-crosshairlabel-visible}




Show/hides the crosshair label associated with this axis.


#### Default Value



* false




#### Example


{% highlight js %}

$("#container").ejChart({

    primaryYAxis: { crosshairLabel: { visible : true } }
                          
});

{% endhighlight %}




### primaryYAxis.desiredIntervals `number`
{:#members:primaryyaxis-desiredintervals}




With this setting, you can request axis to calculate intervals approximately equal to your desired interval.


#### Default Value



* null




#### Example


{% highlight js %}

$("#container").ejChart({

    primaryYAxis: { desiredIntervals: 5 }
                          
});

{% endhighlight %}


### primaryYAxis.labelPlacement `enum`
{:#members:primaryyaxis-labelplacement}

<ts ref="ej.datavisualization.Chart.LabelPlacement"/>

Specifies the placement of labels. 


#### Default Value



* ej.datavisualization.Chart.LabelPlacement.BetweenTicks. See <a href="ejchart.html#members:primaryxaxis-labelplacement">LabelPlacement</a>


#### Example


{% highlight js %}

$("#container").ejChart({

    primaryYAxis: { labelPlacement : "onTicks" }
                          
});

{% endhighlight %}


### primaryYAxis.edgeLabelPlacement `enum`
{:#members:primaryyaxis-edgelabelplacement}

<ts ref="ej.datavisualization.Chart.EdgeLabelPlacement"/>


Specifies the position of labels at the edge of the axis. 


#### Default Value




* ej.datavisualization.Chart.EdgeLabelPlacement.None. See <a href="ejchart.html#members:primaryxaxis-edgelabelplacement">EdgeLabelPlacement</a>




#### Example


{% highlight js %}

$("#container").ejChart({

     primaryYAxis: { edgeLabelPlacement: "shift" }
                           
});

{% endhighlight %}




### primaryYAxis.enableTrim `boolean`
{:#members:primaryyaxis-enabletrim}




Specifies whether to trim the axis label when the width of the label exceeds the maximumLabelWidth. 


#### Default Value



* false 




#### Example


{% highlight js %}

$("#container").ejChart({

    primaryYAxis: { enableTrim : true }
                          
});

{% endhighlight %}




### primaryYAxis.font `object`
{:#members:primaryyaxis-font}




Options for customizing the font of the axis Labels.






### primaryYAxis.font.fontFamily `string`
{:#members:primaryyaxis-font-fontfamily}




Font family of labels.


#### Default Value



* "Segoe UI"




#### Example


{% highlight js %}

$("#container").ejChart({

    primaryYAxis: { font: { fontFamily : "Algerian" } }
                          
});

{% endhighlight %}




### primaryYAxis.font.fontStyle `enum`
{:#members:primaryyaxis-font-fontstyle}


<ts ref="ej.datavisualization.Chart.FontStyle"/>

Font style of labels.


#### Default Value




ej.datavisualization.Chart.FontStyle.Normal. See <a href="global.html#enum:fontstyle">FontStyle</a>




#### Example


{% highlight js %}

$("#container").ejChart({

    primaryYAxis: { font: { fontStyle : "italic" } }
                          
});

{% endhighlight %}




### primaryYAxis.font.fontWeight `enum`
{:#members:primaryyaxis-font-fontweight}


<ts ref="ej.datavisualization.Chart.FontWeight"/>

Font weight of the label.


#### Default Value




* ej.datavisualization.Chart.FontWeight.Regular. See <a href="global.html#enum:fontweight">FontWeight</a>




#### Example


{% highlight js %}

$("#container").ejChart({

    primaryYAxis: { font: { fontWeight : "normal" } }
                          
});

{% endhighlight %}




### primaryYAxis.font.opacity `number`
{:#members:primaryyaxis-font-opacity}




Opacity of the axis labels.


#### Default Value



* 1




#### Example


{% highlight js %}

$("#container").ejChart({

    primaryYAxis: { font: { opacity : 0.5 } }
                          
});

{% endhighlight %}




### primaryYAxis.font.size `string`
{:#members:primaryyaxis-font-size}




Font size of the axis labels.


#### Default Value



* "13px"




#### Example


{% highlight js %}

$("#container").ejChart({

    primaryYAxis: { font: { size : "12px" } }
                          
});

{% endhighlight %}

Try it: [JS Playground Sample](http://jsplayground.syncfusion.com/s1dshld4))


### primaryYAxis.intervalType `enum`
{:#members:primaryyaxis-intervaltype}

<ts ref="ej.datavisualization.Chart.IntervalType"/>


Specifies the type of interval in date time axis.


#### Default Value




* null. See <a href="ejchart.html#members:primaryxaxis-intervaltype">IntervalType</a>




#### Example


{% highlight js %}

$("#container").ejChart({

    primaryYAxis: { intervalType: "days" }
                          
});

{% endhighlight %}

Try it: [JS Playground Sample](http://jsplayground.syncfusion.com/n2dwkjtr)


### primaryYAxis.isInversed `boolean`
{:#members:primaryyaxis-isinversed}




Specifies whether to inverse the axis.


#### Default Value



* false




#### Example


{% highlight js %}

$("#container").ejChart({

     primaryYAxis: { isInversed : true}
                           
});

{% endhighlight %}

Try it: [JS Playground Sample](http://jsplayground.syncfusion.com/mnnwkac1)


### primaryYAxis.labelFormat `string`
{:#members:primaryyaxis-labelformat}




Custom formatting for axis label and supports all standard formatting type of numerical and date time values.


#### Default Value



* null




#### Example


{% highlight js %}

$("#container").ejChart({

    primaryYAxis: { labelFormat: "{value}F" }
                          
});

{% endhighlight %}

Try it: [JS Playground Sample](http://jsplayground.syncfusion.com/n2dwkjtr)


### primaryYAxis.labelIntersectAction `enum`
{:#members:primaryyaxis-labelintersectaction}


<ts ref="ej.datavisualization.Chart.LabelIntersectAction"/>

Specifies the action to take when the axis labels are overlapping with each other. 


#### Default Value



* ej.datavisualization.Chart.LabelIntersectAction.None




#### Example


{% highlight js %}

$("#container").ejChart({

     primaryYAxis: { labelIntersectAction: "multipleRows" }
                           
});

{% endhighlight %}

Try it: [JS Playground Sample](http://jsplayground.syncfusion.com/pm2ksurr)


### primaryYAxis.labelPosition `enum`
{:#members:primaryyaxis-labelposition}

<ts ref="ej.datavisualization.Chart.LabelPosition"/>

Specifies the position of the axis labels.


#### Default Value



* "outside". See <a href="ejchart.html#members:primaryxaxis-labelposition">LabelPosition</a>




#### Example


{% highlight js %}

$("#container").ejChart({

    primaryYAxis: { labelPosition : "inside" }
                           
});

{% endhighlight %}




### primaryYAxis.alignment `enum`
{:#members:primaryyaxis-alignment}

<ts ref="ej.datavisualization.Chart.LabelAlignment"/>

Specifies the position of the axis labels.


#### Default Value



* "center". See <a href="ejchart.html#members:primaryxaxis-alignment">Alignment</a>




#### Example


{% highlight js %}

$("#container").ejChart({

    primaryYAxis: { alignment : "near" }
                           
});

{% endhighlight %}


### primaryYAxis.logBase `number`
{:#members:primaryyaxis-logbase}




Logarithmic base value. This is applicable only for logarithmic axis.


#### Default Value




* 10




#### Example


{% highlight js %}

$("#container").ejChart({

    primaryYAxis: { logBase: 5 }
                          
});

{% endhighlight %}

Try it: [JS Playground Sample](http://jsplayground.syncfusion.com/nfviof2i)


### primaryYAxis.majorGridLines `object`
{:#members:primaryyaxis-majorgridlines}




Options for customizing major gird lines.






### primaryYAxis.majorGridLines.dashArray `string`
{:#members:primaryyaxis-majorgridlines-dasharray}




Pattern of dashes and gaps used to stroke the major grid lines.


#### Default Value



* null




#### Example


{% highlight js %}

$("#container").ejChart({

    primaryYAxis: { majorGridLines : {dashArray : "2,3"} }
                      
});

{% endhighlight %}


### primaryYAxis.majorGridLines.color `string`
{:#members:primaryyaxis-majorgridlines-color}




Color of the major grid lines.


#### Default Value



* null



#### Example


{% highlight js %}

$("#container").ejChart({

    primaryYAxis: { majorGridLines : {color : "red"} }
                      
});

{% endhighlight %}


### primaryYAxis.majorGridLines.opacity `number`
{:#members:primaryyaxis-majorgridlines-opacity}




Opacity of major grid lines.


#### Default Value



* 1




#### Example


{% highlight js %}

$("#container").ejChart({

    primaryYAxis: { majorGridLines : {opacity : 0.5} }
                          
});

{% endhighlight %}




### primaryYAxis.majorGridLines.visible `boolean`
{:#members:primaryyaxis-majorgridlines-visible}




Show/hides the major grid lines.


#### Default Value



* true




#### Example


{% highlight js %}

$("#container").ejChart({

    primaryYAxis: { majorGridLines : {visible : false} }
                          
});

{% endhighlight %}




### primaryYAxis.majorGridLines.width `number`
{:#members:primaryyaxis-majorgridlines-width}




Width of the major grid lines.


#### Default Value



* 1




#### Example


{% highlight js %}

$("#container").ejChart({

    primaryYAxis: { majorGridLines : {width : 2} }
                          
});

{% endhighlight %}

Try it: [JS Playground Sample](http://jsplayground.syncfusion.com/jaqmz0ox)


### primaryYAxis.majorTickLines `object`
{:#members:primaryyaxis-majorticklines}




Options for customizing the major tick lines.






### primaryYAxis.majorTickLines.size `number`
{:#members:primaryyaxis-majorticklines-size}




Length of the major tick lines.


#### Default Value



* 5




#### Example


{% highlight js %}

$("#container").ejChart({

    primaryYAxis: { majorTickLines : {size : 2} }
                      
});

{% endhighlight %}




### primaryYAxis.majorTickLines.visible `boolean`
{:#members:primaryyaxis-majorticklines-visible}




Show/hides the major tick lines.


#### Default Value



* true




#### Example


{% highlight js %}

$("#container").ejChart({

    primaryYAxis: { majorTickLines : {visible : false} }
                          
});

{% endhighlight %}




### primaryYAxis.majorTickLines.width `number`
{:#members:primaryyaxis-majorticklines-width}




Width of the major tick lines.


#### Default Value



* 1




#### Example


{% highlight js %}

$("#container").ejChart({

    primaryYAxis: { majorTickLines : {width : 2} }
                          
});
</script>  
{% endhighlight %}

Try it: [JS Playground Sample](http://jsplayground.syncfusion.com/dumkxazd)


### primaryYAxis.maximumLabels `number`
{:#members:primaryyaxis-maximumlabels}




Maximum number of labels to be displayed in every 100 pixels.


#### Default Value



* 3




#### Example


{% highlight js %}

$("#container").ejChart({

    primaryYAxis: { maximumLabels: 5 }
                          
});

{% endhighlight %}




### primaryYAxis.maximumLabelWidth `number`
{:#members:primaryyaxis-maximumlabelwidth}




Maximum width of the axis label. When the label exceeds the width, the label gets trimmed when the enableTrim is set to true.


#### Default Value



* ej.datavisualization.Chart.maximumLabelWidth type {int}




#### Example


{% highlight js %}

$("#container").ejChart({

    primaryYAxis: { maximumLabelWidth :34.5 }
                          
});

{% endhighlight %}




### primaryYAxis.minorGridLines `object`
{:#members:primaryyaxis-minorgridlines}




Options for customizing the minor grid lines.






### primaryYAxis.minorGridLines.dashArray `string`
{:#members:primaryyaxis-minorgridlines-dasharray}




Patterns of dashes and gaps used to stroke the minor grid lines.


#### Default Value



* null




#### Example


{% highlight js %}

$("#container").ejChart({

    primaryYAxis: { minorGridLines : {dashArray : "2,3"} }
                          
});

{% endhighlight %}




### primaryYAxis.minorGridLines.visible `boolean`
{:#members:primaryyaxis-minorgridlines-visible}




Show/hides the minor grid lines.


#### Default Value



* true




#### Example


{% highlight js %}

$("#container").ejChart({

    primaryYAxis: { minorGridLines : {visible : true} }
                          
});

{% endhighlight %}




### primaryYAxis.minorGridLines.width `number`
{:#members:primaryyaxis-minorgridlines-width}




Width of the minorGridLines.


#### Default Value



* 1




#### Example


{% highlight js %}

$("#container").ejChart({

    primaryYAxis: { minorGridLines : {width : 2} }
                          
});

{% endhighlight %}

Try it: [JS Playground Sample](http://jsplayground.syncfusion.com/3ijc021x)


### primaryYAxis.minorTickLines `object`
{:#members:primaryyaxis-minorticklines}




Options for customizing the minor tick lines.






### primaryYAxis.minorTickLines.size `number`
{:#members:primaryyaxis-minorticklines-size}




Length of the minor tick lines.


#### Default Value



* 5




#### Example


{% highlight js %}


$("#container").ejChart({

    primaryYAxis: { minorTickLines : {size : 2} }
                          
});

{% endhighlight %}




### primaryYAxis.minorTickLines.visible `boolean`
{:#members:primaryyaxis-minorticklines-visible}




Show/hides the minor tick lines.


#### Default Value



* true




#### Example


{% highlight js %}

$("#container").ejChart({

    primaryYAxis: { minorTickLines : {visible : true} }    
                  
});
</script>  
{% endhighlight %}




### primaryYAxis.minorTickLines.width `number`
{:#members:primaryyaxis-minorticklines-width}




Width of the minor tick line


#### Default Value



* 1




#### Example


{% highlight js %}

$("#container").ejChart({

    primaryYAxis: { minorTickLines : {width : 2} }
                          
});

{% endhighlight %}




### primaryYAxis.minorTicksPerInterval `number`
{:#members:primaryyaxis-minorticksperinterval}




Specifies the number of minor ticks per interval.


#### Default Value



* null




#### Example


{% highlight js %}

$("#container").ejChart({

    primaryYAxis: { minorTicksPerInterval: 3 }
                          
});

{% endhighlight %}

Try it: [JS Playground Sample](http://jsplayground.syncfusion.com/tbbhdw21)


### primaryYAxis.name `string`
{:#members:primaryyaxis-name}




Unique name of the axis. To associate an axis with the series, you have to set this name to the xAxisName/yAxisName property of the series.


#### Default Value



* null




#### Example


{% highlight js %}

$("#container").ejChart({

    primaryYAxis: { name: "yAxis" }
                          
});

{% endhighlight %}




### primaryYAxis.opposedPosition `boolean`
{:#members:primaryyaxis-opposedposition}




Specifies whether to render the axis at the opposite side of its default position.


#### Default Value



* false




#### Example


{% highlight js %}

$("#container").ejChart({

     primaryYAxis: { opposedPosition : true }
                           
});

{% endhighlight %}


### primaryYAxis.orientation `enum`
{:#members:primaryyaxis-orientation}

<ts ref="ej.datavisualization.Chart.AxisOrientation"/>


Specifies the orientation of the axis line in the chart.


#### Default Value



* Vertical




#### Example


{% highlight js %}

$("#container").ejChart({

    primaryYAxis: { orientation : 'Horizontal' }
                          
});

{% endhighlight %}




### primaryYAxis.plotOffset `number`
{:#members:primaryyaxis-plotoffset}




Specifies the padding for the plot area.


#### Default Value



* 10




#### Example


{% highlight js %}

$("#container").ejChart({

    primaryYAxis: { plotOffset: 5 }
                          
});

{% endhighlight %}

Try it: [JS Playground Sample](http://jsplayground.syncfusion.com/ls2i5oiv)



### primaryYAxis.range `object`
{:#members:primaryyaxis-range}


Options to customize the range of the axis.

 


### primaryYAxis.range.min `number`
{:#members:primaryyaxis-range-min}




Minimum value of the axis range.


#### Default Value

* null




#### Example


{% highlight js %}

$("#container").ejChart({

    primaryYAxis: { range : { min: 10 } }
                          
});

{% endhighlight %}


### primaryYAxis.range.max `number`
{:#members:primaryyaxis-range-max}




Maximum value of the axis range.


#### Default Value

* null




#### Example


{% highlight js %}

$("#container").ejChart({

    primaryYAxis: { range : { max: 100 } }
                          
});

{% endhighlight %}



### primaryYAxis.range.interval `number`
{:#members:primaryyaxis-range-interval}




Interval for the range.


#### Default Value

* null




#### Example


{% highlight js %}

$("#container").ejChart({

    primaryYAxis: { range : { interval: 10 } }
                          
});

{% endhighlight %}



### primaryYAxis.rangePadding `enum`
{:#members:primaryyaxis-rangepadding}

<ts ref="ej.datavisualization.Chart.RangePadding"/>


Specifies the padding for the axis range.


#### Default Value




* ej.datavisualization.Chart.RangePadding.None. See <a href="ejchart.html#members:primaryyaxis-rangepadding">RangePadding</a>




#### Example


{% highlight js %}

$("#container").ejChart({

    primaryYAxis: { rangePadding : "none" }
                          
});

{% endhighlight %}




### primaryYAxis.roundingPlaces `number`
{:#members:primaryyaxis-roundingplaces}




Rounds the number to the given number of decimals.


#### Default Value



* null




#### Example


{% highlight js %}

$("#container").ejChart({

    primaryYAxis: { roundingPlaces: 2 }  
                    
});

{% endhighlight %}

Try it: [JS Playground Sample](http://jsplayground.syncfusion.com/ad225rnj)


### primaryYAxis.rowIndex `number`
{:#members:primaryyaxis-rowindex}




Specifies the index of the row to which the axis is associated, when the chart area is divided into multiple plot areas by using rowDefinitions.


#### Default Value



* null




#### Example


{% highlight js %}

$("#container").ejChart({

     primaryYAxis: { rowIndex: 1 }                      
});
</script> 
{% endhighlight %}




### primaryYAxis.rowSpan `number`
{:#members:primaryyaxis-rowspan}




Specifies the number of row or plot areas an axis has to span vertically.


#### Default Value



* null




#### Example


{% highlight js %}

$("#container").ejChart({

    primaryYAxis: { rowSpan: 2 }
                          
});

{% endhighlight %}

Try it: [JS Playground Sample](http://jsplayground.syncfusion.com/fitf4tn3)


### primaryYAxis.multiLevelLabels `array`
{:#members:primaryyaxis-multilevellabels}


Options for customizing the multi level labels.


#### Default Value



* [ ]







### primaryYAxis.multiLevelLabels.visible `boolean`
{:#members:primaryyaxis-multilevellabels-visible}




Visibility of the multi level labels.


#### Default Value



* false




#### Example


{% highlight js %}

$("#container").ejChart({
 
    primaryYAxis: { multiLevelLabels:[{ visible: true }]}
                          
});

{% endhighlight %}


### primaryYAxis.multiLevelLabels.text `string`
{:#members:primaryyaxis-multilevellabels-text}




Text of the multi level labels.


#### Default Value



* ""




#### Example


{% highlight js %}

$("#container").ejChart({
 
    primaryYAxis: { multiLevelLabels:[{ text: "2016" }]}
                          
});

{% endhighlight %}


### primaryYAxis.multiLevelLabels.start `number`
{:#members:primaryyaxis-multilevellabels-start}




Starting value of the multi level labels.


#### Default Value



* null




#### Example


{% highlight js %}

$("#container").ejChart({
 
    primaryYAxis: { multiLevelLabels:[{ start: 1 }]}
                          
});

{% endhighlight %}

### primaryYAxis.multiLevelLabels.end `number`
{:#members:primaryyaxis-multilevellabels-end}




Ending value of the multi level labels.


#### Default Value



* null




#### Example


{% highlight js %}

$("#container").ejChart({
 
    primaryYAxis: { multiLevelLabels:[{ end: 4 }]}
                          
});

{% endhighlight %}


### primaryYAxis.multiLevelLabels.level `number`
{:#members:primaryyaxis-multilevellabels-level}




Specifies the level of multi level labels.


#### Default Value



* 0




#### Example


{% highlight js %}

$("#container").ejChart({
 
    primaryYAxis: { multiLevelLabels:[{ level: 2 }]}
                          
});

{% endhighlight %}


### primaryYAxis.multiLevelLabels.maximumTextWidth `number`
{:#members:primaryyaxis-multilevellabels-maximumtextwidth}




Specifies the maximum width of the text in multi level labels.


#### Default Value



* null




#### Example


{% highlight js %}

$("#container").ejChart({
 
    primaryYAxis: { multiLevelLabels:[{ maximumTextWidth: 30 }]}
                          
});

{% endhighlight %}



### primaryYAxis.multiLevelLabels.textAlignment `enum`
{:#members:primaryyaxis-multilevellabels-textalignment}

<ts ref="ej.datavisualization.Chart.TextAlignment"/>


Specifies the alignment of the text in multi level labels.


#### Default Value



* "center". See <a href="ejchart.html#members:primaryyaxis-multilevellabels-textalignment">TextAlignment</a>




#### Example


{% highlight js %}

$("#container").ejChart({
 
    primaryYAxis: { multiLevelLabels:[{ textAlignment: "near" }]}
                          
});

{% endhighlight %}


### primaryYAxis.multiLevelLabels.textOverflow `enum`
{:#members:primaryyaxis-multilevellabels-textoverflow}

<ts ref="ej.datavisualization.Chart.TextOverflow"/>


Specifies the handling of text over flow in multi level labels.


#### Default Value



* "center". See <a href="ejchart.html#members:primaryyaxis-multilevellabels-textoverflow">TextOverflow</a>




#### Example


{% highlight js %}

$("#container").ejChart({
 
    primaryYAxis: { multiLevelLabels:[{ textOverflow: "trim" }]}
                          
});

{% endhighlight %}



### primaryYAxis.multiLevelLabels.font `object`
{:#members:primaryyaxis-multilevellabels-font}




Options for customizing the font of the text.






### primaryYAxis.multiLevelLabels.font.color `string`
{:#members:primaryyaxis-multilevellabels-font-color}




Font color of the multi level labels text.


#### Default Value



* null




#### Example


{% highlight js %}

$("#container").ejChart({

     primaryYAxis: { multiLevelLabels:[{ font : { color: "green"} }]}
                           
});

{% endhighlight %}




### primaryYAxis.multiLevelLabels.font.fontFamily `string`
{:#members:primaryyaxis-multilevellabels-font-fontfamily}




Font family of the multi level labels text.


#### Default Value



* "Segoe UI"




#### Example


{% highlight js %}

$("#container").ejChart({

    primaryYAxis: { multiLevelLabels:[{ font : { fontFamily : "Algerian"} }]}
                          
});

{% endhighlight %}




### primaryYAxis.multiLevelLabels.font.fontStyle `enum`
{:#members:primaryyaxis-multilevellabels-font-fontstyle}

<ts ref="ej.datavisualization.Chart.FontStyle"/>


Font style of the multi level labels text.


#### Default Value



* "Normal"




#### Example


{% highlight js %}

$("#container").ejChart({ 

    primaryYAxis: { multiLevelLabels:[{ font : { fontStyle: "Bold"} }]}
                          
});

{% endhighlight %}




### primaryYAxis.multiLevelLabels.font.fontWeight `string`
{:#members:primaryyaxis-multilevellabels-font-fontweight}




Font weight of the multi level label text.


#### Default Value



* "regular"




#### Example


{% highlight js %}

$("#container").ejChart({

      primaryYAxis: { multiLevelLabels:[{ font : { fontWeight: "lighter"} }]}
                            
});

{% endhighlight %}




### primaryYAxis.multiLevelLabels.font.opacity `number`
{:#members:primaryyaxis-multilevellabels-font-opacity}




Opacity of the multi level label text.


#### Default Value



* 1




#### Example


{% highlight js %}

$("#container").ejChart({

primaryYAxis: { multiLevelLabels:[{ font : { opacity: 0.5} }]}
                      
});

{% endhighlight %}




### primaryYAxis.multiLevelLabels.font.size `string`
{:#members:primaryyaxis-multilevellabels-font-size}




Font size of the multi level label text.


#### Default Value



* "12px"




#### Example


{% highlight js %}

$("#container").ejChart({

        primaryYAxis: { multiLevelLabels:[{ font : { size: "15px"} }]}
                              
});

{% endhighlight %}


### primaryYAxis.multiLevelLabels.border `object`
{:#members:primaryyaxis-multilevellabels-border}




Options for customizing the border of the series.






### primaryYAxis.multiLevelLabels.border.color `string`
{:#members:primaryyaxis-multilevellabels-border-color}




Border color of the multi level labels.


#### Default Value



*  null




#### Example


{% highlight js %}
 
 
$("#container").ejChart({
        primaryYAxis: { multiLevelLabels:[{border :{ color : "green" } }]}                  
});
{% endhighlight %}




### primaryYAxis.multiLevelLabels.border.width `number`
{:#members:primaryyaxis-multilevellabels-border-width}




Border width of the multi level labels.


#### Default Value



* 1




#### Example


{% highlight js %}
 

$("#container").ejChart({
        primaryYAxis: { multiLevelLabels:[{border :{ width : 2 } }]}                  
});
{% endhighlight %}


### primaryYAxis.multiLevelLabels.border.type `enum`
{:#members:primaryyaxis-multilevellabels-border-type}


<ts ref="ej.datavisualization.Chart.MultiLevelLabelsBorderType"/>


Border type of the multi level labels.


#### Default Value



* "rectangle". See <a href="ejchart.html#members:primaryyaxis-multilevellabels-border-type">Type</a>




#### Example


{% highlight js %}
 

$("#container").ejChart({
        primaryYAxis: { multiLevelLabels:[{border :{ type : "brace" } }]}                  
});
{% endhighlight %}

### primaryYAxis.showNextToAxisLine `boolean`
{:#members:primaryyaxis-shownexttoaxisline}



Specifies whether the axis elements need to be placed nearby the axis line, while crossing.



#### Default Value



* true




#### Example


{% highlight js %}

$("#container").ejChart({

    primaryYAxis: { showNextToAxisLine : false }
                          
});

{% endhighlight %}



### primaryYAxis.scrollbarSettings `object`
{:#members:primaryyaxis-scrollbarsettings}




Options for customizing the axis scrollbar.


### primaryYAxis.scrollbarSettings.visible `boolean`
{:#members:primaryyaxis-scrollbarsettings-visible}




Specifies to enable or disable the scrollbar.


#### Default Value



* false




#### Example


{% highlight js %}

$("#container").ejChart({

    primaryYAxis: { scrollbarSettings:{visible:true} }
                      
});

{% endhighlight %}


### primaryYAxis.scrollbarSettings.canResize `boolean`
{:#members:primaryyaxis-scrollbarsettings-canresize}




Controls whether scrollbar has to be responsive in the chart.


#### Default Value



* false




#### Example


{% highlight js %}

$("#container").ejChart({

    primaryYAxis: { scrollbarSettings:{canResize:true} }
                      
});

{% endhighlight %}



### primaryYAxis.scrollbarSettings.range `object`
{:#members:primaryyaxis-scrollbarsettings-range}


Options to customize the range for the scrollbar in the axis.

 


### primaryYAxis.scrollbarSettings.range.min `number`
{:#members:primaryyaxis-scrollbarsettings-range-min}




Minimum value of the scrollbar range.


#### Default Value

* null




#### Example


{% highlight js %}

$("#container").ejChart({

    primaryYAxis: { scrollbarSettings : { range : { min: 10 } } }
                          
});

{% endhighlight %}


### primaryYAxis.scrollbarSettings.range.max `number`
{:#members:primaryyaxis-scrollbarsettings-range-max}




Maximum value for the scrollbar range .


#### Default Value

* null




#### Example


{% highlight js %}

$("#container").ejChart({

    primaryYAxis: { scrollbarSettings : { range : { max: 100 } } } 
                          
});

{% endhighlight %}


### primaryYAxis.scrollbarSettings.pointsLength `number`
{:#members:primaryyaxis-scrollbarsettings-pointslength}




The maximum number of points to be displayed in the scrollbar. 


#### Default Value

* null




#### Example


{% highlight js %}

$("#container").ejChart({

    primaryYAxis: { scrollbarSettings : { pointsLength : 50 } } 
                          
});

{% endhighlight %}







### primaryYAxis.stripLine `array`
{:#members:primaryyaxis-stripline}




Options for customizing the strip lines.


#### Default Value



* [ ]







### primaryYAxis.stripLine.borderColor `string`
{:#members:primaryyaxis-stripline-bordercolor}




Border color of the strip line.


#### Default Value



* "gray"




#### Example


{% highlight js %}

$("#container").ejChart({

    primaryYAxis: { stripLine:[{ borderColor: "green" }]}
                          
});

{% endhighlight %}




### primaryYAxis.stripLine.color `string`
{:#members:primaryyaxis-stripline-color}




Background color of the strip line.


#### Default Value



* "gray"




#### Example


{% highlight js %}

$("#container").ejChart({

    primaryYAxis: { stripLine:[{ color: "green" }]}
                          
});

{% endhighlight %}




### primaryYAxis.stripLine.end `number`
{:#members:primaryyaxis-stripline-end}




End value of the strip line.


#### Default Value



* null




#### Example


{% highlight js %}

$("#container").ejChart({

    primaryYAxis: { stripLine:[{ end: 5 }]}
                          
});

{% endhighlight %}




### primaryYAxis.stripLine.font `object`
{:#members:primaryyaxis-stripline-font}




Options for customizing the font of the text.






### primaryYAxis.stripLine.font.color `string`
{:#members:primaryyaxis-stripline-font-color}




Font color of the strip line text.


#### Default Value



* "black"




#### Example


{% highlight js %}

$("#container").ejChart({

    primaryYAxis: { stripLine:[{ font : { color: "green"} }]}
                          
});

{% endhighlight %}




### primaryYAxis.stripLine.font.fontFamily `string`
{:#members:primaryyaxis-stripline-font-fontfamily}




Font family of the strip line text.


#### Default Value



* "Segoe UI"




#### Example


{% highlight js %}

$("#container").ejChart({

    primaryYAxis: { stripLine:[{ font : { fontFamily : "Algerian"} }]}
                          
});

{% endhighlight %}




### primaryYAxis.stripLine.font.fontStyle `enum`
{:#members:primaryyaxis-stripline-font-fontstyle}

<ts ref="ej.datavisualization.Chart.FontStyle"/>


Font style of the strip line text.


#### Default Value



* "Normal"




#### Example


{% highlight js %}

$("#container").ejChart({

primaryYAxis: { stripLine:[{ font : { fontStyle: "Bold"} }]}
                      
});

{% endhighlight %}




### primaryYAxis.stripLine.font.fontWeight `string`
{:#members:primaryyaxis-stripline-font-fontweight}




Font weight of the strip line text.


#### Default Value



* "regular"




#### Example


{% highlight js %}

$("#container").ejChart({

    primaryYAxis: { stripLine:[{ font : { fontWeight: "lighter"} }]}
                      
});

{% endhighlight %}




### primaryYAxis.stripLine.font.opacity `number`
{:#members:primaryyaxis-stripline-font-opacity}




Opacity of the strip line text.


#### Default Value



* 1




#### Example


{% highlight js %}

$("#container").ejChart({

    primaryYAxis: { stripLine:[{ font : { opacity: 0.5} }]}
                          
});

{% endhighlight %}




### primaryYAxis.stripLine.font.size `string`
{:#members:primaryyaxis-stripline-font-size}




Font size of the strip line text.


#### Default Value



* "12px"




#### Example


{% highlight js %}

$("#container").ejChart({

    primaryYAxis: { stripLine:[{ font : { size: "15px"} }]}
                          
});

{% endhighlight %}




### primaryYAxis.stripLine.start `number`
{:#members:primaryyaxis-stripline-start}




Start value of the strip line.


#### Default Value



* null




#### Example


{% highlight js %}

$("#container").ejChart({

    primaryYAxis: { stripLine:[{ start: 2 }]}
                          
});

{% endhighlight %}




### primaryYAxis.stripLine.startFromAxis `boolean`
{:#members:primaryyaxis-stripline-startfromaxis}




Indicates whether to render the strip line from the minimum/start value of the axis. This property won’t work when start property is set.


#### Default Value



* false




#### Example


{% highlight js %}

$("#container").ejChart({

    primaryYAxis: { stripLine:[{ startFromAxis : true }]} 
                     
});

{% endhighlight %}




### primaryYAxis.stripLine.text `string`
{:#members:primaryyaxis-stripline-text}




Specifies text to be displayed inside the strip line.


#### Default Value



* "stripLine"




#### Example


{% highlight js %}

$("#container").ejChart({

    primaryYAxis: { stripLine:[{ text : "Empty Point" }]}
                          
});

{% endhighlight %}




### primaryYAxis.stripLine.textAlignment `enum`
{:#members:primaryyaxis-stripline-textalignment}

<ts ref="ej.datavisualization.Chart.TextAlignment"/>


Specifies the alignment of the text inside the strip line.


#### Default Value




* "middlecenter". See <a href="ejchart.html#members:primaryyaxis-stripline-textalignment">TextAlignment</a>




#### Example


{% highlight js %}

$("#container").ejChart({

    primaryYAxis: { stripLine:[{ textAlignment : "middletop" }]}
                          
});

{% endhighlight %}




### primaryYAxis.stripLine.visible `boolean`
{:#members:primaryyaxis-stripline-visible}




Show/hides the strip line.


#### Default Value



* false




#### Example


{% highlight js %}

$("#container").ejChart({

    primaryYAxis: { stripLine:[{ visible : true }]}
                          
});

{% endhighlight %}




### primaryYAxis.stripLine.width `number`
{:#members:primaryyaxis-stripline-width}




Width of the strip line.


#### Default Value



* 0




#### Example


{% highlight js %}

$("#container").ejChart({

    primaryYAxis: { stripLine:[{ width : 0 }]}                      
});

{% endhighlight %}




### primaryYAxis.stripLine.zIndex `enum`
{:#members:primaryyaxis-stripline-zindex}

<ts ref="ej.datavisualization.Chart.ZIndex"/>



Specifies the order in which strip line and the series have to be rendered. When Z-order is “behind”, strip line is rendered below the series and when it is “over”, it is rendered above the series.


#### Default Value




* "over". See <a href="ejchart.html#members:primaryyaxis-stripline-zindex">ZIndex</a>



#### Example


{% highlight js %}

$("#container").ejChart({

    primaryYAxis: { stripLine:[{ zIndex: "behind" }]}
                          
});

{% endhighlight %}

Try it: [JS Playground Sample](http://jsplayground.syncfusion.com/pigg3hc0)


### primaryYAxis.tickLinesPosition `enum`
{:#members:primaryyaxis-ticklinesposition}

<ts ref="ej.datavisualization.Chart.TickLinesPosition"/>



Specifies the position of the axis tick lines.


#### Default Value




* "outside". See <a href="ejchart.html#members:primaryyaxis-ticklinesposition">TickLinesPosition</a>




#### Example


{% highlight js %}

$("#container").ejChart({

    primaryYAxis: { tickLinesPosition : "inside" }
                           
});

{% endhighlight %}


### primaryYAxis.labelBorder `object`
{:#members:primaryyaxis-labelborder}




Options for customizing the border of the labels.






### primaryYAxis.labelBorder.color `string`
{:#members:primaryyaxis-labelborder-color}




Specifies the color of the label border.


#### Default Value



* null




#### Example


{% highlight js %}

$("#container").ejChart({

    primaryYAxis: { labelBorder:{color: "green"} }
                      
});

{% endhighlight %}



### primaryYAxis.labelBorder.width `number`
{:#members:primaryyaxis-labelborder-width}




Specifies the width of the label border.


#### Default Value



* 1




#### Example


{% highlight js %}

$("#container").ejChart({

    primaryYAxis: { labelBorder:{width: 2} }
                      
});

{% endhighlight %}



### primaryYAxis.title `object`
{:#members:primaryyaxis-title}




Options for customizing the axis title.






### primaryYAxis.title.enableTrim `boolean`
{:#members:primaryyaxis-title-enabletrim}




Specifies whether to trim the axis title when it exceeds the chart area or the maximum width of the title.


#### Default Value



* ej.datavisualization.Chart.enableTrim




#### Example


{% highlight js %}

$("#container").ejChart({

      primaryXAxis: { title:{enableTrim:true} }
                            
});

{% endhighlight %}




### primaryYAxis.title.font `object`
{:#members:primaryyaxis-title-font}




Options for customizing the title font.






### primaryYAxis.title.font.fontFamily `string`
{:#members:primaryyaxis-title-font-fontfamily}




Font family of the title text.


#### Default Value



* "Segoe UI"




#### Example


{% highlight js %}

$("#container").ejChart({

    primaryYAxis: { title :{ font :{ fontFamily: "Algerian" } } }
                          
});

{% endhighlight %}




### primaryYAxis.title.font.fontStyle `enum`
{:#members:primaryyaxis-title-font-fontstyle}


<ts ref="ej.datavisualization.Chart.FontStyle"/>

Font style of the title text.


#### Default Value



* ej.datavisualization.Chart.FontStyle.Normal




#### Example


{% highlight js %}

$("#container").ejChart({

    primaryYAxis: { title :{ font :{ fontStyle : "Italic" } } }
                          
});

{% endhighlight %}




### primaryYAxis.title.font.fontWeight `enum`
{:#members:primaryyaxis-title-font-fontweight}

<ts ref="ej.datavisualization.Chart.FontWeight"/>


Font weight of the title text.


#### Default Value



* ej.datavisualization.Chart.FontWeight.Regular. See <a href="ejchart.html#members:commonseriesoptions-title-font-fontweight">FontWeight</a>




#### Example


{% highlight js %}

$("#container").ejChart({

    primaryYAxis: { title :{ font :{ fontWeight: "normal" } } }
                          
});

{% endhighlight %}




### primaryYAxis.title.font.opacity `number`
{:#members:primaryyaxis-title-font-opacity}




Opacity of the axis title text.


#### Default Value



* 1




#### Example


{% highlight js %}

$("#container").ejChart({

    primaryYAxis: { title :{ font :{ opacity: 0.5 } } }
                          
});

{% endhighlight %}




### primaryYAxis.title.font.size `string`
{:#members:primaryyaxis-title-font-size}




Font size of the axis title.


#### Default Value



* "16px"




#### Example


{% highlight js %}

$("#container").ejChart({

    primaryYAxis: { title :{ font :{ size: "12px" } } }
                          
});

{% endhighlight %}




### primaryYAxis.title.maximumTitleWidth `number`
{:#members:primaryyaxis-title-maximumtitlewidth}




Maximum width of the title, when the title exceeds this width, the title gets trimmed, when enableTrim is true. 


#### Default Value



* ej.datavisualization.Chart.maximumTitleWidth.null




#### Example


{% highlight js %}

$("#container").ejChart({

    primaryYAxis: { title:{maximumTitleWidth: null} }
                          
});

{% endhighlight %}




### primaryYAxis.title.text `string`
{:#members:primaryyaxis-title-text}




Title for the axis.


#### Default Value



* ""




#### Example


{% highlight js %}

$("#container").ejChart({

    primaryYAxis: { title :{ text: "yAxis" } }
                          
});

{% endhighlight %}




### primaryYAxis.title.visible `boolean`
{:#members:primaryyaxis-title-visible}




Controls the visibility of axis title.


#### Default Value



* true




#### Example


{% highlight js %}

$("#container").ejChart({

    primaryYAxis: { title: { visible: false } }
                          
});

{% endhighlight %}


### primaryYAxis.title.offset `number`
{:#members:primaryyaxis-title-offset}




offset value for axis title.


#### Default Value



* 0




#### Example


{% highlight js %}

$("#container").ejChart({

    primaryYAxis: { title: { offset: 0 } }
                          
});

{% endhighlight %}

### primaryYAxis.title.position `enum`
{:#members:primaryyaxis-title-position}

<ts ref="ej.datavisualization.Chart.LabelPosition"/>

Specifies the position of the axis title.


#### Default Value



* "outside". See <a href="ejchart.html#members:primaryyaxis-title-position">Position</a>




#### Example


{% highlight js %}

$("#container").ejChart({

    primaryYAxis: { title: { position : "inside" }}
                           
});

{% endhighlight %}

### primaryYAxis.title.alignment `enum`
{:#members:primaryyaxis-title-alignment}

<ts ref="ej.datavisualization.Chart.TextAlignment"/>

Specifies the position of the axis title.


#### Default Value



* "center". See <a href="ejchart.html#members:primaryyaxis-title-alignment">Alignment</a>




#### Example


{% highlight js %}

$("#container").ejChart({

    primaryYAxis: { title: { alignment : "near" }}
                           
});

{% endhighlight %}



### primaryYAxis.valueType `enum`
{:#members:primaryyaxis-valuetype}

<ts ref="ej.datavisualization.Chart.ValueType"/>


Specifies the type of data the axis is handling.


#### Default Value




* null. See <a href="ejchart.html#members:primaryyaxis-valuetype">ValueType</a>




#### Example


{% highlight js %}

$("#container").ejChart({

    primaryYAxis: { valueType: "double" }
                          
});

{% endhighlight %}




### primaryYAxis.visible `boolean`
{:#members:primaryyaxis-visible}




Show/hides the axis.


#### Default Value



* true




#### Example


{% highlight js %}

$("#container").ejChart({

    primaryYAxis: { visible : false }
                          
});

{% endhighlight %}




### primaryYAxis.zoomFactor `number`
{:#members:primaryyaxis-zoomfactor}




The axis is scaled by this factor. When zoomFactor is 0.5, the chart is scaled by 200% along this axis. Values ranges from 0 to 1.


#### Default Value



* 1




#### Example


{% highlight js %}

$("#container").ejChart({

    primaryYAxis: { zoomFactor : 0.5 }
                          
});

{% endhighlight %}




### primaryYAxis.zoomPosition `number`
{:#members:primaryyaxis-zoomposition}




Position of the zoomed axis. Value ranges from 0 to 1


#### Default Value



* 0




#### Example


{% highlight js %}

$("#container").ejChart({

    primaryYAxis: { zoomPosition : 0.5 }
                          
});

{% endhighlight %}




### rotation `number`
{:#members:rotation}




Rotation angle of the 3D view. This property is applicable only when 3D view is enabled.


#### Default Value



* 0




#### Example


{% highlight js %}

$("#container").ejChart({

     rotation : 45
             
});

{% endhighlight %}


Try it: [JS Playground Sample](http://jsplayground.syncfusion.com/pf23aw13)




### rowDefinitions `array`
{:#members:rowdefinitions}




Options to split Chart into multiple plotting areas horizontally. Each object in the collection represents a plotting area in Chart.


Try it: [JS Playground Sample](http://jsplayground.syncfusion.com/jydjcqbo)




### rowDefinitions.unit `enum`
{:#members:rowdefinitions-unit}

<ts name="ej.datavisualization.Chart.Unit"/>
Specifies the unit to measure the height of the row in plotting area.


<table class="props">
<thead>
<tr>
<th>Name</th>
<th>Type</th> 
<th class="last">Description</th>
</tr>
</thead>
<tbody>
<tr>
<td class="name">
Pixel</td>
<td class="type">string</td> 
<td class="description"> Specifies the height of the row in pixels.</td>
</tr>
<tr>
<td class="name">
Percentage</td>
<td class="type">string</td>
<td class="description">Specifies the height of the row in  percentage</td>
</tr> 
</tbody>
</table>





#### Default Value

* 'pixel'. See <a href="ejchart.html#members:rowDefinitions.unit">Unit</a>




#### Example


{% highlight js %}
 
$("#container").ejChart({

   rowDefinitions :[{ unit : "percentage" }]                     

});

{% endhighlight %}




### rowDefinitions.rowHeight `number`
{:#members:rowdefinitions-rowheight}




Height of the row in plotting area. Height is measured in either pixel or percentage based on the value of unit property.


#### Default Value

* 50




#### Example


{% highlight js %}
 
$("#container").ejChart({

   rowDefinitions :[{ rowHeight : 50 }]                     

});

{% endhighlight %}




### rowDefinitions.lineColor `string`
{:#members:rowdefinitions-linecolor}




Color of the line that indicates the starting point of the row in plotting area.


#### Default Value

* "transparent"




#### Example


{% highlight js %}
 
$("#container").ejChart({

   rowDefinitions :[{ lineColor : "green" }]                     

});

{% endhighlight %}




### rowDefinitions.lineWidth `number`
{:#members:rowdefinitions-linewidth}




Width of the line that indicates the starting point of the row in plot area.


#### Default Value

* 1




#### Example


{% highlight js %}
 
$("#container").ejChart({

   rowDefinitions :[{ lineWidth : 2 }]                     

});

{% endhighlight %}




### series `array`
{:#members:series}




Specifies the properties used for customizing the series.






### series.bearFillColor `string`
{:#members:series-bearfillcolor}




Color of the point, where the close is up in financial chart.


#### Default Value



* null




#### Example


{% highlight js %}
 
 
$("#container").ejChart({
series : [{bearFillColor: "blue" }]                   
});
 {% endhighlight %}
 
 
 Try it: [JS Playground Sample](http://jsplayground.syncfusion.com/p404ugol)
 



### series.border `object`
{:#members:series-border}




Options for customizing the border of the series.






### series.border.color `string`
{:#members:series-border-color}




Border color of the series.


#### Default Value



*  "transparent"




#### Example


{% highlight js %}
 
 
$("#container").ejChart({
series :[{border :{ color : "green" } }]                  
});
{% endhighlight %}




### series.border.width `number`
{:#members:series-border-width}




Border width of the series.


#### Default Value



* 1




#### Example


{% highlight js %}
 

$("#container").ejChart({
series :[{border :{ width : 2 } }]                  
});
{% endhighlight %}



### series.border.dashArray `string`
{:#members:series-border-dasharray}




DashArray for border of the series.



#### Default Value



 * null




#### Example


{% highlight js %}
 
 
$("#container").ejChart({
series : [{
      border: {

           dashArray: "5,3"
       } 
    }]                   
});

{% endhighlight %}
 
 
Try it : [JS Playground Sample](http://jsplayground.syncfusion.com/vf2xong1)

### series.animationDuration `string`
{:#members:series-animationduration}

Specifies animation duration for series rendering.

#### Default Value

 * null

#### Example

{% highlight js %} 
$("#container").ejChart({
series : [{
            animationDuration : 2000 
        }]                   
});
{% endhighlight %}

### series.bullFillColor `string`
{:#members:series-bullfillcolor}




Color of the point, where the close is down in financial chart.


#### Default Value



 * null



#### Example


{% highlight js %}
 
 
$("#container").ejChart({
series : [{bullFillColor: "green" }]                   
});
{% endhighlight %}


Try it: [JS Playground Sample](http://jsplayground.syncfusion.com/v540kjyb)



### series.columnFacet `enum`
{:#members:series-columnfacet}

<ts ref="ej.datavisualization.Chart.ColumnFacet"/>

To render the column and bar type series in rectangle/cylinder shape. See <a href="global.html#commonseriesoptions-columnfacet">ColumnFacet</a>


#### Default Value

 * "rectangle"


#### Example


{% highlight js %}
 

$('#container').ejChart({

    series: {
    
        //change to cylinder chart
		columnFacet: "cylinder"

    },

    //...

});

{% endhighlight %}

Try it: [JS Playground Sample](http://jsplayground.syncfusion.com/yxqlqo2x)


### series.columnWidth `number`
{:#members:series-columnwidth}




Relative width of the columns in column type series. Value ranges from 0 to 1. Width also depends upon **columnSpacing** property.



#### Default Value



 * 0.7




#### Example


{% highlight js %}
 

$('#container').ejChart({

    series: [{
    
        //Width of columns in column type series
		columnWidth: 0.8

        //... 
    }],

    //...

});

{% endhighlight %}




### series.columnSpacing `number`
{:#members:series-columnspacing}




Spacing between columns of different series. Value ranges from 0 to 1



#### Default Value



 * 0




#### Example


{% highlight js %}
 

$('#container').ejChart({

    series: [{
    
        //20% Spacing between columns
		columnWidth: 0.2

    }],

    //...

});

{% endhighlight %}


### series.stackingGroup `string`
{:#members:series-stackinggroup}




To group the series of stacking collection.


#### Default Value



* ""




#### Example


{% highlight js %}
 

$("#container").ejChart({
series :[{stackingGroup : " "}]                  
});
 {% endhighlight %}



### series.dashArray `string`
{:#members:series-dasharray}




Pattern of dashes and gaps used to stroke the line type series.


#### Default Value



* ""




#### Example


{% highlight js %}
 

$("#container").ejChart({
series :[{dashArray : "2,3"}]                  
});
 {% endhighlight %}


Try it: [JS Playground Sample](http://jsplayground.syncfusion.com/322c4ex3)



### series.dataSource `object`
{:#members:series-datasource}




Specifies the dataSource for the series. It can be an array of JSON objects or an instance of ej.DataManager.


#### Default Value



* null




#### Example


{% highlight js %}
 
 
$("#container").ejChart({
series : [{dataSource: data }]                   
});
 {% endhighlight %}


Try it : [JS Playground Sample](http://jsplayground.syncfusion.com/soesgx0m)

### series.cardinalSplineTension `number`
{:#members:series-cardinalsplinetension}

Specifies spline tension values for cardinal spline type.Value ranges from 0 to 1.

#### Default Value

* 0.5

#### Example

{% highlight js %} 
$("#container").ejChart({
series : [{cadinalSplineTension : 0.5 }]                   
});
{% endhighlight %}

### series.doughnutCoefficient `number`
{:#members:series-doughnutcoefficient}




Controls the size of the hole in doughnut series. Value ranges from 0 to 1.


#### Default Value



* 0.4




#### Example


{% highlight js %}
 
 
$("#container").ejChart({
series : [{doughnutCoefficient : 0.5 }]                   
});
{% endhighlight %}


Try it : [JS Playground Sample](http://jsplayground.syncfusion.com/1xjrwrxl)


### series.doughnutSize `number`
{:#members:series-doughnutsize}




Controls the size of the doughnut series. Value ranges from 0 to 1.


#### Default Value



*  0.8




#### Example


{% highlight js %}
 
 
$("#container").ejChart({
series : [{doughnutSize : 0.6 }]                   
});
{% endhighlight %}


Try it : [JS Playground Sample](http://jsplayground.syncfusion.com/eyi1qmre)

### series.drawType `enum`
{:#members:series-drawtype}

<ts ref="ej.datavisualization.Chart.DrawType"/>


Type of series to be drawn in radar or polar series. 


#### Default Value



* "line". See <a href="ejchart.html#members:commonseriesoptions-drawtype">DrawType</a>




#### Example


{% highlight js %}
 
$("#container").ejChart({
series : [{drawType : "column" }]                   
});
 {% endhighlight %}


Try it : [JS Playground Sample](http://jsplayground.syncfusion.com/pg04h4gh)


### series.enableAnimation `boolean`
{:#members:series-enableanimation}




Enable/disable the animation of series.


#### Default Value



* false




#### Example


{% highlight js %}
 
 
$("#container").ejChart({
series : [{enableAnimation : true }]                   
});
{% endhighlight %}


Try it : [JS Playground Sample](http://jsplayground.syncfusion.com/w4mkzixd)


### series.enableSmartLabels `number`
{:#members:series-enablesmartlabels}




To avoid overlapping of data labels smartly. 


#### Default Value



 * null




#### Example


{% highlight js %}
 
 
$("#container").ejChart({
series : [{enableSmartLabels : false }]                   
});
 {% endhighlight %}


Try it : [JS Playground Sample](http://jsplayground.syncfusion.com/40docuib)


### series.endAngle `number`
{:#members:series-endangle}




End angle of pie/doughnut series. For a complete circle, it has to be 360, by default.


#### Default Value



 * null




#### Example


{% highlight js %}
 
$("#container").ejChart({
series : [{endAngle: 270 }]                   
});

{% endhighlight %}

Try it : [JS Playground Sample](http://jsplayground.syncfusion.com/fqpf3ort)



### series.explode `boolean`
{:#members:series-explode}




Explodes the pie/doughnut slices on mouse move.


#### Default Value



* false




#### Example


{% highlight js %}
 
 
$("#container").ejChart({
series : [{explode: true }]                   
});
{% endhighlight %}


Try it : [JS Playground Sample](http://jsplayground.syncfusion.com/prpei1ld)


### series.explodeAll `boolean`
{:#members:series-explodeall}




Explodes all the slice of pie/doughnut on render.


#### Default Value



 * null




#### Example


{% highlight js %}
 
 
$("#container").ejChart({
series : [{explodeAll: true }]                   
});
{% endhighlight %}


Try it : [JS Playground Sample](http://jsplayground.syncfusion.com/n3if1tnn)


### series.explodeIndex `number`
{:#members:series-explodeindex}




Index of the point to be exploded from pie/doughnut/pyramid/funnel.


#### Default Value



* null




#### Example


{% highlight js %}
 
 
$("#container").ejChart({
series : [{explodeIndex : 2 }]                   
});
 {% endhighlight %}


Try it : [JS Playground Sample](http://jsplayground.syncfusion.com/taccivfh)



### series.explodeOffset `number`
{:#members:series-explodeoffset}




Specifies the distance of the slice from the center, when it is exploded.


#### Default Value



 * 25




#### Example


{% highlight js %}
 
 
$("#container").ejChart({
series : [{explodeOffset : 20 }]                   
});
 {% endhighlight %}
 

Try it : [JS Playground Sample](http://jsplayground.syncfusion.com/2j040lr0)



### series.fill `string`
{:#members:series-fill}




Fill color of the series.


#### Default Value



 * null




#### Example


{% highlight js %}
 
 
$("#container").ejChart({
series :[{fill : "green"}]                 
});
{% endhighlight %}


Try it : [JS Playground Sample](http://jsplayground.syncfusion.com/sit3agft)


### series.font `object`
{:#members:series-font}




Options for customizing the series font.






### series.font.color `string`
{:#members:series-font-color}




Font color of the series text.


#### Default Value



* "#707070"




#### Example


{% highlight js %}
 
 
$("#container").ejChart({
series :[{font :{color : "green"}}]                 
});
{% endhighlight %}




### series.font.fontFamily `string`
{:#members:series-font-fontfamily}




Font Family of the series.


#### Default Value



* "Segoe UI"




#### Example


{% highlight js %}
 
 
$("#container").ejChart({
series :[{ font : { fontFamily : "Algerian"}}]                 
});
 {% endhighlight %}




### series.font.fontStyle `enum`
{:#members:series-font-fontstyle}


<ts ref="ej.datavisualization.Chart.FontStyle"/>

Font Style of the series.


#### Default Value



* "Normal"




#### Example


{% highlight js %}
 
 
$("#container").ejChart({
series : [{font :{fontStyle : "italic"}} ]                
});
{% endhighlight %}




### series.font.fontWeight `enum`
{:#members:series-font-fontweight}

<ts ref="ej.datavisualization.Chart.FontWeight"/>


Font weight of the series.


#### Default Value



* "Regular"




#### Example


{% highlight js %}
 
 
$("#container").ejChart({
series :[{font :{fontWeight : "lighter"}}]                 
});
{% endhighlight %}




### series.font.opacity `number`
{:#members:series-font-opacity}




Opacity of series text.


#### Default Value



* 1




#### Example


{% highlight js %}
 
 
$("#container").ejChart({
series :[{font :{opacity : 0.5}}]                 
});
{% endhighlight %}




### series.font.size `string`
{:#members:series-font-size}




Size of the series text.


#### Default Value



* "12px"




#### Example


{% highlight js %}
 
 
$("#container").ejChart({
series :[{font :{size : "14px"}}]                 
});
 {% endhighlight %}

Try it : [JS Playground Sample](http://jsplayground.syncfusion.com/g0jeybnt)


### series.funnelHeight `string`
{:#members:series-funnelheight}




Specifies the height of the funnel in funnel series. Values can be in both pixel and percentage.


#### Default Value



* "32.7%"




#### Example


{% highlight js %}
 
 
$("#container").ejChart({
series : [{funnelHeight : '40%' }]                   
});
 {% endhighlight %}


Try it : [JS Playground Sample](http://jsplayground.syncfusion.com/5gqzqndn)


### series.funnelWidth `string`
{:#members:series-funnelwidth}




Specifies the width of the funnel in funnel series. Values can be in both pixel and percentage.


#### Default Value



* "11.6%"




#### Example


{% highlight js %}
 
 
$("#container").ejChart({
series : [{funnelWidth : '40%' }]                   
});
 {% endhighlight %}


Try it : [JS Playground Sample](http://jsplayground.syncfusion.com/u0f5hsbw)


### series.gapRatio `number`
{:#members:series-gapratio}




Gap between the slices of pyramid/funnel series.


#### Default Value



 * 0




#### Example


{% highlight js %}
 
 
$("#container").ejChart({
series : [{gapRatio : 0.2 }]                   
});
 {% endhighlight %}

Try it : [JS Playground Sample](http://jsplayground.syncfusion.com/cjocyfce)


### series.isClosed `boolean`
{:#members:series-isclosed}




Specifies whether to join start and end point of a line/area series used in polar/radar chart to form a closed path.


#### Default Value



* true




#### Example


{% highlight js %}
 
 
$("#container").ejChart({
series : [{isClosed : false }]                   
});
 {% endhighlight %}

Try it : [JS Playground Sample](http://jsplayground.syncfusion.com/ktrsbcrh)


### series.isStacking `boolean`
{:#members:series-isstacking}




Specifies whether to stack the column series in polar/radar charts.


#### Default Value



 * true




#### Example


{% highlight js %}
 
 
$("#container").ejChart({
series : [{isStacking : false }]                   
});
 {% endhighlight %}


Try it : [JS Playground Sample](http://jsplayground.syncfusion.com/mj2qdclr)




### series.isTransposed `boolean`
{:#members:series-isTransposed}




Renders the chart vertically. This is applicable only for Cartesian type series.


#### Default Value



* false




#### Example


{% highlight js %}
 
 
$("#container").ejChart({
series : [{isTransposed : false }]                   
});
{% endhighlight %}


Try it : [JS Playground Sample](http://jsplayground.syncfusion.com/1ypcv5bf)



### series.showMedian `boolean`
{:#members:series-showmedian}




Render the x mark in the center of the box and whisker series type.x represents the average value of the box and whisker series.


#### Default Value



* true




#### Example


{% highlight js %}
 
 
$("#container").ejChart({
series : [{showMedian : true }]                   
});
{% endhighlight %}




### series.labelPosition `enum`
{:#members:series-labelposition}

<ts ref="ej.datavisualization.Chart.LabelPosition"/>


Position of the data label in pie/doughnut/pyramid/funnel series. OutsideExtended position is not applicable for pyramid/funnel.



#### Default Value



* "inside". See <a href="ejchart.html#members:commonseriesoptions-labelposition">LabelPosition</a>



#### Example


{% highlight js %}
 
 
$("#container").ejChart({
series : [{labelPosition : "outside" }]                   
});
 {% endhighlight %}
 
 
 Try it: [JS Playground Sample](http://jsplayground.syncfusion.com/q013nk40)


 ### series.splitMode `enum`
{:#members:series-splitmode}

<ts ref="ej.datavisualization.Chart.SplitMode"/>


Specifies the mode for splitting the data points in pieOfPie series.



#### Default Value



* "value". See <a href="ejchart.html#members:commonseriesoptions-splitmode">SplitMode</a>



#### Example


{% highlight js %}
 
 
$("#container").ejChart({
series : [{splitMode : "percentage" }]                   
});
 {% endhighlight %}



### series.boxPlotMode `enum`
{:#members:series-boxplotmode}

<ts ref="ej.datavisualization.Chart.LabelPosition"/>


Quartile calculation has been performed in three different formulas to render the boxplot series .



#### Default Value



* "exclusive".See <a href="ejchart.html#members:commonseriesoptions-boxplotmode">BoxPlotMode</a>



#### Example


{% highlight js %}
 
 
$("#container").ejChart({
series : [{boxPlotMode : "inclusive" }]                   
});
 {% endhighlight %}
 


### series.bubbleOptions `object`
{:#members:series-bubbleoptions}

Options for customizing the bubble options of the Bubble series 

### series.bubbleOptions.radiusMode `enum`
{:#members:series-bubbleoptions-radiusmode}



<ts ref="ej.datavisualization.Chart.RadiusMode"/>


Used for the calculation of the bubble radius based on the mode selected 


#### Default Value



* "minMax" .See <a href="ejchart.html#members:commonseriesoptions-bubbleoptions-radiusmode">RadiusMode</a>



#### Example


{% highlight js %}
 

$("#container").ejChart({
series : [{ bubbleOptions: { radiusMode: "minMax" }}]                  
});

 {% endhighlight %}
 
### series.bubbleOptions.minRadius `number`
{:#members:series-bubbleoptions-minradius}



Used for the setting the minimum radius of the bubble 


#### Default Value



* 1



#### Example


{% highlight js %}
 

$("#container").ejChart({
series : [ { bubbleOptions: { minRadius: 3 }} ]                 
});

 {% endhighlight %}


### series.bubbleOptions.maxRadius `number`
{:#members:series-bubbleoptions-maxradius}



Used for setting the maximum radius of the bubble 


#### Default Value



* 3



#### Example


{% highlight js %}
 

$("#container").ejChart({
series : [ { bubbleOptions: { maxRadius: 7 }} ]                  
});

 {% endhighlight %}

Try it: [JS Playground Sample](http://jsplayground.syncfusion.com/zdnbwech)

### series.splineType `enum`
{:#members:series-splinetype}

<ts ref="ej.datavisualization.Chart.SplineType"/>


Specifies the different types of spline curve. 


#### Default Value



* "Natural". See <a href="ejchart.html#members:commonseriesoptions-splinetype">SplineType</a>




#### Example


{% highlight js %}
 
 
$("#container").ejChart({
series :[{splineType : "cardinal"}]                  
});
{% endhighlight %}


### series.lineCap `enum`
{:#members:series-linecap}

<ts ref="ej.datavisualization.Chart.LineCap"/>


Specifies the line cap of the series. 


#### Default Value



* "Butt". See <a href="ejchart.html#members:commonseriesoptions-linecap">LineCap</a>




#### Example


{% highlight js %}
 
 
$("#container").ejChart({
series :[{lineCap : "butt"}]                  
});
{% endhighlight %}




### series.lineJoin `enum`
{:#members:series-linejoin}

<ts ref="ej.datavisualization.Chart.LineJoin"/>


Specifies the type of shape to be used where two lines meet.


#### Default Value



* "Round". See <a href="ejchart.html#members:commonseriesoptions-linejoin">LineJoin</a>


#### Example


{% highlight js %}
 
 
$("#container").ejChart({
series :[{lineJoin : "round"}]                  
});
{% endhighlight %}





### series.marker `object`
{:#members:series-marker}




Options for displaying and customizing marker for individual point in a series. Marker contains shapes and/or data labels.






### series.marker.border `object`
{:#members:series-marker-border}




Options for customizing the border of the marker shape.






### series.marker.border.color `string`
{:#members:series-marker-border-color}




Border color of the marker shape. 


#### Default Value



* "white"




#### Example


{% highlight js %}
 
 
$("#container").ejChart({
series :[{marker:{border:{color : "green"}}}]                  
});
{% endhighlight %}




### series.marker.border.width `number`
{:#members:series-marker-border-width}




Border width of the marker shape. 


#### Default Value



* 3




#### Example


{% highlight js %}
 

$("#container").ejChart({
series :[{marker :{border :{width : 2}}}]                  
});
{% endhighlight %}


Try it: [JS Playground Sample](http://jsplayground.syncfusion.com/po32cgmg)



### series.marker.dataLabel `object`
{:#members:series-marker-datalabel}




Options for displaying and customizing data labels.






### series.marker.dataLabel.angle `number`
{:#members:series-marker-datalabel-angle}




Angle of the data label in degrees. Only the text gets rotated, whereas the background and border does not rotate. 


#### Default Value



* null




#### Example


{% highlight js %}
 
 
$("#container").ejChart({
series :[{marker :{dataLabel :{angle : 90}}]                  
});
{% endhighlight %}


Try it: [JS Playground Sample](http://jsplayground.syncfusion.com/ulhda01g)


### series.marker.dataLabel.maximumLabelWidth `number`
{:#members:series-marker-datalabel-maximumlabelwidth}


Maximum label width of the data label. 


#### Default Value

 * null


#### Example


{% highlight js %}
 
 
$("#container").ejChart({
series :[{marker :{dataLabel :{maximumLabelWidth : 80}}]                  
});
 {% endhighlight %}


Try it: [JS Playground Sample](http://jsplayground.syncfusion.com/klibjzkp)



### series.marker.dataLabel.enableWrap `boolean`
{:#members:series-marker-datalabel-enablewrap}

Enable the wrap option to the data label. 

#### Default Value

 * false

#### Example

{% highlight js %}
 
 
$("#container").ejChart({
series :[{marker :{dataLabel :{enableWrap : true}}]            
});
 {% endhighlight %}


Try it: [JS Playground Sample](http://jsplayground.syncfusion.com/klibjzkp)

### series.marker.dataLabel.enableContrastColor `boolean`
{:#members:series-marker-datalabel-enablecontrastcolor}

Enables saturation to the data label. 

#### Default Value

 * false

#### Example

{% highlight js %}
$("#container").ejChart({
series :[{marker :{dataLabel :{enableContrastColor : true}}]            
});
 {% endhighlight %}


### series.marker.dataLabel.showEdgeLabels `boolean`
{:#members:series-marker-datalabel-showedgelabels}

Displays the partially visible data labels inside the chart Area.

#### Default Value

 * false

#### Example

{% highlight js %}
$("#container").ejChart({
series :[{marker :{dataLabel :{showEdgeLabels : true}}]            
});
 {% endhighlight %}


### series.marker.dataLabel.border `object`
{:#members:series-marker-datalabel-border}




Options for customizing the border of the data label.






### series.marker.dataLabel.border.color `string`
{:#members:series-marker-datalabel-border-color}




Border color of the data label. 

#### Default Value



* null




#### Example


{% highlight js %}
 
 
$("#container").ejChart({
series :[{marker :{dataLabel :{border : {color : "green"}}}}]                 
});
{% endhighlight %}




### series.marker.dataLabel.border.width `number`
{:#members:series-marker-datalabel-border-width}




Border width of the data label. 


#### Default Value



* 0.1




#### Example


{% highlight js %}
 
 
$("#container").ejChart({
series :[{marker :{dataLabel :{border :{ width :2 }}}}]                 
});
 {% endhighlight %}




### series.marker.dataLabel.connectorLine `object`
{:#members:series-marker-datalabel-connectorline}




Options for displaying and customizing the line that connects point and data label.






### series.marker.dataLabel.connectorLine.type `enum`
{:#members:series-marker-datalabel-connectorline-type}

<ts ref="ej.datavisualization.Chart.Type"/>


Specifies when the connector has to be drawn as Bezier curve or straight line. This is applicable only for Pie and Doughnut chart types. 


#### Default Value



 * "line". See <a href="ejchart.html#members:commonseriesoptions-marker-datalabel-connectorline-type">ConnectorLineType</a>



#### Example


{% highlight js %}
 
 
$("#container").ejChart({
series :[{marker :{dataLabel :{connectorLine :{ type : "bezier" }}}}]                 
});
{% endhighlight %}




### series.marker.dataLabel.connectorLine.width `number`
{:#members:series-marker-datalabel-connectorline-width}




Width of the connector. 


#### Default Value



 * 0.5




#### Example


{% highlight js %}
 
 
$("#container").ejChart({
series :[{marker :{dataLabel :{connectorLine :{ width : 2 }}}}]                 
});
 {% endhighlight %}


Try it: [JS Playground Sample](http://jsplayground.syncfusion.com/fjr0nbgc)


### series.marker.dataLabel.connectorLine.color `string`
{:#members:series-marker-datalabel-connectorline-color}




Color of the connector. 


#### Default Value



 * null




#### Example


{% highlight js %}
 
 
$("#container").ejChart({
series :[{marker :{dataLabel :{connectorLine :{ color : "red" }}}}]                 
});
 {% endhighlight %}
 
 
 
 
 ### series.marker.dataLabel.connectorLine.height `number`
{:#members:series-marker-datalabel-connectorline-color}




Height of the connector. 


#### Default Value



 * null




#### Example


{% highlight js %}
 
 
$("#container").ejChart({
series :[{marker :{dataLabel :{connectorLine :{ height : 10 }}}}]                 
});
 {% endhighlight %}


 



### series.marker.dataLabel.fill `string`
{:#members:series-marker-datalabel-fill}




Background color of the data label. 


#### Default Value



 * null




#### Example


{% highlight js %}
 
 
$("#container").ejChart({
series :[{marker :{dataLabel :{fill : "green"}}}]                 
});
 {% endhighlight %}




### series.marker.dataLabel.font `object`
{:#members:series-marker-datalabel-font}




Options for customizing the data label font.






### series.marker.dataLabel.font.fontFamily `string`
{:#members:series-marker-datalabel-font-fontfamily}




Font family of the data label. 


#### Default Value



* "Segoe UI"




#### Example


{% highlight js %}
 

$("#container").ejChart({
series :[{marker :{dataLabel :{ font :{fontFamily : "algerian"}}}}]                 
});
 {% endhighlight %}


### series.marker.dataLabel.font.color `string`
{:#members:series-marker-datalabel-font-color}

Font color of the data label text. 

#### Default Value

 * null

#### Example

{% highlight js %}

 
$("#container").ejChart({
series :[{marker :{dataLabel :{ font :{color : "red"}}}}]               
});
{% endhighlight %}

### series.marker.dataLabel.font.fontStyle `enum`
{:#members:series-marker-datalabel-font-fontstyle}

<ts ref="ej.datavisualization.Chart.FontStyle"/>


Font style of the data label.  


#### Default Value



* "normal". See <a href="ejchart.html#members:commonseriesoptions-marker-datalabel-font-fontstyle">FontStyle</a>




#### Example


{% highlight js %}
 
 
$("#container").ejChart({
series :[{marker :{dataLabel :{font :{ fontStyle : "italic" }}}}]                 
});
 {% endhighlight %}




### series.marker.dataLabel.font.fontWeight `enum`
{:#members:series-marker-datalabel-font-fontweight}

<ts ref="ej.datavisualization.Chart.FontWeight"/>


Font weight of the data label. 


#### Default Value



* "regular". See <a href="ejchart.html#members:commonseriesoptions-marker-datalabel-font-fontweight">FontWeight</a>


#### Example


{% highlight js %}
 
 
$("#container").ejChart({
series :[{marker :{dataLabel :{font : { fontWeight : "lighter" }}}}]                 
});
{% endhighlight %}




### series.marker.dataLabel.font.opacity `number`
{:#members:series-marker-datalabel-font-opacity}




Opacity of the text. 


#### Default Value



* 1




#### Example


{% highlight js %}
 
 
$("#container").ejChart({
series :[{marker :{dataLabel :{font :{ opacity : 0.5 }}}}]                 
});
{% endhighlight %}




### series.marker.dataLabel.font.size `string`
{:#members:series-marker-datalabel-font-size}




Font size of the data label. 


#### Default Value



 * "12px"




#### Example


{% highlight js %}
 
 
$("#container").ejChart({
series :[{marker :{dataLabel :{font : { size : "14px" }}}}]                 
});
{% endhighlight %}



Try it: [JS Playground Sample](http://jsplayground.syncfusion.com/fjr0nbgc)



### series.marker.dataLabel.horizontalTextAlignment `enum`
{:#members:series-marker-datalabel-horizontaltextalignment}

<ts ref="ej.datavisualization.Chart.HorizontalTextAlignment"/>


Horizontal alignment of the data label. 


#### Default Value



* "center"




#### Example


{% highlight js %}
 
 
$("#container").ejChart({
series :[{marker :{dataLabel :{horizontalTextAlignment : "far"}}}]                  
});
{% endhighlight %}




### series.marker.dataLabel.margin `object`
{:#members:series-marker-datalabel-margin}




Margin of the text to its background shape. The size of the background shape increases based on the margin applied to its text.






### series.marker.dataLabel.margin.bottom `number`
{:#members:series-marker-datalabel-margin-bottom}




Bottom margin of the text. 


#### Default Value



* 5




#### Example


{% highlight js %}
 
 
$("#container").ejChart({
series :[{marker :{dataLabel :{margin :{ bottom :10 }}}}]                 
});
{% endhighlight %}




### series.marker.dataLabel.margin.left `number`
{:#members:series-marker-datalabel-margin-left}




Left margin of the text. 


#### Default Value



 * 5




#### Example


{% highlight js %}
 
 
$("#container").ejChart({
series :[{marker :{dataLabel :{margin :{ left : 10}}}}]                 
});
{% endhighlight %}




### series.marker.dataLabel.margin.right `number`
{:#members:series-marker-datalabel-margin-right}




Right margin of the text. 


#### Default Value



* 5




#### Example


{% highlight js %}
 
 
$("#container").ejChart({
series :[{marker :{dataLabel :{margin :{ right :10 }}}}]                 
});
{% endhighlight %}




### series.marker.dataLabel.margin.top `number`
{:#members:series-marker-datalabel-margin-top}




Top margin of the text. 


#### Default Value



* 5




#### Example


{% highlight js %}
 
 
$("#container").ejChart({
series :[{marker :{dataLabel :{margin :{ top :10 } }}}]                 
});
{% endhighlight %}


Try it: [JS Playground Sample](http://jsplayground.syncfusion.com/3yoplr42)



### series.marker.dataLabel.opacity `number`
{:#members:series-marker-datalabel-opacity}




Opacity of the data label. 


#### Default Value



* 1




#### Example


{% highlight js %}
 
 
$("#container").ejChart({
series :[{marker :{dataLabel :{opacity : 0.5}}}]                 
});
{% endhighlight %}




### series.marker.dataLabel.shape `enum`
{:#members:series-marker-datalabel-shape}

<ts ref="ej.datavisualization.Chart.Shape"/>


Background shape of the data label. 


#### Default Value



* No shape is rendered by default, so its value is ‘none’. See <a href="ejchart.html#members:commonseriesoptions-marker-datalabel-shape">Shape</a>


#### Example


{% highlight js %}
 
 
$("#container").ejChart({
series :[{marker :{dataLabel :{shape : "circle"}}}]                 
});
{% endhighlight %}




### series.marker.dataLabel.textMappingName `string`
{:#members:series-marker-datalabel-textmappingname}




Name of a field in data source where datalabel text is displayed.  


#### Default Value



* ""


#### Example


{% highlight js %}
 
 
$("#container").ejChart({
series :[{marker :{dataLabel :{textMappingName : "TextFieldName"}}}]                 
});
{% endhighlight %}




### series.marker.dataLabel.textPosition `enum`
{:#members:series-marker-datalabel-textposition}

<ts ref="ej.datavisualization.Chart.TextPosition"/>


Specifies the position of the data label. This property can be used only for the series such as column, bar, stacked column, stacked bar, 100% stacked column, 100% stacked bar, candle and OHLC. 


#### Default Value



* "top". See <a href="ejchart.html#members:commonseriesoptions-marker-datalabel-textposition">TextPosition</a>


#### Example


{% highlight js %}
 
 
$("#container").ejChart({
series :[{marker :{dataLabel :{textPosition : "bottom"}}}]                 
});
{% endhighlight %}




### series.marker.dataLabel.verticalTextAlignment `enum`
{:#members:series-marker-datalabel-verticaltextalignment}

<ts ref="ej.datavisualization.Chart.VerticalTextAlignment"/>


Vertical alignment of the data label. 


#### Default Value



* 'center'




#### Example


{% highlight js %}
 

$("#container").ejChart({
series :[{marker :{dataLabel :{verticalTextAlignment : "far"}}}]                  
});
{% endhighlight %}


Try it: [JS Playground Sample](http://jsplayground.syncfusion.com/emylj2pu)


### series.marker.dataLabel.visible `boolean`
{:#members:series-marker-datalabel-visible}




Controls the visibility of the data labels. 


#### Default Value



* false




#### Example


{% highlight js %}
 

$("#container").ejChart({
series :[{marker :{dataLabel :{visible : true}}}]                  
});
 {% endhighlight %}


### series.marker.dataLabel.template `string`
{:#members:series-marker-datalabel-template}




Custom template to format the data label content. Use “point.x” and “point.y” as a placeholder text to display the corresponding data point’s x and y value.


#### Default Value



* ""




#### Example


{% highlight js %}
 

$("#container").ejChart({
series :[{marker :{dataLabel :{template : "item"}}}]                  
});
 {% endhighlight %}
 
 Try it: [JS Playground Sample](http://jsplayground.syncfusion.com/l5pmkkgr)
 
 
 
 
### series.marker.dataLabel.offset `object|number`
{:#members:series-marker-datalabel-offset}

Options for customizing the datalabel positions

### series.marker.dataLabel.offset.x `number`

{:#members:series-marker-datalabel-offset-x}




X value or horizontal offset to position the labels in chart.


#### Default Value

* 0




#### Example


{% highlight js %}
 
$("#container").ejChart({

   series :[{  marker :{dataLabel :{offset : { x:10 }}} }]                    

});

{% endhighlight %}




### series.marker.dataLabel.offset.y `number`
{:#members:series-marker-datalabel-offset-y}




Y value or vertical offset to position the labels.


#### Default Value

* 0




#### Example


{% highlight js %}
 
$("#container").ejChart({

   series :[{  marker :{dataLabel :{offset : { y:10 }}} }]                  

});

{% endhighlight %}



### series.marker.fill `string`
{:#members:series-marker-fill}




Color of the marker shape. 


#### Default Value



* null




#### Example


{% highlight js %}
 
 
$("#container").ejChart({
series :[{marker : { fill : "green" } }]                  
});
{% endhighlight %}




### series.marker.imageUrl `string`
{:#members:series-marker-imageurl}




The URL for the Image that is to be displayed as marker. In order to display image as marker, set series.marker.shape as ‘image’.


#### Default Value



* ""




#### Example


{% highlight js %}
 
 
$("#container").ejChart({
series :[{marker :{ imageUrl: "../images/sample.png"}}]                  
});
{% endhighlight %}




### series.marker.opacity `number`
{:#members:series-marker-opacity}




Opacity of the marker. 


#### Default Value



 * 1




#### Example


{% highlight js %}
 
 
$("#container").ejChart({
series :[{marker :{ opacity : 0.5 }}]                  
});
{% endhighlight %}


Try it: [JS Playground Sample](http://jsplayground.syncfusion.com/1bavaoqq)



### series.marker.shape `enum`
{:#members:series-marker-shape}

<ts ref="ej.datavisualization.Chart.Shape"/>


Specifies the shape of the marker.  


#### Default Value



* "circle". See <a href="ejchart.html#members:commonseriesoptions-marker-shape">Shape</a>


#### Example


{% highlight js %}
 
 
$("#container").ejChart({
series :[{marker :{ shape: "rectangle"}]                  
});
{% endhighlight %}


Try it: [JS Playground Sample](http://jsplayground.syncfusion.com/vd552nid)


### series.marker.size `object`
{:#members:series-marker-size}




Options for customizing the size of the marker shape.






### series.marker.size.height `number`
{:#members:series-marker-size-height}




Height of the marker. 


#### Default Value



* 6




#### Example


{% highlight js %}
 
 
$("#container").ejChart({
series :[{marker :{size :{height : 5}}}]                 
});
{% endhighlight %}




### series.marker.size.width `number`
{:#members:series-marker-size-width}




Width of the marker. 


#### Default Value



* 6




#### Example


{% highlight js %}
 
 
$("#container").ejChart({
series :[{marker :{ size :{ width : 2 } } }]                  
});
{% endhighlight %}


Try it: [JS Playground Sample](http://jsplayground.syncfusion.com/53gkiuse)


### series.marker.visible `boolean`
{:#members:series-marker-visible}




Controls the visibility of the marker shape. 


#### Default Value



* false




#### Example


{% highlight js %}
 
 
$("#container").ejChart({
series :[{marker :{ visible : true}}]                  
});
 {% endhighlight %}


### series.name `string`
{:#members:series-name}




Name of the series, that is to be displayed in the legend.



#### Default Value


Add a comment to this line

 * ""


#### Example


{% highlight js %}
 
$("#container").ejChart({
   series : [{name: "India" }]                   
});

{% endhighlight %} 


### series.opacity `number`
{:#members:series-opacity}




Opacity of the series.


#### Default Value



* 1




#### Example


{% highlight js %}
 
 
$("#container").ejChart({
series :[{opacity : 0.5}]                  
});
 {% endhighlight %}



### series.outlierSettings `object`
{:#members:series-outliersettings}




Options for customizing the outlier of individual series.


### series.outlierSettings.shape `enum`
{:#members:series-outliersettings-shape}

<ts ref="ej.datavisualization.Chart.Shape"/>


Specifies the shape of the outlier.  


#### Default Value



* "circle". See <a href="ejchart.html#members:commonseriesoptions-outliersettings-shape">Shape</a>


#### Example


{% highlight js %}
 
 
$("#container").ejChart({
series :[{outlierSettings :{ shape: "rectangle"}]                  
});
{% endhighlight %}





### series.outlierSettings.size `object`
{:#members:series-outliersettings-size}




Options for customizing the size of the outlier shape.






### series.outlierSettings.size.height `number`
{:#members:series-outliersettings-size-height}




Height of the outlier shape. 


#### Default Value



* 6




#### Example


{% highlight js %}
 
 
$("#container").ejChart({
series :[{outlierSettings :{size :{height : 5}}}]                 
});
{% endhighlight %}








### series.outlierSettings.size.width `number`
{:#members:series-outliersettings-size-width}




Width of the outlier shape. 


#### Default Value



* 6




#### Example


{% highlight js %}
 
 
$("#container").ejChart({
series :[{outlierSettings :{ size :{ width : 2 } } }]                  
});
{% endhighlight %}



 
 
 
 
### series.palette `string`
{:#members:series-palette}




Name of a field in data source where fill color for all the data points is generated.


#### Default Value



* ""




#### Example


{% highlight js %}
 
 
$("#container").ejChart({
series :[{palette : "ColorFieldName"}]                  
});
{% endhighlight %}




### series.pieCoefficient `number`
{:#members:series-piecoefficient}




Controls the size of pie series. Value ranges from 0 to 1.




#### Default Value



 * 0.8




#### Example


{% highlight js %}
 
 
$("#container").ejChart({
series : [{pieCoefficient : 0.6 }]                   
});
 {% endhighlight %}



Try it: [JS Playground Sample](http://jsplayground.syncfusion.com/hpl0ffff)

### series.pieOfPieCoefficient `number`
{:#members:series-pieofpiecoefficient}




Controls the size of the second pie in pieOfPie series. Value ranges from 0 to 1.




#### Default Value



 * 0.6




#### Example


{% highlight js %}
 
 
$("#container").ejChart({
series : [{pieOfPieCoefficient : 0.8 }]                   
});
 {% endhighlight %}

### series.splitValue `string`
{:#members:series-splitvalue}


Split Value of pieOfPie series.


#### Default Value



 * null



#### Example


{% highlight js %}
 
 
$("#container").ejChart({
series : [{splitValue: "40" }]                   
});
{% endhighlight %}

### series.gapWidth `number`
{:#members:series-gapwidth}




Distance between the two pie's in pieOfPie series.


#### Default Value



 * 50




#### Example


{% highlight js %}
 
 
$("#container").ejChart({
series : [{gapWidth : 300 }]                   
});
 {% endhighlight %}

### series.emptyPointSettings `object`
{:#members:series-emptypointsettings}




Options for customizing the empty point in the series.


### series.emptyPointSettings.visible `boolean`
{:#members:series-emptypointsettings-visible}




Controls the visibility of the empty point.



#### Default Value



 * true




#### Example


{% highlight js %}
 
 
$("#container").ejChart({
series : [{
      emptyPointSettings: {

           visible : false,
       } 
    }]                   
});
 {% endhighlight %}



Try it: [JS Playground Sample](http://jsplayground.syncfusion.com/hpl0ffff)


### series.emptyPointSettings.displayMode `enum`
{:#members:series-emptypointsettings-displaymode}

<ts ref="ej.datavisualization.Chart.EmptyPointMode"/>


Specifies the mode of empty point.



#### Default Value



 * "gap"




#### Example


{% highlight js %}
 
 
$("#container").ejChart({
series : [{
      emptyPointSettings: {

           displayMode : "gap",
       } 
    }]                   
});
 {% endhighlight %}
 
See [Mode](https://help.syncfusion.com/api/js/global#members:mode). 

 
### series.emptyPointSettings.style `object`
{:#members:series-emptypointsettings-style}




Options for customizing the color and border of the empty point in the series.


### series.emptyPointSettings.style.color `string`
{:#members:series-emptypointsettings-style-color}




Color of the empty point.



#### Default Value



 * ""




#### Example


{% highlight js %}
 
 
$("#container").ejChart({
series : [{
      emptyPointSettings: {

           style: { color : "red" }
       } 
    }]                   
});
 {% endhighlight %}
 
 
### series.emptyPointSettings.style.border `object`
{:#members:series-emptypointsettings-style-border}




Options for customizing border of the empty point in the series.
 

### series.emptyPointSettings.style.border.color `string`
{:#members:series-emptypointsettings-style-border-color}




Border color of the empty point.



#### Default Value



 * ""




#### Example


{% highlight js %}
 
 
$("#container").ejChart({
series : [{
      emptyPointSettings: {

           style: { border: { color : "red" } }
       } 
    }]                   
});
 {% endhighlight %}
 

### series.emptyPointSettings.style.border.width `number`
{:#members:series-emptypointsettings-style-border-width}




Border width of the empty point.



#### Default Value



 * 1




#### Example


{% highlight js %}
 
 
$("#container").ejChart({
series : [{
      emptyPointSettings: {

           style: { border: { width : 1.2 } }
       } 
    }]                   
});
 {% endhighlight %}
 

 
### series.positiveFill `string`
{:#members:series-positivefill}




Fill color for the positive column of the waterfall.



#### Default Value



 * null




#### Example


{% highlight js %}
 
 
$("#container").ejChart({
series : [{
                positiveFill : “Red”
    }]                   
});
 {% endhighlight %}     
 
 Try it: [JS Playground Sample](http://jsplayground.syncfusion.com/t5dhe5d0)
 
 
### series.connectorLine `object`
{:#members:series-connectorline}




Options for customizing the waterfall connector line.

Try it: [JS Playground Sample](http://jsplayground.syncfusion.com/t5dhe5d0)


### series.connectorLine.width `number`
{:#members:series-connectorline-width}




Width of the connector line.



#### Default Value



 * 1




#### Example


{% highlight js %}
 
 
$("#container").ejChart({
series : [{
             connectorLine: {width : 1 }
    }]                   
});
 {% endhighlight %} 
 

### series.connectorLine.color `string`
{:#members:series-connectorline-color}




Color of the connector line.



#### Default Value



 * "#565656"




#### Example


{% highlight js %}
 
 
$("#container").ejChart({
    series : [{
             connectorLine: {color : "grey" }
    }]                   
});
 {% endhighlight %} 
 
 

### series.connectorLine.dashArray `string`
{:#members:series-connectorline-dasharray}




DashArray of the connector line.



#### Default Value



 * null




#### Example


{% highlight js %}
 
 
$("#container").ejChart({
    series : [{
             connectorLine: {dashArray : "2,3" }
    }]                   
});
 {% endhighlight %} 
 



### series.connectorLine.opacity `number`
{:#members:series-connectorline-opacity}




Opacity of the connector line.



#### Default Value



 * 1




#### Example


{% highlight js %}
 
 
$("#container").ejChart({
    series : [{
             connectorLine: {opacity : 0.5 }
    }]                   
});
 {% endhighlight %} 


 
### series.dragSettings `object`
{:#members:series-dragsettings}

Options to customize the drag and drop in series.

### series.dragSettings.enable `boolean`
{:#members:series-dragsettings-enable}

drag/drop the series

#### Default Value

* "false"

#### Example


{% highlight js %}
 
 
$("#container").ejChart({
    series : [{
          dragSettings:{enable: true}
    }]                  
});

 {% endhighlight %} 

### series.dragSettings.type `string`
{:#members:series-dragsettings-type}


Specifies the type of drag settings.


#### Default Value


* "xy"

#### Example


{% highlight js %}
 
 
$("#container").ejChart({
    series : [{
          dragSettings:{type: "x"}
    }]                   
});
 {% endhighlight %} 
 

### series.errorBar `object`
{:#members:series-errorbar}


Options to customize the error bar in series.



### series.errorBar.visibility `boolean`
{:#members:series-errorbar-visibility}


Show/hides the error bar

#### Default Value



 * "visible"




#### Example


{% highlight js %}
 
 
$("#container").ejChart({
    series : [{
          errorBar:{visibility: "hidden"}
    }]                   
});
 {% endhighlight %} 
 
 
 Try it: [JS Playground Sample](http://jsplayground.syncfusion.com/t5dhe5d0) 
   
### series.errorBar.type `enum`
{:#members:series-errorbar-type}

<ts ref="ej.datavisualization.Chart.ErrorBarType"/>

Specifies the type of error bar.

#### Default Value



 * "FixedValue"




#### Example


{% highlight js %}
 
 
$("#container").ejChart({
    series : [{
          errorBar:{type: "Percentage"}
    }]                   
});
 {% endhighlight %} 
 
 Try it: [JS Playground Sample](http://jsplayground.syncfusion.com/t5dhe5d0) 
 
### series.errorBar.mode `enum`
{:#members:series-errorbar-mode}

<ts ref="ej.datavisualization.Chart.ErrorBarMode"/>
Specifies the mode of error bar.

#### Default Value



 * "vertical"




#### Example


{% highlight js %}
 
 
$("#container").ejChart({
    series : [{
          errorBar:{mode: "Horizontal"}
    }]                   
});
 {% endhighlight %} 
 
 Try it: [JS Playground Sample](http://jsplayground.syncfusion.com/t5dhe5d0) 
 

### series.errorBar.direction `enum`
{:#members:series-errorbar-direction}

<ts ref="ej.datavisualization.Chart.ErrorBarDirection"/>

Specifies the direction of error bar.

#### Default Value



 * "both"




#### Example


{% highlight js %}
 
 
$("#container").ejChart({
    series : [{
          errorBar:{direction: "plus"}
    }]                   
});
 {% endhighlight %} 
 
 Try it: [JS Playground Sample](http://jsplayground.syncfusion.com/t5dhe5d0) 
 

### series.errorBar.verticalErrorValue `number`
{:#members:series-errorbar-verticalerrorvalue}


Value of vertical error bar.

#### Default Value



 * 3




#### Example


{% highlight js %}
 
 
$("#container").ejChart({
    series : [{
          errorBar:{verticalErrorValue: 1}
    }]                   
});
 {% endhighlight %} 
 
Try it: [JS Playground Sample](http://jsplayground.syncfusion.com/t5dhe5d0) 

### series.errorBar.horizontalErrorValue `number`
{:#members:series-errorbar-horizontalerrorvalue}


Value of horizontal  error bar.

#### Default Value



 * 1




#### Example


{% highlight js %}
 
 
$("#container").ejChart({
    series : [{
          errorBar:{horizontalErrorValue: 1}
    }]                   
});
 {% endhighlight %} 
 
Try it: [JS Playground Sample](http://jsplayground.syncfusion.com/t5dhe5d0) 


### series.errorBar.horizontalPositiveErrorValue `number`
{:#members:series-errorbar-horizontalpositiveerrorvalue}


Value of positive horizontal error bar.

#### Default Value



 * 1




#### Example


{% highlight js %}
 
 
$("#container").ejChart({
    series : [{
          errorBar:{horizontalPositiveErrorValue: 1}
    }]                   
});
 {% endhighlight %} 
 
Try it: [JS Playground Sample](http://jsplayground.syncfusion.com/t5dhe5d0) 



### series.errorBar.horizontalNegativeErrorValue `number`
{:#members:series-errorbar-horizontalnegativeerrorvalue}


Value of negative horizontal error bar.

#### Default Value



 * 1




#### Example


{% highlight js %}
 
 
$("#container").ejChart({
    series : [{
          errorBar:{horizontalNegativeErrorValue: 1}
    }]                   
});
 {% endhighlight %} 
 
Try it: [JS Playground Sample](http://jsplayground.syncfusion.com/t5dhe5d0) 


### series.errorBar.verticalPositiveErrorValue `number`
{:#members:series-errorbar-verticalpositiveerrorvalue}


Value of positive vertical error bar.

#### Default Value



 * 5




#### Example


{% highlight js %}
 
 
$("#container").ejChart({
    series : [{
          errorBar:{verticalPositiveErrorValue: 1}
    }]                   
});
 {% endhighlight %} 
 
Try it: [JS Playground Sample](http://jsplayground.syncfusion.com/t5dhe5d0) 



### series.errorBar.verticalNegativeErrorValue `number`
{:#members:series-errorbar-verticalnegativeerrorvalue}


Value of negative vertical error bar.

#### Default Value



 * 5




#### Example


{% highlight js %}
 
 
$("#container").ejChart({
    series : [{
          errorBar:{verticalNegativeErrorValue: 1}
    }]                   
});
 {% endhighlight %} 
 
Try it: [JS Playground Sample](http://jsplayground.syncfusion.com/t5dhe5d0) 


### series.errorBar.fill `string`
{:#members:series-errorbar-fill}


Fill color of the error bar.

#### Default Value



 * "#000000"




#### Example


{% highlight js %}
 
 
$("#container").ejChart({
    series : [{
        errorBar:{       
           fill:”red”
        }

    }]                   
});
 {% endhighlight %} 
 
Try it: [JS Playground Sample](http://jsplayground.syncfusion.com/t5dhe5d0) 
    

### series.errorBar.width `number`
{:#members:series-errorbar-width}


Width of the error bar.

#### Default Value



 * 1




#### Example


{% highlight js %}
 
 
$("#container").ejChart({
    series : [{
        errorBar:{       
           width: 1
        }

    }]                   
});
 {% endhighlight %} 



### series.errorBar.cap `object`
{:#members:series-errorbar-cap}


Options for customizing the error bar cap.

Try it: [JS Playground Sample](http://jsplayground.syncfusion.com/t5dhe5d0) 


### series.errorBar.cap.visible `boolean`
{:#members:series-errorbar-cap-visible}

Show/Hides the error bar cap.

#### Default Value



 * true




#### Example


{% highlight js %}
 
 
$("#container").ejChart({
    series : [{
       errorBar:{       
         cap:{visible:false}
        }
    }]                   
});
 {% endhighlight %} 
 

### series.errorBar.cap.width `number`
{:#members:series-errorbar-cap-width}

Width of the error bar cap.

#### Default Value



 * 1




#### Example


{% highlight js %}
 
 
$("#container").ejChart({
    series : [{
       errorBar:{       
         cap:{width:1}
        }
    }]                   
});
 {% endhighlight %} 
 
 
 
### series.errorBar.cap.length `number`
{:#members:series-errorbar-cap-length}

Length of the error bar cap.

#### Default Value



 * 1




#### Example


{% highlight js %}
 
 
$("#container").ejChart({
    series : [{
       errorBar:{       
         cap:{length: 10}
        }
    }]                   
});
 {% endhighlight %} 
 

### series.errorBar.cap.fill `string`
{:#members:series-errorbar-cap-fill}

Color of the error bar cap.

#### Default Value



 *  "#000000"




#### Example


{% highlight js %}
 
 
$("#container").ejChart({
    series : [{
       errorBar:{       
         cap:{fill: "red"}
        }
    }]                   
});
 {% endhighlight %} 
 
  

### series.points `array`
{:#members:series-points}




Option to add data points; each point should have x and y property. Also, optionally, you can customize the points color, border, marker by using fill, border and marker options.




### series.points.border `object`
{:#members:series-points-border}




Options for customizing the border of a point. This is applicable only for column type series and accumulation type series.






### series.points.border.color `string`
{:#members:series-points-border-color}




Border color of the point. 


#### Default Value



* null




#### Example


{% highlight js %}
 
 
$("#container").ejChart({
series :[{ points:[{ border:{color : "green"} }] }]                  
});
{% endhighlight %}




### series.points.border.width `number`
{:#members:series-points-border-width}




Border width of the point. 


#### Default Value



* null




#### Example


{% highlight js %}
 

$("#container").ejChart({
series :[{ points:[{ border :{width : 2} }] }]                  
});
{% endhighlight %}


Try it: [JS Playground Sample](http://jsplayground.syncfusion.com/t5dhe5d0)




### series.points.visibleOnLegend `string`
{:#members:series-points-visibleonlegend}




Enables or disables the visibility of legend item.



#### Default Value



 * "visible"




#### Example


{% highlight js %}
 

$("#container").ejChart({
      series : [{
          points: [{x: "Wheat", y: 394, visibleOnLegend: "hidden" },
             //...
           ] 
      }]                   
});
{% endhighlight %}


### series.points.showIntermediateSum `boolean`
{:#members:series-points-showintermediatesum}




To show/hide the intermediate summary from the last intermediate point.


#### Default Value



* false




#### Example


{% highlight js %}
 

$("#container").ejChart({
series :[{ points:[{ showIntermediateSum : true }] }]                  
});
{% endhighlight %}


Try it: [JS Playground Sample](http://jsplayground.syncfusion.com/Sync_t1fwledt)

### series.points.showTotalSum `boolean`
{:#members:series-points-showtotalsum}




To show/hide the total summary of the waterfall series.


#### Default Value



* false




#### Example


{% highlight js %}
 

$("#container").ejChart({
series :[{ points:[{ showTotalSum : true }] }]                  
});
{% endhighlight %}


Try it: [JS Playground Sample](http://jsplayground.syncfusion.com/Sync_t1fwledt)


### series.points.close `number`
{:#members:series-points-close}




Close value of the point. Close value is applicable only for financial type series.


#### Default Value



* null




#### Example


{% highlight js %}
 
 
$("#container").ejChart({
series :[{ points:[{ close : 50 }] }]                  
});
{% endhighlight %}


### series.points.size `number`
{:#members:series-points-size}




Size of a bubble in the bubble series. This is applicable only for the bubble series.


#### Default Value



* null




#### Example


{% highlight js %}
 
 
$("#container").ejChart({
series :[{ points:[{ size : 5 }] }]                  
});
{% endhighlight %}




### series.points.fill `string`
{:#members:series-points-fill}




Background color of the point. This is applicable only for column type series and accumulation type series. 


#### Default Value



* null




#### Example


{% highlight js %}
 
 
$("#container").ejChart({
series :[{ points:[{ fill : "green" }] }]                  
});
{% endhighlight %}




### series.points.high `number`
{:#members:series-points-high}




High value of the point. High value is applicable only for financial type series, range area series and range column series.


#### Default Value



* null




#### Example


{% highlight js %}
 
 
$("#container").ejChart({
series :[{ points:[{ high : 120 }] }]                  
});
{% endhighlight %}




### series.points.low `number`
{:#members:series-points-x}




Low value of the point. Low value is applicable only for financial type series, range area series and range column series.


#### Default Value



* null




#### Example


{% highlight js %}
 
 
$("#container").ejChart({
series :[{ points:[{ low : 70 }] }]                  
});
{% endhighlight %}




### series.points.marker `object`
{:#members:series-points-marker}




Options for displaying and customizing marker for a data point. Marker contains shapes and/or data labels.






### series.points.marker.border `object`
{:#members:series-points-marker-border}




Options for customizing the border of the marker shape.






### series.points.marker.border.color `string`
{:#members:series-points-marker-border-color}




Border color of the marker shape. 


#### Default Value



* "white"




#### Example


{% highlight js %}
 
 
$("#container").ejChart({
series :[{ points:[{ marker:{border:{color : "green"}} }] }]                  
});
{% endhighlight %}




### series.points.marker.border.width `number`
{:#members:series-points-marker-border-width}




Border width of the marker shape. 


#### Default Value



* 3




#### Example


{% highlight js %}
 

$("#container").ejChart({
series :[{ points:[{ marker :{border :{width : 2}} }] }]                  
});
{% endhighlight %}


Try it: [JS Playground Sample](http://jsplayground.syncfusion.com/3vkjgyc0)



### series.points.marker.dataLabel `object`
{:#members:series-points-marker-datalabel}




Options for displaying and customizing data label.






### series.points.marker.dataLabel.angle `number`
{:#members:series-points-marker-datalabel-angle}




Angle of the data label in degrees. Only the text gets rotated, whereas the background and border does not rotate. 


#### Default Value



* null




#### Example


{% highlight js %}
 
 
$("#container").ejChart({
series :[{ points:[{ marker :{dataLabel :{angle : 90} }] }]                  
});
{% endhighlight %}


Try it: [JS Playground Sample](http://jsplayground.syncfusion.com/d3r5mcfc)


### series.points.marker.dataLabel.border `object`
{:#members:series-points-marker-datalabel-border}




Options for customizing the border of the data label.






### series.points.marker.dataLabel.border.color `string`
{:#members:series-points-marker-datalabel-border-color}




Border color of the data label. 

#### Default Value



* null




#### Example


{% highlight js %}
 
 
$("#container").ejChart({
series :[{ points:[{ marker :{dataLabel :{border : {color : "green"}}} }] }]                 
});
{% endhighlight %}




### series.points.marker.dataLabel.border.width `number`
{:#members:series-points-marker-datalabel-border-width}




Border width of the data label. 


#### Default Value



* 0.1




#### Example


{% highlight js %}
 
 
$("#container").ejChart({
series :[{ points:[{ marker :{dataLabel :{border :{ width :2 }}} }] }]                 
});
 {% endhighlight %}




### series.points.marker.dataLabel.connectorLine `object`
{:#members:series-points-marker-datalabel-connectorline}




Options for displaying and customizing the line that connects point and data label.






### series.points.marker.dataLabel.connectorLine.type `enum`
{:#members:series-points-marker-datalabel-connectorline-type}

<ts ref="ej.datavisualization.Chart.ConnectorLineType"/>


Specifies when the connector has to be drawn as Bezier curve or straight line. This is applicable only for Pie and Doughnut chart types. 


#### Default Value



 * "line". See <a href="ejchart.html#members:commonseriesoptions-points-marker-datalabel-connectorline-type">ConnectorLineType</a>



#### Example


{% highlight js %}
 
 
$("#container").ejChart({
series :[{ points:[{ marker :{dataLabel :{connectorLine :{ type : "bezier" }}} }] }]                 
});
{% endhighlight %}




### series.points.marker.dataLabel.connectorLine.width `number`
{:#members:series-points-marker-datalabel-connectorline-width}




Width of the connector. 


#### Default Value



 * 0.5




#### Example


{% highlight js %}
 
 
$("#container").ejChart({
series :[{ points:[{ marker :{dataLabel :{connectorLine :{ width : 2 }}} }] }]                 
});
 {% endhighlight %}


Try it: [JS Playground Sample](http://jsplayground.syncfusion.com/tm0wneyn)



### series.points.marker.dataLabel.fill `string`
{:#members:series-points-marker-datalabel-fill}




Background color of the data label. 


#### Default Value



 * null




#### Example


{% highlight js %}
 
 
$("#container").ejChart({
series :[{ points:[{ marker :{dataLabel :{fill : "green"}}}]}]                 
});
 {% endhighlight %}




### series.points.marker.dataLabel.font `object`
{:#members:series-points-marker-datalabel-font}




Options for customizing the data label font.






### series.points.marker.dataLabel.font.fontFamily `string`
{:#members:series-points-marker-datalabel-font-fontfamily}




Font family of the data label. 


#### Default Value



* "Segoe UI"




#### Example


{% highlight js %}
 

$("#container").ejChart({
series :[{ points:[{marker :{dataLabel :{ font :{fontFamily : "algerian"}}}}]}]                 
});
 {% endhighlight %}




### series.points.marker.dataLabel.font.fontStyle `enum`
{:#members:series-points-marker-datalabel-font-fontstyle}

<ts ref="ej.datavisualization.Chart.FontStyle"/>



Font style of the data label.  


#### Default Value



* "normal". See <a href="ejchart.html#members:commonseriesoptions-points-marker-datalabel-font-fontstyle">FontStyle</a>




#### Example


{% highlight js %}
 
 
$("#container").ejChart({
series :[{points:[{marker :{dataLabel :{font :{ fontStyle : "italic" }}}}]}]                 
});
 {% endhighlight %}




### series.points.marker.dataLabel.font.fontWeight `enum`
{:#members:series-points-marker-datalabel-font-fontweight}

<ts ref="ej.datavisualization.Chart.FontWeight"/>


Font weight of the data label. 


#### Default Value



* "regular". See <a href="ejchart.html#members:commonseriesoptions-points-marker-datalabel-font-fontweight">FontWeight</a>


#### Example


{% highlight js %}
 
 
$("#container").ejChart({
series :[{ points:[{ marker :{dataLabel :{font : { fontWeight : "lighter" }}}}] }]                 
});
{% endhighlight %}




### series.points.marker.dataLabel.font.opacity `number`
{:#members:series-points-marker-datalabel-font-opacity}




Opacity of the text. 


#### Default Value



* 1




#### Example


{% highlight js %}
 
 
$("#container").ejChart({
series :[{ points:[{ marker :{dataLabel :{font :{ opacity : 0.5 }}}}] }]                 
});
{% endhighlight %}




### series.points.marker.dataLabel.font.size `string`
{:#members:series-points-marker-datalabel-font-size}




Font size of the data label. 


#### Default Value



 * "12px"




#### Example


{% highlight js %}
 
 
$("#container").ejChart({
series :[{ points:[{ marker :{dataLabel :{font : { size : "14px" }}}}] }]                 
});
{% endhighlight %}



Try it: [JS Playground Sample](http://jsplayground.syncfusion.com/v4rp3aio)



### series.points.marker.dataLabel.horizontalTextAlignment `enum`
{:#members:series-points-marker-datalabel-horizontaltextalignment}

<ts ref="ej.datavisualization.Chart.HorizontalTextAlignment"/>


Horizontal alignment of the data label. 


#### Default Value



* "center"




#### Example


{% highlight js %}
 
 
$("#container").ejChart({
series :[{ points:[{ marker :{dataLabel :{horizontalTextAlignment : "far"}}}] }]                  
});
{% endhighlight %}




### series.points.marker.dataLabel.margin `object`
{:#members:series-points-marker-datalabel-margin}




Margin of the text to its background shape. The size of the background shape increases based on the margin applied to its text.






### series.points.marker.dataLabel.margin.bottom `number`
{:#members:series-points-marker-datalabel-margin-bottom}




Bottom margin of the text. 


#### Default Value



* 5




#### Example


{% highlight js %}
 
 
$("#container").ejChart({
series :[{ points:[{ marker :{dataLabel :{margin :{ bottom :10 }}}}] }]                 
});
{% endhighlight %}




### series.points.marker.dataLabel.margin.left `number`
{:#members:series-points-marker-datalabel-margin-left}




Left margin of the text. 


#### Default Value



 * 5




#### Example


{% highlight js %}
 
 
$("#container").ejChart({
series :[{ points: [{ marker :{dataLabel :{margin :{ left : 10}}}}] }]                 
});
{% endhighlight %}




### series.points.marker.dataLabel.margin.right `number`
{:#members:series-points-marker-datalabel-margin-right}




Right margin of the text. 


#### Default Value



* 5




#### Example


{% highlight js %}
 
 
$("#container").ejChart({
series :[{ points:[{ marker :{dataLabel :{margin :{ right :10 }}}}] }]                 
});
{% endhighlight %}




### series.points.marker.dataLabel.margin.top `number`
{:#members:series-points-marker-datalabel-margin-top}




Top margin of the text. 


#### Default Value



* 5




#### Example


{% highlight js %}
 
 
$("#container").ejChart({
series :[{ points:[{ marker :{dataLabel :{margin :{ top :10 } }}}] }]                 
});
{% endhighlight %}


Try it: [JS Playground Sample](http://jsplayground.syncfusion.com/rezz5cjo)



### series.points.marker.dataLabel.opacity `number`
{:#members:series-points-marker-datalabel-opacity}




Opacity of the data label. 


#### Default Value



* 1




#### Example


{% highlight js %}
 
 
$("#container").ejChart({
series :[{ points:[{ marker :{dataLabel :{opacity : 0.5}}}] }]                 
});
{% endhighlight %}




### series.points.marker.dataLabel.shape `enum`
{:#members:series-points-marker-datalabel-shape}


<ts ref="ej.datavisualization.Chart.Shape"/>

Background shape of the data label. 


#### Default Value



* No shape is rendered by default, so its value is ‘none’. See <a href="ejchart.html#members:commonseriesoptions-points-marker-datalabel-shape">Shape</a>


#### Example


{% highlight js %}
 
 
$("#container").ejChart({
series :[{ points:[{ marker :{dataLabel :{shape : "circle"}}}] }]                 
});
{% endhighlight %}




### series.points.marker.dataLabel.textPosition `enum`
{:#members:series-points-marker-datalabel-textposition}


<ts ref="ej.datavisualization.Chart.TextPosition"/>

Specifies the position of the data label. This property can be used only for the series such as column, bar, stacked column, stacked bar, 100% stacked column, 100% stacked bar, candle and OHLC. 


#### Default Value



* "top". See <a href="ejchart.html#members:commonseriesoptions-points-marker-datalabel-textposition">TextPosition</a>


#### Example


{% highlight js %}
 
 
$("#container").ejChart({
series :[{ points:[{ marker :{dataLabel :{textPosition : "bottom"}}}] }]                 
});
{% endhighlight %}




### series.points.marker.dataLabel.verticalTextAlignment `enum`
{:#members:series-points-marker-datalabel-verticaltextalignment}

<ts ref="ej.datavisualization.Chart.VerticalTextAlignment"/>


Vertical alignment of the data label. 


#### Default Value



* 'center'




#### Example


{% highlight js %}
 

$("#container").ejChart({
series :[{ points: [{ marker :{dataLabel :{verticalTextAlignment : "far"}}}] }]                  
});
{% endhighlight %}


Try it: [JS Playground Sample](http://jsplayground.syncfusion.com/k5e5rltz)


### series.points.marker.dataLabel.visible `boolean`
{:#members:series-points-marker-datalabel-visible}




Controls the visibility of the data labels. 


#### Default Value



* false




#### Example


{% highlight js %}
 

$("#container").ejChart({
series :[{ points: [{ marker :{dataLabel :{visible : true}}}] }]                  
});
 {% endhighlight %}


### series.points.marker.dataLabel.template `string`
{:#members:series-points-marker-datalabel-template}




Custom template to format the data label content. Use “point.x” and “point.y” as a placeholder text to display the corresponding data point’s x and y value.


#### Default Value



* ""




#### Example


{% highlight js %}
 

$("#container").ejChart({
series :[{ points:[{ marker :{dataLabel :{template : "item"}}}] }]                  
});
 {% endhighlight %}
 
 Try it: [JS Playground Sample](http://jsplayground.syncfusion.com/lzjtnka5)

 
 
 
### series.points.marker.dataLabel.offset `number`
{:#members:series-points-marker-datalabel-offset}




Moves the label vertically by specified offset.


#### Default Value



* 0




#### Example


{% highlight js %}
 

$("#container").ejChart({
series :[{ points:[{ marker :{dataLabel :{offset : 10}}}] }]                  
});
 {% endhighlight %}



### series.points.marker.fill `string`
{:#members:series-points-marker-fill}




Color of the marker shape. 


#### Default Value



* null




#### Example


{% highlight js %}
 
 
$("#container").ejChart({
series :[{ points:[{ marker : { fill : "green" } }] }]                  
});
{% endhighlight %}




### series.points.marker.imageUrl `string`
{:#members:series-points-marker-imageurl}




The URL for the Image that is to be displayed as marker. In order to display image as marker, set series.marker.shape as ‘image’.


#### Default Value



* ""




#### Example


{% highlight js %}
 
 
$("#container").ejChart({
series :[{ points:[{ marker :{ imageUrl: "../images/sample.png"}}] }]                  
});
{% endhighlight %}




### series.points.marker.opacity `number`
{:#members:series-points-marker-opacity}




Opacity of the marker. 


#### Default Value



 * 1




#### Example


{% highlight js %}
 
 
$("#container").ejChart({
series :[{ points:[{ marker :{ opacity : 0.5 }}] }]                  
});
{% endhighlight %}


Try it: [JS Playground Sample](http://jsplayground.syncfusion.com/fr1zj5v3)



### series.points.marker.shape `enum`
{:#members:series-points-marker-shape}

<ts ref="ej.datavisualization.Chart.Shape"/>


Specifies the shape of the marker.  


#### Default Value



* "circle". See <a href="ejchart.html#members:commonseriesoptions-points-marker-shape">Shape</a>


#### Example


{% highlight js %}
 
 
$("#container").ejChart({
series :[{ points:[{ marker :{ shape: "rectangle"}] }]                  
});
{% endhighlight %}


Try it: [JS Playground Sample](http://jsplayground.syncfusion.com/5cgrkynp)


### series.points.marker.size `object`
{:#members:series-points-marker-size}




Options for customizing the size of the marker shape.






### series.points.marker.size.height `number`
{:#members:series-points-marker-size-height}




Height of the marker. 


#### Default Value



* 6




#### Example


{% highlight js %}
 
 
$("#container").ejChart({
series :[{ points:[{ marker :{size :{height : 5}}}] }]                 
});
>{% endhighlight %}




### series.points.marker.size.width `number`
{:#members:series-points-marker-size-width}




Width of the marker. 


#### Default Value



* 6




#### Example


{% highlight js %}
 
 
$("#container").ejChart({
series :[{ points:[{ marker :{ size :{ width : 2 } } }] }]                  
});
{% endhighlight %}


Try it: [JS Playground Sample](http://jsplayground.syncfusion.com/hcnmls5c)


### series.points.marker.visible `boolean`
{:#members:series-points-marker-visible}




Controls the visibility of the marker shape. 


#### Default Value



* false




#### Example


{% highlight js %}
 
 
$("#container").ejChart({
series :[{ points:[{ marker :{ visible : true}}] }]                  
});
{% endhighlight %}




### series.points.open `number`
{:#members:series-points-open}




Open value of the point. This is applicable only for financial type series.


#### Default Value



* null




#### Example


{% highlight js %}
 
 
$("#container").ejChart({
series :[{ points:[{ open : 30 }] }]                  
});
{% endhighlight %}




### series.points.text `string` 
{:#members:series-points-text}




Datalabel text for the point.


#### Default Value



* null




#### Example


{% highlight js %}
 
 
$("#container").ejChart({
series :[{ points:[{ text : "20%" }] }]                  
});
{% endhighlight %}




### series.points.x `number`
{:#members:series-points-x}




X value of the point.


#### Default Value



* null




#### Example


{% highlight js %}
 
 
$("#container").ejChart({
series :[{ points:[{ x : 1 }] }]                  
});
{% endhighlight %}




### series.points.y `number`
{:#members:series-points-y}




Y value of the point.


#### Default Value



* null




#### Example


{% highlight js %}
 
 
$("#container").ejChart({
series :[{ points:[{ y : 20 }] }]                  
});
{% endhighlight %}




### series.pyramidMode `enum`
{:#members:series-pyramidmode}

<ts ref="ej.datavisualization.Chart.PyramidMode"/>


Specifies the mode of the pyramid series.


#### Default Value



* "linear"




#### Example


{% highlight js %}
 
 
$("#container").ejChart({
series : [{pyramidMode : "linear" }]                   
});
{% endhighlight %}


Try it: [JS Playground Sample](http://jsplayground.syncfusion.com/xlnaeyog)



### series.query `object`
{:#members:series-query}




Specifies ej.Query to select data from dataSource. This property is applicable only when the dataSource is ej.DataManager.


#### Default Value



* null




#### Example


{% highlight js %}
 
 
var query =  ej.Query().from("Orders").take(10);
$("#container").ejChart({
series : [{query: query }]                   
});
{% endhighlight %}



Try it: [JS Playground Sample](http://jsplayground.syncfusion.com/5ffbprmm)



### series.startAngle `number`
{:#members:series-startangle}




Start angle from where the pie/doughnut series renders. It starts from 0, by default.


#### Default Value



* null




#### Example


{% highlight js %}
 

$("#container").ejChart({
series : [{startAngle: 140 }]                   
});
 {% endhighlight %}



Try it: [JS Playground Sample](http://jsplayground.syncfusion.com/cw1zlin3)



### series.cornerRadius `object`
{:#members:series-cornerradius}




Options for customizing the corner radius. cornerRadius property also takes the numeric input and applies it for all the four corners of the column.


#### Example


{% highlight js %}
 
 
$("#container").ejChart({
series : [{
             cornerRadius: 10 
    }]                   
});
 {% endhighlight %} 



### series.cornerRadius.topLeft `number`
{:#members:series-cornerradius-topleft}




Specifies the radius for the top left corner.



#### Default Value



 * 0




#### Example


{% highlight js %}
 
 
$("#container").ejChart({
series : [{
             cornerRadius: {topLeft : 10 }
    }]                   
});
 {% endhighlight %} 


### series.cornerRadius.topRight `number`
{:#members:series-cornerradius-topright}




Specifies the radius for the top right corner.



#### Default Value



 * 0




#### Example


{% highlight js %}
 
 
$("#container").ejChart({
series : [{
             cornerRadius: {topRight : 10 }
    }]                   
});
 {% endhighlight %} 



### series.cornerRadius.bottomLeft `number`
{:#members:series-cornerradius-bottomleft}




Specifies the radius for the bottom left corner.



#### Default Value



 * 0




#### Example


{% highlight js %}
 
 
$("#container").ejChart({
series : [{
             cornerRadius: {bottomLeft : 10 }
    }]                   
});
 {% endhighlight %} 


### series.cornerRadius.bottomRight `number`
{:#members:series-cornerradius-bottomright}




Specifies the radius for the bottom right corner.



#### Default Value



 * 0




#### Example


{% highlight js %}
 
 
$("#container").ejChart({
series : [{
             cornerRadius: {bottomRight : 10 }
    }]                   
});
 {% endhighlight %} 



### series.tooltip `object`
{:#members:series-tooltip}




Options for customizing the tooltip of chart.






### series.tooltip.border `object`
{:#members:series-tooltip-border}




Options for customizing the border of the tooltip.



### series.tooltip.border.color `string`
{:#members:series-tooltip-border-color}




Border Color of the tooltip.


#### Default Value



 * null




#### Example


{% highlight js %}
 
 
$("#container").ejChart({
series : [{tooltip : {border : { color :"green"} }]                   
});
 {% endhighlight %}




### series.tooltip.border.width `number`
{:#members:series-tooltip-border-width}




Border Width of the tooltip.


#### Default Value



 * 1




#### Example


{% highlight js %}
 
 
$("#container").ejChart({
series : [{tooltip : {border : { width :2} }]                   
});
 {% endhighlight %}


### series.tooltip.rx `number`
{:#members:series-tooltip-rx}




Customize the corner radius of the tooltip rectangle.


#### Default Value



0




#### Example


{% highlight js %}
 
 
$("#container").ejChart({
series :[{
    tooltip :{ry: 10}
    }]                 
});
  {% endhighlight %}



Try it: [JS Playground Sample](http://jsplayground.syncfusion.com/y4bnt0gl)


### series.tooltip.ry `number`
{:#members:series-tooltip-ry}




Customize the corner radius of the tooltip rectangle.


#### Default Value



0




#### Example


{% highlight js %}
 
 
$("#container").ejChart({
series :[{
    tooltip :{ry: 10}
    }]                  
});
  {% endhighlight %}



Try it: [JS Playground Sample](http://jsplayground.syncfusion.com/y4bnt0gl)


### series.tooltip.duration `string`
{:#members:series-tooltip-duration}




Specifies the duration, the tooltip has to be displayed.


#### Default Value



* "500ms"




#### Example


{% highlight js %}
 
 
$("#container").ejChart({
series : [{tooltip : { duration: "300ms" }]                   
});
 {% endhighlight %}




### series.tooltip.enableAnimation `boolean`
{:#members:series-tooltip-enableanimation}




Enables/disables the animation of the tooltip when moving from one point to another.


#### Default Value



* true




#### Example


{% highlight js %}
 
 
$("#container").ejChart({
series : [{tooltip : { enableAnimation: false }]                   
});
 {% endhighlight %}




### series.tooltip.fill `string`
{:#members:series-tooltip-fill}




Background color of the tooltip.


#### Default Value



 * null




#### Example


{% highlight js %}
 
 
$("#container").ejChart({
series : [{tooltip : {fill : "green"} }]                   
});
{% endhighlight %}


Try it: [JS Playground Sample](http://jsplayground.syncfusion.com/xz1asbhm)



### series.tooltip.format `string`
{:#members:series-tooltip-format}




Format of the tooltip content.



#### Default Value



* "#point.x# : #point.y#"




#### Example


{% highlight js %}
 
 
$("#container").ejChart({
series : [{tooltip : {format : "#point.x# : #point.y#"} }]                   
});
 {% endhighlight %}


Try it: [JS Playground Sample](http://jsplayground.syncfusion.com/ykkxirn1)


### series.tooltip.opacity `number`
{:#members:series-tooltip-opacity}




Opacity of the tooltip.


#### Default Value



 * 0.95




#### Example


{% highlight js %}
 
 
$("#container").ejChart({
series : [{tooltip : { opacity: 0.5 }]                   
});
 {% endhighlight %}




### series.tooltip.template `string`
{:#members:series-tooltip-template}




Custom template to format the tooltip content. Use “point.x” and “point.y” as a placeholder text to display the corresponding data point’s x and y value.


#### Default Value



* null




#### Example


{% highlight js %}
 
 <div id="item" style="display: none;"> 
    <div>
       <div>#point.x#</div>
        <div>#point.y#</div>
       </div>       
 </div>


$("#container").ejChart({
series : [{ tooltip: { template : "item" }}]                  
});
 {% endhighlight %}



Try it: [JS Playground Sample](http://jsplayground.syncfusion.com/j0twqmow)



### series.tooltip.visible `boolean`
{:#members:series-tooltip-visible}




Controls the visibility of the tooltip.


#### Default Value



* false




#### Example


{% highlight js %}
 
 
$("#container").ejChart({
series : [{tooltip : {visible : true} }]                   
});
 {% endhighlight %}




### series.type `enum`
{:#members:series-type}


<ts ref="ej.datavisualization.Chart.Type"/>

Specifies the type of the series to render in chart.


#### Default Value



* "column". see <a href="ejchart.html#members:commonseriesoptions.type">Type</a>



#### Example


{% highlight js %}
 
 
$("#container").ejChart({
series : [{type : "column" }]                   
});
 {% endhighlight %}


Try it: [JS Playground Sample](http://jsplayground.syncfusion.com/xab3pr0x)


### series.visibility `string`
{:#members:series-visibility}




Controls the visibility of the series.



#### Default Value



 * "visible"




#### Example


{% highlight js %}
 

$("#container").ejChart({
series : [{visibility: "hidden" }]                   
});
{% endhighlight %}


Try it: [JS Playground Sample](http://jsplayground.syncfusion.com/mg5325qz)




### series.visibleOnLegend `string`
{:#members:series-visibleonlegend}




Enables or disables the visibility of legend item.



#### Default Value



 * "visible"




#### Example


{% highlight js %}
 

$("#container").ejChart({
series : [{visibleOnLegend: "hidden" }]                   
});
{% endhighlight %}


### series.xAxisName `string`
{:#members:series-xaxisname}




Specifies the name of the x-axis that has to be associated with this series. Add an axis instance with this name to axes collection.


#### Default Value



* null




#### Example


{% highlight js %}
 

$("#container").ejChart({
series : [{xAxisName: "xAxis" }]                   
});
{% endhighlight %}


Try it: [JS Playground Sample](http://jsplayground.syncfusion.com/hz4rz01v)


### series.xName `string`
{:#members:series-xname}




Name of the property in the datasource that contains x value for the series.


#### Default Value



 * null




#### Example


{% highlight js %}
 

$("#container").ejChart({
series : [{xName: "XValue" }]                   
});
 {% endhighlight %}


Try it: [JS Playground Sample](http://jsplayground.syncfusion.com/5ffbprmm)


### series.yAxisName `string`
{:#members:series-yaxisname}




Specifies the name of the y-axis that has to be associated with this series. Add an axis instance with this name to axes collection.


#### Default Value



* null




#### Example


{% highlight js %}
 

$("#container").ejChart({
series : [{yAxisName: "yAxis" }]                   
});
 {% endhighlight %}


Try it: [JS Playground Sample](http://jsplayground.syncfusion.com/xn2uktf2)



### series.yName `string`
{:#members:series-yname}




Name of the property in the datasource that contains y value for the series.


#### Default Value



 * null




#### Example


{% highlight js %}
 
 
$("#container").ejChart({
series : [{yName: "YValue" }]                   
});
{% endhighlight %}




### series.high `string`
{:#members:series-high}




Name of the property in the datasource that contains high value for the series.


#### Default Value



 * null




#### Example


{% highlight js %}
 
 
$("#container").ejChart({
series : [{high: "high" }]                   
});
{% endhighlight %}




### series.low `string`
{:#members:series-low}




Name of the property in the datasource that contains low value for the series.


#### Default Value



 * null




#### Example


{% highlight js %}
 
 
$("#container").ejChart({
series : [{low: "low" }]                   
});
{% endhighlight %}


Try it: [JS Playground Sample](http://jsplayground.syncfusion.com/pqshst44)



### series.open `string`
{:#members:series-open}




Name of the property in the datasource that contains open value for the series.


#### Default Value



 * null




#### Example


{% highlight js %}
 
 
$("#container").ejChart({
series : [{open: "oepn" }]                   
});
{% endhighlight %}



### series.close `string`
{:#members:series-close}


Name of the property in the datasource that contains close value for the series.


#### Default Value



 * null




#### Example


{% highlight js %}
 
 
$("#container").ejChart({
series : [{close: "close" }]                   
});
{% endhighlight %}


Try it: [JS Playground Sample](http://jsplayground.syncfusion.com/pqshst44)




### series.pointColorMappingName `string`
{:#members:series-pointcolormappingname}




Name of the property in the datasource that contains fill color for the series.


#### Default Value



* null




#### Example


{% highlight js %}
 
 
$("#container").ejChart({
   series : [{pointColorMappingName: "color" }]                   
});
 {% endhighlight %}
 
 
 
 ### series.zOrder `number`
{:#members:series-zOrder}




Z-order of the series.


#### Default Value



* 0




#### Example


{% highlight js %}
 
 
$("#container").ejChart({
series :[{zOrder : 1}]                  
});
 {% endhighlight %}
 


### series.size `string`
{:#members:series-size}




Name of the property in the datasource that contains the size value for the bubble series.


#### Default Value



* null




#### Example


{% highlight js %}
 
 
$("#container").ejChart({
series : [{size: "size" }]                   
});
{% endhighlight %}


Try it: [JS Playground Sample](http://jsplayground.syncfusion.com/xsmhbrfn)


### series.trendlines `array`
{:#members:series-trendlines}




Option to add trendlines to chart.




### series.trendlines.visibility `boolean`
{:#members:series-trendlines-visibility}




Show/hides the trendline.


#### Default Value



* ""




#### Example


{% highlight js %}
 
 
$("#container").ejChart({
series :[{trendlines:[{ visibility:'visible' }]}]                  
});
{% endhighlight %}





### series.trendlines.type `string`
{:#members:series-trendlines-type}




Specifies the type of trendline for the series.


#### Default Value



* "linear". See <a href="global.html#members:trendlinestype">TrendlinesType</a>




#### Example


{% highlight js %}
 
 
$("#container").ejChart({
series :[{trendlines:[{ type:'linear' }]}]                  
});
{% endhighlight %}



### series.trendlines.name `string`
{:#members:series-trendlines-name}




Name for the trendlines that is to be displayed in legend text.


#### Default Value



* "Trendline"



#### Example


{% highlight js %}
 
 
$("#container").ejChart({
series :[{trendlines:[{ name:'Trendline' }]}]                  
});
{% endhighlight %}




### series.trendlines.fill `string`
{:#members:series-trendlines-fill}




Fill color of the trendlines.


#### Default Value



* "#0000FF"



#### Example


{% highlight js %}
 
 
$("#container").ejChart({
series :[{trendlines:[{ fill:'#0000FF' }]}]                  
});
{% endhighlight %}




### series.trendlines.width `number`
{:#members:series-trendlines-width}




Width of the trendlines.


#### Default Value



* 1



#### Example


{% highlight js %}
 
 
$("#container").ejChart({
series :[{trendlines:[{ width:1 }]}]                  
});
{% endhighlight %}



### series.trendlines.opacity `number`
{:#members:series-trendlines-opacity}




Opacity of the trendline.


#### Default Value



* 1



#### Example


{% highlight js %}
 
 
$("#container").ejChart({
series :[{trendlines:[{ opacity:1 }]}]                  
});
{% endhighlight %}




### series.trendlines.dashArray `string`
{:#members:series-trendlines-dasharray}




Pattern of dashes and gaps used to stroke the trendline.


#### Default Value



* ""



#### Example


{% highlight js %}
 
 
$("#container").ejChart({
series :[{trendlines:[{ dashArray:"" }]}]                  
});
{% endhighlight %}



### series.trendlines.forwardForecast `number`
{:#members:series-trendlines-forwardforecast}




Future trends of the current series.


#### Default Value



* 0



#### Example


{% highlight js %}
 
 
$("#container").ejChart({
series :[{trendlines:[{ forwardForeCast:2 }]}]                  
});
{% endhighlight %}



### series.trendlines.backwardForecast `number`
{:#members:series-trendlines-backwardforecast}




Past trends of the current series.


#### Default Value



* 0



#### Example


{% highlight js %}
 
 
$("#container").ejChart({
series :[{trendlines:[{ backwardForeCast:2 }]}]                  
});
{% endhighlight %}

Try it: [JS Playground Sample](http://jsplayground.syncfusion.com/d3gntcp0)



### series.trendlines.polynomialOrder `number`
{:#members:series-trendlines-polynomialorder}




Specifies the order of polynomial trendlines.


#### Default Value



* 0



#### Example


{% highlight js %}
 
 
$("#container").ejChart({
series :[{trendlines:[{ polynomialOrder:2 }]}]             
});
{% endhighlight %}

Try it: [JS Playground Sample](http://jsplayground.syncfusion.com/gdpriupt)

### series.trendlines.period `number`
{:#members:series-trendlines-period}




Specifies the moving average starting period  value.


#### Default Value



* 2



#### Example


{% highlight js %}
 
 
$("#container").ejChart({
series :[{trendlines:[{ period: 3 }]}]             
});
{% endhighlight %}

Try it: [JS Playground Sample](http://jsplayground.syncfusion.com/gdpriupt)



### series.trendlines.tooltip `object`
{:#members:series-trendlines-tooltip}




Options for customizing the trendline tooltip


### series.trendlines.tooltip.border `object`
{:#members:series-trendlines-tooltip-border}




Options for customizing the border of the trendline tooltip.




### series.trendlines.tooltip.border.color `string`
{:#members:series-trendlines-tooltip-border-color}




Specify the Border color of the  trendline tooltip.


#### Default Value



* null




#### Example


{% highlight js %}
 
 
$("#container").ejChart({        
series :[{ trendlines:[{ tooltip :{border:{ color : "green" }} }]}]                  
});
 {% endhighlight %}




### series.trendlines.tooltip.border.width `number`
{:#members:series-trendlines-tooltip-border-width}




Border width of the trendline tooltip.


#### Default Value



* 1




#### Example


{% highlight js %}
 
 
$("#container").ejChart({
series :[{ trendlines:[{ tooltip :{border:{  width : 2 }} }]}]                   
});
  {% endhighlight %}



Try it: [JS Playground Sample](http://jsplayground.syncfusion.com/dmvqb51g)



### series.trendlines.tooltip.rx `number`
{:#members:series-trendlines-tooltip-rx}




Customize the corner radius of the trendline tooltip rectangle.


#### Default Value



0




#### Example


{% highlight js %}
 
 
$("#container").ejChart({
series :[{ trendlines:[{ tooltip :{rx: 10} }]}]                  
});
  {% endhighlight %}



Try it: [JS Playground Sample](http://jsplayground.syncfusion.com/y4bnt0gl)


### series.trendlines.tooltip.ry `number`
{:#members:series-trendlines-tooltip-ry}




Customize the corner radius of the trendline tooltip rectangle.


#### Default Value



0




#### Example


{% highlight js %}
 
 
$("#container").ejChart({
series :[{ trendlines:[{ tooltip :{ry: 10} }]}]                  
});
  {% endhighlight %}



Try it: [JS Playground Sample](http://jsplayground.syncfusion.com/y4bnt0gl)



### series.trendlines.tooltip.duration `string`
{:#members:series-trendlines-tooltip-duration}




Specifies the duration of the trendline tooltip to be displayed.


#### Default Value



* "500ms"




#### Example


{% highlight js %}
 
 
$("#container").ejChart({
series :[{ trendlines:[{ tooltip :{duration : "300ms"} }]}]                   
});
  {% endhighlight %}



### series.trendlines.tooltip.enableAnimation `boolean`
{:#members:series-trendlines-tooltip-enableanimation}




Enables/disables the animation of the trendline tooltip when moving from one point to other.


#### Default Value



* true




#### Example


{% highlight js %}
 
 
$("#container").ejChart({
series :[{ trendlines:[{ tooltip :{enableAnimation : false} }]}]                   
});
{% endhighlight %}



### series.trendlines.tooltip.fill `string`
{:#members:series-trendlines-tooltip-fill}




Background color of the trendline tooltip.


#### Default Value



* null




#### Example


{% highlight js %}
 
 
$("#container").ejChart({
series :[{ trendlines:[{ tooltip :{fill : "green"} }]}]                   
});
 {% endhighlight %}



### series.trendlines.tooltip.format `string`
{:#members:series-trendlines-tooltip-format}




Format of the trendline tooltip content.


#### Default Value



* "#point.x# : #point.y#"




#### Example


{% highlight js %}
 
 
$("#container").ejChart({
series :[{ trendlines:[{ tooltip :{format : "#point.x# : #point.y#%"} }]}]                  
});
 {% endhighlight %}



Try it: [JS Playground Sample](http://jsplayground.syncfusion.com/rzxmpi0c)



### series.trendlines.tooltip.opacity `number`
{:#members:series-trendlines-tooltip-opacity}





Opacity of the trendline tooltip.


#### Default Value



* 0.5




#### Example


{% highlight js %}
 
 
$("#container").ejChart({
series :[{ trendlines:[{ tooltip :{opacity : 0.5} }]}]                 
});
{% endhighlight %}



### series.trendlines.visibleOnLegend `string`
{:#members:series-trendlines-visibleonlegend}


Show/hides the trendline legend.


#### Default Value



* visible




#### Example


{% highlight js %}
 
 
$("#container").ejChart({
series :[{trendlines:[{ visibleOnLegend:'hidden' }]}]                  
});
{% endhighlight %}



### series.trendlines.intercept `number`
{:#members:series-trendlines-intercept}


Specifies the trendline intercept value


#### Default Value



* null




#### Example


{% highlight js %}
 
 
$("#container").ejChart({
series :[{ trendlines:[{ intercept : 10 }]}]                 
});
{% endhighlight %}



### series.highlightSettings `object`
{:#members:series-highlightsettings}




Options for customizing the appearance of the series or data point while highlighting.




### series.highlightSettings.enable `boolean`
{:#members:series-highlightsettings-enable}




Enables/disables the ability to highlight series or data point interactively.


#### Default Value



* false




#### Example


{% highlight js %}
 
 
$("#container").ejChart({
series :[{highlightSettings:{enable:true}}]                  
});
{% endhighlight %}



### series.highlightSettings.mode `enum`
{:#members:series-highlightsettings-mode}

<ts ref="ej.datavisualization.Chart.Mode"/>


Specifies whether series or data point has to be highlighted.


#### Default Value



* "series". See <a href="ejchart.html#members:commonseriesoptions-highlightsettings-mode">Mode</a>




#### Example


{% highlight js %}
 
 
$("#container").ejChart({
series :[{highlightSettings:{mode:"point"}}]                  
});
{% endhighlight %}



### series.highlightSettings.color `string`
{:#members:series-highlightsettings-color}




Color of the series/point on highlight.


#### Default Value



* ""

 

#### Example


{% highlight js %}
 
 
$("#container").ejChart({
series :[{highlightSettings:{color:"red"}}]                  
});
{% endhighlight %}



### series.highlightSettings.opacity `number`
{:#members:series-highlightsettings-opacity}




Opacity of the series/point on highlight.


#### Default Value



* 0.6

 

#### Example


{% highlight js %}
 
 
$("#container").ejChart({
series :[{highlightSettings:{opacity:1}}]                  
});
{% endhighlight %}



### series.highlightSettings.border `object`
{:#members:series-highlightsettings-border}



Options for customizing the border of series on highlight.



### series.highlightSettings.border.color `string`
{:#members:series-highlightsettings-border-color}



Border color of the series/point on highlight.


#### Default Value



* ""

 

#### Example


{% highlight js %}
 
 
$("#container").ejChart({
series :[{highlightSettings:{border:{color:"black"}}}]                  
});
{% endhighlight %}



### series.highlightSettings.border.width `string`
{:#members:series-highlightsettings-border-width}



Border width of the series/point on highlight.


#### Default Value



* 2

 

#### Example


{% highlight js %}
 
 
$("#container").ejChart({
series :[{highlightSettings:{border:{width:1}}}]                  
});
{% endhighlight %}


Try it: [JS Playground Sample](http://jsplayground.syncfusion.com/ormhp3rz)


### series.highlightSettings.pattern `string`
{:#members:series-highlightsettings-pattern}




Specifies the pattern for the series/point on highlight.

#### Default Value



* "none". See <a href="global.html#members:pattern">Pattern</a>

 

#### Example


{% highlight js %}
 
 
$("#container").ejChart({
series :[{highlightSettings:{pattern:"chessboard"}}]                  
});
{% endhighlight %}


Try it: [JS Playground Sample](http://jsplayground.syncfusion.com/gcdopi4d)



### series.highlightSettings.customPattern `string`
{:#members:series-highlightsettings-custompattern}




Custom pattern for the series on highlight.

#### Default Value



* ""

 

#### Example


{% highlight js %}
 
 
$("#container").ejChart({
series :[{highlightSettings:{customPattern:""}}]                  
});
{% endhighlight %}


Try it: [JS Playground Sample](http://jsplayground.syncfusion.com/zmumutbx)



### series.selectionSettings `object`
{:#members:series-selectionsettings}




Options for customizing the appearance of the series/data point on selection.



### series.selectionSettings.enable `boolean`
{:#members:series-selectionsettings-enable}




Enables/disables the ability to select a series/data point interactively.


#### Default Value



* false




#### Example


{% highlight js %}
 
 
$("#container").ejChart({
series :[{selectionSettings:{enable:true}}]                  
});
{% endhighlight %}



### series.selectionSettings.mode `enum`
{:#members:series-selectionsettings-mode}

<ts ref="ej.datavisualization.Chart.Mode"/>


Specifies whether series or data point has to be selected.


#### Default Value



* "series". See <a href="ejchart.html#members:commonseriesoptions-selectionSettings-mode">Mode</a>




#### Example


{% highlight js %}
 
 
$("#container").ejChart({
series :[{selectionSettings:{mode:"point"}}]                  
});
{% endhighlight %}

Try it: [JS Playground Sample](http://jsplayground.syncfusion.com/f0udmdts)


### series.selectionSettings.type `enum`
{:#members:series-selectionsettings-type}

<ts ref="ej.datavisualization.Chart.SelectionType"/>

Specifies the type of selection.


#### Default Value



* "single"

See. [Type](https://help.syncfusion.com/api/js/global.html#LabelPosition)
 

#### Example


{% highlight js %}
 
 
$("#container").ejChart({
     series: [{
      selectionSettings:{
              type : 'multiple'
             }
	  }]
  }); 

{% endhighlight %}



### series.selectionSettings.rangeType `enum`
{:#members:series-selectionsettings-rangetype}

<ts ref="ej.datavisualization.Chart.RangeType"/>

Specifies the drawn rectangle type.


<table class="props">
<thead>
<tr>
<th>Name</th>
<th>Type</th>
<th class="last">Description</th>
</tr>
</thead>
<tbody>
<tr>
<td class="name">
XY</td>
<td class="type">string</td>
<td class="description">It will be draw a range rectangle in both horizontal and vertically.</td>
</tr>
<tr>
<td class="name">
X</td>
<td class="type">string</td>
<td class="description">It will be draw a range rectangle in horizontally.</td>
<td class="name">
Y</td>
<td class="type">string</td>
<td class="description">It will be draw a range rectangle in vertically.</td>
</tr>
</tbody>
</table>


#### Default Value



* "xy"
 

#### Example


{% highlight js %}
 
 
$("#container").ejChart({
     series: [{
      selectionSettings:{
              rangeType : 'x'
             }
	  }]
  }); 

{% endhighlight %}


### series.selectionSettings.color `string`
{:#members:series-selectionsettings-color}




Color of the series/point on selection.


#### Default Value



* ""

 

#### Example


{% highlight js %}
 
 
$("#container").ejChart({
series :[{selectionSettings:{color:"red"}}]                  
});
{% endhighlight %}



### series.selectionSettings.opacity `number`
{:#members:series-selectionsettings-opacity}




Opacity of the series/point on selection.


#### Default Value



* 0.6

 

#### Example


{% highlight js %}
 
 
$("#container").ejChart({
series :[{selectionSettings:{opacity:1}}]                  
});
{% endhighlight %}


### series.selectionSettings.border `object`
{:#members:series-selectionsettings-border}



Options for customizing the border of series on selection.



### series.selectionSettings.border.color `string`
{:#members:series-selectionsettings-border-color}



Border color of the series/point on selection.


#### Default Value



* ""

 

#### Example


{% highlight js %}
 
 
$("#container").ejChart({
series :[{selectionSettings:{border:{color:"black"}}}]                  
});
{% endhighlight %}



### series.selectionSettings.border.width `string`
{:#members:series-selectionsettings-border-width}



Border width of the series/point on selection.


#### Default Value



* 2

 

#### Example


{% highlight js %}
 
 
$("#container").ejChart({
series :[{selectionSettings:{border:{width:1}}}]                  
});
{% endhighlight %}



### series.selectionSettings.pattern `string`
{:#members:series-selectionsettings-pattern}




Specifies the pattern for the series/point on selection.

#### Default Value



* "none". See <a href="global.html#members:pattern">Pattern</a>

 

#### Example


{% highlight js %}
 
 
$("#container").ejChart({
series :[{selectionSettings:{pattern:"chessboard"}}]                  
});
{% endhighlight %}


Try it: [JS Playground Sample](http://jsplayground.syncfusion.com/cuee3fgt)


### series.selectionSettings.customPattern `string`
{:#members:series-selectionsettings-custompattern}



Custom pattern for the series on selection.

#### Default Value



* ""

 

#### Example


{% highlight js %}
 
 
$("#container").ejChart({
series :[{selectionSettings:{customPattern:""}}]                  
});
{% endhighlight %}


Try it: [JS Playground Sample](http://jsplayground.syncfusion.com/wlovhaqi)




### sideBySideSeriesPlacement `boolean`
{:#members:sidebysideseriesplacement}




Controls whether data points has to be displayed side by side or along the depth of the axis. 


#### Default Value



* false




#### Example


{% highlight js %}
 
$("#container").ejChart({
    
        sideBySideSeriesPlacement : true
             
});

{% endhighlight %}


Try it: [JS Playground Sample](http://jsplayground.syncfusion.com/lhtjjczw)


### size `object`
{:#members:size}




Options to customize the Chart size.


Try it: [JS Playground Sample](http://jsplayground.syncfusion.com/wpvk5t3p)




### size.height `string`
{:#members:size-height}




Height of the Chart. Height can be specified in either pixel or percentage.


#### Default Value

* '450'




#### Example


{% highlight js %}
 
$("#container").ejChart({

   size :{height : '80%'}          

});

{% endhighlight %}




### size.width `string`
{:#members:size-width}




Width of the Chart. Width can be specified in either pixel or percentage.


#### Default Value

* '450'




#### Example


{% highlight js %}
 
$("#container").ejChart({

   size :{width : '80%'}          

});

{% endhighlight %}




### theme `enum`
{:#members:theme}

<ts name="ej.datavisualization.Chart.Theme"/>
Specifies the theme for Chart.

<table class="props">
<thead>
<tr>
<th>Name</th>
<th>Type</th> 
<th class="last">Description</th>
</tr>
</thead>
<tbody>
<tr>
<td class="name">
Azure</td>
<td class="type">string</td> 
<td class="description">The Chart will be displayed in azure theme</td>
</tr>
<tr>
<td class="name">
FlatLight</td>
<td class="type">string</td>
<td class="description">The Chart will be displayed in light flat theme</td>
</tr> 
<tr>
<td class="name">
FlatDark</td>
<td class="type">string</td>
<td class="description">The Chart will be displayed in dark flat theme</td>
</tr> 
<tr>
<td class="name">
Azuredark</td>
<td class="type">string</td>
<td class="description">The Chart will be displayed in dark azure theme</td>
</tr> 
<tr>
<td class="name">
Lime</td>
<td class="type">string</td>
<td class="description">The Chart will be displayed in lime theme</td>
</tr> 
<tr>
<td class="name">
LimeDark</td>
<td class="type">string</td>
<td class="description">The Chart will be displayed in dark lime theme</td>
</tr> 
<tr>
<td class="name">
Saffron</td>
<td class="type">string</td>
<td class="description">The Chart will be displayed in saffron theme</td>
</tr> 
<tr>
<td class="name">
SaffronDark</td>
<td class="type">string</td>
<td class="description">The Chart will be displayed in dark saffron theme</td>
</tr> 
<tr>
<td class="name">
GradientLight</td>  
<td class="type">string</td>
<td class="description">The Chart will be displayed in light gradient theme</td>
</tr> 
<tr>
<td class="name">
GradientDark</td>
<td class="type">string</td>
<td class="description">The Chart will be displayed in dark gradient theme</td>
</tr> 
</tbody>
</table>





#### Default Value

* "Flatlight". See <a href="ejchart.html#members:theme">Theme</a>




#### Example


{% highlight js %}
 
$("#container").ejChart({

   theme : "flatdark"            

});

{% endhighlight %}


Try it: [JS Playground Sample](http://jsplayground.syncfusion.com/jael2rfm)




### tilt `number`
{:#members:tilt}




Slope angle of 3D Chart. This property is applicable only when 3D view is enabled.


#### Default Value



* 0




#### Example


{% highlight js %}
 
$("#container").ejChart({

      tilt : 5
             
});

{% endhighlight %}


Try it: [JS Playground Sample](http://jsplayground.syncfusion.com/p0cd1lvx)




### title `object`
{:#members:title}




Options for customizing the title and subtitle of Chart.




### title.background `string`
{:#members:title-background}




Background color for the chart title.


#### Default Value

* "transparent"




#### Example


{% highlight js %}
 
$("#container").ejChart({

   title : { background : "red" }                     

});

{% endhighlight %}

Try it: [JS Playground Sample](http://jsplayground.syncfusion.com/vq3sp2j2)


### title.border `object`
{:#members:title-border}




Options to customize the border of the title.


Try it: [JS Playground Sample](http://jsplayground.syncfusion.com/vq3sp2j2)


### title.border.width `number`
{:#members:title-border-width}




Width of the title border.


#### Default Value

* 1




#### Example


{% highlight js %}
 
$("#container").ejChart({

       title:{ 
          border : { width:1}
      }  
                     

});

{% endhighlight %}


### title.border.color `string`
{:#members:title-border-color}




color of the title border.


#### Default Value

* "transparent"




#### Example


{% highlight js %}
 
$("#container").ejChart({

       title:{ 
          border : { color: "black"}
      }  
                     

});

{% endhighlight %}


### title.border.opacity `number`
{:#members:title-border-opacity}




opacity of the title border.


#### Default Value

* 0.8




#### Example


{% highlight js %}
 
$("#container").ejChart({

       title:{ 
          border : { opacity: 1 }
      }  
                     

});

{% endhighlight %}


### title.border.cornerRadius `number`
{:#members:title-border-cornerradius}




opacity of the title border.


#### Default Value

* 0.8




#### Example


{% highlight js %}
 
$("#container").ejChart({

       title:{ 
          border : { cornerRadius: 2 }
      }  
                     

});

{% endhighlight %}





### title.font `object`
{:#members:title-font}




Options for customizing the font of Chart title.


Try it: [JS Playground Sample](http://jsplayground.syncfusion.com/fhtgy2vx)




### title.font.fontFamily `string`
{:#members:title-font-fontfamily}




Font family for Chart title.


#### Default Value

* "Segoe UI"




#### Example


{% highlight js %}
 
$("#container").ejChart({

   title : { font : { fontFamily : "Algerian" } }                     

});

{% endhighlight %}




### title.font.fontStyle `enum`
{:#members:title-font-fontstyle}

<ts ref="ej.datavisualization.Chart.FontStyle"/>


Font style for Chart title.


#### Default Value

* "Normal". See <a href="ejchart.html#members:title-font-fontstyle">FontStyle</a>




#### Example


{% highlight js %}
 
$("#container").ejChart({

   title : { font : { fontStyle : "italic" } }                     

});

{% endhighlight %}




### title.font.fontWeight `enum`
{:#members:title-font-fontweight}


<ts ref="ej.datavisualization.Chart.FontWeight"/>

Font weight for Chart title.


#### Default Value

* "Regular". See <a href="ejchart.html#members:title-font-fontweight">FontWeight</a>




#### Example


{% highlight js %}
 
$("#container").ejChart({

   title : { font : { fontWeight : "lighter" } }                     

});

{% endhighlight %}




### title.font.opacity `number`
{:#members:title-font-opacity}




Opacity of the Chart title.


#### Default Value

* 0.5




#### Example


{% highlight js %}
 
$("#container").ejChart({

   title : { font : { opacity : 0.8 } }                     

});

{% endhighlight %}




### title.font.size `string`
{:#members:title-font-size}




Font size for Chart title.


#### Default Value

* "20px"




#### Example


{% highlight js %}
 
$("#container").ejChart({

   title : { font : { size : "22px" } }                     

});

{% endhighlight %}



### title.visible `boolean`
{:#members:title-visible}




Controls the visibility of the Chart title


#### Default Value

* true




#### Example


{% highlight js %}
 
$("#container").ejChart({

   title : { visible : false }                     

});

{% endhighlight %}


### title.enableTrim `boolean`
{:#members:title-enableTrim}




Specifies whether to trim the Chart Title when the width of the title exceeds the maximumWidth.


#### Default Value

* false




#### Example


{% highlight js %}
 
$("#container").ejChart({

   title : { enableTrim : true }                     

});

{% endhighlight %}



### title.maximumWidth `string`
{:#members:title-maximumwidth}


Maximum width of the title, when the title exceeds this width, the title gets trimmed, when enableTrim is true. 


#### Default Value

* auto




#### Example


{% highlight js %}
 
$("#container").ejChart({

   title : { maximumWidth : 150 }                     

});

{% endhighlight %}



### title.textOverflow `enum`
{:#members:title-textoverflow}

<ts ref="ej.datavisualization.Chart.TextOverflow"/>

Specifies the action taken when the Chart width is more than the titleWidth. 


#### Default Value

* trim.


#### Example


{% highlight js %}
 
$("#container").ejChart({

   title : { textOverflow : "trim" }                     

});

{% endhighlight %}


### title.subTitle `object`
{:#members:title-subtitle}




Options to customize the sub title of Chart.




### title.subTitle.font `object`
{:#members:title-subtitle-font}




Options for customizing the font of sub title.


Try it: [JS Playground Sample](http://jsplayground.syncfusion.com/vq3sp2j2)




### title.subTitle.font.fontFamily `string`
{:#members:title-subtitle-font-fontfamily}




Font family of sub title.


#### Default Value

* "Segoe UI"




#### Example


{% highlight js %}
 
$("#container").ejChart({

   title: {subTitle : {font :{ fontFamily : "Algerian" } } }                      

});

{% endhighlight %}




### title.subTitle.font.fontStyle `enum`
{:#members:title-subtitle-font-fontstyle}

<ts ref="ej.datavisualization.Chart.FontStyle"/>


Font style for sub title.


#### Default Value

* "Normal". See <a href="ejchart.html#members:title-subtitle-font-fontstyle">FontStyle</a>




#### Example


{% highlight js %}
 
$("#container").ejChart({

   title: { subTitle : {font :{ fontStyle : "Normal" } } }                     

});

{% endhighlight %}




### title.subTitle.font.fontWeight `enum` 
{:#members:title-subtitle-font-fontweight}

<ts ref="ej.datavisualization.Chart.FontWeight"/>


Font weight for sub title.


#### Default Value

* "Regular". See <a href="ejchart.html#members:title-subtitle-font-fontweight">FontWeight</a>




#### Example


{% highlight js %}
 
$("#container").ejChart({

   title: { subTitle : {font :{ fontWeight : "regular" } } }                     

});

{% endhighlight %}




### title.subTitle.font.opacity `number`
{:#members:title-subtitle-font-opacity}




Opacity of the sub title.


#### Default Value

* 1




#### Example


{% highlight js %}
 
$("#container").ejChart({

   title: { subTitle : {font :{ opacity : 0.5 } } }                     

});

{% endhighlight %}




### title.subTitle.font.size `string`
{:#members:title-subtitle-font-size}




Font size for sub title.


#### Default Value

* "12px"




#### Example


{% highlight js %}
 
$("#container").ejChart({

   title: { subTitle : {font :{ size : "14px" } } }                     

});

{% endhighlight %}



### title.subTitle.background `string`
{:#members:title-subtitle-background}




Background color for the chart subtitle.


#### Default Value

* "transparent"




#### Example


{% highlight js %}
 
$("#container").ejChart({

   title : {  subTitle:{ background : "red" } }                     

});

{% endhighlight %}

Try it: [JS Playground Sample](http://jsplayground.syncfusion.com/vq3sp2j2)



### title.subTitle.border `object`
{:#members:title-subtitle-border}




Options to customize the border of the title.


Try it: [JS Playground Sample](http://jsplayground.syncfusion.com/vq3sp2j2)


### title.subTitle.border.width `number`
{:#members:title-subtitle-border-width}




Width of the subtitle border.


#### Default Value

* 1




#### Example


{% highlight js %}
 
$("#container").ejChart({

       title:{ 
         subTitle:{ border : { width:1} }
      }  
                     

});

{% endhighlight %}


### title.subTitle.border.color `string`
{:#members:title-subtitle-border-color}




color of the subtitle border.


#### Default Value

* "transparent"




#### Example


{% highlight js %}
 
$("#container").ejChart({

       title:{ 
         subTitle:{ border : { color: "black"}}
      }  
                     

});

{% endhighlight %}


### title.subTitle.border.opacity `number`
{:#members:title-subtitle-border-opacity}




opacity of the subtitle border.


#### Default Value

* 0.8




#### Example


{% highlight js %}
 
$("#container").ejChart({

       title:{ 
          subTitle:{ border : { opacity: 1 } }
      }  
                     

});

{% endhighlight %}


### title.subTitle.border.cornerRadius `number`
{:#members:title-subtitle-border-cornerradius}




opacity of the subtitle border.


#### Default Value

* 0.8




#### Example


{% highlight js %}
 
$("#container").ejChart({

       title:{ 
         subTitle:{  border : { cornerRadius: 2 } }
      }  
                     

});

{% endhighlight %}

### title.subTitle.text `string`
{:#members:title-subtitle-text}




Text to be displayed in sub title.


#### Default Value

* ""




#### Example


{% highlight js %}
 
$("#container").ejChart({

   title: { subTitle: { text : "Performance chart" } }                      

});

{% endhighlight %}


Try it: [JS Playground Sample](http://jsplayground.syncfusion.com/e3thfz5p)




### title.subTitle.textAlignment `enum`
{:#members:title-subtitle-textalignment}

<ts ref="ej.datavisualization.Chart.Alignment"/>


Alignment of sub title text.


#### Default Value

* "far". See <a href="ejchart.html#members:title-subtitle-textalignment">TextAlignment</a>




#### Example


{% highlight js %}
 
$("#container").ejChart({

   title: { subTitle: { textAlignment : "near" } }                      

});

{% endhighlight %}


Try it: [JS Playground Sample](http://jsplayground.syncfusion.com/yh1hzrly)


### title.subTitle.visible `boolean`
{:#members:title-subtitle-visible}




Controls the visibility of the Chart SubTitle


#### Default Value

* true




#### Example


{% highlight js %}
 
$("#container").ejChart({

   title :{ subTitle: { visible : false }  }                   

});

{% endhighlight %}


### title.subTitle.enableTrim `boolean`
{:#members:title-subtitle-enableTrim}




Specifies whether to trim the Chart SubTitle when the width of the Subtitle exceeds the maximumWidth.


#### Default Value

* false




#### Example


{% highlight js %}
 
$("#container").ejChart({

   title : { subTitle:{ enableTrim : true } }                    

});

{% endhighlight %}



### title.subTitle.maximumWidth `string`
{:#members:title-subtitle-maximumwidth}


Maximum width of the Subtitle, when the Subtitle exceeds this width, the Subtitle gets trimmed, when enableTrim is true. 


#### Default Value

* auto




#### Example


{% highlight js %}
 
$("#container").ejChart({

   title : { subTitle: { maximumWidth : 150 }  }                   

});

{% endhighlight %}



### title.subTitle.textOverflow `enum`
{:#members:title-subtitle-textoverflow}

<ts ref="ej.datavisualization.Chart.TextOverflow"/>

Specifies the action taken when the Chart width is more than the SubTitleWidth. 


#### Default Value

* trim.


#### Example


{% highlight js %}
 
$("#container").ejChart({

   title : { subTitle: { textOverflow : "trim" }  }                   

});

{% endhighlight %}



### title.text `string`
{:#members:title-text}




Text to be displayed in Chart title.


#### Default Value

* ""




#### Example


{% highlight js %}
 
$("#container").ejChart({

   title : { text : "Power Production"}                     

});

{% endhighlight %}


Try it: [JS Playground Sample](http://jsplayground.syncfusion.com/rk0x1e5u)




### title.textAlignment `enum`
{:#members:title-textalignment}

<ts ref="ej.datavisualization.Chart.Alignment"/>


Alignment of the title text.


#### Default Value

* "Center". See <a href="ejchart.html#members:title-textalignment">TextAlignment</a>




#### Example


{% highlight js %}
 
$("#container").ejChart({

   title : { textAlignment : "near"}                     

});

{% endhighlight %}


Try it: [JS Playground Sample](http://jsplayground.syncfusion.com/p1vsex5m)




### wallSize `number`
{:#members:wallsize}




Width of the wall used in 3D Chart. Wall is present only in Cartesian type 3D series and not in 3D pie or Doughnut series. This property is applicable only when 3D view is enabled.


#### Default Value



* 2




#### Example


{% highlight js %}
 
$("#container").ejChart({

      wallSize : 5
             
});

{% endhighlight %}

Try it: [JS Playground Sample](http://jsplayground.syncfusion.com/q4nv04rw)




### zooming `object`
{:#members:zooming}




Options for enabling zooming feature of chart.






### zooming.enable `boolean`
{:#members:zooming-enable}




Enables or disables zooming.


#### Default Value

* false




#### Example


{% highlight js %}
 
$("#container").ejChart({

   zooming :{enable :true}          

});

{% endhighlight %}




### zooming.enablePinching `boolean`
{:#members:zooming-enablePinching}




Enables or disables pinch zooming.


#### Default Value

* true




#### Example


{% highlight js %}
 
$("#container").ejChart({

   zooming :{enablePinching :true}          

});

{% endhighlight %}




### zooming.enableDeferredZoom `boolean`
{:#members:zooming-enabledeferredzoom}




Enable or disables the differed zooming. When it is enabled, chart is updated only on mouse up action while zooming and panning.


#### Default Value

* false




#### Example


{% highlight js %}
 
$("#container").ejChart({

   zooming:{enableDeferredZoom : true}            

});

{% endhighlight %}




### zooming.enableMouseWheel `boolean`
{:#members:zooming-enablemousewheel}




Enables/disables the ability to zoom the chart on moving the mouse wheel.


#### Default Value

* false




#### Example


{% highlight js %}
 
$("#container").ejChart({

   zooming:{enableMouseWheel : true}            

});

{% endhighlight %}


Try it: [JS Playground Sample](http://jsplayground.syncfusion.com/0gkvnyi3)




### zooming.type `string`
{:#members:zooming-type}




Specifies whether to allow zooming the chart vertically or horizontally or in both ways.


#### Default Value

* 'x,y'




#### Example


{% highlight js %}
 
$("#container").ejChart({

   zooming :{type : "y"}            

});

{% endhighlight %}


Try it: [JS Playground Sample](http://jsplayground.syncfusion.com/hqmmhpgk)



### zooming.enableScrollbar `boolean`
{:#members:zooming-enablescrollbar}




Toggles the visibility of the scrollbar, which will be displayed while zooming.


#### Default Value

* false




#### Example


{% highlight js %}
 
$("#container").ejChart({

   zooming :{ enableScrollbar : true }            

});

{% endhighlight %}



### zooming.toolbarItems `array`
{:#members:zooming-toolbaritems}



To display user specified buttons in zooming toolbar.


#### Default Value

* ["zoomIn", "zoomOut", "zoom", "pan", "reset"]




#### Example


{% highlight js %}
 
$("#container").ejChart({

  zooming : { toolbarItems: [“zoomin”] }        

});

{% endhighlight %}


Try it: [JS Playground Sample](http://jsplayground.syncfusion.com/hqmmhpgk)


## Methods




### animate(options)
{:#methods:animate}


Animates the series and/or indicators in Chart. When parameter is not passed to this method, then all the series and indicators present in Chart are animated.

Following are the parameters that you can pass to this method.


#### Returns: void


<table class="params">
<thead>
<tr>
<th>Parameters</th>
<th>Type</th>
<th class="last">Description</th>
</tr>
</thead>
<tbody>
<tr>
<td class="name">options</td>
<td class="type"><span class="param-type">object</span></td>
<td class="description last">If an array collection is passed as parameter, series and indicator objects passed in array collection are animated.
<br/><br/>
Example

{% highlight js %}
var chartObj  = $("#container").data("ejChart");
//animating series array
chartObj.animate(chartObj.model.series);
{% endhighlight %}

<br/>
If a series or indicator object is passed to this method, then the specific series or indicator is animated.
<br/><br/>
Example,

{% highlight js %}
var chartObj  = $("#container").data("ejChart");
//animating a specific indicator
chartObj.animate(chartObj.model.indicators[0]);
{% endhighlight %}
</td>
</tr>
</tbody>
</table>


### print()
{:#methods:print}

Prints the rendered chart.


#### Returns: void


#### Example


{% highlight js %}
// Print Chart
var chartObj = $("#container").data("ejChart");
chartObj.print();
{% endhighlight %}

If you wish to print multiple charts on a same page, then you need to pass the ID of those elements as arguments to the print method.

<div id="container1"></div> 
<div id="container2"></div> 

{% highlight js %}
// Print Chart
var chartObj = $("#container1").data("ejChart");
chartObj.print("container1","container2");
{% endhighlight %}


### export(type, URL, exportMultipleChart)
{:#methods:export}



Exports chart as an image or to an excel file. Chart can be exported as an image only when exportCanvasRendering option is set to true.

Following are the parameters that you can pass to this method,



#### Returns: object



<table class="params">
<thead>
<tr>
<th>Parameters</th>
<th>Type</th>
<th class="last">Description</th>
</tr>
</thead>
<tbody>
<tr>
<td class="name">type</td>
<td class="type"><span class="param-type">string</span></td>
<td class="description last">Type of the export operation to be performed. Following are the two export types that are supported now,
<br/>
1. 'image'
2. 'excel'
<br/><br./>
Example

{% highlight js %}
var chartObj  = $("#container").data("ejChart");
chartObj.export(‘image’);
{% endhighlight %}
</td>
</tr>
<tr>
<td class="name">URL</td>
<td class="type"><span class="param-type">string</span></td>
<td class="description last">
URL of the service, where the chart will be exported to excel.
<br/><br/>
Example,

{% highlight js %}
var chartObj  = $("#container").data("ejChart");
chartObj.export("excel", 'http://js.syncfusion.com/ExportingServices/api/JSChartExport/ExcelExport')
{% endhighlight %}
</td>
</tr>
<tr>
<td class="name">
exportMultipleChart</td>
<td class="type"><span class="param-type">boolean</span></td>
<td class="description last">
When this parameter is true, all the chart objects initialized to the same document are exported to a single excel file. This is an optional parameter. By default, it is false.
<br/><br/>
Example,

{% highlight js %}
var chartObj  = $("#container").data("ejChart");
chartObj.export("excel", 'http://js.syncfusion.com/ExportingServices/api/JSChartExport/ExcelExport', true)
{% endhighlight %}
</td>
</tr>
</tbody>
</table>




### redraw()
{:#methods:redraw}




Redraws the entire chart. You can call this method whenever you update, add or remove points from the data source or whenever you want to refresh the UI.


#### Returns: void


#### Example


{% highlight js %}
// Redraw Chart
var chartObj = $("#container").data("ejChart");
chartObj.redraw();
{% endhighlight %}


{% highlight js %}
 
$("#container").ejChart("redraw");      
{% endhighlight %}



## Events




### animationComplete
{:#events:animationcomplete}




Fires after the series animation is completed. This event will be triggered for each series when animation is enabled.

Example:
{:.example}


{% highlight js %}

//animationComplete event for chart

$("#container").ejChart({

     animationComplete: function (argument) {
     //Do something
 }
});


{% endhighlight %}


<table class="params">
<thead>
<tr>
<th>Name</th>
<th>Type</th>
<th class="last">Description</th>
</tr>
</thead>
<tbody>
<tr>
<td class="name">{% highlight js %}
data{% endhighlight %}</td>
<td class="type"><span class="param-type">Object</span></td>
<td class="description last"><ul> <li>series - Instance of the series that completed has animation.</li></ul></td>
</tr>
<tr>
<td class="name">{% highlight js %}
cancel{% endhighlight %}</td>
<td class="type"><span class="param-type">boolean</span></td>
<td class="description last">Set this option to true to cancel the event</td>
</tr>
<tr>
<td class="name">{% highlight js %}
model{% endhighlight %}</td>
<td class="type"><span class="param-type">object</span></td>
<td class="description last">Instance of the chart model object</td>
</tr>
<tr>
<td class="name">{% highlight js %}
type{% endhighlight %}</td>
<td class="type"><span class="param-type">string</span></td>
<td class="description last">Name of the event</td>
</tr>
</tbody>
</table>


### axesLabelRendering
{:#events:axeslabelrendering}




Fires before rendering the labels. This event is fired for each label in axis. You can use this event to add custom text to axis labels.

#### Example


{% highlight js %}
 
//axesLabelRendering event for chart

$("#container").ejChart({

    axesLabelRendering: function (args) {
            //Do something
    }
   
});

{% endhighlight %}


<table class="params">
<thead>
<tr>
<th>Name</th>
<th>Type</th>
<th class="last">Description</th>
</tr>
</thead>
<tbody>
<tr>
<td class="name">{% highlight js %}
data{% endhighlight %}</td>
<td class="type"><span class="param-type">Object</span></td>
<td class="description last"><ul><li>axis - Instance of the corresponding axis.
    </li>
    <li>label - Arguments of axis label value and text.</li>
                             </ul></td>
</tr>
<tr>
<td class="name">{% highlight js %}
cancel{% endhighlight %}</td>
<td class="type"><span class="param-type">boolean</span></td>
<td class="description last">Set this option to true to cancel the event.</td>
</tr>
<tr>
<td class="name">{% highlight js %}
model{% endhighlight %}</td>
<td class="type"><span class="param-type">object</span></td>
<td class="description last">Instance of the chart model object.</td>
</tr>
<tr>
<td class="name">{% highlight js %}
type{% endhighlight %}</td>
<td class="type"><span class="param-type">string</span></td>
<td class="description last">Name of the event</td>
</tr>
</tbody>
</table>



### axesLabelsInitialize
{:#events:axeslabelsinitialize}




Fires during the initialization of axis labels.


#### Example


{% highlight js %}
 
//axesLabelsInitialize event for chart

$("#container").ejChart({

    axesLabelsInitialize: function (args) {
            //Do something
    }
    
});

{% endhighlight %}


<table class="params">
<thead>
<tr>
<th>Name</th>
<th>Type</th>
<th class="last">Description</th>
</tr>
</thead>
<tbody>
<tr>
<td class="name">{% highlight js %}
data{% endhighlight %}</td>
<td class="type"><span class="param-type">Object</span></td>
<td class="description last"> <b>dataAxes</b> - Collection of axes in Chart</td>
</tr>
<tr>
<td class="name">{% highlight js %}
cancel{% endhighlight %}</td>
<td class="type"><span class="param-type">boolean</span></td>
<td class="description last">Set this option to true to cancel the event.</td>
</tr>
<tr>
<td class="name">{% highlight js %}
model{% endhighlight %}</td>
<td class="type"><span class="param-type">object</span></td>
<td class="description last">Instance of the chart model object.</td>
</tr>
<tr>
<td class="name">{% highlight js %}
type{% endhighlight %}</td>
<td class="type"><span class="param-type">string</span></td>
<td class="description last">Name of the event</td>
</tr>
</tbody>
</table>


### axesRangeCalculate
{:#events:axesrangecalculate}




Fires during axes range calculation. This event is fired for each axis present in Chart. You can use this event to customize axis range as required.

#### Example


{% highlight js %}
 
//axesRangeCalculate event for chart

$("#container").ejChart({

      axesRangeCalculate: function (args) {
              //Do something
      }
      
});

{% endhighlight %}

<table class="params">
<thead>
<tr>
<th>Name</th>
<th>Type</th>
<th class="last">Description</th>
</tr>
</thead>
<tbody>
<tr>
<td class="name">{% highlight js %}
data{% endhighlight %}</td>
<td class="type"><span class="param-type">object</span></td>
<td class="description last"><ul><li>delta - Difference between minimum and maximum value of axis range.</li>
    <li>interval - Interval value of axis range. Grid lines, tick lines and axis labels are drawn based on this interval value.</li>
    <li>max - Maximum value of axis range.</li>
    <li>min - Minimum value of axis range.</li>    
                             </ul></td>
</tr>
<tr>
<td class="name">{% highlight js %}
cancel{% endhighlight %}</td>
<td class="type"><span class="param-type">boolean</span></td>
<td class="description last">Set this option to true to cancel the event.</td>
</tr>
<tr>
<td class="name">{% highlight js %}
model{% endhighlight %}</td>
<td class="type"><span class="param-type">object</span></td>
<td class="description last">Instance of the chart model object.</td>
</tr>
<tr>
<td class="name">{% highlight js %}
type{% endhighlight %}</td>
<td class="type"><span class="param-type">string</span></td>
<td class="description last">Name of the event</td>
</tr>
</tbody>
</table>


### axesTitleRendering
{:#events:axestitlerendering}




Fires before rendering the axis title. This event is triggered for each axis with title. You can use this event to add custom text to axis title.


#### Example


{% highlight js %}
 
//axesTitleRendering event for chart

$("#container").ejChart({

     axesTitleRendering: function (args) {
             //Do something
     }
     
});

{% endhighlight %}

<table class="params">
<thead>
<tr>
<th>Name</th>
<th>Type</th>
<th class="last">Description</th>
</tr>
</thead>
<tbody>
<tr>
<td class="name">{% highlight js %}
data{% endhighlight %}</td>
<td class="type"><span class="param-type">Object</span></td>
<td class="description last"><ul><li>
    axes - Instance of the axis whose title is being rendered</li>
    <li>locationX - X-coordinate of title location</li>
    <li>locationY - Y-coordinate of title location</li>
    <li>title - Axis title text. You can add custom text to the title.</li>
</ul></td>
</tr>
<tr>
<td class="name">{% highlight js %}
cancel{% endhighlight %}</td>
<td class="type"><span class="param-type">boolean</span></td>
<td class="description last">Set this option to true to cancel the event.</td>
</tr>
<tr>
<td class="name">{% highlight js %}
model{% endhighlight %}</td>
<td class="type"><span class="param-type">object</span></td>
<td class="description last">Instance of the chart model object.</td>
</tr>
<tr>
<td class="name">{% highlight js %}
type{% endhighlight %}</td>
<td class="type"><span class="param-type">string</span></td>
<td class="description last">Name of the event</td>
</tr>
</tbody>
</table>


### chartAreaBoundsCalculate
{:#events:chartareaboundscalculate}




Fires during the calculation of chart area bounds. You can use this event to customize the bounds of chart area.


#### Example


{% highlight js %}
 
//chartAreaBoundsCalculate event for chart

$("#container").ejChart({

    chartAreaBoundsCalculate: function (args) {
            //Do something
    }
    
}); 

{% endhighlight %}


<table class="params">
<thead>
<tr>
<th>Name</th>
<th>Type</th>
<th class="last">Description</th>
</tr>
</thead>
<tbody>
<tr>
<td class="name">{% highlight js %}
data{% endhighlight %}</td>
<td class="type"><span class="param-type">object</span></td>
<td class="description last"><ul><li>areaBoundsHeight - Height of the chart area.</li>
    <li>areaBoundsWidth - Width of the chart area.</li>
    <li>areaBoundsX - X-coordinate of the chart area.</li>
    <li>areaBoundsY - Y-coordinate of the chart area.</li>
</ul></td>
</tr>
<tr>
<td class="name">{% highlight js %}
cancel{% endhighlight %}</td>
<td class="type"><span class="param-type">boolean</span></td>
<td class="description last">Set this option to true to cancel the event.</td>
</tr>
<tr>
<td class="name">{% highlight js %}
model{% endhighlight %}</td>
<td class="type"><span class="param-type">object</span></td>
<td class="description last">Instance of the chart model object.</td>
</tr>
<tr>
<td class="name">{% highlight js %}
type{% endhighlight %}</td>
<td class="type"><span class="param-type">string</span></td>
<td class="description last">Name of the event</td>
</tr>
</tbody>
</table>


### create
{:#events:create}




Fires after chart is created.



#### Example


{% highlight js %}
 
//Create event for chart

$("#container").ejChart({

     create: function (args) {
             //Do something
     }
     
});

{% endhighlight %}

<table class="params">
<thead>
<tr>
<th>Name</th>
<th>Type</th>
<th class="last">Description</th>
</tr>
</thead>
<tbody>
<tr>
<td class="name">{% highlight js %}
cancel{% endhighlight %}</td>
<td class="type"><span class="param-type">boolean</span></td>
<td class="description last">Set this option to true to cancel the event.</td>
</tr>
<tr>
<td class="name">{% highlight js %}
model{% endhighlight %}</td>
<td class="type"><span class="param-type">object</span></td>
<td class="description last">Instance of the chart model object.</td>
</tr>
<tr>
<td class="name">{% highlight js %}
type{% endhighlight %}</td>
<td class="type"><span class="param-type">string</span></td>
<td class="description last">Name of the event</td>
</tr>
</tbody>
</table>




### destroy
{:#events:destroy}




Fires when chart is destroyed completely.



#### Example


{% highlight js %}
 
//Destroy event for chart

$("#container").ejChart({

     destroy: function (args) {
             //Do something
     }
     
});

{% endhighlight %}

<table class="params">
<thead>
<tr>
<th>Name</th>
<th>Type</th>
<th class="last">Description</th>
</tr>
</thead>
<tbody>
<tr>
<td class="name">{% highlight js %}
cancel{% endhighlight %}</td>
<td class="type"><span class="param-type">boolean</span></td>
<td class="description last">Set this option to true to cancel the event.</td>
</tr>
<tr>
<td class="name">{% highlight js %}
model{% endhighlight %}</td>
<td class="type"><span class="param-type">object</span></td>
<td class="description last">Instance of the chart model object.</td>
</tr>
<tr>
<td class="name">{% highlight js %}
type{% endhighlight %}</td>
<td class="type"><span class="param-type">string</span></td>
<td class="description last">Name of the event</td>
</tr>
</tbody>
</table>




### displayTextRendering
{:#events:displaytextrendering}




Fires before rendering the data labels. This event is triggered for each data label in the series. You can use this event to add custom text in data labels.


#### Example


{% highlight js %}
 
//displayTextRendering event for chart

$("#container").ejChart({

    displayTextRendering: function (args) {
             //Do something
    }
	
});

{% endhighlight %}
 	

<table class="params">
<thead>
<tr>
<th>Name</th>
<th>Type</th>
<th class="last">Description</th>
</tr>
</thead>
<tbody>
<tr>
<td class="name">{% highlight js %}
data{% endhighlight %}</td>
<td class="type"><span class="param-type">object</span></td>
<td class="description last"><ul><li>text - Text displayed in data label. You can add custom text to the data label</li>
    <li>locationX - X-coordinate of data label location</li>
    <li>locationY - Y-coordinate of data label location</li>
    <li>seriesIndex - Index of the series in series Collection whose data label is being rendered</li>
    <li>pointIndex - Index of the point in series whose data label is being rendered</li>
</ul></td>
</tr>
<tr>
<td class="name">{% highlight js %}
cancel{% endhighlight %}</td>
<td class="type"><span class="param-type">boolean</span></td>
<td class="description last">Set this option to true to cancel the event.</td>
</tr>
<tr>
<td class="name">{% highlight js %}
model{% endhighlight %}</td>
<td class="type"><span class="param-type">object</span></td>
<td class="description last">Instance of the chart model object.</td>
</tr>
<tr>
<td class="name">{% highlight js %}
type{% endhighlight %}</td>
<td class="type"><span class="param-type">string</span></td>
<td class="description last">Name of the event</td>
</tr>
</tbody>
</table>



### legendBoundsCalculate
{:#events:legendboundscalculate}




Fires during the calculation of legend bounds. You can use this event to customize the bounds of legend.

#### Example


{% highlight js %}
 
//legendBoundsCalculate event for chart

$("#container").ejChart({

     legendBoundsCalculate: function (args) {
              //Do something
     }
     
});

{% endhighlight %}


<table class="params">
<thead>
<tr>
<th>Name</th>
<th>Type</th>
<th class="last">Description</th>
</tr>
</thead>
<tbody>
<tr>
<td class="name">{% highlight js %}
data{% endhighlight %}</td>
<td class="type"><span class="param-type">object</span></td>
<td class="description last"><ul><li>legendBoundsHeight - Height of the legend</li>
    <li>legendBoundsWidth - Width of the legend.</li>
    <li>legendBoundsRows - Number of rows to display the legend items</li>
</ul></td>
</tr>
<tr>
<td class="name">{% highlight js %}
cancel{% endhighlight %}</td>
<td class="type"><span class="param-type">boolean</span></td>
<td class="description last">Set this option to true to cancel the event.</td>
</tr>
<tr>
<td class="name">{% highlight js %}
model{% endhighlight %}</td>
<td class="type"><span class="param-type">object</span></td>
<td class="description last">Instance of the chart model object.</td>
</tr>
<tr>
<td class="name">{% highlight js %}
type{% endhighlight %}</td>
<td class="type"><span class="param-type">string</span></td>
<td class="description last">Name of the event</td>
</tr>
</tbody>
</table>


### legendItemClick
{:#events:legenditemclick}




Fires on clicking the legend item. 


#### Example


{% highlight js %}
 
//legendItemClick event for chart

$("#container").ejChart({

     legendItemClick: function (args) {
              //Do something
     }
     
});{% endhighlight %}



<table class="params">
<thead>
<tr>
<th>Name</th>
<th>Type</th>
<th class="last">Description</th>
</tr>
</thead>
<tbody>
<tr>
<td class="name">{% highlight js %}
cancel{% endhighlight %}</td>
<td class="type"><span class="param-type">boolean</span></td>
<td class="description last">Set this option to true to cancel the event</td>
</tr>
<tr>
<td class="name">{% highlight js %}
model{% endhighlight %}</td>
<td class="type"><span class="param-type">Object</span></td>
<td class="description last">Instance of the chart model object</td>
</tr>
<tr>
<td class="name">{% highlight js %}
type{% endhighlight %}</td>
<td class="type"><span class="param-type">string</span></td>
<td class="description last">Name of the event</td>
</tr>
<tr>
<td class="name">{% highlight js %}
data{% endhighlight %}</td>
<td class="type"><span class="param-type">object</span></td>
<td class="description last"><ul><li>startX - X-coordinate of legend item in pixel</li>
    <li>startY - Y-coordinate of legend item in pixel</li>
    <li>LegendItem - Instance of the legend item object that is about to be rendered</li>
    <li>style - Options to customize the legend item styles such as border, color, size, etc…,</li>
    <li>Bounds - Instance that holds information about legend bounds and legend item bounds.</li>
    <li>symbolShape - Name of the legend item shape. Use this option to customize legend item shape before rendering</li>
    <li>series - Instance of the series object corresponding to the legend item</li>
</ul></td>
</tr>
</tbody>
</table>


### legendItemMouseMove
{:#events:legenditemmousemove}




Fires when moving mouse over legend item. You can use this event for hit testing on legend items.

#### Example


{% highlight js %}
 
//legendItemMouseMove event for chart

$("#container").ejChart({

    legendItemMouseMove: function (args) {
             //Do something
    }
    
});

{% endhighlight %}


<table class="params">
<thead>
<tr>
<th>Name</th>
<th>Type</th>
<th class="last">Description</th>
</tr>
</thead>
<tbody>
<tr>
<td class="name">{% highlight js %}
cancel{% endhighlight %}</td>
<td class="type"><span class="param-type">boolean</span></td>
<td class="description last">Set this option to true to cancel the event</td>
</tr>
<tr>
<td class="name">{% highlight js %}
model{% endhighlight %}</td>
<td class="type"><span class="param-type">object</span></td>
<td class="description last">Instance of the chart model object</td>
</tr>
<tr>
<td class="name">{% highlight js %}
type{% endhighlight %}</td>
<td class="type"><span class="param-type">string</span></td>
<td class="description last">Name of the event</td>
</tr>
<tr>
<td class="name">{% highlight js %}
data{% endhighlight %}</td>
<td class="type"><span class="param-type">object</span></td>
<td class="description last"><ul><li>startX - X-coordinate of legend item in pixel</li>
    <li>startY - Y-coordinate of legend item in pixel</li>
    <li>LegendItem - Instance of the legend item object that is about to be rendered</li>
    <li>style - Options to customize the legend item styles such as border, color, size, etc…,</li>
    <li>Bounds - Instance that holds information about legend bounds and legend item bounds.</li>
    <li>symbolShape - Name of the legend item shape. Use this option to customize legend item shape before rendering</li>
    <li>series - Instance of the series object corresponding to the legend item</li>
</ul></td>
</tr>
</tbody>
</table>



### legendItemRendering
{:#events:legenditemrendering}




Fires before rendering the legend item. This event is fired for each legend item in Chart. You can use this event to customize legend item shape or add custom text to legend item.


#### Example


{% highlight js %}
 
//legendItemRendering event for chart

$("#container").ejChart({

    legendItemRendering: function (args) {
            //Do something
    }
    
});

{% endhighlight %}


<table class="params">
<thead>
<tr>
<th>Name</th>
<th>Type</th>
<th class="last">Description</th>
</tr>
</thead>
<tbody>
<tr>
<td class="name">{% highlight js %}
cancel{% endhighlight %}</td>
<td class="type"><span class="param-type">boolean</span></td>
<td class="description last">Set this option to true to cancel the event</td>
</tr>
<tr>
<td class="name">{% highlight js %}
model{% endhighlight %}</td>
<td class="type"><span class="param-type">object</span></td>
<td class="description last">Instance of the chart model object</td>
</tr>
<tr>
<td class="name">{% highlight js %}
type{% endhighlight %}</td>
<td class="type"><span class="param-type">string</span></td>
<td class="description last">Name of the event</td>
</tr>
<tr>
<td class="name">{% highlight js %}
data{% endhighlight %}</td>
<td class="type"><span class="param-type">object</span></td>
<td class="description last"><ul><li>startX - X-coordinate of legend item in pixel</li>
    <li>startY - Y-coordinate of legend item in pixel</li>
    <li>legendItem - Instance of the legend item object that is about to be rendered</li>
    <li>style - Options to customize the legend item styles such as border, color, size, etc.</li>
    <li>symbolShape - Name of the legend item shape. Use this option to customize legend item shape before rendering</li>
</ul></td>
</tr>
</tbody>
</table>



### load
{:#events:load}




Fires before loading the chart.


#### Example


{% highlight js %}
 
//load event for chart

$("#container").ejChart({

    load: function (args) {
             //Do something
    }
    
});

{% endhighlight %}



<table class="params">
<thead>
<tr>
<th>Name</th>
<th>Type</th>
<th class="last">Description</th>
</tr>
</thead>
<tbody>
<tr>
<td class="name">{% highlight js %}
cancel{% endhighlight %}</td>
<td class="type"><span class="param-type">boolean</span></td>
<td class="description last">Set this option to true to cancel the event</td>
</tr>
<tr>
<td class="name">{% highlight js %}
model{% endhighlight %}</td>
<td class="type"><span class="param-type">object</span></td>
<td class="description last">Instance of the chart model object</td>
</tr>
<tr>
<td class="name">{% highlight js %}
type{% endhighlight %}</td>
<td class="type"><span class="param-type">string</span></td>
<td class="description last">Name of the event</td>
</tr>
</tbody>
</table>


### zoomed
{:#events:zoomed}


Fires while performing rectangle zooming in chart.

#### Example


{% highlight js %}
 
//zoomed event for chart

$("#container").ejChart({

    zoomed: function (args) {
            //Do something
    }
   
});

{% endhighlight %}


<table class="params">
<thead>
<tr>
<th>Name</th>
<th>Type</th>
<th class="last">Description</th>
</tr>
</thead>
<tbody>
<tr>
<td class="name">{% highlight js %}
cancel{% endhighlight %}</td>
<td class="type"><span class="param-type">boolean</span></td>
<td class="description last">Set this option to true to cancel the event</td>
</tr>
<tr>
<td class="name">{% highlight js %}
model{% endhighlight %}</td>
<td class="type"><span class="param-type">object</span></td>
<td class="description last">Instance of the chart model object</td>
</tr>
<tr>
<td class="name">{% highlight js %}
type{% endhighlight %}</td>
<td class="type"><span class="param-type">string</span></td>
<td class="description last">Name of the event</td>
</tr>
<tr>
<td class="name">{% highlight js %}
data{% endhighlight %}</td>
<td class="type"><span class="param-type">object</span></td>
<td class="description last">Selected data collection of object</td>
</tr>
</tbody>
</table>



### rangeSelected
{:#events:rangeselected}




Fires after selected the data in chart.


#### Example


{% highlight js %}
 
//rangeSelected event for chart

$("#container").ejChart({

    rangeSelected: function (args) {
             //Do something
    }
    
});

{% endhighlight %}


<table class="params">
<thead>
<tr>
<th>Name</th>
<th>Type</th>
<th class="last">Description</th>
</tr>
</thead>
<tbody>
<tr>
<td class="name">{% highlight js %}
cancel{% endhighlight %}</td>
<td class="type"><span class="param-type">boolean</span></td>
<td class="description last">Set this option to true to cancel the event</td>
</tr>
<tr>
<td class="name">{% highlight js %}
model{% endhighlight %}</td>
<td class="type"><span class="param-type">object</span></td>
<td class="description last">Instance of the chart model object</td>
</tr>
<tr>
<td class="name">{% highlight js %}
type{% endhighlight %}</td>
<td class="type"><span class="param-type">string</span></td>
<td class="description last">Name of the event</td>
</tr>
<tr>
<td class="name">{% highlight js %}
data{% endhighlight %}</td>
<td class="type"><span class="param-type">object</span></td>
<td class="description last">Selected data collection of object</td>
</tr>
</tbody>
</table>



### pointRegionClick
{:#events:pointregionclick}




Fires on clicking a point in chart. You can use this event to handle clicks made on points.

#### Example


{% highlight js %}
 
//pointRegionClick event for chart

$("#container").ejChart({

    pointRegionClick: function (args) {
             //Do something
    }
    
});

{% endhighlight %}


<table class="params">
<thead>
<tr>
<th>Name</th>
<th>Type</th>
<th class="last">Description</th>
</tr>
</thead>
<tbody>
<tr>
<td class="name">{% highlight js %}
cancel{% endhighlight %}</td>
<td class="type"><span class="param-type">boolean</span></td>
<td class="description last">Set this option to true to cancel the event</td>
</tr>
<tr>
<td class="name">{% highlight js %}
model{% endhighlight %}</td>
<td class="type"><span class="param-type">object</span></td>
<td class="description last">Instance of the chart model object</td>
</tr>
<tr>
<td class="name">{% highlight js %}
type{% endhighlight %}</td>
<td class="type"><span class="param-type">string</span></td>
<td class="description last">Name of the event</td>
</tr>
<tr>
<td class="name">{% highlight js %}
data{% endhighlight %}</td>
<td class="type"><span class="param-type">object</span></td>
<td class="description last"><ul>
    <li>locationX - X-coordinate of point in pixel</li>
    <li>locationY - Y-coordinate of point in pixel</li>
    <li>seriesIndex - Index of the series in series collection to which the point belongs</li>
    <li>pointIndex - Index of the point in series</li>
</ul></td>
</tr>
</tbody>
</table>


### pointRegionMouseMove
{:#events:pointregionmousemove}




Fires when mouse is moved over a point. 

#### Example


{% highlight js %}
 
//pointRegionMouseMove event for chart

$("#container").ejChart({

    pointRegionMouseMove: function (args) {
                  //Do something
    }
   
});{% endhighlight %}


<table class="params">
<thead>
<tr>
<th>Name</th>
<th>Type</th>
<th class="last">Description</th>
</tr>
</thead>
<tbody>
<tr>
<td class="name">{% highlight js %}
cancel{% endhighlight %}</td>
<td class="type"><span class="param-type">boolean</span></td>
<td class="description last">Set this option to true to cancel the event</td>
</tr>
<tr>
<td class="name">{% highlight js %}
model{% endhighlight %}</td>
<td class="type"><span class="param-type">object</span></td>
<td class="description last">Instance of the chart model object</td>
</tr>
<tr>
<td class="name">{% highlight js %}
type{% endhighlight %}</td>
<td class="type"><span class="param-type">string</span></td>
<td class="description last">Name of the event</td>
</tr>
<tr>
<td class="name">{% highlight js %}
data{% endhighlight %}</td>
<td class="type"><span class="param-type">object</span></td>
<td class="description last"><ul>
    <li>locationX - X-coordinate of point in pixel</li>
    <li>locationY - Y-coordinate of point in pixel</li>
    <li>seriesIndex - Index of the series in series collection to which the point belongs</li>
    <li>pointIndex - Index of the point in series</li>
</ul></td>
</tr>
</tbody>
</table>


### preRender
{:#events:prerender}




Fires before rendering chart. 


#### Example


{% highlight js %}
 
//preRender event for chart

$("#container").ejChart({

    preRender: function (args) {
              //Do something
    }
   
});

{% endhighlight %}

<table class="params">
<thead>
<tr>
<th>Name</th>
<th>Type</th>
<th class="last">Description</th>
</tr>
</thead>
<tbody>
<tr>
<td class="name">{% highlight js %}
cancel{% endhighlight %}</td>
<td class="type"><span class="param-type">boolean</span></td>
<td class="description last">Set this option to true to cancel the event</td>
</tr>
<tr>
<td class="name">{% highlight js %}
model{% endhighlight %}</td>
<td class="type"><span class="param-type">object</span></td>
<td class="description last">Instance of the chart model object</td>
</tr>
<tr>
<td class="name">{% highlight js %}
type{% endhighlight %}</td>
<td class="type"><span class="param-type">string</span></td>
<td class="description last">Name of the event</td>
</tr>
</tbody>
</table>


### seriesRegionClick
{:#events:seriesregionclick}




Fires after selecting a series. This event is triggered after selecting a series only if selection mode is series.

#### Example


{% highlight js %}
 
//seriesRendering event for chart

$("#container").ejChart({

    seriesRegionClick: function (args) {
              //Do something
    }
    
});

{% endhighlight %}


<table class="params">
<thead>
<tr>
<th>Name</th>
<th>Type</th>
<th class="last">Description</th>
</tr>
</thead>
<tbody>
<tr>
<td class="name">{% highlight js %}
cancel{% endhighlight %}</td>
<td class="type"><span class="param-type">boolean</span></td>
<td class="description last">Set this option to true to cancel the event</td>
</tr>
<tr>
<td class="name">{% highlight js %}
model{% endhighlight %}</td>
<td class="type"><span class="param-type">object</span></td>
<td class="description last">Instance of the chart model object</td>
</tr>
<tr>
<td class="name">{% highlight js %}
type{% endhighlight %}</td>
<td class="type"><span class="param-type">string</span></td>
<td class="description last">Name of the event</td>
</tr>
    <tr>
<td class="name">{% highlight js %}
data{% endhighlight %}</td>
<td class="type"><span class="param-type">object</span></td>
<td class="description last"><ul>
    <li>series - Instance of the selected series</li>
    <li>seriesIndex - Index of the selected series</li>
</ul></td>
</tr>
</tbody>
</table>


### seriesRendering
{:#events:seriesrendering}




Fires before rendering a series. This event is fired for each series in Chart.

#### Example


{% highlight js %}
 
//seriesRendering event for chart

$("#container").ejChart({

    seriesRendering: function (args) {
              //Do something
    }
    
});

{% endhighlight %}


<table class="params">
<thead>
<tr>
<th>Name</th>
<th>Type</th>
<th class="last">Description</th>
</tr>
</thead>
<tbody>
<tr>
<td class="name">{% highlight js %}
cancel{% endhighlight %}</td>
<td class="type"><span class="param-type">boolean</span></td>
<td class="description last">Set this option to true to cancel the event</td>
</tr>
<tr>
<td class="name">{% highlight js %}
model{% endhighlight %}</td>
<td class="type"><span class="param-type">object</span></td>
<td class="description last">Instance of the chart model object</td>
</tr>
<tr>
<td class="name">{% highlight js %}
type{% endhighlight %}</td>
<td class="type"><span class="param-type">string</span></td>
<td class="description last">Name of the event</td>
</tr>
<tr>
<td class="name">{% highlight js %}
data{% endhighlight %}</td>
<td class="type"><span class="param-type">Object</span></td>
<td class="description last"><b>series</b> - Instance of the series which is about to get rendered</td>
</tr>
</tbody>
</table>


### symbolRendering
{:#events:symbolrendering}




Fires before rendering the marker symbols. This event is triggered for each marker in Chart.

#### Example


{% highlight js %}
 
//symbolRendering event for chart

$("#container").ejChart({
 
    symbolRendering: function (args) {
              //Do something
    }
    
});

{% endhighlight %}



<table class="params">
<thead>
<tr>
<th>Name</th>
<th>Type</th>
<th class="last">Description</th>
</tr>
</thead>
<tbody>
<tr>
<td class="name">{% highlight js %}
cancel{% endhighlight %}</td>
<td class="type"><span class="param-type">boolean</span></td>
<td class="description last">Set this option to true to cancel the event    </td>
</tr>
<tr>
<td class="name">{% highlight js %}
model{% endhighlight %}</td>
<td class="type"><span class="param-type">object</span></td>
<td class="description last">Instance of the chart model object</td>
</tr>
<tr>
<td class="name">{% highlight js %}
type{% endhighlight %}</td>
<td class="type"><span class="param-type">string</span></td>
<td class="description last">Name of the event</td>
</tr>
<tr>
<td class="name">{% highlight js %}
data{% endhighlight %}</td>
<td class="type"><span class="param-type">object</span></td>
<td class="description last"><ul>
    <li>location - Instance that holds the location of marker symbol</li>
    <li>style - Options to customize the marker style such as color, border and size</li>
</ul></td>
</tr>
</tbody>
</table>


### titleRendering
{:#events:titlerendering}




Fires before rendering the Chart title. You can use this event to add custom text in Chart title.


#### Example


{% highlight js %}
 
//titleRendering event for chart

$("#container").ejChart({

    titleRendering: function (args) {
              //Do something
    }
    
});

{% endhighlight %}

<table class="params">
<thead>
<tr>
<th>Name</th>
<th>Type</th>
<th class="last">Description</th>
</tr>
</thead>
<tbody>
<tr>
<td class="name">{% highlight js %}
cancel{% endhighlight %}</td>
<td class="type"><span class="param-type">boolean</span></td>
<td class="description last">Set this option to true to cancel the event    </td>
</tr>
<tr>
<td class="name">{% highlight js %}
model{% endhighlight %}</td>
<td class="type"><span class="param-type">object</span></td>
<td class="description last">Instance of the chart model object</td>
</tr>
<tr>
<td class="name">{% highlight js %}
type{% endhighlight %}</td>
<td class="type"><span class="param-type">string</span></td>
<td class="description last">Name of the event</td>
</tr>
<tr>
<td class="name">{% highlight js %}
data{% endhighlight %}</td>
<td class="type"><span class="param-type">object</span></td>
<td class="description last"><ul>
    <li>location - Option to customize the title location in pixels</li>
    <li>size - Read-only option to find the size of the title</li>
    <li>title - Use this option to add custom text in title</li>
</ul></td>
</tr>
</tbody>
</table>


### toolTipInitialize
{:#events:tooltipinitialize}




Fires before rendering the tooltip. This event is fired when tooltip is enabled and mouse is hovered on a Chart point. You can use this event to customize tooltip before rendering.

#### Example


{% highlight js %}
 
//toolTipInitialize event for chart
 
$("#container").ejChart({

    toolTipInitialize: function (args) {
              //Do something
    }
    
});{% endhighlight %}



<table class="params">
<thead>
<tr>
<th>Name</th>
<th>Type</th>
<th class="last">Description</th>
</tr>
</thead>
<tbody>
<tr>
<td class="name">{% highlight js %}
cancel{% endhighlight %}</td>
<td class="type"><span class="param-type">boolean</span></td>
<td class="description last">Set this option to true to cancel the event    </td>
</tr>
<tr>
<td class="name">{% highlight js %}
model{% endhighlight %}</td>
<td class="type"><span class="param-type">object</span></td>
<td class="description last">Instance of the chart model object</td>
</tr>
<tr>
<td class="name">{% highlight js %}
type{% endhighlight %}</td>
<td class="type"><span class="param-type">string</span></td>
<td class="description last">Name of the event</td>
</tr>
<tr>
<td class="name">{% highlight js %}
data{% endhighlight %}</td>
<td class="type"><span class="param-type">object</span></td>
<td class="description last"><ul>
    <li>currentText - Text to be displayed in tooltip. Set this option to customize the text displayed in tooltip</li>
    <li>pointIndex - Index of the point on which mouse is hovered</li>
    <li>seriesIndex - Index of the series in series collection whose point is hovered by mouse</li>
</ul></td>
</tr>
</tbody>
</table>


### trackAxisToolTip
{:#events:trackaxistooltip}




Fires before rendering crosshair tooltip in axis. This event is fired for each axis with crosshair label enabled. You can use this event to customize crosshair label before rendering


#### Example


{% highlight js %}
 
//trackAxisToolTip event for chart

$("#container").ejChart({

    trackAxisToolTip: function (args) {
              //Do something
    }
    
});

{% endhighlight %}

<table class="params">
<thead>
<tr>
<th>Name</th>
<th>Type</th>
<th class="last">Description</th>
</tr>
</thead>
<tbody>
<tr>
<td class="name">{% highlight js %}
cancel{% endhighlight %}</td>
<td class="type"><span class="param-type">boolean</span></td>
<td class="description last">Set this option to true to cancel the event    </td>
</tr>
<tr>
<td class="name">{% highlight js %}
model{% endhighlight %}</td>
<td class="type"><span class="param-type">object</span></td>
<td class="description last">Instance of the chart model object</td>
</tr>
<tr>
<td class="name">{% highlight js %}
type{% endhighlight %}</td>
<td class="type"><span class="param-type">string</span></td>
<td class="description last">Name of the event</td>
</tr>
<tr>
<td class="name">{% highlight js %}
data{% endhighlight %}</td>
<td class="type"><span class="param-type">object</span></td>
<td class="description last"><ul>
    <li>location - Location of the crosshair label in pixels</li>
    <li>axisIndex - Index of the axis for which crosshair label is displayed</li>
    <li>crossAxis - Instance of the chart axis object for which cross hair label is displayed</li>
    <li>currentTrackText - Text to be displayed in crosshair label. Use this option to add custom text in crosshair label</li>
</ul></td>
</tr>
</tbody>
</table>


### trackToolTip
{:#events:tracktooltip}




Fires before rendering trackball tooltip. This event is fired for each series in Chart because trackball tooltip is displayed for all the series. You can use this event to customize the text displayed in trackball tooltip.


#### Example


{% highlight js %}
 
//trackToolTip event for chart

$("#container").ejChart({

    trackToolTip: function (args) {
              //Do something
    }
   
});

{% endhighlight %}

<table class="params">
<thead>
<tr>
<th>Name</th>
<th>Type</th>
<th class="last">Description</th>
</tr>
</thead>
<tbody>
<tr>
<td class="name">{% highlight js %}
cancel{% endhighlight %}</td>
<td class="type"><span class="param-type">boolean</span></td>
<td class="description last">Set this option to true to cancel the event    </td>
</tr>
<tr>
<td class="name">{% highlight js %}
model{% endhighlight %}</td>
<td class="type"><span class="param-type">object</span></td>
<td class="description last">Instance of the chart model object</td>
</tr>
<tr>
<td class="name">{% highlight js %}
type{% endhighlight %}</td>
<td class="type"><span class="param-type">string</span></td>
<td class="description last">Name of the event</td>
</tr>
<tr>
<td class="name">{% highlight js %}
data{% endhighlight %}</td>
<td class="type"><span class="param-type">object</span></td>
<td class="description last"><ul>
    <li>location - Location of the trackball tooltip in pixels</li>
    <li>pointIndex - Index of the point for which trackball tooltip is displayed</li>
    <li>seriesIndex - Index of the series in series collection</li>
    <li>currentText - Text to be displayed in trackball tooltip. Use this option to add custom text in trackball tooltip</li>
    <li>series - Instance of the series object for which trackball tooltip is displayed.</li>
</ul></td>
</tr>
</tbody>
</table>



### axisLabelClick
{:#events:axislabelclick}




Fires, on clicking the axis label.


#### Example


{% highlight js %}
 
//axisLabelClick event for chart

$("#container").ejChart({

    axisLabelClick: function (args) {
              //Do something
    }
   
});

{% endhighlight %}

<table class="params">
<thead>
<tr>
<th>Name</th>
<th>Type</th>
<th class="last">Description</th>
</tr>
</thead>
<tbody>
<tr>
<td class="name">{% highlight js %}
cancel{% endhighlight %}</td>
<td class="type"><span class="param-type">boolean</span></td>
<td class="description last">Set this option to true to cancel the event    </td>
</tr>
<tr>
<td class="name">{% highlight js %}
model{% endhighlight %}</td>
<td class="type"><span class="param-type">object</span></td>
<td class="description last">Instance of the chart model object</td>
</tr>
<tr>
<td class="name">{% highlight js %}
type{% endhighlight %}</td>
<td class="type"><span class="param-type">string</span></td>
<td class="description last">Name of the event</td>
</tr>
<tr>
<td class="name">{% highlight js %}
data{% endhighlight %}</td>
<td class="type"><span class="param-type">Object</span></td>
<td class="description last"><ul><li> location - X and Y co-ordinate of the labels in chart area. 
    </li>
    <li>index - Index of the label.</li>
    <li>axis - Instance of the corresponding axis.</li>
    <li>text - Label that is clicked.</li>
                             </ul></td>
</tr>
</tbody>
</table>



### axisLabelMouseMove
{:#events:axislabelmousemove}




Fires on moving mouse over the axis label.


#### Example


{% highlight js %}
 
//axisLabelMouseMove event for chart

$("#container").ejChart({

    axisLabelMouseMove: function (args) {
              //Do something
    }
   
});

{% endhighlight %}

<table class="params">
<thead>
<tr>
<th>Name</th>
<th>Type</th>
<th class="last">Description</th>
</tr>
</thead>
<tbody>
<tr>
<td class="name">{% highlight js %}
cancel{% endhighlight %}</td>
<td class="type"><span class="param-type">boolean</span></td>
<td class="description last">Set this option to true to cancel the event    </td>
</tr>
<tr>
<td class="name">{% highlight js %}
model{% endhighlight %}</td>
<td class="type"><span class="param-type">object</span></td>
<td class="description last">Instance of the chart model object</td>
</tr>
<tr>
<td class="name">{% highlight js %}
type{% endhighlight %}</td>
<td class="type"><span class="param-type">string</span></td>
<td class="description last">Name of the event</td>
</tr>
<tr>
<td class="name">{% highlight js %}
data{% endhighlight %}</td>
<td class="type"><span class="param-type">Object</span></td>
<td class="description last"><ul><li>location - X and Y co-ordinate of the labels in chart area. 
    </li>
    <li>index - Index of the label.</li>
    <li>axis - Instance of the corresponding axis.</li>
    <li>text - Label that is hovered.</li>
                             </ul></td>
</tr>
</tbody>
</table>


### chartClick
{:#events:chartclick}




Fires, on the clicking the chart.


#### Example


{% highlight js %}
 
//chartClick event for chart

$("#container").ejChart({

    chartClick: function (args) {
              //Do something
    }
   
});

{% endhighlight %}

<table class="params">
<thead>
<tr>
<th>Name</th>
<th>Type</th>
<th class="last">Description</th>
</tr>
</thead>
<tbody>
<tr>
<td class="name">{% highlight js %}
cancel{% endhighlight %}</td>
<td class="type"><span class="param-type">boolean</span></td>
<td class="description last">Set this option to true to cancel the event    </td>
</tr>
<tr>
<td class="name">{% highlight js %}
model{% endhighlight %}</td>
<td class="type"><span class="param-type">object</span></td>
<td class="description last">Instance of the chart model object</td>
</tr>
<tr>
<td class="name">{% highlight js %}
type{% endhighlight %}</td>
<td class="type"><span class="param-type">string</span></td>
<td class="description last">Name of the event</td>
</tr>
<tr>
<td class="name">{% highlight js %}
data{% endhighlight %}</td>
<td class="type"><span class="param-type">Object</span></td>
<td class="description last"><ul><li>location - X and Y co-ordinate of the points with respect to chart area.</li>
<li>id - ID of the target element.</li>
    <li>size - Width and height of the chart.</li>
    <li>pageX - x-coordinate of the pointer, relative to the page</li>
    <li>pageY - y-coordinate of the pointer, relative to the page</li>
</ul>  </td>
</tr>
</tbody>
</table>


### multiLevelLabelClick
{:#events:multilevellabelclick}




Fires, on the clicking the Multi level labels of the chart .


#### Example


{% highlight js %}
 
//MultilevelLabelsClick event for chart

$("#container").ejChart({

    multiLevelLabelClick: function (args) {
              //Do something
    }
   
});

{% endhighlight %}

<table class="params">
<thead>
<tr>
<th>Name</th>
<th>Type</th>
<th class="last">Description</th>
</tr>
</thead>
<tbody>
<tr>
<td class="name">{% highlight js %}
cancel{% endhighlight %}</td>
<td class="type"><span class="param-type">boolean</span></td>
<td class="description last">Set this option to true to cancel the event    </td>
</tr>
<tr>
<td class="name">{% highlight js %}
model{% endhighlight %}</td>
<td class="type"><span class="param-type">object</span></td>
<td class="description last">Instance of the chart model object</td>
</tr>
<tr>
<td class="name">{% highlight js %}
type{% endhighlight %}</td>
<td class="type"><span class="param-type">string</span></td>
<td class="description last">Name of the event</td>
</tr>
<tr>
<td class="name">{% highlight js %}
data{% endhighlight %}</td>
<td class="type"><span class="param-type">object</span></td>
<td class="description last"><ul><li>location - X and Y co-ordinate of the points with respect to chart area.</li>
    <li>axis - axis of the multi level labels.</li>
    <li>multiLevelLabel - Multi level label details</li>
</ul></td>
</tr>
</tbody>
</table>

### chartMouseMove
{:#events:chartmousemove}




Fires on moving mouse over the chart.


#### Example


{% highlight js %}
 
//chartMouseMove event for chart

$("#container").ejChart({

    chartMouseMove: function (args) {
              //Do something
    }
   
});

{% endhighlight %}

<table class="params">
<thead>
<tr>
<th>Name</th>
<th>Type</th>
<th class="last">Description</th>
</tr>
</thead>
<tbody>
<tr>
<td class="name">{% highlight js %}
cancel{% endhighlight %}</td>
<td class="type"><span class="param-type">boolean</span></td>
<td class="description last">Set this option to true to cancel the event    </td>
</tr>
<tr>
<td class="name">{% highlight js %}
model{% endhighlight %}</td>
<td class="type"><span class="param-type">object</span></td>
<td class="description last">Instance of the chart model object</td>
</tr>
<tr>
<td class="name">{% highlight js %}
type{% endhighlight %}</td>
<td class="type"><span class="param-type">string</span></td>
<td class="description last">Name of the event</td>
</tr>
<tr>
<td class="name">{% highlight js %}
data{% endhighlight %}</td>
<td class="type"><span class="param-type">Object</span></td>
<td class="description last"><ul><li>location - X and Y co-ordinate of the points with respect to chart area.</li>
<li>id - ID of the target element.</li>
    <li>size - Width and height of the chart.</li>
    <li>pageX - x-coordinate of the pointer, relative to the page</li>
    <li>pageY - y-coordinate of the pointer, relative to the page</li>
</ul>  </td>
</tr>
</tbody>
</table>

### chartDoubleClick
{:#events:chartdoubleclick}




Fires, on double clicking the chart.


#### Example


{% highlight js %}
 
//chartDoubleClick event for chart

$("#container").ejChart({

    chartDoubleClick: function (args) {
              //Do something
    }
   
});

{% endhighlight %}

<table class="params">
<thead>
<tr>
<th>Name</th>
<th>Type</th>
<th class="last">Description</th>
</tr>
</thead>
<tbody>
<tr>
<td class="name">{% highlight js %}
cancel{% endhighlight %}</td>
<td class="type"><span class="param-type">boolean</span></td>
<td class="description last">Set this option to true to cancel the event    </td>
</tr>
<tr>
<td class="name">{% highlight js %}
model{% endhighlight %}</td>
<td class="type"><span class="param-type">object</span></td>
<td class="description last">Instance of the chart model object</td>
</tr>
<tr>
<td class="name">{% highlight js %}
type{% endhighlight %}</td>
<td class="type"><span class="param-type">string</span></td>
<td class="description last">Name of the event</td>
</tr>
<tr>
<td class="name">{% highlight js %}
data{% endhighlight %}</td>
<td class="type"><span class="param-type">Object</span></td>
<td class="description last"><ul><li>location - X and Y co-ordinate of the points with respect to chart area.</li>
<li>id - ID of the target element.</li>
    <li>size - Width and height of the chart.</li>
    <li>pageX - x-coordinate of the pointer, relative to the page</li>
    <li>pageY - y-coordinate of the pointer, relative to the page</li>
</ul>  </td>
</tr>
</tbody>
</table>


### chartMouseLeave
{:#events:chartmouseleave}




Fires when the mouse pointer leaves the chart


#### Example


{% highlight js %}
 
//chartMouseLeave event for chart

$("#container").ejChart({

    chartMouseLeave: function (args) {
              //Do something
    }
   
});

{% endhighlight %}

<table class="params">
<thead>
<tr>
<th>Name</th>
<th>Type</th>
<th class="last">Description</th>
</tr>
</thead>
<tbody>
<tr>
<td class="name">{% highlight js %}
cancel{% endhighlight %}</td>
<td class="type"><span class="param-type">boolean</span></td>
<td class="description last">Set this option to true to cancel the event    </td>
</tr>
<tr>
<td class="name">{% highlight js %}
model{% endhighlight %}</td>
<td class="type"><span class="param-type">object</span></td>
<td class="description last">Instance of the chart model object</td>
</tr>
<tr>
<td class="name">{% highlight js %}
type{% endhighlight %}</td>
<td class="type"><span class="param-type">string</span></td>
<td class="description last">Name of the event</td>
</tr>
<tr>
<td class="name">{% highlight js %}
data{% endhighlight %}</td>
<td class="type"><span class="param-type">Object</span></td>
<td class="description last"><ul><li>location - X and Y co-ordinate of the points with respect to chart area.</li>
<li>id - ID of the target element.</li>
    <li>size - Width and height of the chart.</li>
    <li>pageX - x-coordinate of the pointer, relative to the page</li>
    <li>pageY - y-coordinate of the pointer, relative to the page</li>
</ul>  </td>
</tr>
</tbody>
</table>

### annotationClick
{:#events:annotationclick}




Fires on clicking the annotation.


#### Example


{% highlight js %}
 
//annotationClick event for chart

$("#container").ejChart({

    annotationClick: function (args) {
              //Do something
    }
   
});

{% endhighlight %}

<table class="params">
<thead>
<tr>
<th>Name</th>
<th>Type</th>
<th class="last">Description</th>
</tr>
</thead>
<tbody>
<tr>
<td class="name">{% highlight js %}
cancel{% endhighlight %}</td>
<td class="type"><span class="param-type">boolean</span></td>
<td class="description last">Set this option to true to cancel the event    </td>
</tr>
<tr>
<td class="name">{% highlight js %}
model{% endhighlight %}</td>
<td class="type"><span class="param-type">object</span></td>
<td class="description last">Instance of the chart model object</td>
</tr>
<tr>
<td class="name">{% highlight js %}
type{% endhighlight %}</td>
<td class="type"><span class="param-type">string</span></td>
<td class="description last">Name of the event</td>
</tr>
<tr>
<td class="name">{% highlight js %}
data{% endhighlight %}</td>
<td class="type"><span class="param-type">Object</span></td>
<td class="description last"><ul>
    <li>location - X and Y co-ordinate of the annotation in chart area. </li>
    <li>contentData - Information about the annotation, like Coordinate unit, Region, content</li>
    <li>pageX- x-coordinate of the pointer, relative to the page</li>
    <li>pageY - y-coordinate of the pointer, relative to the page</li>
                             </ul> </td>
</tr>
</tbody>
</table>

### afterResize
{:#events:afterresize}




Fires, after the chart is resized.


#### Example


{% highlight js %}
 
//afterResize event for chart

$("#container").ejChart({

    afterResize: function (args) {
              //Do something
    }
   
});

{% endhighlight %}

<table class="params">
<thead>
<tr>
<th>Name</th>
<th>Type</th>
<th class="last">Description</th>
</tr>
</thead>
<tbody>
<tr>
<td class="name">{% highlight js %}
cancel{% endhighlight %}</td>
<td class="type"><span class="param-type">boolean</span></td>
<td class="description last">Set this option to true to cancel the event    </td>
</tr>
<tr>
<td class="name">{% highlight js %}
model{% endhighlight %}</td>
<td class="type"><span class="param-type">object</span></td>
<td class="description last">Instance of the chart model object</td>
</tr>
<tr>
<td class="name">{% highlight js %}
type{% endhighlight %}</td>
<td class="type"><span class="param-type">string</span></td>
<td class="description last">Name of the event</td>
</tr>
<tr>
<td class="name">{% highlight js %}
data{% endhighlight %}</td>
<td class="type"><span class="param-type">object</span></td>
<td class="description last"><ul><li>
    width - Chart width, after resize</li>
    <li>height - Chart height, after resize</li>
    <li>prevWidth - Chart width, before resize</li>
    <li>prevHeight - Chart height, before resize</li>
    <li>originalWidth- Chart width, when the chart was first rendered</li>
    <li>originalHeight - Chart height, when the chart was first rendered </li>
</ul>
</td>
</tr>
</tbody>
</table>




### beforeResize
{:#events:beforeresize}




Fires, when chart size is changing.


#### Example


{% highlight js %}
 
//beforeResize event for chart

$("#container").ejChart({

    beforeResize: function (args) {
              //Do something
    }
   
});

{% endhighlight %}

<table class="params">
<thead>
<tr>
<th>Name</th>
<th>Type</th>
<th class="last">Description</th>
</tr>
</thead>
<tbody>
<tr>
<td class="name">{% highlight js %}
cancel{% endhighlight %}</td>
<td class="type"><span class="param-type">boolean</span></td>
<td class="description last">Set this option to true to cancel the event    </td>
</tr>
<tr>
<td class="name">{% highlight js %}
model{% endhighlight %}</td>
<td class="type"><span class="param-type">object</span></td>
<td class="description last">Instance of the chart model object</td>
</tr>
<tr>
<td class="name">{% highlight js %}
type{% endhighlight %}</td>
<td class="type"><span class="param-type">string</span></td>
<td class="description last">Name of the event</td>
</tr>
<tr>
<td class="name">{% highlight js %}
data{% endhighlight %}</td>
<td class="type"><span class="param-type">object</span></td>
<td class="description last"><ul><li>currentWidth - Chart width, before resize</li>
    <li>currentHeight - Chart height, before resize</li>
    <li>newWidth - Chart width, after resize</li>
    <li>newHeight - Chart height, after resize</li>
</ul> </td>
</tr>
</tbody>
</table>





### errorBarRendering
{:#events:errorbarrendering}




Fires, when error bar is rendering.


#### Example


{% highlight js %}
 
//errorBarRendering event for chart

$("#container").ejChart({

    errorBarRendering: function (args) {
              //Do something
    }
   
});

{% endhighlight %}

<table class="params">
<thead>
<tr>
<th>Name</th>
<th>Type</th>
<th class="last">Description</th>
</tr>
</thead>
<tbody>
<tr>
<td class="name">{% highlight js %}
cancel{% endhighlight %}</td>
<td class="type"><span class="param-type">boolean</span></td>
<td class="description last">Set this option to true to cancel the event    </td>
</tr>
<tr>
<td class="name">{% highlight js %}
model{% endhighlight %}</td>
<td class="type"><span class="param-type">object</span></td>
<td class="description last">Instance of the chart model object</td>
</tr>
<tr>
<td class="name">{% highlight js %}
type{% endhighlight %}</td>
<td class="type"><span class="param-type">string</span></td>
<td class="description last">Name of the event</td>
</tr>
<tr>
<td class="name">{% highlight js %}
data{% endhighlight %}</td>
<td class="type"><span class="param-type">object</span></td>
<td class="description last"> <b>errorBar</b> - Error bar Object  </td>
</tr>
</tbody>
</table>


### multiLevelLabelRendering
{:#events:multilevellabelrendering}




Fires, when multi level labels are rendering.


#### Example


{% highlight js %}
 
//multi level labels rendering event for chart

$("#container").ejChart({

  multiLevelLabelRendering: function (args) {
              //Do something
    }
   
});

{% endhighlight %}

<table class="params">
<thead>
<tr>
<th>Name</th>
<th>Type</th>
<th class="last">Description</th>
</tr>
</thead>
<tbody>
<tr>
<td class="name">{% highlight js %}
cancel{% endhighlight %}</td>
<td class="type"><span class="param-type">boolean</span></td>
<td class="description last">Set this option to true to cancel the event    </td>
</tr>
<tr>
<td class="name">{% highlight js %}
model{% endhighlight %}</td>
<td class="type"><span class="param-type">object</span></td>
<td class="description last">Instance of the chart model object</td>
</tr>
<tr>
<td class="name">{% highlight js %}
type{% endhighlight %}</td>
<td class="type"><span class="param-type">string</span></td>
<td class="description last">Name of the event</td>
</tr>
<tr>
<td class="name">{% highlight js %}
data{% endhighlight %}</td>
<td class="type"><span class="param-type">object</span></td>
<td class="description last"><b>MultiLevelLabels</b> - MultiLevel Label Object  </td>
</tr>
</tbody>
</table>


### trendlineRendering
{:#events:trendlinerendering}




Fires, when trendlines are rendering.


#### Example


{% highlight js %}
 
//trendline rendering event for chart

$("#container").ejChart({

  trendlineRendering: function (args) {
              //Do something
    }
   
});

{% endhighlight %}

<table class="params">
<thead>
<tr>
<th>Name</th>
<th>Type</th>
<th class="last">Description</th>
</tr>
</thead>
<tbody>
<tr>
<td class="name">{% highlight js %}
cancel{% endhighlight %}</td>
<td class="type"><span class="param-type">boolean</span></td>
<td class="description last">Set this option to true to cancel the event    </td>
</tr>
<tr>
<td class="name">{% highlight js %}
model{% endhighlight %}</td>
<td class="type"><span class="param-type">object</span></td>
<td class="description last">Instance of the chart model object</td>
</tr>
<tr>
<td class="name">{% highlight js %}
type{% endhighlight %}</td>
<td class="type"><span class="param-type">string</span></td>
<td class="description last">Name of the event</td>
</tr>
<tr>
<td class="name">{% highlight js %}
data{% endhighlight %}</td>
<td class="type"><span class="param-type">object</span></td>
<td class="description last"><ul>
    <li>trendlines - Trendline Object</li>
    <li>series - Series data of the chart</li>
    <li>forwardForecast - Forward Forecast value for the trendline</li>
    <li>backwardForecast - Backward Forecast value for the trendline</li>
</ul></td>
</tr>
</tbody>
</table>



### scrollChanged
{:#events:scrollchanged}


Trigger, after the scrollbar position is changed.



<table class="params">
<thead>
<tr>
<th>Name</th>
<th>Type</th>
<th class="last">Description</th>
</tr>
</thead>
<tbody>
<tr>
<td class="name">{% highlight js %}
data{% endhighlight %}</td>
<td class="type"><span class="param-type">object</span></td>
<td class="description last"><ul>
    <li>oldRange - returns the scrollbar position old start and end range value on change end of scrollbar</li>
    <li>newRange - returns the scrollbar position new start and end range value on change end of scrollbar</li>
</ul></td>
</tr>
<tr>
<td class="name">{% highlight html %}
cancel{% endhighlight %}</td>
<td class="type"><span class="param-type">boolean</span></td>
<td class="description last">if the event should be canceled; otherwise, false.</td>
</tr>
<tr>
<td class="name">{% highlight html %}
model{% endhighlight %}</td>
<td class="type"><span class="param-type">object</span></td>
<td class="description last">returns the RangeNavigator model</td>
</tr>
<tr>
<td class="name">{% highlight html %}
type{% endhighlight %}</td>
<td class="type"><span class="param-type">string</span></td>
<td class="description last">returns the name of the event</td>
</tr>
</tbody>
</table>


#### Example


{% highlight js %}
 
//scrollbarChanged event for chart
$("#container").ejChart({
   scrollChanged: function (args) {}
});{% endhighlight %}



### scrollStart
{:#events:scrollstart}


Event triggered when scroll starts


<table class="params">
<thead>
<tr>
<th>Name</th>
<th>Type</th>
<th class="last">Description</th>
</tr>
</thead>
<tbody>
<tr>
<td class="name">{% highlight js %}
data{% endhighlight %}</td>
<td class="type"><span class="param-type">object</span></td>
<td class="description last"><ul>
    <li>startRange - returns the scrollbar position starting range value on changing scrollbar</li>
    <li>endRange - returns the scrollbar position end range value on changing scrollbar</li>
</ul></td>
</tr>
<tr>
<td class="name">{% highlight html %}
cancel{% endhighlight %}</td>
<td class="type"><span class="param-type">boolean</span></td>
<td class="description last">if the event should be canceled; otherwise, false.</td>
</tr>
<tr>
<td class="name">{% highlight html %}
model{% endhighlight %}</td>
<td class="type"><span class="param-type">object</span></td>
<td class="description last">returns the RangeNavigator model</td>
</tr>
<tr>
<td class="name">{% highlight html %}
type{% endhighlight %}</td>
<td class="type"><span class="param-type">string</span></td>
<td class="description last">returns the name of the event</td>
</tr>
</tbody>
</table>


#### Example


{% highlight js %}
 
//scrollbarChanged event for chart
$("#container").ejChart({
   scrollStart: function (args) {}
});{% endhighlight %}



### scrollEnd
{:#events:scrollend}


Event triggered when scroll end



<table class="params">
<thead>
<tr>
<th>Name</th>
<th>Type</th>
<th class="last">Description</th>
</tr>
</thead>
<tbody>
<tr>
<td class="name">{% highlight js %}
data{% endhighlight %}</td>
<td class="type"><span class="param-type">object</span></td>
<td class="description last"><ul>
    <li>oldRange - returns the scrollbar position old start and end range value on change end of scrollbar</li>
    <li>newRange - returns the scrollbar position new start and end range value on change end of scrollbar</li>
</ul></td>
</tr>
<tr>
<td class="name">{% highlight html %}
cancel{% endhighlight %}</td>
<td class="type"><span class="param-type">boolean</span></td>
<td class="description last">if the event should be canceled; otherwise, false.</td>
</tr>
<tr>
<td class="name">{% highlight html %}
model{% endhighlight %}</td>
<td class="type"><span class="param-type">object</span></td>
<td class="description last">returns the RangeNavigator model</td>
</tr>
<tr>
<td class="name">{% highlight html %}
type{% endhighlight %}</td>
<td class="type"><span class="param-type">string</span></td>
<td class="description last">returns the name of the event</td>
</tr>
</tbody>
</table>


#### Example


{% highlight js %}
 
//scrollbarChanged event for chart
$("#container").ejChart({
   scrollEnd: function (args) {}
});{% endhighlight %}



### dragStart
{:#events:dragstart}




Fires when the dragging is started


#### Example


{% highlight js %}
 
//Drag Start event for chart

$("#container").ejChart({

    dragStart: function (args) {
              //Do something
    }
   
});

{% endhighlight %}

<table class="params">
<thead>
<tr>
<th>Name</th>
<th>Type</th>
<th class="last">Description</th>
</tr>
</thead>
<tbody>
<tr>
<td class="name">{% highlight js %}
cancel{% endhighlight %}</td>
<td class="type"><span class="param-type">boolean</span></td>
<td class="description last">Set this option to true to cancel the event    </td>
</tr>
<tr>
<td class="name">{% highlight js %}
model{% endhighlight %}</td>
<td class="type"><span class="param-type">object</span></td>
<td class="description last">Instance of the chart model object</td>
</tr>
<tr>
<td class="name">{% highlight js %}
type{% endhighlight %}</td>
<td class="type"><span class="param-type">string</span></td>
<td class="description last">Name of the event</td>
</tr>
<tr>
<td class="name">{% highlight js %}
data{% endhighlight %}</td>
<td class="type"><span class="param-type">object</span></td>
<td class="description last"><ul><li>seriesIndex - Series Index of the point held for dragging</li>
    <li>pointIndex - PointIndex of the point held for dragging</li>
    <li>point - Information of the point held for dragging</li>
</ul>  </td>
</tr>
</tbody>
</table>



### dragging
{:#events:dragging}




Fires while  dragging 


#### Example


{% highlight js %}
 
//Dragging event for chart

$("#container").ejChart({

    dragging: function (args) {
              //Do something
    }
   
});

{% endhighlight %}

<table class="params">
<thead>
<tr>
<th>Name</th>
<th>Type</th>
<th class="last">Description</th>
</tr>
</thead>
<tbody>
<tr>
<td class="name">{% highlight js %}
cancel{% endhighlight %}</td>
<td class="type"><span class="param-type">boolean</span></td>
<td class="description last">Set this option to true to cancel the event    </td>
</tr>
<tr>
<td class="name">{% highlight js %}
model{% endhighlight %}</td>
<td class="type"><span class="param-type">object</span></td>
<td class="description last">Instance of the chart model object</td>
</tr>
<tr>
<td class="name">{% highlight js %}
type{% endhighlight %}</td>
<td class="type"><span class="param-type">string</span></td>
<td class="description last">Name of the event</td>
</tr>
<tr>
<td class="name">{% highlight js %}
data{% endhighlight %}</td>
<td class="type"><span class="param-type">object</span></td>
<td class="description last"><ul><li>seriesIndex - Series Index of the point held for dragging</li>
    <li>pointIndex - PointIndex of the point held for dragging</li>
    <li>oldValue - Previous value of the point before dragging</li>
    <li>newValue - Current value of the point</li>
</ul>  </td>
</tr>
</tbody>
</table>


### dragEnd
{:#events:dragend}




Fires when the dragging is completed 


#### Example


{% highlight js %}
 
//DragEnd event for chart

$("#container").ejChart({

    dragEnd: function (args) {
              //Do something
    }
   
});

{% endhighlight %}

<table class="params">
<thead>
<tr>
<th>Name</th>
<th>Type</th>
<th class="last">Description</th>
</tr>
</thead>
<tbody>
<tr>
<td class="name">{% highlight js %}
cancel{% endhighlight %}</td>
<td class="type"><span class="param-type">boolean</span></td>
<td class="description last">Set this option to true to cancel the event    </td>
</tr>
<tr>
<td class="name">{% highlight js %}
model{% endhighlight %}</td>
<td class="type"><span class="param-type">object</span></td>
<td class="description last">Instance of the chart model object</td>
</tr>
<tr>
<td class="name">{% highlight js %}
type{% endhighlight %}</td>
<td class="type"><span class="param-type">string</span></td>
<td class="description last">Name of the event</td>
</tr>
<tr>
<td class="name">{% highlight js %}
data{% endhighlight %}</td>
<td class="type"><span class="param-type">object</span></td>
<td class="description last"><ul><li>seriesIndex - Series Index of the point held for dragging</li>
    <li>pointIndex - PointIndex of the point held for dragging</li>
    <li>oldValue - Previous value of the point before dragging</li>
    <li>newValue - Current value of the point</li>
    <li>series - Contains the all the series information of the chart</li>
</ul>  </td>
</tr>
</tbody>
</table>

### subTitleRendering
{:#events:subtitlerendering}




Fires when the sub Title of the chart is rendered


#### Example


{% highlight js %}
 
//Subtitle rendering event for chart

$("#container").ejChart({

    subTitleRendering: function (args) {
              //Do something
    }
   
});

{% endhighlight %}

<table class="params">
<thead>
<tr>
<th>Name</th>
<th>Type</th>
<th class="last">Description</th>
</tr>
</thead>
<tbody>
<tr>
<td class="name">{% highlight js %}
cancel{% endhighlight %}</td>
<td class="type"><span class="param-type">boolean</span></td>
<td class="description last">Set this option to true to cancel the event    </td>
</tr>
<tr>
<td class="name">{% highlight js %}
model{% endhighlight %}</td>
<td class="type"><span class="param-type">object</span></td>
<td class="description last">Instance of the chart model object</td>
</tr>
<tr>
<td class="name">{% highlight js %}
type{% endhighlight %}</td>
<td class="type"><span class="param-type">string</span></td>
<td class="description last">Name of the event</td>
</tr>
<tr>
<td class="name">{% highlight js %}
data{% endhighlight %}</td>
<td class="type"><span class="param-type">object</span></td>
<td class="description last"><ul>
    <li>location - location of the subTitle text</li>
    <li>subtitle - text of the subtitle</li>
    <li>size - Size of the Subtitle text</li>
</ul></td>
</tr>
</tbody>
</table>

