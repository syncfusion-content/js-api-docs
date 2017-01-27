---
layout: post
title: API reference for ejSunburst
description: What are the options, methods and events available in Essential JavaScript Sunburst.
documentation: API
platform: js-api
keywords: ejSunburst, API, Essential JS Sunburst, Sunburst
metaname: 
metacontent: 
---

# ejSunburst
<ts root="datavisualization" />

Essential Sunburst can be easily configured to the DOM element, such as div. You can create a Sunburst with highly customizable look and feel.

#### Syntax

{% highlight js %}

$(element).ejSunburst();

{% endhighlight %}

#### Example

{% highlight html %}
 
<div id="container"></div> 
 
<script>
// Create Sunburst
$('#container').ejSunburst();      
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
 
$("#container").ejSunburst({

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

$("#container").ejSunburst({

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
                             
$("#container").ejSunburst({

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
 
$("#container").ejSunburst({

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
                             
$("#container").ejSunburst({

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
 
$("#container").ejSunburst({

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
 
$("#container").ejSunburst({
    
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
 
$("#container").ejSunburst({
    palette : "ColorFieldName"                  
});
{% endhighlight %}

### parentNode `string`
{:#members:parentNode}

Parent node of the data points.

#### Default Value

 * null

#### Example

{% highlight js %}

$("#container").ejSunburst({
    
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

$("#container").ejSunburst({
    
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

$("#container").ejSunburst({
    
    yName: "YValue"
                       
});

{% endhighlight %}


### isResponsive `boolean`
{:#members:isresponsive}

Controls wheather sunburst has to be responsive or not.

#### Default Value

* true


#### Example

{% highlight js %}
 
$("#container").ejSunburst({

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
 
$("#container").ejSunburst({

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
 
$("#container").ejSunburst({

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
 
$("#container").ejSunburst({

   visible : true             

});

{% endhighlight %}



### tooltip `object`
{:#members:tooltip}

Options to customize the Sunburst tooltip.





### tooltip.visible `boolean`
{:#members:tooltip-visible}

Tooltip visibility of the Sunburst.

#### Default Value

* true

#### Example

{% highlight js %}
 
$("#container").ejSunburst({

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
 
$("#container").ejSunburst({
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

$("#container").ejSunburst({
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
 
$("#container").ejSunburst({
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
  
$("#container").ejSunburst({
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

$("#container").ejSunburst({
tooltip :{ font : { fontFamily : "Algerian"}}                 
});
 {% endhighlight %}
 
 
### tooltip.font.fontStyle `enum`
{:#members:tooltip-font-fontstyle}

<ts name = "ej.datavisualization.Sunburst.FontStyle"/>

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
 

$("#container").ejSunburst({
tooltip : {font :{fontStyle : "italic"}}                 
});
{% endhighlight %}


### tooltip.font.fontWeight `enum`
{:#members:tooltip-font-fontweight}


<ts name = "ej.datavisualization.Sunburst.FontWeight"/>


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
 

$("#container").ejSunburst({
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
 

$("#container").ejSunburst({
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
 
 
$("#container").ejSunburst({
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

$("#container").ejSunburst({
    tooltip :{template : "item"}                  
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
                             
$("#container").ejSunburst({

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
                             
$("#container").ejSunburst({

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
                             
$("#container").ejSunburst({

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
                             
$("#container").ejSunburst({

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
 
$("#container").ejSunburst({

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
 
$("#container").ejSunburst({

    endAngle : 360             

});

{% endhighlight %}

### sunburstCoefficient `number`
{:#members:sunburstCoefficient}

Sunburst outer radius value

#### Default Value

* 1

#### Example

{% highlight js %}
 
$("#container").ejSunburst({

    sunburstCoefficient : 0.8             

});

{% endhighlight %}

### sunburstHoleCoefficient `number`
{:#members:sunburstHoleCoefficient}

Sunburst inner radius value

#### Default Value

* 0.4

#### Example

{% highlight js %}
 
$("#container").ejSunburst({

    sunburstHoleCoefficient : 0.2            

});

{% endhighlight %}



### dataLabel `object`
{:#members:dataLabel}

Options to customize the Sunburst dataLabel.



### dataLabel.visible `boolean`
{:#members:dataLabel-visible}

Datalabel visibility of the Sunburst.

#### Default Value

* false

#### Example

{% highlight js %}
 
$("#container").ejSunburst({

   dataLabel :{visible : true}          

});

{% endhighlight %}


### dataLabel.labelRotationMode `enum`
{:#members:dataLabel-labelRotationMode}

<ts name = "ej.datavisualization.Sunburst.dataLabelAlignment"/>

Alginment of sunburst datalabel


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

* "Angle". See <a href="global.html#members:DataLabelAlignment">DatalabelAlignment</a>


#### Example

{% highlight js %}
 
$("#container").ejSunburst({

   dataLabel :{labelRotationMode : "normal"}                    

});

{% endhighlight %}


### dataLabel.font `object`
{:#members:datalabel-font}


Options for customizing the data label font.


### dataLabel.font.fontFamily `string`
{:#members:datalabel-font-fontfamily}


Font family of the data label. 

#### Default Value


* "Segoe UI"


#### Example


{% highlight js %}
 
 
$("#container").ejSunburst({
    dataLabel :{ font :{fontFamily : "algerian"}}                 
});
{% endhighlight %}




### dataLabel.font.fontStyle `enum`
{:#members:datalabel-font-fontstyle}

<ts ref="ej.datavisualization.Sunburst.FontStyle"/>


Font style of the data label.   


#### Default Value


* "normal". See <a href="global.html#fontstyle">FontStyle</a>


#### Example


{% highlight js %}
 
 
$("#container").ejSunburst({
    dataLabel :{font :{ fontStyle : "italic" }}                 
});
 {% endhighlight %}



### dataLabel.font.fontWeight `enum`
{:#members:datalabel-font-fontweight}


<ts ref="ej.datavisualization.Sunburst.FontWeight"/>


Font weight of the data label.  


#### Default Value


* "regular". See <a href="global.html#members:fontweight">FontWeight</a>


#### Example


{% highlight js %}
 
 
$("#container").ejSunburst({
    dataLabel :{font : { fontWeight : "lighter" }}                 
});
{% endhighlight %}



### dataLabel.font.opacity `number`
{:#members:datalabel-font-opacity}


Opacity of the text. 


#### Default Value


 * 1


#### Example


{% highlight js %}
 
 
$("#container").ejSunburst({
    dataLabel :{font :{ opacity : 0.5 }}               
});
{% endhighlight %}

### dataLabel.font.color `string`
{:#members:datalabel-font-color}

Font color of the data label text. 

#### Default Value

 * null

#### Example

{% highlight js %}

 
$("#container").ejSunburst({
    dataLabel :{font :{ color : "red" }}                 
});
{% endhighlight %}


### dataLabel.font.size `string`
{:#members:datalabel-font-size}


Font size of the data label. 


#### Default Value


* "12px"


#### Example


{% highlight js %}
 

$("#container").ejSunburst({
    dataLabel :{font : { size : "14px" }}               
});
{% endhighlight %}



### dataLabel.template `string`
{:#members:datalabel-template}

Custome template for datalabel 


#### Default Value


* "null"


#### Example


{% highlight js %}
 

$("#container").ejSunburst({
    dataLabel :{ template: "item" }               
});
{% endhighlight %}


### dataLabel.fill `string`
{:#members:datalabel-fill}

Fill color for the datalable


#### Default Value


* null


#### Example


{% highlight js %}
 

$("#container").ejSunburst({
    dataLabel :{ fill: "yellow" }               
});
{% endhighlight %}



### dataLabel.labelOverflowMode `enum`
{:#members:dataLabel-labelOverflowMode}

<ts name = "ej.datavisualization.Sunburst.LabelOverflowMode"/>

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
<td class="description"> Datalable displayed in normal format</td>
</tr>
</tbody>
</table>

#### Default Value

* "Trim". See <a href="global.html#members:LabelOverflowMode">LabelOverflowMode</a>


#### Example

{% highlight js %}
 
$("#container").ejSunburst({

   dataLabel :{labelOverflowMode : "hide"}                    

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
 
$("#container").ejSunburst({

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
 
$("#container").ejSunburst({

   title : { visible: false }                     

});

{% endhighlight %}



### title.textAlignment `enum`
{:#members:title-textAlignment}

<ts name = "ej.datavisualization.Sunburst.TextAlignment"/>

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

* "center". See <a href="global.html#members:TextAlignment">TextAlignment</a>


#### Example

{% highlight js %}
 
$("#container").ejSunburst({

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
 
$("#container").ejSunburst({

   title : { font : { fontFamily : "Algerian" } }                     

});

{% endhighlight %}



### title.font.fontStyle `enum`
{:#members:title-font-fontstyle}

<ts ref="ej.datavisualization.Sunburst.FontStyle"/>


Font style for Sunburst title.


#### Default Value

* "Normal". See <a href="global.html#members:fontstyle">FontStyle</a>


#### Example


{% highlight js %}
 
$("#container").ejSunburst({

   title : { font : { fontStyle : "italic" } }                     

});

{% endhighlight %}



### title.font.fontWeight `enum`
{:#members:title-font-fontweight}


<ts ref="ej.datavisualization.Sunburst.FontWeight"/>

Font weight for Sunburst title.


#### Default Value

* "Regular". See <a href="global.html#members:fontweight">FontWeight</a>


#### Example


{% highlight js %}
 
$("#container").ejSunburst({

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
 
$("#container").ejSunburst({

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
 
$("#container").ejSunburst({

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
 
$("#container").ejSunburst({

   title : { subtitle :{text: "Sunburst Subtitle" }}                 

});

{% endhighlight %}




### title.subtitle.visible `string`
{:#members:title-subtitle-visible}


SubTitle text visibility for sunburst


#### Default Value

* true


#### Example


{% highlight js %}
 
$("#container").ejSunburst({

   title : {subtitle:{visible: false }}                     

});

{% endhighlight %}



### title.subtitle.textAlignment `enum`
{:#members:title-subtitle-textAlignment}

<ts ref="ej.datavisualization.Sunburst.TextAlignment"/>

SubTitle text alignment

#### Default Value

* "far". See <a href="global.html#members:textalignment">TextAlignment</a>


#### Example

{% highlight js %}
 
$("#container").ejSunburst({

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
 
$("#container").ejSunburst({

   title: {subtitle : {font :{ fontFamily : "Algerian" } } }                      

});

{% endhighlight %}




### title.subtitle.font.fontStyle `enum`
{:#members:title-subtitle-font-fontstyle}

<ts ref="ej.datavisualization.Sunburst.FontStyle"/>


Font style for sub title.


#### Default Value

* "Normal". See <a href="global.html#members:fontstyle">FontStyle</a>


#### Example


{% highlight js %}
 
$("#container").ejSunburst({

   title: { subtitle : {font :{ fontStyle : "Normal" } } }                     

});

{% endhighlight %}



### title.subtitle.font.fontWeight `enum` 
{:#members:title-subtitle-font-fontweight}

<ts ref="ej.datavisualization.Sunburst.FontWeight"/>


Font weight for sub title.


#### Default Value

* "Regular". See <a href="global.html#members:fontweight">FontWeight</a>



#### Example


{% highlight js %}
 
$("#container").ejSunburst({

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
 
$("#container").ejSunburst({

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
 
$("#container").ejSunburst({

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
 
 
$("#container").ejSunburst({
    highlightSettings:{enable:true}                 
});
{% endhighlight %}



### highlightSettings.mode `enum`
{:#members:highlightSettings-mode}


<ts name = "ej.datavisualization.Sunburst.Mode"/>


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


* "point". See <a href="global.html#members:mode">Mode</a>


#### Example


{% highlight js %}
 
 
$("#container").ejSunburst({
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
 
 
$("#container").ejSunburst({
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
 
 
$("#container").ejSunburst({
    highlightSettings:{opacity:1}            
});
{% endhighlight %}


### highlightSettings.type `enum`
{:#members:highlightSettings-type}


<ts name = "ej.datavisualization.Sunburst.Type"/>


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


* "opacity". See <a href="global.html#members:type">Mode</a>


#### Example


{% highlight js %}
 
 
$("#container").ejSunburst({
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
 
 
$("#container").ejSunburst({
    selectionSettings:{enable:true}                 
});
{% endhighlight %}



### selectionSettings.mode `enum`
{:#members:selectionSettings-mode}


<ts ref = "ej.datavisualization.Sunburst.Mode"/>


Specifies whether the levels or data point has to be selected.



#### Default Value


* "point". See <a href="global.html#members:mode">Mode</a>


#### Example


{% highlight js %}
 
 
$("#container").ejSunburst({
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
 
 
$("#container").ejSunburst({
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
 
 
$("#container").ejSunburst({
    selectionSettings:{opacity:1}            
});
{% endhighlight %}


### selectionSettings.type `enum`
{:#members:selectionSettings-type}


<ts ref = "ej.datavisualization.Sunburst.Type"/>


Specifies whether the levels or data point has to be selected.




#### Default Value


* "opacity". See <a href="global.html#members:type">Mode</a>


#### Example


{% highlight js %}
 
 
$("#container").ejSunburst({
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

  $("#container").ejSunburst({   
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
 
$("#container").ejSunburst({

   legend : {visible:true}}                     

});

{% endhighlight %}

### legend.mouseInteractiveAction `enum`
{:#members:legend-mouseinteractiveaction}

<ts name = "ej.datavisualization.Sunburst.LegendAction"/>


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

* "toggleSegmentVisibility". See <a href="global.html#members:togglevisibility">Alignment</a>


#### Example


{% highlight js %}
 
$("#container").ejSunburst({

   legend :{mouseInteractiveAction : "toggleSegmentSelection"}                    

});

{% endhighlight %}



### legend.alignment `enum`
{:#members:legend-alignment}

<ts name = "ej.datavisualization.Sunburst.Alignment"/>


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

* "Center". See <a href="global.html#members:alignment">Alignment</a>


#### Example


{% highlight js %}
 
$("#container").ejSunburst({

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
 
$("#container").ejSunburst({

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
 
$("#container").ejSunburst({

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
 
$("#container").ejSunburst({

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
 
$("#container").ejSunburst({

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
 
$("#container").ejSunburst({

   legend :{ font :{fontFamily : "algerian"}}                    

});

{% endhighlight %}



### legend.font.fontStyle `enum`
{:#members:legend-font-fontstyle}

<ts ref="ej.datavisualization.Sunburst.FontStyle"/>


Font style for legend item text.


#### Default Value

* "Normal". See <a href="global.html#members:fontstyle">FontStyle</a>


#### Example


{% highlight js %}
 
$("#container").ejSunburst({

   legend :{ font :{fontStyle : "italic"}}                    

});

{% endhighlight %}



### legend.font.fontWeight `enum`
{:#members:legend-font-fontweight}

<ts ref="ej.datavisualization.Sunburst.FontWeight"/>


Font weight for legend item text.


#### Default Value

* "Regular". See <a href="global.html#members:fontweight">FontWeight</a>



#### Example


{% highlight js %}
 
$("#container").ejSunburst({

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
 
$("#container").ejSunburst({

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
 
$("#container").ejSunburst({

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
 
$("#container").ejSunburst({

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
 
$("#container").ejSunburst({

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
 
$("#container").ejSunburst({

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
 
$("#container").ejSunburst({

   legend :{location : {y : 100}}                  

});

{% endhighlight %}


### legend.position `enum`
{:#members:legend-position}

<ts name = "ej.datavisualization.Sunburst.Position"/>

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

* "Bottom". See <a href="global.html#members:position">Position</a>


#### Example


{% highlight js %}
 
$("#container").ejSunburst({

   legend :{ position : "top"}                    

});

{% endhighlight %}







### legend.shape `enum`
{:#members:legend-shape}

<ts name = "ej.datavisualization.Sunburst.Shape"/>



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

* "None". See <a href="global.html#members:shape">Shape</a>



#### Example


{% highlight js %}
 
$("#container").ejSunburst({

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
 
$("#container").ejSunburst({

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
 
$("#container").ejSunburst({

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
 
$("#container").ejSunburst({

   legend: { title: { font :{fontFamily: "Algerian" } } }                      

});

{% endhighlight %}




### legend.title.font.fontStyle `enum`
{:#members:legend-title-font-fontstyle}

<ts ref="ej.datavisualization.Sunburst.FontStyle"/>


Font style for legend title.


#### Default Value

* "normal". See <a href="global.html#members:fontstyle">FontStyle</a>




#### Example


{% highlight js %}
 
$("#container").ejSunburst({

   legend: { title: { font :{fontStyle: "normal" } } }                      

});

{% endhighlight %}




### legend.title.font.fontWeight `enum`
{:#members:legend-title-font-fontweight}

<ts ref="ej.datavisualization.Sunburst.FontWeight"/>


Font weight for legend title.


#### Default Value

* "normal". See <a href="global.html#members:fontweight">FontWeight</a>




#### Example


{% highlight js %}
 
$("#container").ejSunburst({

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
 
$("#container").ejSunburst({

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
 
$("#container").ejSunburst({

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
 
$("#container").ejSunburst({

   legend: { title: { text : "Countries" } }                      

});

{% endhighlight %}







### legend.title.textAlignment `enum`
{:#members:legend-title-textalignment}

<ts name = "ej.datavisualization.Sunburst.Alignment"/>

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

* "center". See <a href="global.html#members:alignment">Alignment</a>




#### Example


{% highlight js %}
 
$("#container").ejSunburst({

   legend: { title: { textAlignment : "near" } }                      

});

{% endhighlight %}





### theme `enum`
{:#members:theme}

<ts name = "ej.datavisualization.Sunburst.Theme"/>

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

* "Flatlight". See <a href="global.html#members:theme">Theme</a>


#### Example


{% highlight js %}
 
$("#container").ejSunburst({

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
 
$("#container").ejSunburst({

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
 
$("#container").ejSunburst({

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
 
$("#container").ejSunburst({

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
 
$("#container").ejSunburst({

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
 
 
$("#container").ejSunburst({
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
 
 
$("#container").ejSunburst({
    opacity : 0.5              
});
 {% endhighlight %}


### zooming `object`
{:#members:zooming}


Options for enabling zooming feature of chart.



### zooming.enable `boolean`
{:#members:zooming}


Enables or disables zooming.


#### Default Value

* false




#### Example


{% highlight js %}
 
$("#container").ejSunburst({

   zooming :{enable :true}          

});

{% endhighlight %}

### zooming.toolbarHorizontalAlignment `enum`
{:#members:zooming-toolbarhorizontalalignment}

<ts name = "ej.datavisualization.Sunburst.HorizontalAlignment"/>

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

* "right". See <a href="global.html#members:alignment">Alignment</a>




#### Example


{% highlight js %}
 
$("#container").ejSunburst({

   zooming: { toolbarHorizontalAlignment: "center" }                      

});

{% endhighlight %}

### zooming.toolbarVerticalAlignment `enum`
{:#members:zooming-toolbarverticalalignment}

<ts name = "ej.datavisualization.Sunburst.VerticalAlignment"/>

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

* "top". See <a href="global.html#members:alignment">Alignment</a>




#### Example


{% highlight js %}
 
$("#container").ejSunburst({

   zooming: { toolbarVerticalAlignment: "middle" }                      

});

{% endhighlight %}


### animationType `enum`
{:#members:animationtype}

<ts name = "ej.datavisualization.Sunburst.Animation"/>

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
<td class="description">Animates points in fadein</td>
</tr> 
</tbody>
</table>



#### Default Value

* "rotation". See <a href="global.html#members:animation">Alignment</a>




#### Example


{% highlight js %}
 
$("#container").ejSunburst({

   animationType:"fadeIn"                     

});

{% endhighlight %}





### load
{:#events:load}

Fires before loading.


#### Example


{% highlight js %}
 
//load event for sunburst

$("#container").ejSunburst({

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

$("#container").ejSunburst({

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

$("#container").ejSunburst({

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
 
//datalabelrendering event for sunburst

$("#container").ejSunburst({

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


### titleRendering
{:#events:titlerendering}




Fires before rendering sunburst title. 


#### Example


{% highlight js %}
 
//titlerendering event for sunburst

$("#container").ejSunburst({

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

### toolTipInitialize
{:#events:tooltipinitialize}




Fires during initialization of tooltip. 


#### Example


{% highlight js %}
 
//tooltipinitialize event for sunburst

$("#container").ejSunburst({

    toolTipInitialize: function (args) {
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
 
//pointregionclick event for sunburst

$("#container").ejSunburst({

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

### pointRegionMousemove
{:#events:pointregionmousemove}




Fires while moving the mouse over sunburst points

#### Example


{% highlight js %}
 
//pointregionmousemove event for sunburst

$("#container").ejSunburst({

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
 
//drilldownclick event for sunburst

$("#container").ejSunburst({

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
 
//drilldownback event for sunburst

$("#container").ejSunburst({

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
 
//drilldownreset event for sunburst

$("#container").ejSunburst({

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