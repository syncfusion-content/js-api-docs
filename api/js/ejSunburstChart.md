---
layout: post
title: API reference for ejSunburstChart
description: What are the options, methods and events available in Essential JavaScript Sunburst.
documentation: API
platform: js-api
keywords: ejSunburstChart, API, Essential JS Sunburst, Sunburst, SunburstChart
metaname: 
metacontent: 
---

# ejSunburstChart
<ts root="datavisualization" />

Essential Sunburst can be easily configured to the DOM element, such as div. You can create a Sunburst with highly customizable look and feel.

#### Syntax

{% highlight js %}

$(element).ejSunburstChart();

{% endhighlight %}

#### Example

{% highlight html %}
 
<div id="container"></div> 
 
<script>
// Create Sunburst
$('#container').ejSunburstChart();      
</script>

{% endhighlight %}

#### Requires

* module:jQuery.js

* module:ej.core.js

* module:ej.data.js

* module:ej.sunburst.js

* module:ej.globalize.js

## Members

### background `string`
{:#members:background}

Background color of the plot area.

#### Default Value

* null

#### Example

{% highlight js %}
 
$("#container").ejSunburstChart({

    background : "gray" 
                          
});

{% endhighlight %}




### valueMemberPath `string`
{:#members:valueMemberPath}

Bind the data field from the data source.

#### Default Value

* null

#### Example

{% highlight js %}

$("#container").ejSunburstChart({

    valueMemberPath : "Population" 
                          
});

{% endhighlight %}



### border `object`
{:#members:border}

Options for customizing the sunburst border.

### border.color `string`
{:#members:border-color}

Border color of the sunburst.

#### Default Value

* null

#### Example

{% highlight js %}
                             
$("#container").ejSunburstChart({

   border: { color: "green" }                      

});

{% endhighlight %}


### border.width `number`
{:#members:border-width}

Width of the Sunburst border.

#### Default Value

* 2

#### Example

{% highlight js %}
 
$("#container").ejSunburstChart({

   border: { width: 3 }                      

});

{% endhighlight %}

### segmentBorder `object`
{:#members:segmentborder}

Options for customizing the sunburst segment border.

### segmentBorder.color `string`
{:#members:segmentborder-color}

Segment Border color of the sunburst.

#### Default Value

* null

#### Example

{% highlight js %}
                             
$("#container").ejSunburstChart({

   segmentBorder: { color: "green" }                      

});

{% endhighlight %}


### segmentBorder.width `number`
{:#members:segmentborder-width}

Width of the Sunburst segment border.

#### Default Value

* 2

#### Example

{% highlight js %}
 
$("#container").ejSunburstChart({

   segmentBorder: { width: 3 }                      

});

{% endhighlight %}



### dataSource `object`
{:#members:datasource}

Specifies the dataSource to the sunburst.

#### Default Value

* null

#### Example

{% highlight js %}
 
$("#container").ejSunburstChart({
    
    dataSource: data
                       
});

{% endhighlight %}



### palette `string`
{:#members:palette}

Palette color for the data points.

#### Default Value

* null

#### Example

{% highlight js %}
 
$("#container").ejSunburstChart({
    palette : "ColorFieldName"                  
});
{% endhighlight %}

### parentNode `string`
{:#members:parentnode}

Parent node of the data points.

#### Default Value

 * null

#### Example

{% highlight js %}

$("#container").ejSunburstChart({
    
    parentNode: "ParentNode"
                       
});

{% endhighlight %}


### xName `string`
{:#members:xname}

Name of the property in the datasource that contains x values.

#### Default Value

 * null

#### Example

{% highlight js %}

$("#container").ejSunburstChart({
    
    xName: "XValue"
                       
});

{% endhighlight %}



### yName `string`
{:#members:yname}

Name of the property in the datasource that contains y values.

#### Default Value

 * null

#### Example

{% highlight js %}

$("#container").ejSunburstChart({
    
    yName: "YValue"
                       
});

{% endhighlight %}


### isResponsive `boolean`
{:#members:isresponsive}

Controls whether sunburst has to be responsive or not.

#### Default Value

* true


#### Example

{% highlight js %}
 
$("#container").ejSunburstChart({

   isResponsive : true             

});

{% endhighlight %}


### size `object`
{:#members:size}

Options to customize the Sunburst size.



### size.height `string`
{:#members:size-height}

Height of the Sunburst.

#### Default Value

* ''

#### Example

{% highlight js %}
 
$("#container").ejSunburstChart({

   size :{height : '80'}          

});

{% endhighlight %}




### size.width `string`
{:#members:size-width}

Width of the Sunburst. 

#### Default Value

* ''

#### Example

{% highlight js %}
 
$("#container").ejSunburstChart({

   size :{width : '80'}          

});

{% endhighlight %}



### visible `boolean`
{:#members:visible}

Controls the visibility of sunburst.

#### Default Value

* true


#### Example

{% highlight js %}
 
$("#container").ejSunburstChart({

   visible : true             

});

{% endhighlight %}



### tooltip `object`
{:#members:tooltip}

Options to customize the Sunburst tooltip.





### tooltip.visible `boolean`
{:#members:tooltip-visible}

tooltip visibility of the Sunburst.

#### Default Value

* true

#### Example

{% highlight js %}
 
$("#container").ejSunburstChart({

   tooltip :{visible : false}          

});

{% endhighlight %}


### tooltip.border `object`
{:#members:tooltip-border}

Options for customizing the border of the sunburst tooltip.

### tooltip.border.color `string`
{:#members:tooltip-border-color}

Border color of the tooltip. 

#### Default Value

* null

#### Example

{% highlight js %}
 
$("#container").ejSunburstChart({
    tooltip:{
        border:{color : "green"}
    }                  
});

{% endhighlight %}



### tooltip.border.width `number`
{:#members:tooltip-border-width}

Border width of the tooltip. 

#### Default Value

* 5

#### Example

{% highlight js %}

$("#container").ejSunburstChart({
    tooltip :{border :{width : 2}}                  
});

{% endhighlight %}



### tooltip.fill `string`
{:#members:tooltip-fill}

Fill color for the sunburst tooltip.

#### Default Value

* null

#### Example

{% highlight js %}
 
$("#container").ejSunburstChart({
    tooltip:{fill : "green"}                  
});

{% endhighlight %}


### tooltip.font `object`
{:#members:tooltip-font}

Options for customizing the font of the tooltip.

### tooltip.font.color `string`
{:#members:tooltip-font-color}

Font color of the text in the tooltip.

#### Default Value

* null

#### Example

{% highlight js %}
  
$("#container").ejSunburstChart({
tooltip :{font :{color : "green"}}                 
});
{% endhighlight %}

### tooltip.font.fontFamily `string`
{:#members:tooltip-font-fontfamily}

Font Family for the tooltip.

#### Default Value

* "Segoe UI"

#### Example

{% highlight js %} 

$("#container").ejSunburstChart({
tooltip :{ font : { fontFamily : "Algerian"}}                 
});
 {% endhighlight %}
 
 
### tooltip.font.fontStyle `enum`
{:#members:tooltip-font-fontstyle}

<ts name="ej.datavisualization.Sunburst.FontStyle"/>
Specifies the font Style for the tooltip.

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

* "Normal"

#### Example


{% highlight js %}
 

$("#container").ejSunburstChart({
tooltip : {font :{fontStyle : "italic"}}                 
});
{% endhighlight %}


### tooltip.font.fontWeight `enum`
{:#members:tooltip-font-fontweight}


<ts name="ej.datavisualization.Sunburst.FontWeight"/>
Specifies the font weight for the tooltip.


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



* "Regular"




#### Example


{% highlight js %}
 

$("#container").ejSunburstChart({
tooltip :{font :{fontWeight : "lighter"}}                 
});
{% endhighlight %}




### tooltip.font.opacity `number`
{:#members:tooltip-font-opacity}




Opacity for text in the tooltip.


#### Default Value



* 1




#### Example


{% highlight js %}
 

$("#container").ejSunburstChart({
tooltip :{font :{opacity : 0.5}}                 
});
{% endhighlight %}




### tooltip.font.size `string`
{:#members:tooltip-font-size}




Font size for text in the tooltip.

#### Default Value



 * "12px"




#### Example


{% highlight js %}
 
 
$("#container").ejSunburstChart({
tooltip :{font :{size : "14px"}}                 
});
{% endhighlight %}


### tooltip.template `string`
{:#members:tooltip-template}

Custom template to the tooltip.

#### Default Value

* null

#### Example

{% highlight js %}

$("#container").ejSunburstChart({
    tooltip :{template : "item"}                  
});

{% endhighlight %}
 
### tooltip.format `string`
{:#members:tooltip-format}

Setting the format for the data displayed in the tooltip

#### Default Value

* "#point.x# : #point.y#"

#### Example

{% highlight js %}

$("#container").ejSunburstChart({
    tooltip :{format : "#point.x# : #point.y#%"}                  
});

{% endhighlight %}

### tooltip.opacity `number`
{:#members:tooltip-opacity}

Sets the opacity of the displayed tooltip

#### Default Value

* 0.95

#### Example

{% highlight js %}

$("#container").ejSunburstChart({
    tooltip :{opacity : 1}                  
});

{% endhighlight %}





### points `object`
{:#members:points}

Options for customizing sunburst points.

### points.x `string`
{:#members:points-x}

Points x value of the sunburst.

#### Default Value

* null

#### Example

{% highlight js %}
                             
$("#container").ejSunburstChart({

   points: { x: "XValue" }                      

});

{% endhighlight %}


### points.y `number`
{:#members:points-y}

Points y value of the sunburst.

#### Default Value

* null

#### Example

{% highlight js %}
                             
$("#container").ejSunburstChart({

   points: { y: 100 }                      

});

{% endhighlight %}

### points.text `string`
{:#members:points-text}

Points text of the sunburst.

#### Default Value

* null

#### Example

{% highlight js %}
                             
$("#container").ejSunburstChart({

   points: { text: "Other" }                      

});

{% endhighlight %}

### points.fill `string`
{:#members:points-fill}

Points fill color of the sunburst.

#### Default Value

* null

#### Example

{% highlight js %}
                             
$("#container").ejSunburstChart({

   points: { fill: "red" }                      

});

{% endhighlight %}


### startAngle `number`
{:#members:startAngle}

Sunburst rendering will start from the specified value

#### Default Value

* null

#### Example

{% highlight js %}
 
$("#container").ejSunburstChart({

    startAngle : 90             

});

{% endhighlight %}

### endAngle `number`
{:#members:startAngle}

Sunburst rendering will end at the specified value

#### Default Value

* null

#### Example

{% highlight js %}
 
$("#container").ejSunburstChart({

    endAngle : 360             

});

{% endhighlight %}

### radius `number`
{:#members:radius}

Sunburst outer radius value

#### Default Value

* 1

#### Example

{% highlight js %}
 
$("#container").ejSunburstChart({

    radius : 0.8             

});

{% endhighlight %}

### innerRadius `number`
{:#members:innerradius}

Sunburst inner radius value

#### Default Value

* 0.4

#### Example

{% highlight js %}
 
$("#container").ejSunburstChart({

    innerRadius : 0.2            

});

{% endhighlight %}



### dataLabelSettings `object`
{:#members:datalabelsettings}

Options to customize the Sunburst dataLabel.



### dataLabelSettings.visible `boolean`
{:#members:datalabelsettings-visible}

Datalabel visibility of the Sunburst.

#### Default Value

* false

#### Example

{% highlight js %}
 
$("#container").ejSunburstChart({

   dataLabelSettings :{visible : true}          

});

{% endhighlight %}


### dataLabelSettings.labelRotationMode `enum`
{:#members:datalabelsettings-labelrotationmode}

<ts name="ej.datavisualization.Sunburst.SunburstLabelRotationMode"/>
Alignment of sunburst datalabel


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
Angle</td>
<td class="type">string</td> 
<td class="description"> Display the datalabel in angle </td>
</tr>
<tr>
<td class="name">
Normal</td>
<td class="type">string</td>
<td class="description"> Align the datalabel in normal mode</td>
</tr>
</tbody>
</table>

#### Default Value

* "Angle". See <a href="ejsunburstchart.html#members:datalabelsettings-labelrotationmode">DatalabelAlignment</a>


#### Example

{% highlight js %}
 
$("#container").ejSunburstChart({

   dataLabelSettings :{labelRotationMode : "normal"}                    

});

{% endhighlight %}


### dataLabelSettings.font `object`
{:#members:datalabelsettings-font}


Options for customizing the data label font.


### dataLabelSettings.font.fontFamily `string`
{:#members:datalabelsettings-font-fontfamily}


Font family of the data label. 

#### Default Value


* "Segoe UI"


#### Example


{% highlight js %}
 
 
$("#container").ejSunburstChart({
    dataLabelSettings :{ font :{fontFamily : "Algerian"}}                 
});
{% endhighlight %}




### dataLabelSettings.font.fontStyle `enum`
{:#members:datalabelsettings-font-fontstyle}

<ts ref="ej.datavisualization.Sunburst.FontStyle"/>


Font style of the data label.   


#### Default Value


* "normal". See <a href="ejsunburstchart.html#datalabelsettings-font-fontstyle">FontStyle</a>


#### Example


{% highlight js %}
 
 
$("#container").ejSunburstChart({
    dataLabelSettings :{font :{ fontStyle : "italic" }}                 
});
 {% endhighlight %}



### dataLabelSettings.font.fontWeight `enum`
{:#members:datalabelsettings-font-fontweight}


<ts ref="ej.datavisualization.Sunburst.FontWeight"/>


Font weight of the data label.  


#### Default Value


* "regular". See <a href="ejsunburstchart.html#members:datalabelsettings-font-fontweight">FontWeight</a>


#### Example


{% highlight js %}
 
 
$("#container").ejSunburstChart({
    dataLabelSettings :{font : { fontWeight : "lighter" }}                 
});
{% endhighlight %}



### dataLabelSettings.font.opacity `number`
{:#members:datalabelsettings-font-opacity}


Opacity of the text. 


#### Default Value


 * 1


#### Example


{% highlight js %}
 
 
$("#container").ejSunburstChart({
    dataLabelSettings :{font :{ opacity : 0.5 }}               
});
{% endhighlight %}

### dataLabelSettings.font.color `string`
{:#members:datalabelsettings-font-color}

Font color of the data label text. 

#### Default Value

 * null

#### Example

{% highlight js %}

 
$("#container").ejSunburstChart({
    dataLabelSettings :{font :{ color : "red" }}                 
});
{% endhighlight %}


### dataLabelSettings.font.size `string`
{:#members:datalabelsettings-font-size}


Font size of the data label. 


#### Default Value


* "12px"


#### Example


{% highlight js %}
 

$("#container").ejSunburstChart({
    dataLabelSettings :{font : { size : "14px" }}               
});
{% endhighlight %}



### dataLabelSettings.template `string`
{:#members:datalabelsettings-template}

Custom template for datalabel 


#### Default Value


* "null"


#### Example


{% highlight js %}
 

$("#container").ejSunburstChart({
    dataLabelSettings :{ template: "item" }               
});
{% endhighlight %}


### dataLabelSettings.fill `string`
{:#members:datalabelsettings-fill}

Fill color for the datalabel


#### Default Value


* null


#### Example


{% highlight js %}
 

$("#container").ejSunburstChart({
    dataLabelSettings :{ fill: "yellow" }               
});
{% endhighlight %}



### dataLabelSettings.labelOverflowMode `enum`
{:#members:datalabelsettings-labeloverflowmode}

<ts name="ej.datavisualization.Sunburst.SunburstLabelOverflowMode"/>
Datalabel overflow mode


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
Trim</td>
<td class="type">string</td> 
<td class="description"> Trim the datalabel </td>
</tr>
<tr>
<td class="name">
Hide</td>
<td class="type">string</td>
<td class="description"> Hide the datalabel</td>
</tr>
<tr>
<td class="name">
None</td>
<td class="type">string</td>
<td class="description"> Datalabel displayed in normal format</td>
</tr>
</tbody>
</table>

#### Default Value

* "Trim". See <a href="ejsunburstchart.html#members:datalabelsettings-labeloverflowmode">LabelOverflowMode</a>


#### Example

{% highlight js %}
 
$("#container").ejSunburstChart({

   dataLabelSettings :{labelOverflowMode : "hide"}                    

});

{% endhighlight %}


### title `object`
{:#members:title}


Options for customizing the title and subtitle of sunburst.


### title.text `string`
{:#members:title-text}


Title text for sunburst


#### Default Value

* ""


#### Example


{% highlight js %}
 
$("#container").ejSunburstChart({

   title : { text: "Sunburst Chart" }                     

});

{% endhighlight %}




### title.visible `string`
{:#members:title-visible}


Title text visibility for sunburst


#### Default Value

* true


#### Example


{% highlight js %}
 
$("#container").ejSunburstChart({

   title : { visible: false }                     

});

{% endhighlight %}



### title.textAlignment `enum`
{:#members:title-textalignment}

<ts name="ej.datavisualization.Sunburst.SunburstAlignment"/>
Title text alignment

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
<td class="description"> Display the sunburst title center </td>
</tr>
<tr>
<td class="name">
Near</td>
<td class="type">string</td>
<td class="description"> Display the title near to the chart</td>
</tr>
<tr>
<td class="name">
Far</td>
<td class="type">string</td>
<td class="description"> Display the title far to the chart</td>
</tr>
</tbody>
</table>

#### Default Value

* "center". See <a href="ejsunburstchart.html#members:title-textalignment">TextAlignment</a>


#### Example

{% highlight js %}
 
$("#container").ejSunburstChart({

   title :{textAlignment : "near"}                    

});

{% endhighlight %}

### title.font `object`
{:#members:title-font}


Options for customizing the font of sunburst title.





### title.font.fontFamily `string`
{:#members:title-font-fontfamily}



Font family for Sunburst title.


#### Default Value

* "Segoe UI"


#### Example


{% highlight js %}
 
$("#container").ejSunburstChart({

   title : { font : { fontFamily : "Algerian" } }                     

});

{% endhighlight %}



### title.font.fontStyle `enum`
{:#members:title-font-fontstyle}

<ts ref="ej.datavisualization.Sunburst.FontStyle"/>


Font style for Sunburst title.


#### Default Value

* "Normal". See <a href="ejsunburstchart.html#members:title-font-fontstyle">FontStyle</a>


#### Example


{% highlight js %}
 
$("#container").ejSunburstChart({

   title : { font : { fontStyle : "italic" } }                     

});

{% endhighlight %}



### title.font.fontWeight `enum`
{:#members:title-font-fontweight}


<ts ref="ej.datavisualization.Sunburst.FontWeight"/>

Font weight for Sunburst title.


#### Default Value

* "Regular". See <a href="ejsunburstchart.html#members:title-font-fontweight">FontWeight</a>


#### Example


{% highlight js %}
 
$("#container").ejSunburstChart({

   title : { font : { fontWeight : "lighter" } }                     

});

{% endhighlight %}



### title.font.opacity `number`
{:#members:title-font-opacity}


Opacity of the Sunburst title.


#### Default Value

* 1


#### Example


{% highlight js %}
 
$("#container").ejSunburstChart({

   title : { font : { opacity : 0.8 } }                     

});

{% endhighlight %}




### title.font.size `string`
{:#members:title-font-size}



Font size for Sunburst title.


#### Default Value

* "20px"


#### Example


{% highlight js %}
 
$("#container").ejSunburstChart({

   title : { font : { size : "22px" } }                     

});

{% endhighlight %}



### title.subtitle `object`
{:#members:title-subtitle}


Options to customize the sub title of Sunburst.


### title.subtitle.text `string`
{:#members:title--subtitle-text}


Subtitle text for sunburst


#### Default Value

* ""


#### Example


{% highlight js %}
 
$("#container").ejSunburstChart({

   title : { subtitle :{text: "Sunburst Subtitle" }}                 

});

{% endhighlight %}




### title.subtitle.visible `string`
{:#members:title-subtitle-visible}


Sub title text visibility for sunburst


#### Default Value

* true


#### Example


{% highlight js %}
 
$("#container").ejSunburstChart({

   title : {subtitle:{visible: false }}                     

});

{% endhighlight %}



### title.subtitle.textAlignment `enum`
{:#members:title-subtitle-textalignment}

<ts ref="ej.datavisualization.Sunburst.SunburstAlignment"/>

Sub title text alignment

#### Default Value

* "far". See <a href="ejsunburstchart.html#members:title-subtitle-textalignment">TextAlignment</a>


#### Example

{% highlight js %}
 
$("#container").ejSunburstChart({

   title :{subtitle : {textAlignment : "near"}}                    

});

{% endhighlight %}

### title.subtitle.font `object`
{:#members:title-subtitle-font}


Options for customizing the font of sub title.



### title.subtitle.font.fontFamily `string`
{:#members:title-subtitle-font-fontfamily}


Font family of sub title.


#### Default Value

* "Segoe UI"


#### Example


{% highlight js %}
 
$("#container").ejSunburstChart({

   title: {subtitle : {font :{ fontFamily : "Algerian" } } }                      

});

{% endhighlight %}




### title.subtitle.font.fontStyle `enum`
{:#members:title-subtitle-font-fontstyle}

<ts ref="ej.datavisualization.Sunburst.FontStyle"/>


Font style for sub title.


#### Default Value

* "Normal". See <a href="ejsunburstchart.html#members:title-subtitle-font-fontstyle">FontStyle</a>


#### Example


{% highlight js %}
 
$("#container").ejSunburstChart({

   title: { subtitle : {font :{ fontStyle : "Normal" } } }                     

});

{% endhighlight %}



### title.subtitle.font.fontWeight `enum` 
{:#members:title-subtitle-font-fontweight}

<ts ref="ej.datavisualization.Sunburst.FontWeight"/>


Font weight for sub title.


#### Default Value

* "Regular". See <a href="ejsunburstchart.html#members:title-subtitle-font-fontweight">FontWeight</a>



#### Example


{% highlight js %}
 
$("#container").ejSunburstChart({

   title: { subtitle : {font :{ fontWeight : "regular" } } }                     

});

{% endhighlight %}



### title.subtitle.font.opacity `number`
{:#members:title-subtitle-font-opacity}



Opacity of the sub title.


#### Default Value

* 1



#### Example


{% highlight js %}
 
$("#container").ejSunburstChart({

   title: { subtitle : {font :{ opacity : 0.5 } } }                     

});

{% endhighlight %}



### title.subtitle.font.size `string`
{:#members:title-subtitle-font-size}



Font size for sub title.


#### Default Value

* "12px"



#### Example


{% highlight js %}
 
$("#container").ejSunburstChart({

   title: { subtitle : {font :{ size : "14px" } } }                     

});

{% endhighlight %}


### highlightSettings `object`
{:#members:highlightsettings}


Options for customizing the appearance of the levels or point while highlighting.


### highlightSettings.enable `boolean`
{:#members:highlightSettings-enable}


Enables/disables the ability to highlight the levels or point interactively.

#### Default Value


* false


#### Example


{% highlight js %}
 
 
$("#container").ejSunburstChart({
    highlightSettings:{enable:true}                 
});
{% endhighlight %}



### highlightSettings.mode `enum`
{:#members:highlightsettings-mode}


<ts name="ej.datavisualization.Sunburst.SunburstHighlightMode"/>
Specifies whether the levels or point has to be highlighted.


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
Point</td>
<td class="type">string</td> 
<td class="description">Highlight/Select the point in the levels.</td>
</tr>
<tr>
<td class="name">
Parent</td>
<td class="type">string</td>
<td class="description">Highlight/Select the parent of levels.</td>
</tr> 
<tr>
<td class="name">
Child</td>
<td class="type">string</td>
<td class="description">Highlight/Select the child of levels.</td>
</tr> 
<tr>
<td class="name">
All</td>
<td class="type">string</td>
<td class="description">Highlight/Select all the points in levels.</td>
</tr> 
</tbody>
</table>


#### Default Value


* "point". See <a href="ejsunburstchart.html#members:highlightsettings-mode">Mode</a>


#### Example


{% highlight js %}
 
 
$("#container").ejSunburstChart({
    highlightSettings:{mode:"point"}                  
});
{% endhighlight %}



### highlightSettings.color `string`
{:#members:highlightsettings-color}


Color of the levels/point on highlight.


#### Default Value


* "red"
 

#### Example


{% highlight js %}
 
 
$("#container").ejSunburstChart({
    highlightSettings:{color:"red"}               
});
{% endhighlight %}


### highlightSettings.opacity `number`
{:#members:highlightsettings-opacity}


Opacity of the levels/point on highlight.


#### Default Value


* 0.5

 

#### Example


{% highlight js %}
 
 
$("#container").ejSunburstChart({
    highlightSettings:{opacity:1}            
});
{% endhighlight %}


### highlightSettings.type `enum`
{:#members:highlightsettings-type}


<ts name="ej.datavisualization.Sunburst.SunburstHighlightType"/>
Specifies whether the levels or data point has to be highlighted.


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
Opacity</td>
<td class="type">string</td> 
<td class="description">Highlight/Select the point in opacity.</td>
</tr>
<tr>
<td class="name">
Color</td>
<td class="type">string</td>
<td class="description">Highlight/Select the point in color.</td>
</tr> 
</tbody>
</table>


#### Default Value


* "opacity". See <a href="ejsunburstchart.html#members:highlightsettings-type">Mode</a>


#### Example


{% highlight js %}
 
 
$("#container").ejSunburstChart({
    highlightSettings:{type:"color"}                  
});
{% endhighlight %}



### selectionSettings `object`
{:#members:selectionsettings}


Options for customizing the appearance of the levels or data point while selection.


### selectionSettings.enable `boolean`
{:#members:selectionsettings-enable}


Enables/disables the ability to select the levels or data point interactively.

#### Default Value


* false


#### Example


{% highlight js %}
 
 
$("#container").ejSunburstChart({
    selectionSettings:{enable:true}                 
});
{% endhighlight %}



### selectionSettings.mode `enum`
{:#members:selectionsettings-mode}


<ts ref="ej.datavisualization.Sunburst.SunburstHighlightMode"/>


Specifies whether the levels or data point has to be selected.



#### Default Value


* "point". See <a href="ejsunburstchart.html#members:selectionsettings-mode">Mode</a>


#### Example


{% highlight js %}
 
 
$("#container").ejSunburstChart({
    selectionSettings:{mode:"point"}                  
});
{% endhighlight %}



### selectionSettings.color `string`
{:#members:selectionsettings-color}


Color of the levels/point on selection.


#### Default Value


* "green"
 

#### Example


{% highlight js %}
 
 
$("#container").ejSunburstChart({
    selectionSettings:{color:"red"}               
});
{% endhighlight %}


### selectionSettings.opacity `number`
{:#members:selectionsettings-opacity}


Opacity of the levels/point on selection.


#### Default Value


* 0.5

 

#### Example


{% highlight js %}
 
 
$("#container").ejSunburstChart({
    selectionSettings:{opacity:1}            
});
{% endhighlight %}


### selectionSettings.type `enum`
{:#members:selectionsettings-type}


<ts ref="ej.datavisualization.Sunburst.SunburstHighlightType"/>


Specifies whether the levels or data point has to be selected.




#### Default Value


* "opacity". See <a href="ejsunburstchart.html#members:selectionsettings-type">Mode</a>


#### Example


{% highlight js %}
 
 
$("#container").ejSunburstChart({
    selectionSettings:{type:"color"}                  
});
{% endhighlight %}


### levels `array`
{:#members:levels}

Specify levels of sunburst for grouped visualization of data

#### Default Value

* []


### levels.groupMemberPath `string`
{:#members:levels-groupmemberpath}

Specifies the group member path

#### Default Value

* null

#### Example

{% highlight js %}

  $("#container").ejSunburstChart({   
      levels: [{ groupMemberPath: "Continent" }]
  });

{% endhighlight %}


### legend `object`
{:#members:legend}


Options to customize the legend items and legend title.

### legend.visible `boolean`
{:#members:legend-visible}


Visibility of the legend.


#### Default Value

* false


#### Example


{% highlight js %}
 
$("#container").ejSunburstChart({

   legend : {visible:true}}                     

});

{% endhighlight %}

### legend.clickAction `enum`
{:#members:legend-clickaction}

<ts name="ej.datavisualization.Sunburst.SunburstClickAction"/>
Interactive action of legend items.


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
<td class="description"> None of the mouse action performed on legend</td>
</tr>
<tr>
<td class="name">
ToggleSegmentVisibility</td>
<td class="type">string</td>
<td class="description"> Toggle segment visibility action is performed on legend</td>
</tr> 
<tr>
<td class="name">
ToggleSegmentSelection</td>
<td class="type">string</td>
<td class="description"> Toggle segment selection action is performed on legend</td>
</tr> 
</tbody>
</table>

#### Default Value

* "toggleSegmentVisibility". See <a href="ejsunburstchart.html#members:legend-clickaction">Alignment</a>


#### Example


{% highlight js %}
 
$("#container").ejSunburstChart({

   legend :{clickAction : "toggleSegmentSelection"}                    

});

{% endhighlight %}



### legend.alignment `enum`
{:#members:legend-alignment}

<ts name="ej.datavisualization.Sunburst.SunburstAlignment"/>
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

* "Center". See <a href="ejsunburstchart.html#members:legend-alignment">Alignment</a>


#### Example


{% highlight js %}
 
$("#container").ejSunburstChart({

   legend :{alignment : "far"}                    

});

{% endhighlight %}




### legend.border `object`
{:#members:legend-border}


Options for customizing the legend border.




### legend.border.color `string`
{:#members:legend-border-color}


Border color of the legend.


#### Default Value

* null


#### Example


{% highlight js %}
 
$("#container").ejSunburstChart({

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
 
$("#container").ejSunburstChart({

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
 
$("#container").ejSunburstChart({

   legend :{ columnCount : 2}                    

});

{% endhighlight %}




### legend.rowCount `number`
{:#members:legend-rowcount}


Number of rows to arrange the legend items.


#### Default Value

* null


#### Example


{% highlight js %}
 
$("#container").ejSunburstChart({

   legend :{ rowCount : 2}                    

});

{% endhighlight %}





### legend.font `object`
{:#members:legend-font}


Options to customize the font used for legend item text.





### legend.font.fontFamily `string`
{:#members:legend-font-fontfamily}



Font family for legend item text.


#### Default Value

* "Segoe UI"



#### Example


{% highlight js %}
 
$("#container").ejSunburstChart({

   legend :{ font :{fontFamily : "Algerian"}}                    

});

{% endhighlight %}



### legend.font.fontStyle `enum`
{:#members:legend-font-fontstyle}

<ts ref="ej.datavisualization.Sunburst.FontStyle"/>


Font style for legend item text.


#### Default Value

* "Normal". See <a href="ejsunburstchart.html#members:legend-font-fontstyle">FontStyle</a>


#### Example


{% highlight js %}
 
$("#container").ejSunburstChart({

   legend :{ font :{fontStyle : "italic"}}                    

});

{% endhighlight %}



### legend.font.fontWeight `enum`
{:#members:legend-font-fontweight}

<ts ref="ej.datavisualization.Sunburst.FontWeight"/>


Font weight for legend item text.


#### Default Value

* "Regular". See <a href="ejsunburstchart.html#members:legend-font-fontweight">FontWeight</a>



#### Example


{% highlight js %}
 
$("#container").ejSunburstChart({

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
 
$("#container").ejSunburstChart({

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
 
$("#container").ejSunburstChart({

   legend :{itemPadding : 5}                     

});

{% endhighlight %}







### legend.itemStyle `object`
{:#members:legend-itemstyle}


Options to customize the style of legend items.


### legend.itemStyle.height `number`
{:#members:legend-itemstyle-height}


Height of the shape in legend items.


#### Default Value

* 10



#### Example


{% highlight js %}
 
$("#container").ejSunburstChart({

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
 
$("#container").ejSunburstChart({

   legend :{ itemStyle :{width : 15}}                    

});

{% endhighlight %}

### legend.location `object`
{:#members:legend-location}


Options to customize the location of sunburst legend. Legend is placed in provided location only when value of **position** property is **custom**





### legend.location.x `number`
{:#members:legend-location-x}



X value or horizontal offset to position the legend in chart.


#### Default Value

* 0




#### Example


{% highlight js %}
 
$("#container").ejSunburstChart({

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
 
$("#container").ejSunburstChart({

   legend :{location : {y : 100}}                  

});

{% endhighlight %}


### legend.position `enum`
{:#members:legend-position}

<ts name="ej.datavisualization.Sunburst.SunburstLegendPosition"/>
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

* "Bottom". See <a href="ejsunburstchart.html#members:legend-position">Position</a>


#### Example


{% highlight js %}
 
$("#container").ejSunburstChart({

   legend :{ position : "top"}                    

});

{% endhighlight %}







### legend.shape `enum`
{:#members:legend-shape}

<ts name="ej.datavisualization.Sunburst.SunburstLegendShape"/>
Shape of the legend items. 

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
Diamond</td>
<td class="type">string</td> 
<td class="description">Shape of legend will be diamond</td>
</tr>
<tr>
<td class="name">
Pentagon</td>
<td class="type">string</td>
<td class="description">Shape of legend will be pentagon</td>
</tr> 
<tr>
<td class="name">
Rectangle</td>
<td class="type">string</td>
<td class="description">Shape of legend will be rectangle</td>
</tr> 
<tr>
<td class="name">
Circle</td>
<td class="type">string</td>
<td class="description">Shape of legend will be circle.</td>
</tr> 
<tr>
<td class="name">
Cross</td>
<td class="type">string</td>
<td class="description">Shape of legend will be cross.</td>
</tr> 
<tr>
<td class="name">
Triangle</td>
<td class="type">string</td>
<td class="description">Shape of legend will be triangle.</td>
</tr> 
</tbody>
</table>

#### Default Value

* "None". See <a href="ejsunburstchart.html#members:legend-shape">Shape</a>



#### Example


{% highlight js %}
 
$("#container").ejSunburstChart({

   legend :{ shape : "circle" }                      

});

{% endhighlight %}







### legend.size `object`
{:#members:legend-size}



Options to customize the size of the legend.







### legend.size.height `string`
{:#members:legend-size-height}




Height of the legend. Height can be specified in either pixel or percentage.


#### Default Value

* null



#### Example


{% highlight js %}
 
$("#container").ejSunburstChart({

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
 
$("#container").ejSunburstChart({

   legend :{ size :{width : "20%"}}                    

});

{% endhighlight %}



### legend.title `object`
{:#members:legend-title}



Options to customize the legend title.




### legend.title.font `object`
{:#members:legend-title-font}



Options to customize the font used for legend title







### legend.title.font.fontFamily `string`
{:#members:legend-title-font-fontfamily}




Font family for the text in legend title.


#### Default Value

* "Segoe UI"




#### Example


{% highlight js %}
 
$("#container").ejSunburstChart({

   legend: { title: { font :{fontFamily: "Algerian" } } }                      

});

{% endhighlight %}




### legend.title.font.fontStyle `enum`
{:#members:legend-title-font-fontstyle}

<ts ref="ej.datavisualization.Sunburst.FontStyle"/>


Font style for legend title.


#### Default Value

* "normal". See <a href="ejsunburstchart.html#members:legend-title-font-fontstyle">FontStyle</a>




#### Example


{% highlight js %}
 
$("#container").ejSunburstChart({

   legend: { title: { font :{fontStyle: "normal" } } }                      

});

{% endhighlight %}




### legend.title.font.fontWeight `enum`
{:#members:legend-title-font-fontweight}

<ts ref="ej.datavisualization.Sunburst.FontWeight"/>


Font weight for legend title.


#### Default Value

* "normal". See <a href="ejsunburstchart.html#members:legend-title-font-fontweight">FontWeight</a>




#### Example


{% highlight js %}
 
$("#container").ejSunburstChart({

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
 
$("#container").ejSunburstChart({

   legend: { title: { font :{size: "14px" } } }                      

});

{% endhighlight %}

### legend.title.visible `string`
{:#members:legend-title-visible}



Enables or disables the legend title.


#### Default Value

* true




#### Example


{% highlight js %}
 
$("#container").ejSunburstChart({

   legend: { title: { visible: false } }                      

});

{% endhighlight %}


### legend.title.text `string`
{:#members:legend-title-text}


Text to be displayed in legend title.


#### Default Value

* ""




#### Example


{% highlight js %}
 
$("#container").ejSunburstChart({

   legend: { title: { text : "Countries" } }                      

});

{% endhighlight %}







### legend.title.textAlignment `enum`
{:#members:legend-title-textalignment}

<ts name="ej.datavisualization.Sunburst.SunburstAlignment"/>
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

* "center". See <a href="ejsunburstchart.html#members:legend-title-textalignment">Alignment</a>




#### Example


{% highlight js %}
 
$("#container").ejSunburstChart({

   legend: { title: { textAlignment : "near" } }                      

});

{% endhighlight %}





### theme `enum`
{:#members:theme}

<ts name="ej.datavisualization.Sunburst.SunburstTheme"/>
Specifies the theme for Sunburst.

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
</tbody>
</table>



#### Default Value

* "Flatlight". See <a href="ejsunburstchart.html#members:theme">Theme</a>


#### Example


{% highlight js %}
 
$("#container").ejSunburstChart({

   theme : "flatdark"            

});

{% endhighlight %}



### margin `object`
{:#members:margin}


Options to customize the left, right, top and bottom margins of sunburst area.






### margin.left `number`
{:#members:margin-left}



Spacing for the left margin of chart area. Setting positive value decreases the width of the chart area from left side.


#### Default Value

* 10




#### Example


{% highlight js %}
 
$("#container").ejSunburstChart({

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
 
$("#container").ejSunburstChart({

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
 
$("#container").ejSunburstChart({

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
 
$("#container").ejSunburstChart({

   margin : { bottom: 10 }             

});

{% endhighlight %}


### enableAnimation `boolean`
{:#members:enableanimation}


Enable/disable the animation for all the levels.


#### Default Value

* false




#### Example


{% highlight js %}
 
 
$("#container").ejSunburstChart({
    enableAnimation : true                  
});
 {% endhighlight %}



### opacity `number`
{:#members:opacity}

Opacity of the levels.


#### Default Value



* 1




#### Example


{% highlight js %}
 
 
$("#container").ejSunburstChart({
    opacity : 0.5              
});
 {% endhighlight %}


### zoomSettings `object`
{:#members:zoomsettings}


Options for enable zooming feature of chart.



### zoomSettings.enable `boolean`
{:#members:zoomsettings}


Enables or disables zooming.


#### Default Value

* false




#### Example


{% highlight js %}
 
$("#container").ejSunburstChart({

   zoomSettings :{enable :true}          

});

{% endhighlight %}

### zoomSettings.toolbarHorizontalAlignment `enum`
{:#members:zoomsettings-toolbarhorizontalalignment}

<ts name="ej.datavisualization.Sunburst.SunburstHorizontalAlignment"/>
Toolbar horizontal alignment


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
<td class="description">Aligns the toolbar in center</td>
</tr>
<tr>
<td class="name">
Left</td>
<td class="type">string</td>
<td class="description">Aligns the toolbar in left</td>
</tr> 
<tr>
<td class="name">
Right</td>
<td class="type">string</td>
<td class="description">Aligns the toolbar in right</td>
</tr> 
</tbody>
</table>



#### Default Value

* "right". See <a href="ejsunburstchart.html#members:zoomsettings-toolbarhorizontalalignment">Alignment</a>




#### Example


{% highlight js %}
 
$("#container").ejSunburstChart({

   zoomSettings: { toolbarHorizontalAlignment: "center" }                      

});

{% endhighlight %}

### zoomSettings.toolbarVerticalAlignment `enum`
{:#members:zoomsettings-toolbarverticalalignment}

<ts name="ej.datavisualization.Sunburst.SunburstVerticalAlignment"/>
Toolbar vertical alignment


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
<td class="description">Aligns the toolbar in top</td>
</tr>
<tr>
<td class="name">
Bottom</td>
<td class="type">string</td>
<td class="description">Aligns the toolbar in bottom</td>
</tr> 
<tr>
<td class="name">
Middle</td>
<td class="type">string</td>
<td class="description">Aligns the toolbar in center</td>
</tr> 
</tbody>
</table>



#### Default Value

* "top". See <a href="ejsunburstchart.html#members:zoomsettings-toolbarverticalalignment">Alignment</a>




#### Example


{% highlight js %}
 
$("#container").ejSunburstChart({

   zoomSettings: { toolbarVerticalAlignment: "middle" }                      

});

{% endhighlight %}


### animationType `enum`
{:#members:animationtype}

<ts name="ej.datavisualization.Sunburst.Animation"/>
Animation type of sunburst


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
Rotation</td>
<td class="type">string</td> 
<td class="description">Animates points rendering in rotation</td>
</tr>
<tr>
<td class="name">
FadeIn</td>
<td class="type">string</td>
<td class="description">Animates points in fade in</td>
</tr> 
</tbody>
</table>



#### Default Value

* "rotation". See <a href="ejsunburstchart.html#members:animationtype">Alignment</a>




#### Example


{% highlight js %}
 
$("#container").ejSunburstChart({

   animationType:"fadeIn"                     

});

{% endhighlight %}


## Methods


### redraw()
{:#methods:redraw}

Redraws the entire sunburst. You can call this method whenever you update, add or remove points from the data source or whenever you want to refresh the UI.


#### Returns: void


#### Example

{% highlight js %}
// Redraw Sunburst
var sunburstObj = $("#container").data("ejSunburstChart");
sunburstObj.redraw();
{% endhighlight %}


{% highlight js %}
 
$("#container").ejSparkline("redraw");      
{% endhighlight %}


### destroy ()
{:#methods:destroy}


destroy the sunburst


#### Returns: void


#### Example


{% highlight js %}

// Destroy sunburst
var sunburstObj = $("#container").data("ejSunburstChart");
sunburstObj.destroy(); 

{% endhighlight %}


{% highlight js %}

$("#container").ejSunburstChart("destroy"); 
   
{% endhighlight %}



## Events

### load
{:#events:load}

Fires before loading.


#### Example


{% highlight js %}
 
//load event for sunburst

$("#container").ejSunburstChart({

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
data{% endhighlight %}</td>
<td class="type"><span class="param-type">string</span></td>
<td class="description last">Load event data</td>
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
<td class="description last">Instance of the sunburst model object</td>
</tr>
<tr>
<td class="name">{% highlight js %}
type{% endhighlight %}</td>
<td class="type"><span class="param-type">string</span></td>
<td class="description last">Name of the event</td>
</tr>
</tbody>
</table>


### preRender
{:#events:prerender}




Fires before rendering sunburst. 


#### Example


{% highlight js %}
 
//preRender event for sunburst

$("#container").ejSunburstChart({

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
data{% endhighlight %}</td>
<td class="type"><span class="param-type">string</span></td>
<td class="description last">PreRender event data</td>
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
<td class="description last">Instance of the sunburst model object</td>
</tr>
<tr>
<td class="name">{% highlight js %}
type{% endhighlight %}</td>
<td class="type"><span class="param-type">string</span></td>
<td class="description last">Name of the event</td>
</tr>
</tbody>
</table>


### loaded
{:#events:loaded}




Fires after rendering sunburst. 


#### Example


{% highlight js %}
 
//loaded event for sunburst

$("#container").ejSunburstChart({

    loaded: function (args) {
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
<td class="type"><span class="param-type">string</span></td>
<td class="description last">Loaded event data</td>
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
<td class="description last">Instance of the sunburst model object</td>
</tr>
<tr>
<td class="name">{% highlight js %}
type{% endhighlight %}</td>
<td class="type"><span class="param-type">string</span></td>
<td class="description last">Name of the event</td>
</tr>
</tbody>
</table>


### dataLabelRendering
{:#events:datalabelrendering}




Fires before rendering the datalabel 


#### Example


{% highlight js %}
 
//dataLabelRendering event for sunburst

$("#container").ejSunburstChart({

    dataLabelRendering: function (args) {
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
<td class="type"><span class="param-type">string</span></td>
<td class="description last">Sunburst datalabel data</td>
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
<td class="description last">Instance of the sunburst model object</td>
</tr>
<tr>
<td class="name">{% highlight js %}
type{% endhighlight %}</td>
<td class="type"><span class="param-type">string</span></td>
<td class="description last">Name of the event</td>
</tr>
</tbody>
</table>


### segmentRendering
{:#events:segmentrendering}


Fires before rendering each segment


#### Example


{% highlight js %}
 
//segmentRendering event for sunburst

$("#container").ejSunburstChart({

    segmentRendering: function (args) {
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
<td class="type"><span class="param-type">string</span></td>
<td class="description last">Sunburst datalabel data</td>
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
<td class="description last">Instance of the sunburst model object</td>
</tr>
<tr>
<td class="name">{% highlight js %}
type{% endhighlight %}</td>
<td class="type"><span class="param-type">string</span></td>
<td class="description last">Name of the event</td>
</tr>
</tbody>
</table>


### titleRendering
{:#events:titlerendering}




Fires before rendering sunburst title. 


#### Example


{% highlight js %}
 
//titleRendering event for sunburst

$("#container").ejSunburstChart({

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
data{% endhighlight %}</td>
<td class="type"><span class="param-type">string</span></td>
<td class="description last">Sunburst title data</td>
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
<td class="description last">Instance of the sunburst model object</td>
</tr>
<tr>
<td class="name">{% highlight js %}
type{% endhighlight %}</td>
<td class="type"><span class="param-type">string</span></td>
<td class="description last">Name of the event</td>
</tr>
</tbody>
</table>

### tooltipInitialize
{:#events:tooltipinitialize}




Fires during initialization of tooltip. 


#### Example


{% highlight js %}
 
//tooltipInitialize event for sunburst

$("#container").ejSunburstChart({

    tooltipInitialize: function (args) {
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
<td class="type"><span class="param-type">string</span></td>
<td class="description last">Sunburst tooltip data</td>
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
<td class="description last">Instance of the sunburst model object</td>
</tr>
<tr>
<td class="name">{% highlight js %}
type{% endhighlight %}</td>
<td class="type"><span class="param-type">string</span></td>
<td class="description last">Name of the event</td>
</tr>
</tbody>
</table>

### pointRegionClick
{:#events:pointregionclick}




Fires after clicking the point in sunburst


#### Example


{% highlight js %}
 
//pointRegionClick event for sunburst

$("#container").ejSunburstChart({

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
data{% endhighlight %}</td>
<td class="type"><span class="param-type">string</span></td>
<td class="description last">Includes clicked points region data</td>
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
<td class="description last">Instance of the sunburst model object</td>
</tr>
<tr>
<td class="name">{% highlight js %}
type{% endhighlight %}</td>
<td class="type"><span class="param-type">string</span></td>
<td class="description last">Name of the event</td>
</tr>
</tbody>
</table>

### pointRegionMouseMove
{:#events:pointregionmousemove}




Fires while moving the mouse over sunburst points

#### Example


{% highlight js %}
 
//pointRegionMouseMove event for sunburst

$("#container").ejSunburstChart({

    pointRegionMouseMove: function (args) {
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
<td class="type"><span class="param-type">string</span></td>
<td class="description last">Includes data of mouse moved region</td>
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
<td class="description last">Instance of the sunburst model object</td>
</tr>
<tr>
<td class="name">{% highlight js %}
type{% endhighlight %}</td>
<td class="type"><span class="param-type">string</span></td>
<td class="description last">Name of the event</td>
</tr>
</tbody>
</table>

### drillDownClick
{:#events:drilldownclick}




Fires when clicking the point to perform drilldown. 


#### Example


{% highlight js %}
 
//drillDownClick event for sunburst

$("#container").ejSunburstChart({

    drillDownClick: function (args) {
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
<td class="type"><span class="param-type">string</span></td>
<td class="description last">Clicked point data</td>
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
<td class="description last">Instance of the sunburst model object</td>
</tr>
<tr>
<td class="name">{% highlight js %}
type{% endhighlight %}</td>
<td class="type"><span class="param-type">string</span></td>
<td class="description last">Name of the event</td>
</tr>
</tbody>
</table>

### drillDownBack
{:#events:drilldownback}




Fires when resetting drilldown points. 


#### Example


{% highlight js %}
 
//drillDownBack event for sunburst

$("#container").ejSunburstChart({

    drillDownBack: function (args) {
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
<td class="type"><span class="param-type">string</span></td>
<td class="description last">Drill down data of points</td>
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
<td class="description last">Instance of the sunburst model object</td>
</tr>
<tr>
<td class="name">{% highlight js %}
type{% endhighlight %}</td>
<td class="type"><span class="param-type">string</span></td>
<td class="description last">Name of the event</td>
</tr>
</tbody>
</table>


### drillDownReset
{:#events:drilldownreset}




Fires after resetting the sunburst points 


#### Example


{% highlight js %}
 
//drillDownReset event for sunburst

$("#container").ejSunburstChart({

    drillDownReset: function (args) {
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
<td class="type"><span class="param-type">string</span></td>
<td class="description last">Drill down reset data</td>
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
<td class="description last">Instance of the sunburst model object</td>
</tr>
<tr>
<td class="name">{% highlight js %}
type{% endhighlight %}</td>
<td class="type"><span class="param-type">string</span></td>
<td class="description last">Name of the event</td>
</tr>
</tbody>
</table>

### Click
{:#events:click}




Fires, on clicking the sunburst chart.


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
<td class="type"><span class="param-type">string</span></td>
<td class="description last">Includes clicked region data</td>
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
<td class="description last">Instance of the sunburst model object</td>
</tr>
<tr>
<td class="name">{% highlight js %}
type{% endhighlight %}</td>
<td class="type"><span class="param-type">string</span></td>
<td class="description last">Name of the event</td>
</tr>
</tbody>
</table>

#### Example


{% highlight js %}
 
//Click event for sunburst chart

 $("#container").ejSunburstChart({


    click: function (args) {
              //Do something
    }
   
});

{% endhighlight %}


### doubleClick
{:#events:doubleclick}




Fires, on double clicking the sunburst chart.


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
<td class="type"><span class="param-type">string</span></td>
<td class="description last">Includes double clicked region data</td>
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
<td class="description last">Instance of the sunburst model object</td>
</tr>
<tr>
<td class="name">{% highlight js %}
type{% endhighlight %}</td>
<td class="type"><span class="param-type">string</span></td>
<td class="description last">Name of the event</td>
</tr>
</tbody>
</table>

#### Example


{% highlight js %}
 
//DoubleClick event for sunburst chart

 $("#container").ejSunburstChart({


    doubleClick: function (args) {
              //Do something
    }
   
});

{% endhighlight %}



### rightClick
{:#events:rightclick}




Fires, on right clicking the sunburst chart


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
<td class="type"><span class="param-type">string</span></td>
<td class="description last">Includes right clicked region data</td>
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
<td class="description last">Instance of the sunburst model object</td>
</tr>
<tr>
<td class="name">{% highlight js %}
type{% endhighlight %}</td>
<td class="type"><span class="param-type">string</span></td>
<td class="description last">Name of the event</td>
</tr>
</tbody>
</table>

#### Example


{% highlight js %}
 
//RightClick event for sunburst chart

 $("#container").ejSunburstChart({

    rightClick: function (args) {
              //Do something
    }
   
});

{% endhighlight %}