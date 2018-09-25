---
layout: post
title: Properties, Methods and Events of ejMap Widget
description: API reference for ejMap
documentation: API
platform: js-api
keywords: map, ejmap, map api, syncfusion
---

# ejMap
<ts root="datavisualization" />

The map can be easily configured to the DOM element, such as div and can be created with a highly customized look and feel.

#### Syntax

{% highlight js %}

$(element).ejMap();

{% endhighlight %}


#### Example

{% highlight html %}
 
<div id="container"> 
 
<script>
// Create Map
$('#container').ejMap();        
</script> 
  
</div>

{% endhighlight %}


#### Requires

* module:jQuery.js

* module:ej.core.js

* module:ej.data.js

* module:ej.map.js

* module:jsrender.js

* module:properties.js


## Members

### background `string`
{:#members:background}

Specifies the background color for map

#### Default Value

* "transparent"

#### Example

{% highlight js %}
 
//To set background API value during initialization 
  $("#container").ejMap({background:'transparent'});
  
{% endhighlight %}


{% highlight js %}
 
//Get or set the background API, after initialization:

  //Gets the background value
   
  var property = $("#container").data("ejMap").model.background;
  
  //Sets the background value 
  
  $("#container").data("ejMap").model.background="transparent";

{% endhighlight %}


### baseMapIndex `number`
{:#members:basemapindex}

Specifies the index of the map to determine the shape layer to be displayed

#### Default Value

* 0

#### Example

{% highlight js %}
 
//To set baseMapIndex API value during initialization 
  $("#container").ejMap({baseMapIndex:0});

{% endhighlight %}


{% highlight js %}
 
//Get or set the baseMapIndex API, after initialization:

   //Gets the baseMapIndex value 
   
   var property = $("#container").data("ejMap").model.baseMapIndex;
   
   //Sets the baseMapIndex value 
   
   $("#container").data("ejMap").model.baseMapIndex= 0;
   
{% endhighlight %}


### centerPosition `object`
{:#members:centerposition}

Specify the center position where map should be displayed

#### Default Value

* [0,0]

#### Example

{% highlight js %}
  
// Set the centerPosition during initialization.                        
   $("#container").ejMap({centerPosition: [38.5000, -98]});

{% endhighlight %}


{% highlight js %}
 
//Get or set the centerPosition after initialization:

  //Gets the centerPosition from map.
  
  var property =$("#container").data("ejMap").model.centerPosition;
  
  //Sets the centerPosition to map.
  
  $("#container").data("ejMap").model.centerPosition = [38.5000, -98];

{% endhighlight %}

### draggingOnSelection `boolean`
{:#members:draggingonselection}

Controls the selection through dragging

#### Default Value

* false

#### Example

{% highlight js %}
 
//To set draggingOnSelection API value during initialization 
   $("#container").ejMap({draggingOnSelection:true});  

{% endhighlight %}


{% highlight js %}
 
//Get or set the draggingOnSelection API, after initialization:
   
   //Gets the draggingOnSelection value 
   
   var property = $("#container").data("ejMap").model.draggingOnSelection;
         
   //Sets the draggingOnSelection value
    
   $("#container").data("ejMap").model.draggingOnSelection=true }); 

{% endhighlight %}


### enableAnimation `boolean`
{:#members:enableanimation}

Enables or Disables the map animation

#### Default Value

* false

#### Example

{% highlight js %}
 
//To set enableAnimation API value during initialization 
   $("#container").ejMap({enableAnimation:true});  

{% endhighlight %}


{% highlight js %}
 
//Get or set the enableAnimation API, after initialization:
   
   //Gets the enableAnimation value 
   
   var property = $("#container").data("ejMap").model.enableAnimation;
         
   //Sets the enableAnimation value
    
   $("#container").data("ejMap").model.enableAnimation=true }); 

{% endhighlight %}


### enableRTL `boolean`
{:#members:enablertl}

Enables or Disables right to left(RTL) support for maps.

#### Default Value

* false

#### Example

{% highlight js %}

//To set enableRTL API value during initialization
   $("#container").ejMap({enableRTL:false});

{% endhighlight %}


{% highlight js %}

//Get or set the enableRTL API, after initialization:

   //Gets the enableRTL value 

   var property = $("#container").data("ejMap").model.enableRTL;

   //Sets the enableRTL value

   $("#container").data("ejMap").model.enableRTL=true });

{% endhighlight %}


### enableLayerChangeAnimation `boolean`
{:#members:enablelayerchangeanimation}

Enables or Disables the animation for layer change in map

#### Default Value

* false

#### Example


{% highlight js %}
 
//To set enableLayerChangeAnimation API value during initialization 
   $("#container").ejMap({enableLayerChangeAnimation:true});       

{% endhighlight %}


{% highlight js %}
 
//Get or set the enableLayerChangeAnimation API, after initialization:

   //Gets the enableLayerChangeAnimation value 
   
   var property = $("#container").data("ejMap").model.enableLayerChangeAnimation;
              
   //Sets the enableLayerChangeAnimation value
    
   $("#container").data("ejMap").model.enableLayerChangeAnimation=false }); 

{% endhighlight %}


### enablePan `boolean`
{:#members:enablepan}

Enables or Disables the map panning

#### Default Value

* true

#### Example

{% highlight js %}
 
//To set enablePan API value during initialization 
   $("#container").ejMap({enablePan:true});        

{% endhighlight %}


{% highlight js %}
 
//Get or set the enablePan API, after initialization:
 
   //Gets the enablePan value 
   
   var property = $("#container").data("ejMap").model.enablePan;
               
   //Sets the enablePan value
    
   $("#container").data("ejMap").model.enablePan=true });

{% endhighlight %}


### enableResize `boolean`
{:#members:enableresize}

Determines whether map need to resize when container is resized

#### Default Value

* true

#### Example

{% highlight js %}
 
//To set enableResize API value during initialization 
   $("#container").ejMap({enableResize:true});     

{% endhighlight %}


{% highlight js %}
 
//Get or set the enableResize API, after initialization:
   
   //Gets the enableResize value 
   
   var property = $("#container").data("ejMap").model.enableResize;
            
   //Sets the enableResize value 
   
   $("#container").data("ejMap").model.enableResize= true }); 
{% endhighlight %}



### isResponsive `boolean`
{:#members:isresponsive}

Determines whether map need to resize when container is resized

#### Default Value

* true

#### Example

{% highlight js %}
 
//To set isResponsive API value during initialization 
   $("#container").ejMap({isResponsive:true});     

{% endhighlight %}


{% highlight js %}
 
//Get or set the isResponsive API, after initialization:
   
   //Gets the isResponsive value 
   
   var property = $("#container").data("ejMap").model.isResponsive;
            
   //Sets the isResponsive value 
   
   $("#container").data("ejMap").model.isResponsive= true }); 
{% endhighlight %}



### zoomSettings `object`
{:#members:zoomsettings}

Enables or Disables the Zooming for map.

### zoomSettings.animationDuration `string`
{:#members:zoomsettings-animationduration}

Specifies animation duration for map shapes while zooming.

#### Default Value

* 600

#### Example

{% highlight js %}
 
//To set animationDuration API value during initialization 
   $("#container").ejMap({zoomSettings:{animationDuration:1000}});           

{% endhighlight %}


{% highlight js %}
 
//Get or set the animationDuration API, after initialization:

   //Gets the animationDuration value 
   
   var property = $("#container").data("ejMap").model.zoomSettings.animationDuration;
         
   //Sets the animationDuration value
    
   $("#container").data("ejMap").model.zoomSettings.animationDuration=true }); 

{% endhighlight %}

### zoomSettings.enableZoom `boolean`
{:#members:zoomsettings-enablezoom}

Enables or Disables the zooming of map

#### Default Value

* true

#### Example

{% highlight js %}
 
//To set enableZoom API value during initialization 
   $("#container").ejMap({zoomSettings:{enableZoom:true}});           

{% endhighlight %}


{% highlight js %}
 
//Get or set the enableZoom API, after initialization:

   //Gets the enableZoom value 
   
   var property = $("#container").data("ejMap").model.zoomSettings.enableZoom;
         
   //Sets the enableZoom value
    
   $("#container").data("ejMap").model.zoomSettings.enableZoom=true }); 

{% endhighlight %}


### zoomSettings.enableZoomOnSelection `boolean`
{:#members:zoomsettings-enablezoomonselection}

Enables or Disables the zoom on selecting the map shape

#### Default Value

* false

#### Example

{% highlight js %}
 
//To set enableZoomOnSelection API value during initialization 
   $("#container").ejMap({zoomSettings:{enableZoomOnSelection:true}});
             
{% endhighlight %}


{% highlight js %}
 
//Get or set the enableZoomOnSelection API, after initialization:

   //Gets the enableZoomOnSelection value
    
   var property = $("#container").data("ejMap").model.zoomSettings.enableZoomOnSelection;
              
   //Sets the enableZoomOnSelection value
    
   $("#container").data("ejMap").model.zoomSettings.enableZoomOnSelection=true }); 

{% endhighlight %}

### zoomSettings.enableMouseWheelZoom `boolean`
{:#members:zoomsettings-enablemousewheelzoom}

Enables or Disables the zoom on mouse wheel the map.

#### Default Value

* true

#### Example

{% highlight js %}
 
//To set enableMouseWheelZoom API value during initialization 
   $("#container").ejMap({zoomSettings:{enableMouseWheelZoom:true}});
             
{% endhighlight %}


{% highlight js %}
 
//Get or set the enableMouseWheelZoom API, after initialization:

   //Gets the enableMouseWheelZoom value
    
   var property = $("#container").data("ejMap").model.zoomSettings.enableMouseWheelZoom;
              
   //Sets the enableMouseWheelZoom value
    
   $("#container").data("ejMap").model.zoomSettings.enableMouseWheelZoom=true }); 

{% endhighlight %}


### zoomSettings.factor `number`
{:#members:zoomsettings-factor}

Specifies the zoom factor for map zoom value.

#### Default Value

* 1

#### Example

{% highlight js %}
 
//To set zoomFactor API value during initialization 
  $("#container").ejMap({zoomSettings:{factor:1}});
  
{% endhighlight %}


{% highlight js %}
 
//Get or set the zoomFactor API, after initialization:
   
   //Gets the zoomFactor value 
   
   var property = $("#container").data("ejMap").model.zoomSettings.factor;
   
   //Sets the zoomFactor value
    
   $("#container").data("ejMap").model.zoomSettings.factor= 1;

{% endhighlight %}


### zoomSettings.level `number`
{:#members:zoomsettings-level}

Specifies the zoom level value for which map to be zoomed

#### Default Value

* 1

#### Example

{% highlight js %}
 
//To set zoomLevel API value during initialization 
  $("#container").ejMap({zoomSettings:{level:1}});

{% endhighlight %}


{% highlight js %}
 
//Get or set the zoomLevel API, after initialization:
   //Gets the zoomLevel value
    
   var property = $("#container").data("ejMap").model.zoomSettings.level;
   
   //Sets the zoomLevel value
    
   $("#container").data("ejMap").model.zoomSettings.level= 1;

{% endhighlight %}


### zoomSettings.minValue `number`
{:#members:zoomsettings-minvalue}

Specifies the minimum zoomSettings level of the map

#### Default Value

* 1

#### Example

{% highlight js %}
 
//To set minValue API value during initialization 
  $("#container").ejMap({zoomSettings:{minValue:1}});

{% endhighlight %}


{% highlight js %}
 
//Get or set the minValue API, after initialization:
   
   //Gets the minValue value 
   
   var property = $("#container").data("ejMap").model.zoomSettings.minValue;
   
   //Sets the minValue value
    
   $("#container").data("ejMap").model.zoomSettings.minValue= 1;

{% endhighlight %}


### zoomSettings.maxValue `number`
{:#members:zoomsettings-maxvalue}

Specifies the maximum zoom level of the map

#### Default Value

* 100

#### Example

{% highlight js %}
 
//To set maxValue API value during initialization 
  $("#container").ejMap({zoomSettings:{maxValue:100}});

{% endhighlight %}


{% highlight js %}
 
//Get or set the maxValue API, after initialization:
   
   //Gets the maxValue value
    
   var property = $("#container").data("ejMap").model.zoomSettings.maxValue;
   
   //Sets the maxValue value 
   
   $("#container").data("ejMap").model.zoomSettings.maxValue= 100;

{% endhighlight %}


### navigationControl `object`
{:#members:navigationcontrol}

Enables or Disables the navigation control for map to perform zooming and panning on map shapes.


### navigationControl.absolutePosition `object`
{:#members:navigationcontrol-absoluteposition}

Set the absolutePosition for navigation control


#### Default Value

* {x:0,y:0}

#### Example

{% highlight js %}
 
//To set absolutePosition API value during initialization 
   $("#container").ejMap(navigationControl:{absolutePosition:{x:5,y:20}});

{% endhighlight %}


{% highlight js %}
 
//Get or set the absolutePosition, after initialization:
   
   //Gets the absolutePosition value
   
   var property = $("#container").data("ejMap").model.navigationControl.absolutePosition;
   
   //Sets the absolutePosition value
   
   $("#container").data("ejMap").model.navigationControl.absolutePosition={x:5,y:20}});

{% endhighlight %}


### navigationControl.content `string`
{:#members:navigationcontrol-content}

Specifies the navigation control template for map

#### Default Value

* null

#### Example

{% highlight js %}
 
//To set navigation control template for map during initialization 
   $("#container").ejMap(navigationControl:{content:null});

{% endhighlight %}


{% highlight js %}

//Get or set the navigation control template for map, after initialization:

   //Gets the navigation control template
   
   var property = $("#container").data("ejMap").model.navigationControl.content;
   
   //Sets the navigation control template
   
   $("#container").data("ejMap").model.navigationControl.content=null });
{% endhighlight %}


### navigationControl.dockPosition `enum`
{:#members:navigationcontrol-dockposition}

<ts name="ej.datavisualization.Map.Position"/>
Set the dockPosition value for navigation control

<table class="params">
	<thead>
		<tr>
			<th>Name </th>			
			<th>Description</th>
		</tr>
	</thead>
	<tbody>
	    <tr>
			<td class="name">none</td>			
			<td class="description">specifies the none position</td>
		</tr>
		<tr>
			<td class="name">topleft</td>			
			<td class="description">specifies the topleft position</td>
		</tr>
        <tr>
			<td class="name">topcenter</td>			
			<td class="description">specifies the topcenter position</td>
		</tr>
        <tr>
			<td class="name">topright</td>			
			<td class="description">specifies the topright position</td>
		</tr>    
        <tr>
			<td class="name">centerleft</td>			
			<td class="description">specifies the centerleft position</td>
		</tr>
		<tr>
			<td class="name">center</td>			
			<td class="description">specifies the center position</td>
		</tr>
        <tr>
			<td class="name">centerright</td>			
			<td class="description">specifies the centerright position</td>
		</tr>
        <tr>
			<td class="name">bottomleft</td>			
			<td class="description">specifies the bottomleft position</td>
		</tr>
        <tr>
			<td class="name">bottomcenter</td>			
			<td class="description">specifies the bottomcenter position</td>
		</tr>
        <tr>
			<td class="name">bottomright</td>			
			<td class="description">specifies the bottomright position</td>
		</tr>
	</tbody>
</table>

#### Default Value

* centerleft

#### Example

{% highlight js %}
 
//To set dockPosition value during initialization 
   $("#container").ejMap(navigationControl:{dockPosition:'centerleft'});
   
{% endhighlight %}


{% highlight js %}
 
//Get or set the dockPosition value, after initialization:
   
   //Gets the dockPosition value
   
   var property = $("#container").data("ejMap").model.navigationControl.dockPosition;
   
   //Sets the dockPosition value
   
   $("#container").data("ejMap").model.navigationControl.dockPosition='centerleft' });

{% endhighlight %}


### navigationControl.enableNavigation `boolean`
{:#members:navigationcontrol-enablenavigation}

Enables or Disables the Navigation for handling zooming map

#### Default Value

* false

#### Example

{% highlight js %}
 
//To set enableNavigation API value during initialization 
   $("#container").ejMap(navigationControl:{enableNavigation:false});

{% endhighlight %}


{% highlight js %}
 
//Get or set the enableNavigation, after initialization:
   
   //Gets the enableNavigation value
   
   var property = $("#container").data("ejMap").model.navigationControl.enableNavigation;
   
   //Sets the enableNavigation value
   
   $("#container").data("ejMap").model.navigationControl.enableNavigation=false });

{% endhighlight %}


### navigationControl.orientation `enum`
{:#members:navigationcontrol-orientation}

<ts name="ej.datavisualization.Map.LabelOrientation"/>
Set the orientation value for navigation control

<table class="params">
	<thead>
		<tr>
			<th>Name </th>			
			<th>Description</th>
		</tr>
	</thead>
	<tbody>
		<tr>
			<td class="name">horizontal</td>			
			<td class="description">specifies the horizontal position</td>
		</tr>
		<tr>
			<td class="name">vertical</td>			
			<td class="description">specifies the vertical position</td>
		</tr>
	</tbody>
</table>

#### Default Value

* vertical

#### Example

{% highlight js %}
 
//To set orientation value during initialization 
   $("#container").ejMap(navigationControl:{orientation:'vertical'});
   
{% endhighlight %}


{% highlight js %}
 
//Get or set the orientation value, after initialization:
   
   //Gets the orientation value
   
   var property = $("#container").data("ejMap").model.navigationControl.orientation;
   
   //Sets the orientation value
   
   $("#container").data("ejMap").model.navigationControl.orientation='vertical' });

{% endhighlight %}


### locale `string`
{:#members:locale}

Name of the culture based on which map should be localized. Labels are localized with respect to the culture name.
String type properties like template text are not localized automatically. Provide localized text as value to string type properties.

#### Default Value

* "en-US"

#### Example

{% highlight js %}
 
//To set locale for map during initialization 
   $("#container").ejMap(locale:"en-US");

{% endhighlight %}


{% highlight js %}

//Get or set locale for map, after initialization:

   //Gets the locale
   
   var property = $("#container").data("ejMap").model.locale;
   
   //Sets the locale
   
   $("#container").data("ejMap").model.locale= "en-US" });
{% endhighlight %}




### layers `array`
{:#members:layers}

Layer for holding the map shapes


### layers.bingMapType `enum`
{:#members:layers-bingmaptype}

<ts name="ej.datavisualization.Map.BingMapType"/>
to get the type of bing map.

<table class="params">
	<thead>
		<tr>
			<th>Name </th>			
			<th>Description</th>
		</tr>
	</thead>
	<tbody>
		<tr>
			<td class="name">aerial</td>			
			<td class="description">specifies the aerial type</td>
		</tr>
		<tr>
			<td class="name">aerialwithlabel</td>			
			<td class="description">specifies the aerialwithlabel type</td>
		</tr>
        <tr>
			<td class="name">road</td>			
			<td class="description">specifies the road type</td>
		</tr>
	</tbody>
</table>

#### Default Value

* "aerial"

#### Example

{% highlight js %}
  
// Set the type of bing map during initialization.                      
   $("#container").ejMap({layers: [{ bingMapType:'aerial' }]})

{% endhighlight %}


{% highlight js %}
 
//Get or set the type of bing map after initialization:

  //Gets the type of bing map.

  var property =$("#container").data("ejMap").model.layers[layerIndex].bingMapType;

  //Sets the type of bing map.

  $("#container").data("ejMap").model.layers[layerIndex].bingMapType  = 'aerial';
  
{% endhighlight %}


### layers.bubbleSettings `object`
{:#members:layers-bubblesettings}

Specifies the bubble settings for map

#### Example

{% highlight js %}
 
// Set the bubbleSettings of layer during initialization.                       
   $("#container").ejMap({layers: [{ layerType: "geometry", enableMouseHover: true, shapeSettings: { stroke: "black", fill: "#C3E6ED", highlightColor: "#63B7B7", selectionColor: "#207BB2", strokeThickness: "0.5" },bubbleSettings:{ valuePath: "valuePath", minValue: 20, maxValue: 30, color: "#379F64",}, shapeData: mapShapeData }]})

{% endhighlight %}


{% highlight js %}
 
//Get or set the bubbleSettings after initialization:
  
  //Gets the bubbleSettings from map.
  
  var bubbleSettings =$("#container").data("ejMap").model.layers[layerIndex].bubbleSettings;
  
  //Sets the bubbleSettings to map.
  
  $("#container").data("ejMap").model.layers[layerIndex].bubbleSettings  = { valuePath: "valuePath", minValue: 20, maxValue: 30, color: "#379F64"};

{% endhighlight %}


### layers.bubbleSettings.bubbleOpacity `number`
{:#members:layers-bubblesettings-bubbleopacity}

Specifies the bubble Opacity value of bubbles for shape layer in map

#### Default Value

* "0.9"

#### Example

{% highlight js %}
 
//To set bubbleOpacity API value during initialization 
  $("#container").ejMap({layers: {bubbleSettings: {bubbleOpacity:'0.9'}}});

{% endhighlight %}


{% highlight js %}
 
//Get or set the bubbleOpacity API, after initialization:

   //Gets the bubble Opacity value 
   
   var bubbleProperty =$("#container").data("ejMap").model.layers[layerIndex].bubbleSettings.bubbleOpacity;
  
   //Sets the bubble Opacity value 
   
   $("#container").data("ejMap").model.layers[0].bubbleSettings.bubbleOpacity='0.9'; 

{% endhighlight %}


### layers.bubbleSettings.color `string`
{:#members:layers-bubblesettings-color}

Specifies the mouse hover color of the shape layer in map

#### Default Value

* "gray"

#### Example

{% highlight js %}
 
//To set color API value during initialization 
   $("#container").ejMap({layers:{bubbleSettings: {color:'gray'}}});

{% endhighlight %}


{% highlight js %}
 
//Get or set the color API, after initialization:
   
   //Gets the color value 
   
   var bubbleProperty =$("#container").data("ejMap").model.layers[layerIndex].bubbleSettings.color;
  
   //Sets the color value 
   
   $("#container").data("ejMap").model.layers[0].bubbleSettings.color='gray'; 

{% endhighlight %}

### layers.bubbleSettings.colorMappings `object`
{:#members:layers-bubblesettings-colormappings}

Specifies the colorMappings of the shape layer in map

#### Default Value

* null

#### Example

{% highlight js %}
 
//To set colorMappings API value during initialization 
  $("#container").ejMap({layers:{ bubbleSettings: {colorMappings:{rangeColorMapping:{from: 0,to: 100000,gradientColors: ["#9CBF4E", "#B8CE7B"]}}}}});
  
{% endhighlight %}


{% highlight js %}
 
//Get or set the colorMappings API, after initialization:
   
   //Gets the colorMappings value 
   
   var bubbleProperty =$("#container").data("ejMap").model.layers[layerIndex].bubbleSettings.colorMappings;
  
   //Sets the colorMappings value 
   
   $("#container").data("ejMap").model.layers[0].bubbleSettings.colorMappings={rangeColorMapping:{from: 0,to: 100000,gradientColors: ["#9CBF4E", "#B8CE7B"]}}; 

{% endhighlight %}

### layers.bubbleSettings.colorMappings.rangeColorMapping `array`
{:#members:layers-bubbleSettings-colormappings-rangecolormapping}

Specifies the range colorMappings in the bubble layer.

#### Default Value

* null
### layers.bubbleSettings.colorMappings.rangeColorMapping.from `number`
{:#members:layers-bubbleSettings-colormappings-rangecolormapping-from}

Start range colorMappings in the bubble layer.

#### Default Value

* null

#### Example

{% highlight js %}
 
//To set start range colorMapping API value during initialization 
  $("#container").ejMap({layers:{ bubbleSettings: {colorMappings:{rangeColorMapping:[{from: 0,to: 100000,gradientColors: ["#9CBF4E", "#B8CE7B"]}]}}}});
{% endhighlight %}

### layers.bubbleSettings.colorMappings.rangeColorMapping.to `number`
{:#members:layers-bubbleSettings-colormappings-rangecolormapping-to}

End range colorMappings in the bubble layer.

#### Default Value

* null

#### Example

{% highlight js %}
 
//To set to range colorMapping API value during initialization 
  $("#container").ejMap({layers:{ bubbleSettings: {colorMappings:{rangeColorMapping:[{from: 0,to: 100000,gradientColors: ["#9CBF4E", "#B8CE7B"]}]}}}});
{% endhighlight %}

### layers.bubbleSettings.colorMappings.rangeColorMapping.gradientColors `array`
{:#members:layers-bubbleSettings-colormappings-rangecolormapping-gradientcolors}

GradientColors in the bubble layer of map.

### layers.bubbleSettings.colorMappings.rangeColorMapping.color `string`
{:#members:layers-bubbleSettings-colormappings-rangecolormapping-gradientcolors}

Color of the bubble layer.


#### Default Value

* null

#### Example

{% highlight js %}
 
//To set gradientColors API value during initialization 
  $("#container").ejMap({layers:{ bubbleSettings: {colorMappings:{rangeColorMapping:[{from: 0,to: 100000,color:"#9CBF4E"}]}}}});
{% endhighlight %}


### layers.bubbleSettings.colorValuePath `string`
{:#members:layers-bubblesettings-colorvaluepath}

Specifies the bubble color valuePath of the shape layer in map

#### Default Value

* null

#### Example

{% highlight js %}
 
//To set colorValuePath  API value during initialization 
  $("#container").ejMap({layers: {bubbleSettings: {colorValuePath :'sales'}}});

{% endhighlight %}


{% highlight js %}
 
//Get or set the colorValuePath  API, after initialization:
   //Gets the colorValuePath  value 
   
   var bubbleProperty =$("#container").data("ejMap").model.layers[layerIndex].bubbleSettings.colorValuePath ;
        
   //Sets the colorValuePath  value 
   
   $("#container").data("ejMap").model.layers[0].bubbleSettings.colorValuePath ='sales'; 

{% endhighlight %}

### layers.bubbleSettings.maxValue `number`
{:#members:layers-bubblesettings-maxvalue}

Specifies the maximum size value of bubbles for shape layer in map

#### Default Value

* "20"

#### Example

{% highlight js %}
 
//To set maxValue API value during initialization 
  $("#container").ejMap({layers: {bubbleSettings: {maxValue:'20'}}});
  
{% endhighlight %}


{% highlight js %}
 
//Get or set the maxValue API, after initialization:
   
   //Gets the maxValue value 
   
   var bubbleProperty =$("#container").data("ejMap").model.layers[layerIndex].bubbleSettings.maxValue;
       
   //Sets the maxValue value 
   
   $("#container").data("ejMap").model.layers[0].bubbleSettings.maxValue='20'; 

{% endhighlight %}


### layers.bubbleSettings.minValue  `number`
{:#members:layers-bubblesettings-minvalue}

Specifies the minimum size value of bubbles for shape layer in map

#### Default Value

* "10"

#### Example

{% highlight js %}
 
//To set minValue API value during initialization 
  $("#container").ejMap({layers: {bubbleSettings: {minValue:'10'}}});

{% endhighlight %}


{% highlight js %}
 
//Get or set the minValue API, after initialization:
   
   //Gets the minValue value 
   
   var bubbleProperty =$("#container").data("ejMap").model.layers[layerIndex].bubbleSettings.minValue;
       
   //Sets the minValue value 
   
   $("#container").data("ejMap").model.layers[0].bubbleSettings.minValue='10'; 

{% endhighlight %}


### layers.bubbleSettings.showBubble `boolean`
{:#members:layers-bubblesettings-showbubble}

Specifies the showBubble visibility status map

#### Default Value

* true

#### Example

{% highlight js %}
 
//To set showBubble API value during initialization 
  $("#container").ejMap({layers: {bubbleSettings: {showBubble:true}}});
  
{% endhighlight %}


{% highlight js %}
 
//Get or set the showBubble API, after initialization:
   
   //Gets the showBubble value 
   
   var bubbleProperty =$("#container").data("ejMap").model.layers[layerIndex].bubbleSettings.showBubble;
     
   //Sets the showBubble value 
   
   $("#container").data("ejMap").model.layers[0].bubbleSettings.showBubble=true; 

{% endhighlight %}


### layers.bubbleSettings.showTooltip `boolean`
{:#members:layers-bubblesettings-showtooltip}

Specifies the tooltip visibility status of the shape layer in map

#### Default Value

* false

#### Example

{% highlight js %}
 
//To set showTooltip API value during initialization 
  $("#container").ejMap({layers: {bubbleSettings: {showTooltip:false}}});

{% endhighlight %}


{% highlight js %}
 
//Get or set the showTooltip API, after initialization:
   
   //Gets the showTooltip value 
   
   var bubbleProperty =$("#container").data("ejMap").model.layers[layerIndex].bubbleSettings.showTooltip;
    
   //Sets the showTooltip value 
   
   $("#container").data("ejMap").model.layers[0].bubbleSettings.showTooltip=false; 

{% endhighlight %}


### layers.bubbleSettings.tooltipTemplate `string`
{:#members:layers-bubblesettings-tooltiptemplate}

Specifies the bubble tooltip template of the shape layer in map

#### Default Value

* null

#### Example

{% highlight js %}
 
//To set tooltipTemplate API value during initialization 
  $("#container").ejMap({layers: {bubbleSettings: {tooltipTemplate:'template'}}});

{% endhighlight %}


{% highlight js %}
 
//Get or set the tooltipTemplate API, after initialization:
   
   //Gets the tooltipTemplate value 
   
   var bubbleProperty =$("#container").data("ejMap").model.layers[layerIndex].bubbleSettings.tooltipTemplate;
        
   //Sets the tooltipTemplate value 
   
   $("#container").data("ejMap").model.layers[0].bubbleSettings.tooltipTemplate='template'; 

{% endhighlight %}


### layers.bubbleSettings.valuePath `string`
{:#members:layers-bubblesettings-valuepath}

Specifies the bubble valuePath of the shape layer in map

#### Default Value

* null

#### Example

{% highlight js %}
 
//To set valuePath API value during initialization 
  $("#container").ejMap({layers: {bubbleSettings: {valuePath:'name'}}});

{% endhighlight %}


{% highlight js %}
 
//Get or set the valuePath API, after initialization:
   
   //Gets the valuePath value 
   
   var bubbleProperty =$("#container").data("ejMap").model.layers[layerIndex].bubbleSettings.valuePath;
      
   //Sets the valuePath value 
   
   $("#container").data("ejMap").model.layers[0].bubbleSettings.valuePath='name'; 

{% endhighlight %}


### layers.dataSource `object`
{:#members:layers-datasource}

Specifies the datasource for the shape layer

#### Example

{% highlight js %}

// Set the dataSource of layer during initialization.                        
   $("#container").ejMap({layers: [{ layerType: "geometry", dataSource: source,  shapeData: mapShapeData }]})

{% endhighlight %}


{% highlight js %}
 
//Get or set the dataSource after initialization:
   
   //Gets the dataSource from map layer.
   
   var dataSource =$("#container").data("ejMap").model.layers[layerIndex].dataSource;
   
   //Sets the dataSource to map layer.
   
   $("#container").data("ejMap").model.layers[layerIndex].dataSource  = source;

{% endhighlight %}


### layers.shapeDataPath `string`
{:#members:layers-shapedatapath}

Specifies the data path of shape 


#### Example

{% highlight js %}

// Set the shapeDataPath of layer during initialization.                        
   $("#container").ejMap({layers: [{ shapeDataPath: "name"}]})

{% endhighlight %}


{% highlight js %}
 
//Get or set the shapeDataPath after initialization:
   
   //Gets the shapeDataPath from map layer.
   
   var property =$("#container").data("ejMap").model.layers[layerIndex].shapeDataPath;
   
   //Sets the shapeDataPath to map layer.
   
   $("#container").data("ejMap").model.layers[layerIndex].shapeDataPath  = 'name';

{% endhighlight %}


### layers.shapePropertyPath `string`
{:#members:layers-shapepropertypath}

Specifies the data path of shape 


#### Example

{% highlight js %}

// Set the shapePropertyPath of layer during initialization.                        
   $("#container").ejMap({layers: [{ shapePropertyPath: "name"}]})

{% endhighlight %}


{% highlight js %}
 
//Get or set the shapePropertyPath after initialization:
   
   //Gets the shapePropertyPath from map layer.
   
   var property =$("#container").data("ejMap").model.layers[layerIndex].shapePropertyPath;
   
   //Sets the shapePropertyPath to map layer.
   
   $("#container").data("ejMap").model.layers[layerIndex].shapePropertyPath  = 'name';

{% endhighlight %}


### layers.enableMouseHover `boolean`
{:#members:layers-enablemousehover}

Enables or disables the shape mouse hover

#### Default Value

* false

#### Example

{% highlight js %}
  
// Set the enableMouseHover during initialization.                      
   $("#container").ejMap({layers: [{ enableMouseHover:false }]}){% endhighlight %}


{% highlight js %}
 
//Get or set the enableMouseHover after initialization:
   
   //Gets the enableMouseHover from map.
   
   var property =$("#container").data("ejMap").model.layers[layerIndex].enableMouseHover;
   
   //Sets the enableMouseHover to map.
   
   $("#container").data("ejMap").model.layers[layerIndex].enableMouseHover  = false;
   
{% endhighlight %}


### layers.enableSelection `boolean`
{:#members:layers-enableselection}

Enables or disables the shape selection

#### Default Value

* true

#### Example

{% highlight js %}
  
// Set the enableSelection during initialization.                       
   $("#container").ejMap({layers: [{ enableSelection:true }]})

{% endhighlight %}


{% highlight js %}
 
//Get or set the enableSelection after initialization:
   
   //Gets the enableSelection from map.
   
   var property =$("#container").data("ejMap").model.layers[layerIndex].enableSelection;
   
   //Sets the enableSelection to map.
   
   $("#container").data("ejMap").model.layers[layerIndex].enableSelection  = true;

{% endhighlight %}


### layers.key `string`
{:#members:layers-key}}

to get the key of bing map

#### Default Value

* null

#### Example

{% highlight js %}
 
//to get the key of bing map during initialization 
   $("#container").ejMap({layers: [{  layerType: 'bing', key: "" }]})           

{% endhighlight %}


{% highlight js %}
 
//Get or set the key of bing map after initialization:
   
   //Gets the key of bing map value 
   
   var property = =$("#container").data("ejMap").model.layers[layerIndex].key;     
   
   //Sets the bing map key value 
   
   $("#container").data("ejMap").model.layers[layerIndex].key = "";

{% endhighlight %}


### layers.labelSettings `object`
{:#members:layers-labelsettings}

Options for enabling and configuring labelSettings labelPath, smartLabelSize, labelLength etc.,


### layers.labelSettings.enableSmartLabel `boolean`
{:#members:layers-labelsettings-enablesmartlabel}

enable or disable the enableSmartLabel property

#### Default Value

* false

#### Example

{% highlight js %}

// Set the enableSmartLabel value of layer during initialization.                    
   $("#container").ejMap({layers:[{labelSettings: { enableSmartLabel: false}}]})

{% endhighlight %}


{% highlight js %}
 
//Get or set the enableSmartLabel value after initialization:
   
   //Gets the enableSmartLabel value 
   
   var labelSettings =$("#container").data("ejMap").model.layers[layerIndex].labelSettings.enableSmartLabel;
   
   //Sets the enableSmartLabel value
   
   $("#container").data("ejMap").model.layers[layerIndex].labelSettings = { enableSmartLabel: false};                   

{% endhighlight %}


### layers.labelSettings.labelLength `number`
{:#members:layers-labelsettings-labellength}

set the labelLength property

#### Default Value

* '2'

#### Example


{% highlight js %}

// Set the labelLength value of layer during initialization.                         
   $("#container").ejMap({layers:[{labelSettings: { labelLength: 2}}]})

{% endhighlight %}


{% highlight js %}
 
//Get or set the labelLength value after initialization:
   
   //Gets the labelLength value 
   
   var labelSettings =$("#container").data("ejMap").model.layers[layerIndex].labelSettings.labelLength;
   
   //Sets the labelLength value

   $("#container").data("ejMap").model.layers[layerIndex].labelSettings = { labelLength: 2};                     

{% endhighlight %}



### layers.labelSettings.labelPath `string`
{:#members:layers-labelsettings-labelpath}

set the labelPath property

#### Default Value

* null

#### Example
{:.example}


{% highlight js %}

// Set the labelPath value of layer during initialization.                   
   $("#container").ejMap({layers:[{labelSettings: { labelPath: ""}}]})

{% endhighlight %}


{% highlight js %}
 
//Get or set the labelPath value after initialization:
   
   //Gets the labelPath value 
   
   var labelSettings =$("#container").data("ejMap").model.layers[layerIndex].labelSettings.labelPath;
   
   //Sets the labelPath value
   
   $("#container").data("ejMap").model.layers[layerIndex].labelSettings = { labelPath: ""};                      

{% endhighlight %}



### layers.labelSettings.showLabels `boolean`
{:#members:layers-labelsettings-showlabels}

The property specifies whether to show labels or not.

#### Default Value

* false

#### Example

{% highlight js %}
// Set the showLabel value of layer during initialization.                   
   $("#container").ejMap({layers:[{labelSettings: { showLabels: false}}]})
        
{% endhighlight %}


{% highlight js %}
 
//Get or set the showLabel value after initialization:
   
   //Gets the showLabel value 
   
   var labelSettings =$("#container").data("ejMap").model.layers[layerIndex].labelSettings.showLabels;
   
   //Sets the showLabel value
   
   $("#container").data("ejMap").model.layers[layerIndex].labelSettings = { showLabels: false};                  

{% endhighlight %}


### layers.labelSettings.smartLabelSize `enum`
{:#members:layers-labelsettings-smartlabelsize}

<ts name="ej.datavisualization.Map.LabelSize"/>
set the smartLabelSize property

<table class="params">
	<thead>
		<tr>
			<th>Name </th>			
			<th>Description</th>
		</tr>
	</thead>
	<tbody>
		<tr>
			<td class="name">fixed</td>			
			<td class="description">specifies the fixed size</td>
		</tr>
		<tr>
			<td class="name">default</td>			
			<td class="description">specifies the default size</td>
		</tr>
	</tbody>
</table>

#### Default Value

* "fixed"

#### Example

{% highlight js %}
// Set the smartLabelSize value of layer during initialization.                      
   $("#container").ejMap({layers:[{labelSettings: { smartLabelSize: 'fixed'}}]})
 
 {% endhighlight %}


{% highlight js %}
 
//Get or set the smartLabelSize value after initialization:
   
   //Gets the smartLabelSize value 
   
   var labelSettings =$("#container").data("ejMap").model.layers[layerIndex].labelSettings.smartLabelSize;
   
   //Sets the smartLabelSize value
   
   $("#container").data("ejMap").model.layers[layerIndex].labelSettings = { smartLabelSize: 'fixed'};                    

{% endhighlight %}


### layers.labelSettings.font `object`
{:#members:layers-labelsettings-font}




Options for customizing the data label font.






### layers.labelSettings.font.fontFamily `string`
{:#members:layers-labelsettings-font-fontfamily}




Font family of the data label. 


#### Default Value



* "Segoe UI"




#### Example


{% highlight js %}
 
 
$("#container").ejMap({
    layers : [{
         labelSettings:{
             font :{fontFamily : "Algerian"}
         }    
    }]
});
{% endhighlight %}




### layers.labelSettings.font.fontStyle `enum`
{:#members:layers-labelsettings-font-fontstyle}

<ts name="ej.datavisualization.Map.FontStyle"/>


Font style of the data label.  

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



* "normal". 

#### Example


{% highlight js %}
 
 
$("#container").ejMap({
    layers : [{
        labelSettings:{
            font :{fontStyle : "italic"}
        }    
    }]                 
});
 {% endhighlight %}




### layers.labelSettings.font.fontWeight `enum`
{:#members:layers-labelsettings-font-fontweight}


<ts name="ej.datavisualization.Map.FontWeight"/>


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


Font weight of the data label.  


#### Default Value



* "regular". See 



#### Example


{% highlight js %}
 
$("#container").ejMap({
    layers : [{
        labelSettings:{
            font :{fontWeight : "lighter"}
        }    
    }]                 
});
 
{% endhighlight %}




### layers.labelSettings.font.opacity `number`
{:#members:layers-labelsettings-font-opacity}




Opacity of the text. 


#### Default Value



 * 1




#### Example


{% highlight js %}
 
$("#container").ejMap({
    layers : [{
        labelSettings:{
            font :{opacity : 0.5}
        }    
    }]                 
});

{% endhighlight %}

### layers.labelSettings.font.color `string`
{:#members:layers-labelSettings-font-color}

Font color of the data label text. 

#### Default Value

 * null

#### Example

{% highlight js %}

$("#container").ejMap({
    layers : [{
        labelSettings:{
            font :{color : "red"}
        }    
    }]                 
});
 
{% endhighlight %}


### layers.labelSettings.font.size `string`
{:#members:layers-labelSettings-font-size}




Font size of the data label. 


#### Default Value



* "12px"




#### Example


{% highlight js %}

$("#container").ejMap({
    layers : [{
        labelSettings:{
            font :{size : "14px"}
        }    
    }]                 
}); 

{% endhighlight %}




### layers.geometryType `enum`
{:#members:layers-geometrytype}

<ts name="ej.datavisualization.Map.GeometryType"/>
Specifies the map view type.

<table class="params">
	<thead>
		<tr>
			<th>Name </th>			
			<th>Description</th>
		</tr>
	</thead>
	<tbody>
		<tr>
			<td class="name">geographic</td>			
			<td class="description">specifies the geographic view of map</td>
		</tr>
		<tr>
			<td class="name">normal</td>			
			<td class="description">specifies the normal land view of map</td>
		</tr>
	</tbody>
</table>

#### Default Value

* 'geographic'

#### Example

{% highlight js %}
  
// Set the geometryType during initialization.                     
   $("#container").ejMap({layers: [{ geometryType:'geographic' }]})
{% endhighlight %}


{% highlight js %}
 
//Get or set the geometryType after initialization:
   
   //Gets the geometryType from map.
   
   var property =$("#container").data("ejMap").model.layers[layerIndex].geometryType;
   
   //Sets the geometryType to map.
   
   $("#container").data("ejMap").model.layers[layerIndex].geometryType  = 'normal';

{% endhighlight %}


### layers.layerType `enum`
{:#members:layers-layertype}

<ts name="ej.datavisualization.Map.LayerType"/>
Specifies the map type.

<table class="params">
	<thead>
		<tr>
			<th>Name </th>			
			<th>Description</th>
		</tr>
	</thead>
	<tbody>
		<tr>
			<td class="name">geometry</td>			
			<td class="description">specifies the geometry type</td>
		</tr>
		<tr>
			<td class="name">osm</td>			
			<td class="description">specifies the osm type</td>
		</tr>
        <tr>
			<td class="name">bing</td>			
			<td class="description">specifies the bing type</td>
		</tr>
	</tbody>
</table>

#### Default Value

* 'geometry'

#### Example

{% highlight js %}
  
// Set the layerType during initialization.                     
   $("#container").ejMap({layers: [{ layerType:'geometry' }]})
{% endhighlight %}


{% highlight js %}
 
//Get or set the layerType after initialization:
   
   //Gets the layerType from map.
   
   var property =$("#container").data("ejMap").model.layers[layerIndex].layerType;
   
   //Sets the layerType to map.
   
   $("#container").data("ejMap").model.layers[layerIndex].layerType  = 'geometry';

{% endhighlight %}


### layers.legendSettings `object`
{:#members:layers-legendsettings}

Options for enabling and configuring legendSettings position, height, width, mode, type etc.,


### layers.legendSettings.dockOnMap `boolean`
{:#members:layers-legendsettings-dockonmap}

Determines whether the legend should be placed outside or inside the map bounds

#### Default Value

* false

#### Example

{% highlight js %}
 
//To set dockOnMap API value during initialization 
   $("#container").ejMap({layers: [{legendSettings: {dockOnMap:false} }]})           

{% endhighlight %}


{% highlight js %}
 
//Get or set the dockOnMap API, after initialization:
   
   //Gets the dockOnMap value 
   
   var property = =$("#container").data("ejMap").model.layers[layerIndex].legendSettings.dockOnMap;        
   
   //Sets the dockOnMap value 
   
   $("#container").data("ejMap").model.layers[layerIndex].legendSettings  = {dockOnMap:false};

{% endhighlight %}


### layers.legendSettings.dockPosition `enum`
{:#members:layers-legendsettings-dockposition}

<ts name="ej.datavisualization.Map.DockPosition"/>
Determines the legend placement and it is valid only when dockOnMap is true

<table class="params">
	<thead>
		<tr>
			<th>Name </th>			
			<th>Description</th>
		</tr>
	</thead>
	<tbody>
		<tr>
			<td class="name">top</td>			
			<td class="description">specifies the top position</td>
		</tr>
		<tr>
			<td class="name">bottom</td>			
			<td class="description">specifies the bottom position</td>
		</tr>
    <tr>
			<td class="name">right</td>			
			<td class="description">specifies the bottom position</td>
		</tr>
    <tr>
			<td class="name">left</td>			
			<td class="description">specifies the left position</td>
		</tr>
	</tbody>
</table>

#### Default Value

* "top"

#### Example

{% highlight js %}
 
//To set dockPosition value during initialization 
   $("#container").ejMap({layers: [{legendSettings: {dockPosition:"top"} }]})           

{% endhighlight %}


{% highlight js %}
 
//Get or set dockPosition value after initialization:
  
  //Gets the dockPosition value
  
  var property = =$("#container").data("ejMap").model.layers[layerIndex].legendSettings.dockPosition;     
  
  //Sets the dockPosition value value 
  
  $("#container").data("ejMap").model.layers[layerIndex].legendSettings  = {dockPosition:"top"};

{% endhighlight %}


### layers.legendSettings.height `number`
{:#members:layers-legendsettings-height}

height value for legend setting

#### Default Value

* 0

#### Example

{% highlight js %}
 
//To set height value for legend during initialization 
   $("#container").ejMap({layers: [{legendSettings: {height:20} }]})           

{% endhighlight %}


{% highlight js %}
 
//Get or set the height value for legend, after initialization:
   
   //Gets the height value for legend value 
   
   var property = =$("#container").data("ejMap").model.layers[layerIndex].legendSettings.height;   
   
   //Sets the height value for legend value 
   
   $("#container").data("ejMap").model.layers[layerIndex].legendSettings  = {height:20};
   
{% endhighlight %}


### layers.legendSettings.icon `enum`
{:#members:layers-legendsettings-icon}

<ts name="ej.datavisualization.Map.LegendIcons"/>
to get icon value for legend setting

<table class="params">
	<thead>
		<tr>
			<th>Name </th>			
			<th>Description</th>
		</tr>
	</thead>
	<tbody>
		<tr>
			<td class="name">rectangle</td>			
			<td class="description">specifies the rectangle position</td>
		</tr>
		<tr>
			<td class="name">circle</td>			
			<td class="description">specifies the circle position</td>
		</tr>
	</tbody>
</table>

#### Default Value

* "rectangle"

#### Example


{% highlight js %}
 
//To set icon value during initialization 
   $("#container").ejMap({layers: [{legendSettings: {icon:"rectangle"} }]})           

{% endhighlight %}


{% highlight js %}
 
//Get or set icon value after initialization:
   
   //Gets the icon value value 
   
   var property = =$("#container").data("ejMap").model.layers[layerIndex].legendSettings.icon;     
   
   //Sets the icon value value 
   
   $("#container").data("ejMap").model.layers[layerIndex].legendSettings  = {icon:"rectangle"};

{% endhighlight %}


### layers.legendSettings.iconHeight `number`
{:#members:layers-legendsettings-iconheight}

icon height value for legend setting

#### Default Value

* 20

#### Example

{% highlight js %}
 
//To set iconHeight value for legend during initialization 
   $("#container").ejMap({layers: [{legendSettings: {iconHeight:20} }]})           

{% endhighlight %}


{% highlight js %}
 
//Get or set the iconHeight value for legend, after initialization:
   
   //Gets the iconHeight value for legend value 
   
   var property = =$("#container").data("ejMap").model.layers[layerIndex].legendSettings.iconHeight;       
   
   //Sets the iconHeight value for legend value 
   
   $("#container").data("ejMap").model.layers[layerIndex].legendSettings  = {iconHeight:20};

{% endhighlight %}


### layers.legendSettings.iconWidth `number`
{:#members:layers-legendsettings-iconwidth}

icon Width value for legend setting

#### Default Value:

* 20

#### Example


{% highlight js %}
 
//To set iconWidth value for legend during initialization 
   $("#container").ejMap({layers: [{legendSettings: {iconWidth:20} }]})           

{% endhighlight %}

{% highlight js %}
 
//Get or set the iconWidth value for legend, after initialization:
   
   //Gets the iconWidth value for legend value 
   
   var property = =$("#container").data("ejMap").model.layers[layerIndex].legendSettings.iconWidth;        
   
   //Sets the iconWidth value for legend value 
   
   $("#container").data("ejMap").model.layers[layerIndex].legendSettings  = {iconWidth:20};
   
{% endhighlight %}


### layers.legendSettings.labelOrientation `enum`
{:#members:layers-legendsettings-labelorientation}

<ts name="ej.datavisualization.Map.LabelOrientation"/>
set the orientation of legend labels

<table class="params">
	<thead>
		<tr>
			<th>Name </th>			
			<th>Description</th>
		</tr>
	</thead>
	<tbody>
		<tr>
			<td class="name">horizontal</td>			
			<td class="description">specifies the horizontal position</td>
		</tr>
		<tr>
			<td class="name">vertical</td>			
			<td class="description">specifies the vertical position</td>
		</tr>  
	</tbody>
</table>

#### Default Value

* vertical

#### Example

{% highlight js %}
 
//To set label orientation API value for legend setting during initialization 
   $("#container").ejMap({layers: [{legendSettings: {labelOrientation: "vertical"} }]})                      

{% endhighlight %}


{% highlight js %}
 
//Get or set the label orientation API, after initialization:
   
   //Gets the label orientation value 
   
   var property = =$("#container").data("ejMap").model.layers[layerIndex].legendSettings.labelOrientation; 
   
   //Sets the label orientation value 
   
   $("#container").data("ejMap").model.layers[layerIndex].legendSettings  = {labelOrientation: "vertical"};

{% endhighlight %}


### layers.legendSettings.leftLabel `string`
{:#members:layers-legendsettings-leftlabel}

to get leftLabel value for legend setting

#### Default Value

* null

#### Example

{% highlight js %}
 
//To set leftLabel value during initialization 
   $("#container").ejMap({layers: [{legendSettings: {leftLabel:""} }]})           

{% endhighlight %}


{% highlight js %}
 
//Get or set leftLabel value after initialization:
   
   //Gets the leftLabel value value 
   
   var property = =$("#container").data("ejMap").model.layers[layerIndex].legendSettings.leftLabel;        
   
   //Sets the leftLabel value value 
   
   $("#container").data("ejMap").model.layers[layerIndex].legendSettings  = {leftLabel:""};

{% endhighlight %}


### layers.legendSettings.textPath `string`
{:#members:layers-legendsettings-textpath}

To get the field name in the datasource for generating legend items.

#### Default Value

* null

#### Example

{% highlight js %}
 
//To set textPath value during initialization 
   $("#container").ejMap({layers: [{legendSettings: {textPath:""} }]})           

{% endhighlight %}


{% highlight js %}
 
//Get or set textPath value after initialization:
   
   //Gets the textPath value value 
   
   var property = =$("#container").data("ejMap").model.layers[layerIndex].legendSettings.textPath;        
   
   //Sets the textPath value value 
   
   $("#container").data("ejMap").model.layers[layerIndex].legendSettings  = {textPath:""};

{% endhighlight %}


### layers.legendSettings.mode `enum`
{:#members:layers-legendsettings-mode}

<ts name="ej.datavisualization.Map.Mode"/>
to get mode of legend setting

<table class="params">
	<thead>
		<tr>
			<th>Name </th>			
			<th>Description</th>
		</tr>
	</thead>
	<tbody>
		<tr>
			<td class="name">default</td>			
			<td class="description">specifies the default mode</td>
		</tr>
		<tr>
			<td class="name">interactive</td>			
			<td class="description">specifies the interactive mode</td>
		</tr>
	</tbody>
</table>


#### Default Value

* "default"

#### Example

{% highlight js %}
 
//To set legend mode during initialization 
   $("#container").ejMap({layers: [{legendSettings: {mode:"default"} }]})
              
{% endhighlight %}


{% highlight js %}
 
//Get or set the legend mode after initialization:
   
   //Gets the legend mode value 
   
   var property = =$("#container").data("ejMap").model.layers[layerIndex].legendSettings.mode;     
   
   //Sets the legend mode value 
   
   $("#container").data("ejMap").model.layers[layerIndex].legendSettings  = {mode:"default"};

{% endhighlight %}


### layers.legendSettings.position `enum`
{:#members:layers-legendsettings-position}

<ts ref="ej.datavisualization.Map.Position"/>

set the position of legend settings

<table class="params">
	<thead>
		<tr>
			<th>Name </th>			
			<th>Description</th>
		</tr>
	</thead>
	<tbody>
	    <tr>
			<td class="name">none</td>			
			<td class="description">specifies the none position</td>
		</tr>
		<tr>
			<td class="name">topleft</td>			
			<td class="description">specifies the topleft position</td>
		</tr>
        <tr>
			<td class="name">topcenter</td>			
			<td class="description">specifies the topcenter position</td>
		</tr>
        <tr>
			<td class="name">topright</td>			
			<td class="description">specifies the topright position</td>
		</tr>    
        <tr>
			<td class="name">centerleft</td>			
			<td class="description">specifies the centerleft position</td>
		</tr>
		<tr>
			<td class="name">center</td>			
			<td class="description">specifies the center position</td>
		</tr>
        <tr>
			<td class="name">centerright</td>			
			<td class="description">specifies the centerright position</td>
		</tr>
        <tr>
			<td class="name">bottomleft</td>			
			<td class="description">specifies the bottomleft position</td>
		</tr>
        <tr>
			<td class="name">bottomcenter</td>			
			<td class="description">specifies the bottomcenter position</td>
		</tr>
        <tr>
			<td class="name">bottomright</td>			
			<td class="description">specifies the bottomright position</td>
		</tr>
	</tbody>
</table>

#### Default Value

* topleft

#### Example

{% highlight js %}
 
//To set legend position API value for legend setting during initialization 
   $("#container").ejMap({layers: [{legendSettings: {position: "topleft"} }]})                      

{% endhighlight %}


{% highlight js %}
 
//Get or set the legend position API, after initialization:
   
   //Gets the legend position value 
   
   var property = =$("#container").data("ejMap").model.layers[layerIndex].legendSettings.position; 
   
   //Sets the legend position value 
   
   $("#container").data("ejMap").model.layers[layerIndex].legendSettings  = {position: "topleft"};

{% endhighlight %}


### layers.legendSettings.positionX `number`
{:#members:layers-legendsettings-positionx}

x position value for legend setting

#### Default Value

* 0

#### Example

{% highlight js %}
 
//To set x position value during initialization 
   $("#container").ejMap({layers: [{legendSettings: {positionX: 0} }]})           

{% endhighlight %}


{% highlight js %}
 
//Get or set the x position, after initialization:
   
   //Gets the x position value 
   
   var property = =$("#container").data("ejMap").model.layers[layerIndex].legendSettings.positionX;        
   
   //Sets the x position value 
   
   $("#container").data("ejMap").model.layers[layerIndex].legendSettings  = {positionX: 0};

{% endhighlight %}


### layers.legendSettings.positionY `number`
{:#members:layers-legendsettings-positiony}

y position value for legend setting

#### Default Value

* 0

#### Example

{% highlight js %}
 
//To set y position value during initialization 
   $("#container").ejMap({layers: [{legendSettings: {positionY: 0} }]})           
{% endhighlight %}


{% highlight js %}
 
//Get or set the y position, after initialization:
   
   //Gets the y position value 
   
   var property = =$("#container").data("ejMap").model.layers[layerIndex].legendSettings.positionY;        
   
   //Sets the y position value 
   
   $("#container").data("ejMap").model.layers[layerIndex].legendSettings  = {positionY: 0};

{% endhighlight %}


### layers.legendSettings.rightLabel `string`
{:#members:layers-legendsettings-rightlabel}

to get rightLabel value for legend setting

#### Default Value

* null

#### Example

{% highlight js %}
 
//To set rightLabel value during initialization 
   $("#container").ejMap({layers: [{legendSettings: {rightLabel:""} }]})           

{% endhighlight %}


{% highlight js %}
 
//Get or set rightLabel value after initialization:
   
   //Gets the rightLabel value value 
   
   var property = =$("#container").data("ejMap").model.layers[layerIndex].legendSettings.rightLabel;       
   
   //Sets the rightLabel value value 
   
   $("#container").data("ejMap").model.layers[layerIndex].legendSettings  = {rightLabel:""};

{% endhighlight %}


### layers.legendSettings.showLabels `boolean`
{:#members:layers-legendsettings-showlabels}

Enables or Disables the showLabels

#### Default Value

* false

#### Example

{% highlight js %}
 
//To set showLabels API value during initialization 
   $("#container").ejMap({layers: [{legendSettings: {showLabels:false} }]})           

{% endhighlight %}


{% highlight js %}
 
//Get or set the showLabels API, after initialization:
   
   //Gets the showLabels value 
   
   var property = =$("#container").data("ejMap").model.layers[layerIndex].legendSettings.showLabels;       
   
   //Sets the showLabels value 
   
   $("#container").data("ejMap").model.layers[layerIndex].legendSettings  = {showLabels:false};

{% endhighlight %}


### layers.legendSettings.showLegend `boolean`
{:#members:layers-legendsettings-showlegend}

Enables or Disables the showLegend

#### Default Value

* false

#### Example

{% highlight js %}
 
//To set showLegend API value during initialization 
   $("#container").ejMap({layers: [{legendSettings: {showLegend:false} }]})

{% endhighlight %}


{% highlight js %}
 
//Get or set the showLegend API, after initialization:
   
   //Gets the showLegend value 
   
   var property = =$("#container").data("ejMap").model.layers[layerIndex].legendSettings.showLegend;       
   
   //Sets the showLegend value 

   $("#container").data("ejMap").model.layers[layerIndex].legendSettings  = {showLegend:false};
  
{% endhighlight %}


### layers.legendSettings.toggleVisibility `boolean`
{:#members:layers-legendsettings-togglevisibility}

Toggle the visibility of the legend.

#### Default Value

* false

#### Example

{% highlight js %}
 
//To set toggleVisibility API value during initialization 
   $("#container").ejMap({layers: [{legendSettings: {toggleVisibility:true} }]})

{% endhighlight %}


{% highlight js %}
 
//Get or set the toggleVisibility API, after initialization:
   
   //Gets the toggleVisibility value 
   
   var property = =$("#container").data("ejMap").model.layers[layerIndex].legendSettings.toggleVisibility;       
   
   //Sets the toggleVisibility value 

   $("#container").data("ejMap").model.layers[layerIndex].legendSettings  = {toggleVisibility:true};
  
{% endhighlight %}


### layers.legendSettings.title `string`
{:#members:layers-legendsettings-title}

to get title of legend setting

#### Default Value

* null

#### Example

{% highlight js %}
 
//To set legend title during initialization 
   $("#container").ejMap({layers: [{legendSettings: {title: ""} }]})           

{% endhighlight %}


{% highlight js %}
 
//Get or set the legend title after initialization:
   
   //Gets the legend title value 
   
   var property = =$("#container").data("ejMap").model.layers[layerIndex].legendSettings.title;    
   
   //Sets the legend title value 
   
   $("#container").data("ejMap").model.layers[layerIndex].legendSettings  = {title: ""};

{% endhighlight %}


### layers.legendSettings.type `enum`
{:#members:layers-legendsettings-type}

<ts name="ej.datavisualization.Map.LegendType"/>
to get type of legend setting

<table class="params">
	<thead>
		<tr>
			<th>Name </th>			
			<th>Description</th>
		</tr>
	</thead>
	<tbody>
		<tr>
			<td class="name">layers</td>			
			<td class="description">specifies the layers type</td>
		</tr>
		<tr>
			<td class="name">bubbles</td>			
			<td class="description">specifies the bubbles type</td>
		</tr>
	</tbody>
</table>

#### Default Value

* "layers"

#### Example

{% highlight js %}
 
//To set legend type value during initialization 
   $("#container").ejMap({layers: [{legendSettings: {type:"layers"} }]})           

{% endhighlight %}


{% highlight js %}
 
//Get or set the legend type value after initialization:
   
   //Gets the legend type value 
   
   var property = =$("#container").data("ejMap").model.layers[layerIndex].legendSettings.type;     
   
   //Sets the legend type value 
   
   $("#container").data("ejMap").model.layers[layerIndex].legendSettings  = {type:"layers"};

{% endhighlight %}


### layers.legendSettings.width `number`
{:#members:layers-legendsettings-width}

width value for legend setting

#### Default Value

* 0

#### Example

{% highlight js %}
 
//To set width value for legend during initialization 
   $("#container").ejMap({layers: [{legendSettings: {width:20} }]})           

{% endhighlight %}


{% highlight js %}
 
//Get or set the width value for legend, after initialization:
   
   //Gets the width value for legend value 
   
   var property = =$("#container").data("ejMap").model.layers[layerIndex].legendSettings.width;    
   
   //Sets the width value for legend value 
   
   $("#container").data("ejMap").model.layers[layerIndex].legendSettings  = {width:20};

{% endhighlight %}


### layers.mapItemsTemplate `string`
{:#members:layers-mapitemstemplate}

Specifies the map items template for shapes.

#### Example

{% highlight js %}

// Set the mapItemsTemplate of layer during initialization.                  
   $("#container").ejMap({layers: [{ layerType: "geometry", mapItemsTemplate: "Template",  shapeData: mapShapeData }]})

{% endhighlight %}


{% highlight js %}
 
//Get or set the mapItemsTemplate after initialization:
   
   //Gets the mapItemsTemplate from map.
   
   var mapItemsTemplate =$("#container").data("ejMap").model.layers[layerIndex].mapItemsTemplate;
   
   //Sets the mapItemsTemplate to map.
   
   $("#container").data("ejMap").model.layers[layerIndex].mapItemsTemplate  = "Template";

{% endhighlight %}


### layers.markers `Array`
{:#members:layers-markers}

Specify markers for shape layer.

### layers.markers.label `string`

Display the value in the marker 

#### Default Value

* " "

#### Example

{% highlight js %}
  
// Set the markers during initialization.                       
   $("#container").ejMap({layers: [{markers:[{label : "chennai",latitude : 13.08 ,longitude : 80.27}]}]})

{% endhighlight %}


{% highlight js %}
 
//Get or set the markers after initialization:
   
   //Gets the markers from map.
   
   var marker =$("#container").data("ejMap").model.layers[layerIndex].markers[markerIndex];
   
   //Sets the marker to map.
   
   $("#container").data("ejMap").model.layers[layerIndex].markers[markerIndex]  = {label : "chennai",latitude : 13.08 ,longitude : 80.27};

{% endhighlight %}

### layers.markers.latitude `number`

Display the value in the marker 

#### Default Value

* 0

#### Example

{% highlight js %}
  
// Set the markers during initialization.                       
   $("#container").ejMap({layers: [{markers:[{label : "chennai",latitude : 13.08 ,longitude : 80.27}]}]})

{% endhighlight %}


{% highlight js %}
 
//Get or set the markers after initialization:
   
   //Gets the markers from map.
   
   var marker =$("#container").data("ejMap").model.layers[layerIndex].markers[markerIndex];
   
   //Sets the marker to map.
   
   $("#container").data("ejMap").model.layers[layerIndex].markers[markerIndex]  = {label : "chennai",latitude : 13.08 ,longitude : 80.27};

{% endhighlight %}


### layers.markers.longitude `number`

Display the value in the marker 

#### Default Value

* 0

#### Example

{% highlight js %}
  
// Set the markers during initialization.                       
   $("#container").ejMap({layers: [{markers:[{label : "chennai",latitude : 13.08 ,longitude : 80.27}]}]})

{% endhighlight %}


{% highlight js %}
 
//Get or set the markers after initialization:
   
   //Gets the markers from map.
   
   var marker =$("#container").data("ejMap").model.layers[layerIndex].markers[markerIndex];
   
   //Sets the marker to map.
   
   $("#container").data("ejMap").model.layers[layerIndex].markers[markerIndex]  = {label : "chennai",latitude : 13.08 ,longitude : 80.27};

{% endhighlight %}


### layers.markerTemplate `string`
{:#members:layers-markertemplate}

Specifies the map marker template for map layer.

#### Default Value

* null

#### Example

{% highlight js %}

// Set the markerTemplate of layer during initialization.                    
   $("#container").ejMap({layers: [{ layerType: "geometry", markerTemplate: "Template",  shapeData: mapShapeData }]})

{% endhighlight %}


{% highlight js %}
 
//Get or set the markerTemplate after initialization:
   
   //Gets the markerTemplate from map.
   
   var markerTemplate =$("#container").data("ejMap").model.layers[layerIndex].markerTemplate;
   
   //Sets the markerTemplate to map.
   
   $("#container").data("ejMap").model.layers[layerIndex].markerTemplate  = "Template";

{% endhighlight %}


### layers.selectedMapShapes `Array`
{:#members:layers-selectedmapshapes}

Specify selectedMapShapes for shape layer

#### Default Value

* []

#### Example

{% highlight js %}
 
//Gets the selectedMapShapes from map 
   var selectedShapes =$("#container").data("ejMap").model.layers[layerIndex].selectedMapShapes;         

{% endhighlight %}


### layers.selectionMode `enum`
{:#members:layers-selectionmode}

<ts name="ej.datavisualization.Map.SelectionMode"/>
Specifies the selection mode of the map. Accepted selection mode values are Default and Multiple.

<table class="params">
	<thead>
		<tr>
			<th>Name </th>			
			<th>Description</th>
		</tr>
	</thead>
	<tbody>
		<tr>
			<td class="name">default</td>			
			<td class="description">specifies the default position</td>
		</tr>
		<tr>
			<td class="name">multiple</td>			
			<td class="description">specifies the multiple position</td>
		</tr>
	</tbody>
</table>

#### Default Value

* "default"

#### Example


{% highlight js %}
  
// Set the selection mode during initialization.                        
   $("#container").ejMap({layers: [{ selectionMode:'default' }]})

{% endhighlight %}


{% highlight js %}
 
//Get or set the selection mode after initialization:
   
   //Gets the selection mode from map.
   
   var property =$("#container").data("ejMap").model.layers[layerIndex].selectionMode;
   
   //Sets the selection mode to map.
   
   $("#container").data("ejMap").model.layers[layerIndex].selectionMode  = 'default';

{% endhighlight %}


### layers.shapeData `object`
{:#members:layers-shapedata}

Specifies the shape data for the shape layer

#### Example

{% highlight js %}

// Set the shapeData of layer during initialization.                         
   $("#container").ejMap({layers: [{ layerType: "geometry", shapeData: mapShapeData }]})

{% endhighlight %}


{% highlight js %}
 
//Get or set the data after initialization:
   
   //Gets the data from map layer.
   
   var data =$("#container").data("ejMap").model.layers[layerIndex].shapeData;
   
   //Sets the data to map layer.
   
   $("#container").data("ejMap").model.layers[layerIndex].shapeData  = mapShapeData;

{% endhighlight %}


### layers.shapeSettings `object`
{:#members:layers-shapesettings}

Specifies the shape settings of map layer

#### Example

{% highlight js %}

// Set the shapeSettings of layer during initialization.                     
   $("#container").ejMap({layers: [{ layerType: "geometry", enableMouseHover: true, shapeSettings: { stroke: "black", fill: "#C3E6ED", highlightColor: "#63B7B7", selectionColor: "#207BB2", strokeThickness: "0.5" }, shapeData: Africa }]})

{% endhighlight %}


{% highlight js %}
 
//Get or set the shapeSettings after initialization:
   
   //Gets the shapeSettings from map.
   
   var shapeSettings =$("#container").data("ejMap").model.layers[layerIndex].shapeSettings;
   
   //Sets the shapeSettings to map.
   
   $("#container").data("ejMap").model.layers[layerIndex]  = { layerType: "geometry", enableMouseHover: true, shapeSettings: { stroke: "black", fill: "#C3E6ED", highlightColor: "#63B7B7", selectionColor: "#207BB2", strokeThickness: "0.5" }, shapeData: Africa };

{% endhighlight %}


### layers.shapeSettings.autoFill `boolean`
{:#members:layers-shapesettings-autofill}

Enables or Disables the auto fill colors for shape layer in map. When this property value set to true, shapes will be filled with palette colors.

#### Default Value

* false

#### Example

{% highlight js %}
 
//To set autoFill API value during initialization 
  $("#container").ejMap({layers: {shapeSettings: {autoFill:false}}});

{% endhighlight %}


{% highlight js %}
 
//Get or set the autoFill API, after initialization:
   
   //Gets the autoFill value 
   
   var shapeProperty =$("#container").data("ejMap").model.layers[layerIndex].shapeSettings.autoFill;
         
   //Sets the autoFill value 
   
   $("#container").data("ejMap").model.layers[0].shapeSettings.autoFill=false;
    
{% endhighlight %}


### layers.shapeSettings.colorMappings `object`
{:#members:layers-shapesettings-colormappings}

Specifies the colorMappings of the shape layer in map

#### Default Value

* null

#### Example

{% highlight js %}
 
//To set colorMappings API value during initialization 
  $("#container").ejMap({layers:{ shapeSettings: {colorMappings:{rangeColorMapping:[{from: 0,to: 100000,gradientColors: ["#9CBF4E", "#B8CE7B"]}]}}}});
{% endhighlight %}


{% highlight js %}
 
//Get or set the colorMappings API, after initialization:
   
   //Gets the colorMappings value 
   
   var shapeProperty =$("#container").data("ejMap").model.layers[layerIndex].shapeSettings.colorMappings;
    
   //Sets the colorMappings value 
   
   $("#container").data("ejMap").model.layers[0].shapeSettings.colorMappings={rangeColorMapping:[{from: 0,to: 100000,gradientColors: ["#9CBF4E", "#B8CE7B"]}]}; 
{% endhighlight %}



### layers.shapeSettings.colorMappings.rangeColorMapping `array`
{:#members:layers-shapesettings-colormappings-rangecolormapping}

Specifies the range colorMappings in the shape layer of map.

#### Default Value

* null

#### Example

{% highlight js %}
 
//To set rangeColorMapping API value during initialization 
  $("#container").ejMap({layers:{ shapeSettings: {colorMappings:{rangeColorMapping:[{from: 0,to: 100000,gradientColors: ["#9CBF4E", "#B8CE7B"]}]}}}});
{% endhighlight %}

### layers.shapeSettings.colorMappings.rangeColorMapping.from `number`
{:#members:layers-shapesettings-colormappings-rangecolormapping-from}

Specifies the start range colorMappings in the shape layer of map.

#### Default Value

* null

#### Example

{% highlight js %}
 
//To set start range colorMapping API value during initialization 
  $("#container").ejMap({layers:{ shapeSettings: {colorMappings:{rangeColorMapping:[{from: 0,to: 100000,gradientColors: ["#9CBF4E", "#B8CE7B"]}]}}}});
{% endhighlight %}

### layers.shapeSettings.colorMappings.rangeColorMapping.to `number`
{:#members:layers-shapesettings-colormappings-rangecolormapping-to}

Specifies the to range colorMappings in the shape layer of map.

#### Default Value

* null

#### Example

{% highlight js %}
 
//To set to range colorMapping API value during initialization 
  $("#container").ejMap({layers:{ shapeSettings: {colorMappings:{rangeColorMapping:[{from: 0,to: 100000,gradientColors: ["#9CBF4E", "#B8CE7B"]}]}}}});
{% endhighlight %}

### layers.shapeSettings.colorMappings.rangeColorMapping.gradientColors `array`
{:#members:layers-shapesettings-colormappings-rangecolormapping-gradientcolors}

Specifies the gradientColors in the shape layer of map.

#### Default Value

* null

#### Example

{% highlight js %}
 
//To set gradientColors API value during initialization 
  $("#container").ejMap({layers:{ shapeSettings: {colorMappings:{rangeColorMapping:[{from: 0,to: 100000,gradientColors: ["#9CBF4E", "#B8CE7B"]}]}}}});
{% endhighlight %}

### layers.shapeSettings.colorMappings.equalColorMapping `array`
{:#members:layers-shapesettings-colormappings-equalcolormapping}

Specifies the equalColorMapping in the shape layer of map.

#### Default Value

* null

#### Example

{% highlight js %}
 
//To set equalColorMapping API value during initialization 
  $("#container").ejMap({layers:{ shapeSettings: {colorMappings:{equalColorMapping:[{ value: "Romney", color: "#D84444" }]}}}});
{% endhighlight %}

### layers.shapeSettings.colorMappings.equalColorMapping.value `string`
{:#members:layers-shapesettings-colormappings-equalcolormapping-value}

Specifies the equalColorMapping value in the shape layer of map.

#### Default Value

* null

#### Example

{% highlight js %}
 
//To set equalColorMapping value API value during initialization 
  $("#container").ejMap({layers:{ shapeSettings: {colorMappings:{equalColorMapping:[{ value: "Romney", color: "#D84444" }]}}}});
{% endhighlight %}

### layers.shapeSettings.colorMappings.equalColorMapping.color `string`
{:#members:layers-shapesettings-colormappings-equalcolormapping-color}

Specifies the equalColorMapping color in the shape layer of map.

#### Default Value

* null

#### Example

{% highlight js %}
 
//To set equalColorMapping color API value during initialization 
  $("#container").ejMap({layers:{ shapeSettings: {colorMappings:{equalColorMapping:[{ value: "Romney", color: "#D84444" }]}}}});
{% endhighlight %}


{% highlight js %}
 
//Get or set the colorMappings API, after initialization:
   
   //Gets the colorMappings value 
   
   var shapeProperty =$("#container").data("ejMap").model.layers[layerIndex].shapeSettings.colorMappings;
    
   //Sets the colorMappings value 
   
   $("#container").data("ejMap").model.layers[0].shapeSettings.colorMappings={rangeColorMapping:{from: 0,to: 100000,gradientColors: ["#9CBF4E", "#B8CE7B"]}}; 
{% endhighlight %}


### layers.shapeSettings.colorPalette `enum`
{:#members:layers-shapesettings-colorpalette}

<ts name="ej.datavisualization.Map.ColorPalette"/>
Specifies the shape color palette value of the shape layer in map. Accepted colorPalette values are palette1, palette2, palette3 and custompalette.

<table class="params">
	<thead>
		<tr>
			<th>Name </th>			
			<th>Description</th>
		</tr>
	</thead>
	<tbody>
		<tr>
			<td class="name">palette1</td>			
			<td class="description">specifies the palette1 color</td>
		</tr>
		<tr>
			<td class="name">palette2</td>			
			<td class="description">specifies the palette2 color</td>
		</tr>
        <tr>
			<td class="name">palette3</td>			
			<td class="description">specifies the palette3 color</td>
		</tr>
         <tr>
			<td class="name">custompalette</td>			
			<td class="description">specifies the custom color</td>
		</tr>
	</tbody>
</table>

#### Default Value

* "palette1"

#### Example

{% highlight js %}
 
//To set colorPalette API value during initialization 
  $("#container").ejMap({layers: {shapeSettings: {colorPalette:'palette1'}}});

{% endhighlight %}


{% highlight js %}
 
//Get or set the colorPalette API, after initialization:
   
   //Gets the colorPalette value 
   
   var shapeProperty =$("#container").data("ejMap").model.layers[layerIndex].shapeSettings.colorPalette;
     
   //Sets the colorPalette value 
   
   $("#container").data("ejMap").model.layers[0].shapeSettings.colorPalette='palette1'; 

{% endhighlight %}


### layers.shapeSettings.colorValuePath `string`
{:#members:layers-shapesettings-colorvaluepath}

Specifies the shape color valuePath of the shape layer in map

#### Default Value

* null

#### Example

{% highlight js %}
 
//To set colorValuePath  API value during initialization 
  $("#container").ejMap({layers: {shapeSettings: {colorValuePath :'sales'}}});

{% endhighlight %}

{% highlight js %}
 
//Get or set the colorValuePath  API, after initialization:
   
   //Gets the colorValuePath  value 
   
   var shapeProperty =$("#container").data("ejMap").model.layers[layerIndex].shapeSettings.colorValuePath ;
  
   //Sets the colorValuePath  value 
   
   $("#container").data("ejMap").model.layers[0].shapeSettings.colorValuePath ='sales'; 

{% endhighlight %}


### layers.shapeSettings.colorPath `string`
{:#members:layers-shapesettings-colorpath}

Specifies the field name in the datasource that contains color values for each shapes.

#### Default Value

* null

#### Example

{% highlight js %}
 
//To set colorPath  API value during initialization 
  $("#container").ejMap({layers: {shapeSettings: {colorPath :'fill'}}});

{% endhighlight %}

{% highlight js %}
 
//Get or set the colorPath  API, after initialization:
   
   //Gets the colorPath  value 
   
   var shapeProperty =$("#container").data("ejMap").model.layers[layerIndex].shapeSettings.colorPath ;
  
   //Sets the colorValuePath  value 
   
   $("#container").data("ejMap").model.layers[0].shapeSettings.colorPath ='fill'; 

{% endhighlight %}


### layers.shapeSettings.enableGradient `boolean`
{:#members:layers-shapesettings-enablegradient}

Enables or Disables the gradient colors for map shapes.

#### Default Value

* false

#### Example

{% highlight js %}
 
//To set enableGradient API value during initialization 
  $("#container").ejMap({layers: {shapeSettings: {enableGradient:false}}});

{% endhighlight %}


{% highlight js %}
 
//Get or set the enableGradient API, after initialization:
   
   //Gets the enableGradient value 
   
   var shapeProperty =$("#container").data("ejMap").model.layers[layerIndex].shapeSettings.enableGradient;
   
   //Sets the enableGradient value 
   
   $("#container").data("ejMap").model.layers[0].shapeSettings.enableGradient=false; 

{% endhighlight %}


### layers.shapeSettings.fill `string`
{:#members:layers-shapesettings-fill}

Specifies the shape fill color of the shape layer in map

#### Default Value

* "#E5E5E5"

#### Example

{% highlight js %}
 
//To set fill API value during initialization 
  $("#container").ejMap({layers: {shapeSettings: {fill:'#E5E5E5'}}});

{% endhighlight %}


{% highlight js %}
 
//Get or set the fill API, after initialization:

   //Gets the fill value 
   
   var shapeProperty =$("#container").data("ejMap").model.layers[layerIndex].shapeSettings.fill;
     
   //Sets the fill value 
   
   $("#container").data("ejMap").model.layers[0].shapeSettings.fill='#E5E5E5'; 

{% endhighlight %}


### layers.shapeSettings.highlightBorderWidth `number`
{:#members:layers-shapesettings-highlightborderwidth}

Specifies the mouse over width of the shape layer in map

#### Default Value

* 1

#### Example

{% highlight js %}
 
//To set highlightBorderWidth API value during initialization 
  $("#container").ejMap({layers: {shapeSettings: {highlightBorderWidth:1}}});

{% endhighlight %}


{% highlight js %}
 
//Get or set the highlightBorderWidth API, after initialization:
   
   //Gets the highlightBorderWidth value 
   
   var shapeProperty =$("#container").data("ejMap").model.layers[layerIndex].shapeSettings.highlightBorderWidth;
     
   //Sets the highlightBorderWidth value 
   
   $("#container").data("ejMap").model.layers[0].shapeSettings.highlightBorderWidth=1;
    
{% endhighlight %}


### layers.shapeSettings.highlightColor `string`
{:#members:layers-shapesettings-highlightcolor}

Specifies the mouse hover color of the shape layer in map

#### Default Value

* "gray"

Example

{% highlight js %}
 
//To set highlightColor API value during initialization 
  $("#container").ejMap({layers:{shapeSettings: {highlightColor:'gray'}}});
  
{% endhighlight %}


{% highlight js %}
 
//Get or set the highlightColor API, after initialization:
   
   //Gets the highlightColor value 
   
   var shapeProperty =$("#container").data("ejMap").model.layers[layerIndex].shapeSettings.highlightColor;
   
   //Sets the highlightColor value 
   
   $("#container").data("ejMap").model.layers[0].shapeSettings.highlightColor='gray'; 

{% endhighlight %}


### layers.shapeSettings.highlightStroke `string`
{:#members:layers-shapesettings-highlightstroke}

Specifies the mouse over stroke color of the shape layer in map

#### Default Value

* "#C1C1C1"

#### Example

{% highlight js %}
 
//To set highlightStroke API value during initialization 
  $("#container").ejMap({layers: {shapeSettings: {highlightStroke:'#C1C1C1'}}});

{% endhighlight %}


{% highlight js %}
 
//Get or set the highlightStroke API, after initialization:
   
   //Gets the highlightStroke value 
   
   var shapeProperty =$("#container").data("ejMap").model.layers[layerIndex].shapeSettings.highlightStroke;
  
   //Sets the highlightStroke value 
   
   $("#container").data("ejMap").model.layers[0].shapeSettings.highlightStroke='#C1C1C1'; 

{% endhighlight %}


### layers.shapeSettings.selectionColor `string`
{:#members:layers-shapesettings-selectioncolor}

Specifies the shape selection color of the shape layer in map

#### Default Value

* "gray"

#### Example

{% highlight js %}
 
//To set selectionColor API value during initialization 
  $("#container").ejMap({layers: {shapeSettings: {selectionColor:'gray'}}});

{% endhighlight %}


{% highlight js %}
 
//Get or set the selectionColor API, after initialization:
   
   //Gets the selectionColor value 
   
   var shapeProperty =$("#container").data("ejMap").model.layers[layerIndex].shapeSettings.selectionColor;
   
   //Sets the selectionColor value 
   
   $("#container").data("ejMap").model.layers[0].shapeSettings.selectionColor='gray'; 

{% endhighlight %}


### layers.shapeSettings.selectionStroke `string`
{:#members:layers-shapesettings-selectionstroke}

Specifies the shape selection stroke color of the shape layer in map

#### Default Value

* "#C1C1C1"

#### Example

{% highlight js %}
 
//To set selectionStroke API value during initialization 
  $("#container").ejMap({layers: {shapeSettings: {selectionStroke:'#C1C1C1'}}});

{% endhighlight %}


{% highlight js %}
 
//Get or set the selectionStroke API, after initialization:
   
   //Gets the selectionStroke value 
   
   var shapeProperty =$("#container").data("ejMap").model.layers[layerIndex].shapeSettings.selectionStroke;
  
   //Sets the selectionStroke value 
   
   $("#container").data("ejMap").model.layers[0].shapeSettings.selectionStroke='#C1C1C1'; 

{% endhighlight %}


### layers.shapeSettings.selectionStrokeWidth `number`
{:#members:layers-shapesettings-selectionstrokewidth}

Specifies the shape selection stroke width of the shape layer in map

#### Default Value

* 1

#### Example

{% highlight js %}
 
//To set selectionStrokeWidth API value during initialization 
  $("#container").ejMap({layers: {shapeSettings: {selectionStrokeWidth:1}}});

{% endhighlight %}


{% highlight js %}
 
//Get or set the selectionStrokeWidth API, after initialization:
   
   //Gets the selectionStrokeWidth value 
   
   var shapeProperty =$("#container").data("ejMap").model.layers[layerIndex].shapeSettings.selectionStrokeWidth;
     
   //Sets the selectionStrokeWidth value 
   
   $("#container").data("ejMap").model.layers[0].shapeSettings.selectionStrokeWidth=1; 

{% endhighlight %}


### layers.shapeSettings.stroke `string`
{:#members:layers-shapesettings-stroke}

Specifies the shape stroke color of the shape layer in map

#### Default Value

* "#C1C1C1"

#### Example

{% highlight js %}
 
//To set stroke API value during initialization 
  $("#container").ejMap({layers: {shapeSettings: {stroke:'#C1C1C1'}}});

{% endhighlight %}


{% highlight js %}
 
//Get or set the stroke API, after initialization:
   
   //Gets the stroke value 
   
   var shapeProperty =$("#container").data("ejMap").model.layers[layerIndex].shapeSettings.stroke;
   
   //Sets the stroke value 
   
   $("#container").data("ejMap").model.layers[0].shapeSettings.stroke='#C1C1C1'; 

{% endhighlight %}


### layers.shapeSettings.strokeThickness `number`
{:#members:layers-shapesettings-strokethickness}

Specifies the shape stroke thickness value of the shape layer in map

#### Default Value

* "0.2"

#### Example

{% highlight js %}
 
//To set strokeThickness API value during initialization 
  $("#container").ejMap({layers: {shapeSettings: {strokeThickness:'0.2'}}});

{% endhighlight %}


{% highlight js %}
 
//Get or set the strokeThickness API, after initialization:
   
   //Gets the strokeThickness value 
   
   var shapeProperty =$("#container").data("ejMap").model.layers[layerIndex].shapeSettings.strokeThickness;
  
   //Sets the strokeThickness value 
   
   $("#container").data("ejMap").model.layers[0].shapeSettings.strokeThickness='0.2'; 

{% endhighlight %}


### layers.shapeSettings.valuePath `string`
{:#members:layers-shapesettings-valuepath}

Specifies the shape valuePath of the shape layer in map

#### Default Value

* null

#### Example

{% highlight js %}
 
//To set valuePath API value during initialization 
  $("#container").ejMap({layers: {shapeSettings: {valuePath:'name'}}});

{% endhighlight %}


{% highlight js %}
 
//Get or set the valuePath API, after initialization:
   
   //Gets the valuePath value 
   
   var shapeProperty =$("#container").data("ejMap").model.layers[layerIndex].shapeSettings.valuePath;
        
   //Sets the valuePath value 
   
   $("#container").data("ejMap").model.layers[0].shapeSettings.valuePath='name'; 

{% endhighlight %}


### layers.showMapItems `boolean`
{:#members:layers-showmapitems}

Shows or hides the map items.

#### Default Value

* false

#### Example

{% highlight js %}
  
// Set the showMapItems during initialization.                  
   $("#container").ejMap({layers: [{ showMapItems:false }]})

{% endhighlight %}


{% highlight js %}
 
//Get or set the showMapItems after initialization:

  //Gets the showMapItems from map.

  var property =$("#container").data("ejMap").model.layers[layerIndex].showMapItems;

  //Sets the showMapItems to map.

  $("#container").data("ejMap").model.layers[layerIndex].showMapItems  = false;

{% endhighlight %}


### layers.showTooltip `boolean`
{:#members:layers-showtooltip}

Shows or hides the tooltip for shapes

#### Default Value

* false

#### Example

{% highlight js %}
  
// Set the showTooltip during initialization.                   
   $("#container").ejMap({layers: [{ showTooltip:false }]})

{% endhighlight %}


{% highlight js %}
 
//Get or set the showTooltip after initialization:

  //Gets the showTooltip from map.

  var property =$("#container").data("ejMap").model.layers[layerIndex].showTooltip;

  //Sets the showTooltip to map.

  $("#container").data("ejMap").model.layers[layerIndex].showTooltip  = false;

{% endhighlight %}


### layers.tooltipTemplate `string`
{:#members:layers-tooltiptemplate}

Specifies the tooltip template for shapes.

#### Example

{% highlight js %}

// Set the tooltipTemplate of layer during initialization.                   
        $("#container").ejMap({layers: [{ layerType: "geometry", tooltipTemplate: "Template",  shapeData: mapShapeData }]})

{% endhighlight %}


{% highlight js %}
 
//Get or set the tooltipTemplate after initialization:
   
   //Gets the tooltipTemplate from map.
   
   var tooltipTemplate =$("#container").data("ejMap").model.layers[layerIndex].tooltipTemplate;
   
   //Sets the tooltipTemplate to map.
   
   $("#container").data("ejMap").model.layers[layerIndex].tooltipTemplate  ="Template";

{% endhighlight %}


### layers.urlTemplate `string`
{:#members:layers-urltemplate}

Specifies the URL template for the OSM type map.

#### Default Value

* 'http://a.tile.openstreetmap.org/level/tileX/tileY.png'

#### Example

{% highlight js %}
  
// Set the urlTemplate during initialization.                   
   $("#container").ejMap({layers: [{ urlTemplate:'http://a.tile.openstreetmap.org/level/tileX/tileY.png' }]})

{% endhighlight %}


{% highlight js %}
 
//Get or set the urlTemplate after initialization:
 
   //Gets the urlTemplate from map.
  
   var property =$("#container").data("ejMap").model.layers[layerIndex].urlTemplate;
   
   //Sets the urlTemplate to map.
   
   $("#container").data("ejMap").model.layers[layerIndex].urlTemplate  = 'http://a.tile.openstreetmap.org/level/tileX/tileY.png';

{% endhighlight %}

### layers.subLayers `array`
{:#members:layers-sublayers}

Sublayer is the collection of shape Layer 


### layers.subLayers.bingMapType `enum`
{:#members:layers-sublayers-bingmaptype}

<ts ref="ej.datavisualization.Map.BingMapType"/>

to get the type of bing map.

#### Default Value

* "aerial"

#### Example

{% highlight js %}
  
// Set the type of bing map during initialization.                      
   $("#container").ejMap({layers: [{ sublayers: [{ bingMapType:'aerial' }]} ]})

{% endhighlight %}


{% highlight js %}
 
//Get or set the type of bing map after initialization:

  //Gets the type of bing map.

  var property =$("#container").data("ejMap").model.layers[layerIndex].subLayers[subLayerIndex].bingMapType;

  //Sets the type of bing map.

  $("#container").data("ejMap").model.layers[layerIndex].subLayers[subLayerIndex].bingMapType  = 'aerial';
  
{% endhighlight %}


### layers.subLayers.bubbleSettings `object`
{:#members:layers-sublayers-bubblesettings}

Specifies the bubble settings for map

#### Example

{% highlight js %}
 
// Set the bubbleSettings of layer during initialization.                       
   $("#container").ejMap({layers: [{ sublayers: [{ layerType: "geometry", enableMouseHover: true, shapeSettings: { stroke: "black", fill: "#C3E6ED", highlightColor: "#63B7B7", selectionColor: "#207BB2", strokeThickness: "0.5" },bubbleSettings:{ valuePath: "valuePath", minValue: 20, maxValue: 30, color: "#379F64",}, shapeData: mapShapeData }]} ]})

{% endhighlight %}


{% highlight js %}
 
//Get or set the bubbleSettings after initialization:
  
  //Gets the bubbleSettings from map.
  
  var bubbleSettings =$("#container").data("ejMap").model.layers[layerIndex].subLayers[subLayerIndex].bubbleSettings;
  
  //Sets the bubbleSettings to map.
  
  $("#container").data("ejMap").model.layers[layerIndex].subLayers[subLayerIndex].bubbleSettings  = { valuePath: "valuePath", minValue: 20, maxValue: 30, color: "#379F64"};

{% endhighlight %}


### layers.subLayers.bubbleSettings.bubbleOpacity `number`
{:#members:layers-sublayers-bubblesettings-bubbleopacity}

Specifies the bubble Opacity value of bubbles for shape layer in map

#### Default Value

* "0.9"

#### Example

{% highlight js %}
 
//To set bubbleOpacity API value during initialization 
  $("#container").ejMap({layers:[{ subLayers: [{ bubbleSettings: {bubbleOpacity:'0.9'}}] } ]);

{% endhighlight %}


{% highlight js %}
 
//Get or set the bubbleOpacity API, after initialization:

   //Gets the bubble Opacity value 
   
   var bubbleProperty =$("#container").data("ejMap").model.layers[layerIndex].subLayers[subLayerIndex].bubbleSettings.bubbleOpacity;
  
   //Sets the bubble Opacity value 
   
   $("#container").data("ejMap").model.layers[layerIndex].subLayers[subLayerIndex].bubbleSettings.bubbleOpacity='0.9'; 

{% endhighlight %}


### layers.subLayers.bubbleSettings.color `string`
{:#members:layers-sublayers-bubblesettings-color}

Specifies the mouse hover color of the shape layer in map

#### Default Value

* "gray"

#### Example

{% highlight js %}
 
//To set color API value during initialization 
    $("#container").ejMap({layers:[{ subLayers: [{ bubbleSettings: {color:'gray'}}] } ]);

{% endhighlight %}


{% highlight js %}
 
//Get or set the color API, after initialization:
   
   //Gets the color value 
   
   var bubbleProperty =$("#container").data("ejMap").model.layers[layerIndex].subLayers[subLayerIndex].bubbleSettings.color;
  
   //Sets the color value 
   
   $("#container").data("ejMap").model.layers[layerIndex].subLayers[subLayerIndex].bubbleSettings.color='gray'; 

{% endhighlight %}

### layers.subLayers.bubbleSettings.colorMappings `object`
{:#members:layers-sublayers-bubblesettings-colormappings}

Specifies the colorMappings of the shape layer in map

#### Default Value

* null

#### Example

{% highlight js %}
 
//To set colorMappings API value during initialization 
  $("#container").ejMap({layers:[{ subLayers: [{bubbleSettings: {colorMappings:{rangeColorMapping:{from: 0,to: 100000,gradientColors: ["#9CBF4E", "#B8CE7B"]} }}}]}]});
  
{% endhighlight %}


{% highlight js %}
 
//Get or set the colorMappings API, after initialization:
   
   //Gets the colorMappings value 
   
   var bubbleProperty =$("#container").data("ejMap").model.layers[layerIndex].subLayers[subLayerIndex].bubbleSettings.colorMappings;
  
   //Sets the colorMappings value 
   
   $("#container").data("ejMap").model.layers[layerIndex].subLayers[subLayerIndex].bubbleSettings.colorMappings={rangeColorMapping:{from: 0,to: 100000,gradientColors: ["#9CBF4E", "#B8CE7B"]} ]}}; 

{% endhighlight %}

### layers.subLayers.bubbleSettings.colorMappings.rangeColorMapping `array`
{:#members:layers-sublayers-bubbleSettings-colormappings-rangecolormapping}

Specifies the range colorMappings in the bubble layer.

#### Default Value

* null
### layers.subLayers.bubbleSettings.colorMappings.rangeColorMapping.from `number`
{:#members:layers-sublayers-bubbleSettings-colormappings-rangecolormapping-from}

Start range colorMappings in the bubble layer.

#### Default Value

* null

#### Example

{% highlight js %}
 
//To set start range colorMapping API value during initialization 
  $("#container").ejMap({layers:[{ subLayers:[{ bubbleSettings: {colorMappings:{rangeColorMapping:[{from: 0,to: 100000,gradientColors: ["#9CBF4E", "#B8CE7B"]} ]}} }]}]});
{% endhighlight %}

### layers.subLayers.bubbleSettings.colorMappings.rangeColorMapping.to `number`
{:#members:layers-sublayers-bubbleSettings-colormappings-rangecolormapping-to}

End range colorMappings in the bubble layer.

#### Default Value

* null

#### Example

{% highlight js %}
 
//To set to range colorMapping API value during initialization 
  $("#container").ejMap({layers:[{ subLayers: [{ bubbleSettings: {colorMappings:{rangeColorMapping:[{from: 0,to: 100000,gradientColors: ["#9CBF4E", "#B8CE7B"]} ]}}}]}}]});
{% endhighlight %}

### layers.subLayers.bubbleSettings.colorMappings.rangeColorMapping.gradientColors `array`
{:#members:layers-sublayers-bubbleSettings-colormappings-rangecolormapping-gradientcolors}

GradientColors in the bubble layer of map.

### layers.subLayers.bubbleSettings.colorMappings.rangeColorMapping.color `string`
{:#members:layers-sublayers-bubbleSettings-colormappings-rangecolormapping-gradientcolors}

Color of the bubble layer.


#### Default Value

* null

#### Example

{% highlight js %}
 
//To set gradientColors API value during initialization 
  $("#container").ejMap({layers:[{ subLayers:[{ bubbleSettings: {colorMappings:{rangeColorMapping:[{from: 0,to: 100000,color:"#9CBF4E"}]}}]}]});
{% endhighlight %}


### layers.subLayers.bubbleSettings.colorValuePath `string`
{:#members:layers-sublayers-bubblesettings-colorvaluepath}

Specifies the bubble color valuePath of the shape layer in map

#### Default Value

* null

#### Example

{% highlight js %}
 
//To set colorValuePath  API value during initialization 
  $("#container").ejMap({layers:[{ subLayers: [{bubbleSettings: {colorValuePath :'sales'}}]}]});

{% endhighlight %}


{% highlight js %}
 
//Get or set the colorValuePath  API, after initialization:
   //Gets the colorValuePath  value 
   
   var bubbleProperty =$("#container").data("ejMap").model.layers[layerIndex].subLayers[subLayerIndex].bubbleSettings.colorValuePath ;
        
   //Sets the colorValuePath  value 
   
   $("#container").data("ejMap").model.layers[layerIndex].subLayers[subLayersIndex].bubbleSettings.colorValuePath ='sales'; 

{% endhighlight %}

### layers.subLayers.bubbleSettings.colorPath `string`
{:#members:layers-sublayers-bubblesettings-colorpath}

Specifies the field name in the datasource that contains color values for each bubbles.

#### Default Value

* null

#### Example

{% highlight js %}
 
//To set colorPath  API value during initialization 
  $("#container").ejMap({layers:[{ subLayers: [{bubbleSettings: {colorPath :'fill'}}]}]});

{% endhighlight %}


{% highlight js %}
 
//Get or set the colorPath  API, after initialization:
   //Gets the colorPath  value 
   
   var bubbleProperty =$("#container").data("ejMap").model.layers[layerIndex].subLayers[subLayerIndex].bubbleSettings.colorPath ;
        
   //Sets the colorPath  value 
   
   $("#container").data("ejMap").model.layers[layerIndex].subLayers[subLayersIndex].bubbleSettings.colorPath ='fill'; 

{% endhighlight %}

### layers.subLayers.bubbleSettings.maxValue `number`
{:#members:layers-sublayers-bubblesettings-maxvalue}

Specifies the maximum size value of bubbles for shape layer in map

#### Default Value

* "20"

#### Example

{% highlight js %}
 
//To set maxValue API value during initialization 
  $("#container").ejMap({layers:[{ subLayers: [{bubbleSettings: {maxValue:'20'}}]}] });
  
{% endhighlight %}


{% highlight js %}
 
//Get or set the maxValue API, after initialization:
   
   //Gets the maxValue value 
   
   var bubbleProperty =$("#container").data("ejMap").model.layers[layerIndex].subLayers[subLayerIndex].bubbleSettings.maxValue;
       
   //Sets the maxValue value 
   
   $("#container").data("ejMap").model.layers[layerIndex].subLayers[subLayersIndex].bubbleSettings.maxValue='20'; 

{% endhighlight %}


### layers.subLayers.bubbleSettings.minValue  `number`
{:#members:layers-sublayers-bubblesettings-minvalue}

Specifies the minimum size value of bubbles for shape layer in map

#### Default Value

* "10"

#### Example

{% highlight js %}
 
//To set minValue API value during initialization 
  $("#container").ejMap({layers:[{ subLayers: [{bubbleSettings: {minValue:'10'}}]}]});

{% endhighlight %}


{% highlight js %}
 
//Get or set the minValue API, after initialization:
   
   //Gets the minValue value 
   
   var bubbleProperty =$("#container").data("ejMap").model.layers[layerIndex].subLayers[subLayerIndex].bubbleSettings.minValue;
       
   //Sets the minValue value 
   
   $("#container").data("ejMap").model.layers[layerIndex].subLayers[subLayersIndex].bubbleSettings.minValue='10'; 

{% endhighlight %}


### layers.subLayers.bubbleSettings.showBubble `boolean`
{:#members:layers-sublayers-bubblesettings-showbubble}

Specifies the showBubble visibility status map

#### Default Value

* true

#### Example

{% highlight js %}
 
//To set showBubble API value during initialization 
  $("#container").ejMap({layers:[{ subLayers: [{bubbleSettings: {showBubble:true}}]}]});
  
{% endhighlight %}


{% highlight js %}
 
//Get or set the showBubble API, after initialization:
   
   //Gets the showBubble value 
   
   var bubbleProperty =$("#container").data("ejMap").model.layers[layerIndex].subLayers[subLayerIndex].bubbleSettings.showBubble;
     
   //Sets the showBubble value 
   
   $("#container").data("ejMap").model.layers[layerIndex].subLayers[subLayersIndex].bubbleSettings.showBubble=true; 

{% endhighlight %}


### layers.subLayers.bubbleSettings.showTooltip `boolean`
{:#members:layers-sublayers-bubblesettings-showtooltip}

Specifies the tooltip visibility status of the shape layer in map

#### Default Value

* false

#### Example

{% highlight js %}
 
//To set showTooltip API value during initialization 
  $("#container").ejMap({layers:[{ subLayers: [{bubbleSettings: {showTooltip:false}}]}]});

{% endhighlight %}


{% highlight js %}
 
//Get or set the showTooltip API, after initialization:
   
   //Gets the showTooltip value 
   
   var bubbleProperty =$("#container").data("ejMap").model.layers[layerIndex].subLayers[subLayerIndex].bubbleSettings.showTooltip;
    
   //Sets the showTooltip value 
   
   $("#container").data("ejMap").model.layers[layerIndex].subLayers[subLayersIndex].bubbleSettings.showTooltip=false; 

{% endhighlight %}


### layers.subLayers.bubbleSettings.tooltipTemplate `string`
{:#members:layers-sublayers-bubblesettings-tooltiptemplate}

Specifies the bubble tooltip template of the shape layer in map

#### Default Value

* null

#### Example

{% highlight js %}
 
//To set tooltipTemplate API value during initialization 
  $("#container").ejMap({layers:[{ subLayers: [{bubbleSettings: {tooltipTemplate:'template'}}]}]});

{% endhighlight %}


{% highlight js %}
 
//Get or set the tooltipTemplate API, after initialization:
   
   //Gets the tooltipTemplate value 
   
   var bubbleProperty =$("#container").data("ejMap").model.layers[layerIndex].subLayers[subLayerIndex].bubbleSettings.tooltipTemplate;
        
   //Sets the tooltipTemplate value 
   
   $("#container").data("ejMap").model.layers[layerIndex].subLayers[subLayersIndex].bubbleSettings.tooltipTemplate='template'; 

{% endhighlight %}


### layers.subLayers.bubbleSettings.valuePath `string`
{:#members:layers-sublayers-bubblesettings-valuepath}

Specifies the bubble valuePath of the shape layer in map

#### Default Value

* null

#### Example

{% highlight js %}
 
//To set valuePath API value during initialization 
  $("#container").ejMap({layers:[{ subLayers: [{bubbleSettings: {valuePath:'name'}}]}]});

{% endhighlight %}


{% highlight js %}
 
//Get or set the valuePath API, after initialization:
   
   //Gets the valuePath value 
   
   var bubbleProperty =$("#container").data("ejMap").model.layers[layerIndex].subLayers[subLayerIndex].bubbleSettings.valuePath;
      
   //Sets the valuePath value 
   
   $("#container").data("ejMap").model.layers[layerIndex].subLayers[subLayersIndex].bubbleSettings.valuePath='name'; 

{% endhighlight %}


### layers.subLayers.dataSource `object`
{:#members:layers-sublayers-datasource}

Specifies the datasource for the shape layer

#### Example

{% highlight js %}

// Set the dataSource of layer during initialization.                        
   $("#container").ejMap({layers: [{ subLayers: [{ layerType: "geometry", dataSource: source,  shapeData: mapShapeData }]} ]});

{% endhighlight %}


{% highlight js %}
 
//Get or set the dataSource after initialization:
   
   //Gets the dataSource from map layer.
   
   var dataSource =$("#container").data("ejMap").model.layers[layerIndex].subLayers[subLayerIndex].dataSource;
   
   //Sets the dataSource to map layer.
   
   $("#container").data("ejMap").model.layers[layerIndex].subLayers[subLayerIndex].dataSource  = source;

{% endhighlight %}


### layers.subLayers.shapeDataPath `string`
{:#members:layers-sublayers-shapedatapath}

Specifies the data path of shape 


#### Example

{% highlight js %}

// Set the shapeDataPath of layer during initialization.                        
   $("#container").ejMap({layers: [{ subLayers: [{ shapeDataPath: "name"}]} ]});

{% endhighlight %}


{% highlight js %}
 
//Get or set the shapeDataPath after initialization:
   
   //Gets the shapeDataPath from map layer.
   
   var property =$("#container").data("ejMap").model.layers[layerIndex].subLayers[subLayerIndex].shapeDataPath;
   
   //Sets the shapeDataPath to map layer.
   
   $("#container").data("ejMap").model.layers[layerIndex].subLayers[subLayerIndex].shapeDataPath  = 'name';

{% endhighlight %}


### layers.subLayers.shapePropertyPath `string`
{:#members:layers-sublayers-shapepropertypath}

Specifies the data path of shape 


#### Example

{% highlight js %}

// Set the shapePropertyPath of layer during initialization.                        
   $("#container").ejMap({layers: [{ subLayers: [{ shapePropertyPath: "name"}]} ]});

{% endhighlight %}


{% highlight js %}
 
//Get or set the shapePropertyPath after initialization:
   
   //Gets the shapePropertyPath from map layer.
   
   var property =$("#container").data("ejMap").model.layers[layerIndex].subLayers[subLayerIndex].shapePropertyPath;
   
   //Sets the shapePropertyPath to map layer.
   
   $("#container").data("ejMap").model.layers[layerIndex].subLayers[subLayerIndex].shapePropertyPath  = 'name';

{% endhighlight %}


### layers.subLayers.enableMouseHover `boolean`
{:#members:layers-sublayers-enablemousehover}

Enables or disables the shape mouse hover

#### Default Value

* false

#### Example

{% highlight js %}
  
// Set the enableMouseHover during initialization.                      
   $("#container").ejMap({layers: [{ subLayers: [{ enableMouseHover:false }]} ]});
   {% endhighlight %}


{% highlight js %}
 
//Get or set the enableMouseHover after initialization:
   
   //Gets the enableMouseHover from map.
   
   var property =$("#container").data("ejMap").model.layers[layerIndex].subLayers[subLayerIndex].enableMouseHover;
   
   //Sets the enableMouseHover to map.
   
   $("#container").data("ejMap").model.layers[layerIndex].subLayers[subLayerIndex].enableMouseHover  = false;
   
{% endhighlight %}


### layers.subLayers.enableSelection `boolean`
{:#members:layers-sublayers-enableselection}

Enables or disables the shape selection

#### Default Value

* true

#### Example

{% highlight js %}
  
// Set the enableSelection during initialization.                       
   $("#container").ejMap({layers: [{ subLayers: [{ enableSelection:true }]} ]});

{% endhighlight %}


{% highlight js %}
 
//Get or set the enableSelection after initialization:
   
   //Gets the enableSelection from map.
   
   var property =$("#container").data("ejMap").model.layers[layerIndex].subLayers[subLayerIndex].enableSelection;
   
   //Sets the enableSelection to map.
   
   $("#container").data("ejMap").model.layers[layerIndex].subLayers[subLayerIndex].enableSelection  = true;

{% endhighlight %}


### layers.subLayers.key `string`
{:#members:layers-sublayers-key}}

to get the key of bing map

#### Default Value

* null

#### Example

{% highlight js %}
 
//to get the key of bing map during initialization 
   $("#container").ejMap({layers: [{ subLayers: [{  layerType: 'bing', key: "" }]} ]});           

{% endhighlight %}


{% highlight js %}
 
//Get or set the key of bing map after initialization:
   
   //Gets the key of bing map value 
   
   var property = =$("#container").data("ejMap").model.layers[layerIndex].subLayers[subLayerIndex].key;     
   
   //Sets the bing map key value 
   
   $("#container").data("ejMap").model.layers[layerIndex].subLayers[subLayerIndex].key = "";

{% endhighlight %}


### layers.subLayers.labelSettings `object`
{:#members:layers-sublayers-labelsettings}

Options for enabling and configuring labelSettings labelPath, smartLabelSize, labelLength etc.,


### layers.subLayers.labelSettings.enableSmartLabel `boolean`
{:#members:layers-sublayers-labelsettings-enablesmartlabel}

enable or disable the enableSmartLabel property

#### Default Value

* false

#### Example

{% highlight js %}

// Set the enableSmartLabel value of layer during initialization.                    
   $("#container").ejMap({layers:[{ subLayers: [{labelSettings: { enableSmartLabel: false}}]} ]});

{% endhighlight %}


{% highlight js %}
 
//Get or set the enableSmartLabel value after initialization:
   
   //Gets the enableSmartLabel value 
   
   var labelSettings =$("#container").data("ejMap").model.layers[layerIndex].subLayers[subLayerIndex].labelSettings.enableSmartLabel;
   
   //Sets the enableSmartLabel value
   
   $("#container").data("ejMap").model.layers[layerIndex].subLayers[subLayerIndex].labelSettings = { enableSmartLabel: false};                   

{% endhighlight %}


### layers.subLayers.labelSettings.labelLength `number`
{:#members:layers-sublayers-labelsettings-labellength}

set the labelLength property

#### Default Value

* '2'

#### Example


{% highlight js %}

// Set the labelLength value of layer during initialization.                         
   $("#container").ejMap({layers:[{subLayers: [{labelSettings: { labelLength: 2}}]} ]});

{% endhighlight %}


{% highlight js %}
 
//Get or set the labelLength value after initialization:
   
   //Gets the labelLength value 
   
   var labelSettings =$("#container").data("ejMap").model.layers[layerIndex].subLayers[subLayerIndex].labelSettings.labelLength;
   
   //Sets the labelLength value

   $("#container").data("ejMap").model.layers[layerIndex].subLayers[subLayerIndex].labelSettings = { labelLength: 2};                     

{% endhighlight %}



### layers.subLayers.labelSettings.labelPath `string`
{:#members:layers-sublayers-labelsettings-labelpath}

set the labelPath property

#### Default Value

* null

#### Example
{:.example}


{% highlight js %}

// Set the labelPath value of layer during initialization.                   
   $("#container").ejMap({layers:[{subLayers:[{ labelSettings: { labelPath: ""}}]} ]});

{% endhighlight %}


{% highlight js %}
 
//Get or set the labelPath value after initialization:
   
   //Gets the labelPath value 
   
   var labelSettings =$("#container").data("ejMap").model.layers[layerIndex].subLayers[subLayerIndex].labelSettings.labelPath;
   
   //Sets the labelPath value
   
   $("#container").data("ejMap").model.layers[layerIndex].subLayers[subLayerIndex].labelSettings = { labelPath: ""};                      

{% endhighlight %}



### layers.subLayers.labelSettings.showLabels `boolean`
{:#members:layers-sublayers-labelsettings-showlabels}

The property specifies whether to show labels or not.

#### Default Value

* false

#### Example

{% highlight js %}
// Set the showLabel value of layer during initialization.                   
   $("#container").ejMap({layers:[{ subLayers: [{labelSettings: { showLabels: false}}]} ]});
        
{% endhighlight %}


{% highlight js %}
 
//Get or set the showLabel value after initialization:
   
   //Gets the showLabel value 
   
   var labelSettings =$("#container").data("ejMap").model.layers[layerIndex].subLayers[subLayerIndex].labelSettings.showLabels;
   
   //Sets the showLabel value
   
   $("#container").data("ejMap").model.layers[layerIndex].subLayers[subLayerIndex].labelSettings = { showLabels: false};                  

{% endhighlight %}


### layers.subLayers.labelSettings.smartLabelSize `enum`
{:#members:layers-sublayers-labelsettings-smartlabelsize}

<ts ref="ej.datavisualization.Map.LabelSize"/>

set the smartLabelSize property

#### Default Value

* "fixed"

#### Example

{% highlight js %}
// Set the smartLabelSize value of layer during initialization.                      
   $("#container").ejMap({layers:[{ subLayers:[{ labelSettings: { smartLabelSize: 'fixed'}}]} ]});
 
 {% endhighlight %}


{% highlight js %}
 
//Get or set the smartLabelSize value after initialization:
   
   //Gets the smartLabelSize value 
   
   var labelSettings =$("#container").data("ejMap").model.layers[layerIndex].subLayers[subLayerIndex].labelSettings.smartLabelSize;
   
   //Sets the smartLabelSize value
   
   $("#container").data("ejMap").model.layers[layerIndex].subLayers[subLayerIndex].labelSettings = { smartLabelSize: 'fixed'};                    

{% endhighlight %}



### layers.subLayers.geometryType `enum`
{:#members:layers-sublayers-geometrytype}

<ts ref="ej.datavisualization.Map.GeometryType"/>

Specifies the map view type.

#### Default Value

* 'geographic'

#### Example

{% highlight js %}
  
// Set the geometryType during initialization.                     
   $("#container").ejMap({layers: [{ subLayers: [{ geometryType:'geographic' }]} ]});
{% endhighlight %}


{% highlight js %}
 
//Get or set the geometryType after initialization:
   
   //Gets the geometryType from map.
   
   var property =$("#container").data("ejMap").model.layers[layerIndex].subLayers[subLayerIndex].geometryType;
   
   //Sets the geometryType to map.
   
   $("#container").data("ejMap").model.layers[layerIndex].subLayers[subLayerIndex].geometryType  = 'normal';

{% endhighlight %}


### layers.subLayers.layerType `enum`
{:#members:layers-sublayers-layertype}

<ts ref="ej.datavisualization.Map.LayerType"/>

Specifies the map type.

#### Default Value

* 'geometry'

#### Example

{% highlight js %}
  
// Set the layerType during initialization.                     
   $("#container").ejMap({layers: [{ sublayers: [{ layerType:'geometry' }]} ]});
{% endhighlight %}


{% highlight js %}
 
//Get or set the layerType after initialization:
   
   //Gets the layerType from map.
   
   var property =$("#container").data("ejMap").model.layers[layerIndex].subLayers[subLayerIndex].layerType;
   
   //Sets the layerType to map.
   
   $("#container").data("ejMap").model.layers[layerIndex].subLayers[subLayerIndex].layerType  = 'geometry';

{% endhighlight %}


### layers.subLayers.legendSettings `object`
{:#members:layers-sublayers-legendsettings}

Options for enabling and configuring legendSettings position, height, width, mode, type etc.,


### layers.subLayers.legendSettings.dockOnMap `boolean`
{:#members:layers-sublayers-legendsettings-dockonmap}

Determines whether the legend should be placed outside or inside the map bounds

#### Default Value

* false

#### Example

{% highlight js %}
 
//To set dockOnMap API value during initialization 
   $("#container").ejMap({layers: [{ subLayers: [{legendSettings: {dockOnMap:false} }]} ]});           

{% endhighlight %}


{% highlight js %}
 
//Get or set the dockOnMap API, after initialization:
   
   //Gets the dockOnMap value 
   
   var property = =$("#container").data("ejMap").model.layers[layerIndex].subLayers[subLayerIndex].legendSettings.dockOnMap;        
   
   //Sets the dockOnMap value 
   
   $("#container").data("ejMap").model.layers[layerIndex].subLayers[subLayerIndex].legendSettings  = {dockOnMap:false};

{% endhighlight %}


### layers.subLayers.legendSettings.dockPosition `enum`
{:#members:layers-sublayers-legendsettings-dockposition}

<ts ref="ej.datavisualization.Map.DockPosition"/>

Determines the legend placement and it is valid only when dockOnMap is true

#### Default Value

* "top"

#### Example

{% highlight js %}
 
//To set dockPosition value during initialization 
   $("#container").ejMap({layers: [{ subLayers: [{legendSettings: {dockPosition:"top"} }]} ]});           

{% endhighlight %}


{% highlight js %}
 
//Get or set dockPosition value after initialization:
  
  //Gets the dockPosition value
  
  var property = =$("#container").data("ejMap").model.layers[layerIndex].subLayers[subLayerIndex].legendSettings.dockPosition;     
  
  //Sets the dockPosition value value 
  
  $("#container").data("ejMap").model.layers[layerIndex].subLayers[subLayerIndex].legendSettings  = {dockPosition:"top"};

{% endhighlight %}


### layers.subLayers.legendSettings.height `number`
{:#members:layers-sublayers-legendsettings-height}

height value for legend setting

#### Default Value

* 0

#### Example

{% highlight js %}
 
//To set height value for legend during initialization 
   $("#container").ejMap({layers: [{ subLayers: [{legendSettings: {height:20} }]} ]});           

{% endhighlight %}


{% highlight js %}
 
//Get or set the height value for legend, after initialization:
   
   //Gets the height value for legend value 
   
   var property = =$("#container").data("ejMap").model.layers[layerIndex].subLayers[subLayerIndex].legendSettings.height;   
   
   //Sets the height value for legend value 
   
   $("#container").data("ejMap").model.layers[layerIndex].subLayers[subLayerIndex].legendSettings  = {height:20};
   
{% endhighlight %}


### layers.subLayers.legendSettings.icon `enum`
{:#members:layers-sublayers-legendsettings-icon}

<ts ref="ej.datavisualization.Map.LegendIcons"/>

to get icon value for legend setting

#### Default Value

* "rectangle"

#### Example


{% highlight js %}
 
//To set icon value during initialization 
   $("#container").ejMap({layers: [{ subLayers: [{legendSettings: {icon:"rectangle"} }]} ]});           

{% endhighlight %}


{% highlight js %}
 
//Get or set icon value after initialization:
   
   //Gets the icon value value 
   
   var property = =$("#container").data("ejMap").model.layers[layerIndex].subLayers[subLayerIndex].legendSettings.icon;     
   
   //Sets the icon value value 
   
   $("#container").data("ejMap").model.layers[layerIndex].subLayers[subLayerIndex].legendSettings  = {icon:"rectangle"};

{% endhighlight %}


### layers.subLayers.legendSettings.iconHeight `number`
{:#members:layers-sublayers-legendsettings-iconheight}

icon height value for legend setting

#### Default Value

* 20

#### Example

{% highlight js %}
 
//To set iconHeight value for legend during initialization 
   $("#container").ejMap({layers: [{ subLayers: [{legendSettings: {iconHeight:20} }]} ]}) ;          

{% endhighlight %}


{% highlight js %}
 
//Get or set the iconHeight value for legend, after initialization:
   
   //Gets the iconHeight value for legend value 
   
   var property = =$("#container").data("ejMap").model.layers[layerIndex].subLayers[subLayerIndex].legendSettings.iconHeight;       
   
   //Sets the iconHeight value for legend value 
   
   $("#container").data("ejMap").model.layers[layerIndex].subLayers[subLayerIndex].legendSettings  = {iconHeight:20};

{% endhighlight %}


### layers.subLayers.legendSettings.iconWidth `number`
{:#members:layers-sublayers-legendsettings-iconwidth}

icon Width value for legend setting

#### Default Value:

* 20

#### Example


{% highlight js %}
 
//To set iconWidth value for legend during initialization 
   $("#container").ejMap({layers: [{ subLayers: [{legendSettings: {iconWidth:20} }]} ]});           

{% endhighlight %}

{% highlight js %}
 
//Get or set the iconWidth value for legend, after initialization:
   
   //Gets the iconWidth value for legend value 
   
   var property = =$("#container").data("ejMap").model.layers[layerIndex].subLayers[subLayerIndex].legendSettings.iconWidth;        
   
   //Sets the iconWidth value for legend value 
   
   $("#container").data("ejMap").model.layers[layerIndex].subLayers[subLayerIndex].legendSettings  = {iconWidth:20};
   
{% endhighlight %}


### layers.subLayers.legendSettings.labelOrientation `enum`
{:#members:layers-sublayers-legendsettings-labelorientation}

<ts ref="ej.datavisualization.Map.LabelOrientation"/>

set the orientation of legend labels

#### Default Value

* vertical

#### Example

{% highlight js %}
 
//To set label orientation API value for legend setting during initialization 
   $("#container").ejMap({layers: [{ subLayers: [{legendSettings: {labelOrientation: "vertical"} }]} ]});                      

{% endhighlight %}


{% highlight js %}
 
//Get or set the label orientation API, after initialization:
   
   //Gets the label orientation value 
   
   var property = =$("#container").data("ejMap").model.layers[layerIndex].subLayers[subLayerIndex].legendSettings.labelOrientation; 
   
   //Sets the label orientation value 
   
   $("#container").data("ejMap").model.layers[layerIndex].subLayers[subLayerIndex].legendSettings  = {labelOrientation: "vertical"};

{% endhighlight %}


### layers.subLayers.legendSettings.leftLabel `string`
{:#members:layers-sublayers-legendsettings-leftlabel}

to get leftLabel value for legend setting

#### Default Value

* null

#### Example

{% highlight js %}
 
//To set leftLabel value during initialization 
   $("#container").ejMap({layers: [{ subLayers: [{legendSettings: {leftLabel:""} }]} ]});           

{% endhighlight %}


{% highlight js %}
 
//Get or set leftLabel value after initialization:
   
   //Gets the leftLabel value value 
   
   var property = =$("#container").data("ejMap").model.layers[layerIndex].subLayers[subLayerIndex].legendSettings.leftLabel;        
   
   //Sets the leftLabel value value 
   
   $("#container").data("ejMap").model.layers[layerIndex].subLayers[subLayerIndex].legendSettings  = {leftLabel:""};

{% endhighlight %}


### layers.subLayers.legendSettings.textPath `string`
{:#members:layers-sublayers-legendsettings-textPath}

To get the field name in the datasource for generating legend items.

#### Default Value

* null

#### Example

{% highlight js %}
 
//To set textPath value during initialization 
   $("#container").ejMap({layers: [{ subLayers: [{legendSettings: {textPath:""} }]} ]});           

{% endhighlight %}


{% highlight js %}
 
//Get or set textPath value after initialization:
   
   //Gets the textPath value value 
   
   var property = =$("#container").data("ejMap").model.layers[layerIndex].subLayers[subLayerIndex].legendSettings.textPath;        
   
   //Sets the textPath value value 
   
   $("#container").data("ejMap").model.layers[layerIndex].subLayers[subLayerIndex].legendSettings  = {textPath:""};

{% endhighlight %}


### layers.subLayers.legendSettings.mode `enum`
{:#members:layers-sublayers-legendsettings-mode}

<ts ref="ej.datavisualization.Map.Mode"/>

to get mode of legend setting

#### Default Value

* "default"

#### Example

{% highlight js %}
 
//To set legend mode during initialization 
   $("#container").ejMap({layers: [{ subLayers: [{legendSettings: {mode:"default"} }]} ]});
              
{% endhighlight %}


{% highlight js %}
 
//Get or set the legend mode after initialization:
   
   //Gets the legend mode value 
   
   var property = =$("#container").data("ejMap").model.layers[layerIndex].subLayers[subLayerIndex].legendSettings.mode;     
   
   //Sets the legend mode value 
   
   $("#container").data("ejMap").model.layers[layerIndex].subLayers[subLayerIndex].legendSettings  = {mode:"default"};

{% endhighlight %}


### layers.subLayers.legendSettings.position `enum`
{:#members:layers-sublayers-legendsettings-position}

<ts ref="ej.datavisualization.Map.Position"/>

set the position of legend settings

#### Default Value

* topleft

#### Example

{% highlight js %}
 
//To set legend position API value for legend setting during initialization 
   $("#container").ejMap({layers: [{ subLayers: [{legendSettings: {position: "topleft"} }]} ]});                      

{% endhighlight %}


{% highlight js %}
 
//Get or set the legend position API, after initialization:
   
   //Gets the legend position value 
   
   var property = =$("#container").data("ejMap").model.layers[layerIndex].subLayers[subLayerIndex].legendSettings.position; 
   
   //Sets the legend position value 
   
   $("#container").data("ejMap").model.layers[layerIndex].subLayers[subLayerIndex].legendSettings  = {position: "topleft"};

{% endhighlight %}


### layers.subLayers.legendSettings.positionX `number`
{:#members:layers-sublayers-legendsettings-positionx}

x position value for legend setting

#### Default Value

* 0

#### Example

{% highlight js %}
 
//To set x position value during initialization 
   $("#container").ejMap({layers: [{ subLayers: [{legendSettings: {positionX: 0} }]} ]});           

{% endhighlight %}


{% highlight js %}
 
//Get or set the x position, after initialization:
   
   //Gets the x position value 
   
   var property = =$("#container").data("ejMap").model.layers[layerIndex].subLayers[subLayerIndex].legendSettings.positionX;        
   
   //Sets the x position value 
   
   $("#container").data("ejMap").model.layers[layerIndex].subLayers[subLayerIndex].legendSettings  = {positionX: 0};

{% endhighlight %}


### layers.subLayers.legendSettings.positionY `number`
{:#members:layers-sublayers-legendsettings-positiony}

y position value for legend setting

#### Default Value

* 0

#### Example

{% highlight js %}
 
//To set y position value during initialization 
   $("#container").ejMap({layers: [{ subLayers: [{legendSettings: {positionY: 0} }]} ]});           
{% endhighlight %}


{% highlight js %}
 
//Get or set the y position, after initialization:
   
   //Gets the y position value 
   
   var property = =$("#container").data("ejMap").model.layers[layerIndex].subLayers[subLayerIndex].legendSettings.positionY;        
   
   //Sets the y position value 
   
   $("#container").data("ejMap").model.layers[layerIndex].subLayers[subLayerIndex].legendSettings  = {positionY: 0};

{% endhighlight %}


### layers.subLayers.legendSettings.rightLabel `string`
{:#members:layers-sublayers-legendsettings-rightlabel}

to get rightLabel value for legend setting

#### Default Value

* null

#### Example

{% highlight js %}
 
//To set rightLabel value during initialization 
   $("#container").ejMap({layers: [{ subLayers: [{legendSettings: {rightLabel:""} }]} ]});           

{% endhighlight %}


{% highlight js %}
 
//Get or set rightLabel value after initialization:
   
   //Gets the rightLabel value value 
   
   var property = =$("#container").data("ejMap").model.layers[layerIndex].subLayers[subLayerIndex].legendSettings.rightLabel;       
   
   //Sets the rightLabel value value 
   
   $("#container").data("ejMap").model.layers[layerIndex].subLayers[subLayerIndex].legendSettings  = {rightLabel:""};

{% endhighlight %}


### layers.subLayers.legendSettings.showLabels `boolean`
{:#members:layers-sublayers-legendsettings-showlabels}

Enables or Disables the showLabels

#### Default Value

* false

#### Example

{% highlight js %}
 
//To set showLabels API value during initialization 
   $("#container").ejMap({layers: [{ subLayers: [{legendSettings: {showLabels:false} }]} ]});           

{% endhighlight %}


{% highlight js %}
 
//Get or set the showLabels API, after initialization:
   
   //Gets the showLabels value 
   
   var property = =$("#container").data("ejMap").model.layers[layerIndex].subLayers[subLayerIndex].legendSettings.showLabels;       
   
   //Sets the showLabels value 
   
   $("#container").data("ejMap").model.layers[layerIndex].subLayers[subLayerIndex].legendSettings  = {showLabels:false};

{% endhighlight %}


### layers.subLayers.legendSettings.showLegend `boolean`
{:#members:layers-sublayers-legendsettings-showlegend}

Enables or Disables the showLegend

#### Default Value

* false

#### Example

{% highlight js %}
 
//To set showLegend API value during initialization 
   $("#container").ejMap({layers: [{ subLayers: [{legendSettings: {showLegend:false} }]} ]});

{% endhighlight %}


{% highlight js %}
 
//Get or set the showLegend API, after initialization:
   
   //Gets the showLegend value 
   
   var property = =$("#container").data("ejMap").model.layers[layerIndex].subLayers[subLayerIndex].legendSettings.showLegend;       
   
   //Sets the showLegend value 

   $("#container").data("ejMap").model.layers[layerIndex].subLayers[subLayerIndex].legendSettings  = {showLegend:false};
  
{% endhighlight %}


### layers.subLayers.legendSettings.title `string`
{:#members:layers-sublayers-legendsettings-title}

to get title of legend setting

#### Default Value

* null

#### Example

{% highlight js %}
 
//To set legend title during initialization 
   $("#container").ejMap({layers: [{ subLayers: [{legendSettings: {title: ""} }]} ]}) ;          

{% endhighlight %}


{% highlight js %}
 
//Get or set the legend title after initialization:
   
   //Gets the legend title value 
   
   var property = =$("#container").data("ejMap").model.layers[layerIndex].subLayers[subLayerIndex].legendSettings.title;    
   
   //Sets the legend title value 
   
   $("#container").data("ejMap").model.layers[layerIndex].subLayers[subLayerIndex].legendSettings  = {title: ""};

{% endhighlight %}


### layers.subLayers.legendSettings.type `enum`
{:#members:layers-sublayers-legendsettings-type}

<ts ref="ej.datavisualization.Map.LegendType"/>

to get type of legend setting

#### Default Value

* "layers"

#### Example

{% highlight js %}
 
//To set legend type value during initialization 
   $("#container").ejMap({layers: [{ subLayers: [{legendSettings: {type:"layers"} }]} ]});           

{% endhighlight %}


{% highlight js %}
 
//Get or set the legend type value after initialization:
   
   //Gets the legend type value 
   
   var property = =$("#container").data("ejMap").model.layers[layerIndex].subLayers[subLayerIndex].legendSettings.type;     
   
   //Sets the legend type value 
   
   $("#container").data("ejMap").model.layers[layerIndex].subLayers[subLayerIndex].legendSettings  = {type:"layers"};

{% endhighlight %}


### layers.subLayers.legendSettings.width `number`
{:#members:layers-sublayers-legendsettings-width}

width value for legend setting

#### Default Value

* 0

#### Example

{% highlight js %}
 
//To set width value for legend during initialization 
   $("#container").ejMap({layers: [{ subLayers: [{legendSettings: {width:20} }]} ]}) ;          

{% endhighlight %}


{% highlight js %}
 
//Get or set the width value for legend, after initialization:
   
   //Gets the width value for legend value 
   
   var property = =$("#container").data("ejMap").model.layers[layerIndex].subLayers[subLayerIndex].legendSettings.width;    
   
   //Sets the width value for legend value 
   
   $("#container").data("ejMap").model.layers[layerIndex].subLayers[subLayerIndex].legendSettings  = {width:20};

{% endhighlight %}


### layers.subLayers.mapItemsTemplate `string`
{:#members:layers-sublayers-mapitemstemplate}

Specifies the map items template for shapes.

#### Example

{% highlight js %}

// Set the mapItemsTemplate of layer during initialization.                  
   $("#container").ejMap({layers: [{ subLayers: [{ layerType: "geometry", mapItemsTemplate: "Template",  shapeData: mapShapeData }]} ]});

{% endhighlight %}


{% highlight js %}
 
//Get or set the mapItemsTemplate after initialization:
   
   //Gets the mapItemsTemplate from map.
   
   var mapItemsTemplate =$("#container").data("ejMap").model.layers[layerIndex].subLayers[subLayerIndex].mapItemsTemplate;
   
   //Sets the mapItemsTemplate to map.
   
   $("#container").data("ejMap").model.layers[layerIndex].subLayers[subLayerIndex].mapItemsTemplate  = "Template";

{% endhighlight %}


### layers.subLayers.markers `Array`
{:#members:layers-sublayers-markers}

Specify markers for shape layer.

### layers.subLayers.markers.label `string`

Display the value in the marker 

#### Default Value

* " "

#### Example

{% highlight js %}
  
// Set the markers during initialization.                       
   $("#container").ejMap({layers: [{ subLayers: [{markers:[{label : "chennai",latitude : 13.08 ,longitude : 80.27}]} ]}]} ]});

{% endhighlight %}


{% highlight js %}
 
//Get or set the markers after initialization:
   
   //Gets the markers from map.
   
   var marker =$("#container").data("ejMap").model.layers[layerIndex].subLayers[subLayerIndex].markers[markerIndex];
   
   //Sets the marker to map.
   
   $("#container").data("ejMap").model.layers[layerIndex].subLayers[subLayerIndex].markers[markerIndex]  = {label : "chennai",latitude : 13.08 ,longitude : 80.27};

{% endhighlight %}

### layers.subLayers.markers.latitude `number`

Display the value in the marker 

#### Default Value

* null

#### Example

{% highlight js %}
  
// Set the markers during initialization.                       
   $("#container").ejMap({layers: [{ subLayers: [{markers:[{label : "chennai",latitude : 13.08 ,longitude : 80.27}]} ]}]} ]});

{% endhighlight %}


{% highlight js %}
 
//Get or set the markers after initialization:
   
   //Gets the markers from map.
   
   var marker =$("#container").data("ejMap").model.layers[layerIndex].subLayers[subLayerIndex].markers[markerIndex];
   
   //Sets the marker to map.
   
   $("#container").data("ejMap").model.layers[layerIndex].subLayers[subLayerIndex].markers[markerIndex]  = {label : "chennai",latitude : 13.08 ,longitude : 80.27};

{% endhighlight %}


### layers.subLayers.markers.longitude `number`

Display the value in the marker 

#### Default Value

* null

#### Example

{% highlight js %}
  
// Set the markers during initialization.                       
   $("#container").ejMap({layers: [{ subLayers: [{markers:[{label : "chennai",latitude : 13.08 ,longitude : 80.27}]} ]}]} ]});

{% endhighlight %}


{% highlight js %}
 
//Get or set the markers after initialization:
   
   //Gets the markers from map.
   
   var marker =$("#container").data("ejMap").model.layers[layerIndex].subLayers[subLayerIndex].markers[markerIndex];
   
   //Sets the marker to map.
   
   $("#container").data("ejMap").model.layers[layerIndex].subLayers[subLayerIndex].markers[markerIndex]  = {label : "chennai",latitude : 13.08 ,longitude : 80.27};

{% endhighlight %}


### layers.subLayers.markerTemplate `string`
{:#members:layers-sublayers-markertemplate}

Specifies the map marker template for map layer.

#### Default Value

* null

#### Example

{% highlight js %}

// Set the markerTemplate of layer during initialization.                    
   $("#container").ejMap({layers: [{ subLayers: [{ layerType: "geometry", markerTemplate: "Template",  shapeData: mapShapeData }]} ]});

{% endhighlight %}


{% highlight js %}
 
//Get or set the markerTemplate after initialization:
   
   //Gets the markerTemplate from map.
   
   var markerTemplate =$("#container").data("ejMap").model.layers[layerIndex].subLayers[subLayerIndex].markerTemplate;
   
   //Sets the markerTemplate to map.
   
   $("#container").data("ejMap").model.layers[layerIndex].subLayers[subLayerIndex].markerTemplate  = "Template";

{% endhighlight %}


### layers.subLayers.selectedMapShapes `Array`
{:#members:layers-sublayers-selectedmapshapes}

Specify selectedMapShapes for shape layer

#### Default Value

* []

#### Example

{% highlight js %}
 
//Gets the selectedMapShapes from map 
   var selectedShapes =$("#container").data("ejMap").model.layers[layerIndex].subLayers[subLayerIndex].selectedMapShapes;         

{% endhighlight %}


### layers.subLayers.selectionMode `enum`
{:#members:layers-sublayers-selectionmode}

<ts ref="ej.datavisualization.Map.SelectionMode"/>

Specifies the selection mode of the map. Accepted selection mode values are Default and Multiple.


#### Default Value

* "default"

#### Example


{% highlight js %}
  
// Set the selection mode during initialization.                        
   $("#container").ejMap({layers: [{ subLayers: [{ selectionMode:'default' }]} ]});

{% endhighlight %}


{% highlight js %}
 
//Get or set the selection mode after initialization:
   
   //Gets the selection mode from map.
   
   var property =$("#container").data("ejMap").model.layers[layerIndex].subLayers[subLayerIndex].selectionMode;
   
   //Sets the selection mode to map.
   
   $("#container").data("ejMap").model.layers[layerIndex].subLayers[subLayerIndex].selectionMode  = 'default';

{% endhighlight %}


### layers.subLayers.shapeData `object`
{:#members:layers-sublayers-shapedata}

Specifies the shape data for the shape layer

#### Example

{% highlight js %}

// Set the shapeData of layer during initialization.                         
   $("#container").ejMap({layers: [{ subLayers: [{ layerType: "geometry", shapeData: mapShapeData }]} ]});

{% endhighlight %}


{% highlight js %}
 
//Get or set the data after initialization:
   
   //Gets the data from map layer.
   
   var data =$("#container").data("ejMap").model.layers[layerIndex].subLayers[subLayerIndex].shapeData;
   
   //Sets the data to map layer.
   
   $("#container").data("ejMap").model.layers[layerIndex].subLayers[subLayerIndex].shapeData  = mapShapeData;

{% endhighlight %}


### layers.subLayers.shapeSettings `object`
{:#members:layers-sublayers-shapesettings}

Specifies the shape settings of map layer

#### Example

{% highlight js %}

// Set the shapeSettings of layer during initialization.                     
   $("#container").ejMap({layers: [{ subLayers: [{ layerType: "geometry", enableMouseHover: true, shapeSettings: { stroke: "black", fill: "#C3E6ED", highlightColor: "#63B7B7", selectionColor: "#207BB2", strokeThickness: "0.5" }, shapeData: Africa }]} ]});

{% endhighlight %}


{% highlight js %}
 
//Get or set the shapeSettings after initialization:
   
   //Gets the shapeSettings from map.
   
   var shapeSettings =$("#container").data("ejMap").model.layers[layerIndex].subLayers[subLayerIndex].shapeSettings;
   
   //Sets the shapeSettings to map.
   
   $("#container").data("ejMap").model.layers[layerIndex].subLayers[subLayerIndex]  = { layerType: "geometry", enableMouseHover: true, shapeSettings: { stroke: "black", fill: "#C3E6ED", highlightColor: "#63B7B7", selectionColor: "#207BB2", strokeThickness: "0.5" }, shapeData: Africa };

{% endhighlight %}


### layers.subLayers.shapeSettings.autoFill `boolean`
{:#members:layers-sublayers-shapesettings-autofill}

Enables or Disables the auto fill colors for shape layer in map. When this property value set to true, shapes will be filled with palette colors.

#### Default Value

* false

#### Example

{% highlight js %}
 
//To set autoFill API value during initialization 
  $("#container").ejMap({layers:[{ subLayers: [{shapeSettings: {autoFill:false}}});

{% endhighlight %}


{% highlight js %}
 
//Get or set the autoFill API, after initialization:
   
   //Gets the autoFill value 
   
   var shapeProperty =$("#container").data("ejMap").model.layers[layerIndex].subLayers[subLayerIndex].shapeSettings.autoFill;
         
   //Sets the autoFill value 
   
   $("#container").data("ejMap").model.layers[layerIndex].subLayers[subLayersIndex].shapeSettings.autoFill=false;
    
{% endhighlight %}


### layers.subLayers.shapeSettings.colorMappings `object`
{:#members:layers-sublayers-shapesettings-colormappings}

Specifies the colorMappings of the shape layer in map

#### Default Value

* null

#### Example

{% highlight js %}
 
//To set colorMappings API value during initialization 
  $("#container").ejMap({layers:[{ subLayers: [{ shapeSettings: {colorMappings:{rangeColorMapping:[{from: 0,to: 100000,gradientColors: ["#9CBF4E", "#B8CE7B"]} ]}}}]}]}] });
{% endhighlight %}


{% highlight js %}
 
//Get or set the colorMappings API, after initialization:
   
   //Gets the colorMappings value 
   
   var shapeProperty =$("#container").data("ejMap").model.layers[layerIndex].subLayers[subLayerIndex].shapeSettings.colorMappings;
    
   //Sets the colorMappings value 
   
   $("#container").data("ejMap").model.layers[layerIndex].subLayers[subLayersIndex].shapeSettings.colorMappings={rangeColorMapping:[{from: 0,to: 100000,gradientColors: ["#9CBF4E", "#B8CE7B"]} ]}]} ]}; 
{% endhighlight %}



### layers.subLayers.shapeSettings.colorMappings.rangeColorMapping `array`
{:#members:layers-sublayers-shapesettings-colormappings-rangecolormapping}

Specifies the range colorMappings in the shape layer of map.

#### Default Value

* null

#### Example

{% highlight js %}
 
//To set rangeColorMapping API value during initialization 
  $("#container").ejMap({layers:[{ subLayers:[{ shapeSettings: {colorMappings:{rangeColorMapping:[{from: 0,to: 100000,gradientColors: ["#9CBF4E", "#B8CE7B"]} ]}]} ]}}}}]}]});
{% endhighlight %}

### layers.subLayers.shapeSettings.colorMappings.rangeColorMapping.from `number`
{:#members:layers-sublayers-shapesettings-colormappings-rangecolormapping-from}

Specifies the start range colorMappings in the shape layer of map.

#### Default Value

* null

#### Example

{% highlight js %}
 
//To set start range colorMapping API value during initialization 
  $("#container").ejMap({layers:{ shapeSettings: {colorMappings:{rangeColorMapping:[{from: 0,to: 100000,gradientColors: ["#9CBF4E", "#B8CE7B"]} ]}]} ]}}}});
{% endhighlight %}

### layers.subLayers.shapeSettings.colorMappings.rangeColorMapping.to `number`
{:#members:layers-sublayers-shapesettings-colormappings-rangecolormapping-to}

Specifies the to range colorMappings in the shape layer of map.

#### Default Value

* null

#### Example

{% highlight js %}
 
//To set to range colorMapping API value during initialization 
  $("#container").ejMap({layers:[{ subLayers:[{ shapeSettings: {colorMappings:{rangeColorMapping:[{from: 0,to: 100000,gradientColors: ["#9CBF4E", "#B8CE7B"]} ]}]} ]}}}]}]});
{% endhighlight %}

### layers.subLayers.shapeSettings.colorMappings.rangeColorMapping.gradientColors `array`
{:#members:layers-sublayers-shapesettings-colormappings-rangecolormapping-gradientcolors}

Specifies the gradientColors in the shape layer of map.

#### Default Value

* null

#### Example

{% highlight js %}
 
//To set gradientColors API value during initialization 
  $("#container").ejMap({layers:[{subLayers:[{ shapeSettings: {colorMappings:{rangeColorMapping:[{from: 0,to: 100000,gradientColors: ["#9CBF4E", "#B8CE7B"]} ]}]}}]} ]});
{% endhighlight %}

### layers.subLayers.shapeSettings.colorMappings.equalColorMapping `array`
{:#members:layers-sublayers-shapesettings-colormappings-equalcolormapping}

Specifies the equalColorMapping in the shape layer of map.

#### Default Value

* null

#### Example

{% highlight js %}
 
//To set equalColorMapping API value during initialization 
  $("#container").ejMap({layers:[{ subLayers:[{ shapeSettings: {colorMappings:{equalColorMapping:[{ value: "Romney", color: "#D84444" }]} ]}]}]});
{% endhighlight %}

### layers.subLayers.shapeSettings.colorMappings.equalColorMapping.value `string`
{:#members:layers-sublayers-shapesettings-colormappings-equalcolormapping-value}

Specifies the equalColorMapping value in the shape layer of map.

#### Default Value

* null

#### Example

{% highlight js %}
 
//To set equalColorMapping value API value during initialization 
  $("#container").ejMap({layers:[{ subLayers:[{ shapeSettings: {colorMappings:{equalColorMapping:[{ value: "Romney", color: "#D84444" }]}}}]}]});
{% endhighlight %}

### layers.subLayers.shapeSettings.colorMappings.equalColorMapping.color `string`
{:#members:layers-sublayers-shapesettings-colormappings-equalcolormapping-color}

Specifies the equalColorMapping color in the shape layer of map.

#### Default Value

* null

#### Example

{% highlight js %}
 
//To set equalColorMapping color API value during initialization 
  $("#container").ejMap({layers:[{ subLayers:[{ shapeSettings: {colorMappings:{equalColorMapping:[{ value: "Romney", color: "#D84444" }]}}}]}]});
{% endhighlight %}


{% highlight js %}
 
//Get or set the colorMappings API, after initialization:
   
   //Gets the colorMappings value 
   
   var shapeProperty =$("#container").data("ejMap").model.layers[layerIndex].subLayers[subLayerIndex].shapeSettings.colorMappings;
    
   //Sets the colorMappings value 
   
   $("#container").data("ejMap").model.layers[layerIndex].subLayers[subLayersIndex].shapeSettings.colorMappings={rangeColorMapping:{from: 0,to: 100000,gradientColors: ["#9CBF4E", "#B8CE7B"]} ]}}; 
{% endhighlight %}


### layers.subLayers.shapeSettings.colorPalette `enum`
{:#members:layers-sublayers-shapesettings-colorpalette}

<ts ref="ej.datavisualization.Map.ColorPalette"/>

Specifies the shape color palette value of the shape layer in map. Accepted colorPalette values are palette1, palette2, palette3 and custompalette.

#### Default Value

* "palette1"

#### Example

{% highlight js %}
 
//To set colorPalette API value during initialization 
  $("#container").ejMap({layers:[{ subLayers: [{shapeSettings: {colorPalette:'palette1'}}]}]});

{% endhighlight %}


{% highlight js %}
 
//Get or set the colorPalette API, after initialization:
   
   //Gets the colorPalette value 
   
   var shapeProperty =$("#container").data("ejMap").model.layers[layerIndex].subLayers[subLayerIndex].shapeSettings.colorPalette;
     
   //Sets the colorPalette value 
   
   $("#container").data("ejMap").model.layers[layerIndex].subLayers[subLayersIndex].shapeSettings.colorPalette='palette1'; 

{% endhighlight %}


### layers.subLayers.shapeSettings.colorValuePath `string`
{:#members:layers-sublayers-shapesettings-colorvaluepath}

Specifies the shape color valuePath of the shape layer in map

#### Default Value

* null

#### Example

{% highlight js %}
 
//To set colorValuePath  API value during initialization 
  $("#container").ejMap({layers:[{ subLayers: [{shapeSettings: {colorValuePath :'sales'}}]}]});

{% endhighlight %}

{% highlight js %}
 
//Get or set the colorValuePath  API, after initialization:
   
   //Gets the colorValuePath  value 
   
   var shapeProperty =$("#container").data("ejMap").model.layers[layerIndex].subLayers[subLayerIndex].shapeSettings.colorValuePath ;
  
   //Sets the colorValuePath  value 
   
   $("#container").data("ejMap").model.layers[layerIndex].subLayers[subLayersIndex].shapeSettings.colorValuePath ='sales'; 

{% endhighlight %}


### layers.subLayers.shapeSettings.enableGradient `boolean`
{:#members:layers-sublayers-shapesettings-enablegradient}

Enables or Disables the gradient colors for map shapes.

#### Default Value

* false

#### Example

{% highlight js %}
 
//To set enableGradient API value during initialization 
  $("#container").ejMap({layers:[{ subLayers: [{shapeSettings: {enableGradient:false}}]}]});

{% endhighlight %}


{% highlight js %}
 
//Get or set the enableGradient API, after initialization:
   
   //Gets the enableGradient value 
   
   var shapeProperty =$("#container").data("ejMap").model.layers[layerIndex].subLayers[subLayerIndex].shapeSettings.enableGradient;
   
   //Sets the enableGradient value 
   
   $("#container").data("ejMap").model.layers[layerIndex].subLayers[subLayersIndex].shapeSettings.enableGradient=false; 

{% endhighlight %}


### layers.subLayers.shapeSettings.fill `string`
{:#members:layers-sublayers-shapesettings-fill}

Specifies the shape fill color of the shape layer in map

#### Default Value

* "#E5E5E5"

#### Example

{% highlight js %}
 
//To set fill API value during initialization 
  $("#container").ejMap({layers:[{ subLayers: [{shapeSettings: {fill:'#E5E5E5'}}]}]});

{% endhighlight %}


{% highlight js %}
 
//Get or set the fill API, after initialization:

   //Gets the fill value 
   
   var shapeProperty =$("#container").data("ejMap").model.layers[layerIndex].subLayers[subLayerIndex].shapeSettings.fill;
     
   //Sets the fill value 
   
   $("#container").data("ejMap").model.layers[layerIndex].subLayers[subLayersIndex].shapeSettings.fill='#E5E5E5'; 

{% endhighlight %}


### layers.subLayers.shapeSettings.highlightBorderWidth `number`
{:#members:layers-sublayers-shapesettings-highlightborderwidth}

Specifies the mouse over width of the shape layer in map

#### Default Value

* 1

#### Example

{% highlight js %}
 
//To set highlightBorderWidth API value during initialization 
  $("#container").ejMap({layers:[{ subLayers: [{shapeSettings: {highlightBorderWidth:1}}]}]});

{% endhighlight %}


{% highlight js %}
 
//Get or set the highlightBorderWidth API, after initialization:
   
   //Gets the highlightBorderWidth value 
   
   var shapeProperty =$("#container").data("ejMap").model.layers[layerIndex].subLayers[subLayerIndex].shapeSettings.highlightBorderWidth;
     
   //Sets the highlightBorderWidth value 
   
   $("#container").data("ejMap").model.layers[layerIndex].subLayers[subLayersIndex].shapeSettings.highlightBorderWidth=1;
    
{% endhighlight %}


### layers.subLayers.shapeSettings.highlightColor `string`
{:#members:layers-sublayers-shapesettings-highlightcolor}

Specifies the mouse hover color of the shape layer in map

#### Default Value

* "gray"

Example

{% highlight js %}
 
//To set highlightColor API value during initialization 
  $("#container").ejMap({layers:[{ subLayers: [{shapeSettings: {highlightColor:'gray'}}]}]});
  
{% endhighlight %}


{% highlight js %}
 
//Get or set the highlightColor API, after initialization:
   
   //Gets the highlightColor value 
   
   var shapeProperty =$("#container").data("ejMap").model.layers[layerIndex].subLayers[subLayerIndex].shapeSettings.highlightColor;
   
   //Sets the highlightColor value 
   
   $("#container").data("ejMap").model.layers[layerIndex].subLayers[subLayersIndex].shapeSettings.highlightColor='gray'; 

{% endhighlight %}


### layers.subLayers.shapeSettings.highlightStroke `string`
{:#members:layers-sublayers-shapesettings-highlightstroke}

Specifies the mouse over stroke color of the shape layer in map

#### Default Value

* "#C1C1C1"

#### Example

{% highlight js %}
 
//To set highlightStroke API value during initialization 
  $("#container").ejMap({layers:[{ subLayers: [{shapeSettings: {highlightStroke:'#C1C1C1'}}]}]});

{% endhighlight %}


{% highlight js %}
 
//Get or set the highlightStroke API, after initialization:
   
   //Gets the highlightStroke value 
   
   var shapeProperty =$("#container").data("ejMap").model.layers[layerIndex].subLayers[subLayerIndex].shapeSettings.highlightStroke;
  
   //Sets the highlightStroke value 
   
   $("#container").data("ejMap").model.layers[layerIndex].subLayers[subLayersIndex].shapeSettings.highlightStroke='#C1C1C1'; 

{% endhighlight %}


### layers.subLayers.shapeSettings.selectionColor `string`
{:#members:layers-sublayers-shapesettings-selectioncolor}

Specifies the shape selection color of the shape layer in map

#### Default Value

* "gray"

#### Example

{% highlight js %}
 
//To set selectionColor API value during initialization 
  $("#container").ejMap({layers:[{ subLayers: [{shapeSettings: {selectionColor:'gray'}}]}]});

{% endhighlight %}


{% highlight js %}
 
//Get or set the selectionColor API, after initialization:
   
   //Gets the selectionColor value 
   
   var shapeProperty =$("#container").data("ejMap").model.layers[layerIndex].subLayers[subLayerIndex].shapeSettings.selectionColor;
   
   //Sets the selectionColor value 
   
   $("#container").data("ejMap").model.layers[layerIndex].subLayers[subLayersIndex].shapeSettings.selectionColor='gray'; 

{% endhighlight %}


### layers.subLayers.shapeSettings.selectionStroke `string`
{:#members:layers-sublayers-shapesettings-selectionstroke}

Specifies the shape selection stroke color of the shape layer in map

#### Default Value

* "#C1C1C1"

#### Example

{% highlight js %}
 
//To set selectionStroke API value during initialization 
  $("#container").ejMap({layers:[{ subLayers: [{shapeSettings: {selectionStroke:'#C1C1C1'}}]}]});

{% endhighlight %}


{% highlight js %}
 
//Get or set the selectionStroke API, after initialization:
   
   //Gets the selectionStroke value 
   
   var shapeProperty =$("#container").data("ejMap").model.layers[layerIndex].subLayers[subLayerIndex].shapeSettings.selectionStroke;
  
   //Sets the selectionStroke value 
   
   $("#container").data("ejMap").model.layers[layerIndex].subLayers[subLayersIndex].shapeSettings.selectionStroke='#C1C1C1'; 

{% endhighlight %}


### layers.subLayers.shapeSettings.selectionStrokeWidth `number`
{:#members:layers-sublayers-shapesettings-selectionstrokewidth}

Specifies the shape selection stroke width of the shape layer in map

#### Default Value

* 1

#### Example

{% highlight js %}
 
//To set selectionStrokeWidth API value during initialization 
  $("#container").ejMap({layers:[{ subLayers: [{shapeSettings: {selectionStrokeWidth:1}}]}]});

{% endhighlight %}


{% highlight js %}
 
//Get or set the selectionStrokeWidth API, after initialization:
   
   //Gets the selectionStrokeWidth value 
   
   var shapeProperty =$("#container").data("ejMap").model.layers[layerIndex].subLayers[subLayerIndex].shapeSettings.selectionStrokeWidth;
     
   //Sets the selectionStrokeWidth value 
   
   $("#container").data("ejMap").model.layers[layerIndex].subLayers[subLayersIndex].shapeSettings.selectionStrokeWidth=1; 

{% endhighlight %}


### layers.subLayers.shapeSettings.stroke `string`
{:#members:layers-sublayers-shapesettings-stroke}

Specifies the shape stroke color of the shape layer in map

#### Default Value

* "#C1C1C1"

#### Example

{% highlight js %}
 
//To set stroke API value during initialization 
  $("#container").ejMap({layers:[{ subLayers: [{shapeSettings: {stroke:'#C1C1C1'}}]}]});

{% endhighlight %}


{% highlight js %}
 
//Get or set the stroke API, after initialization:
   
   //Gets the stroke value 
   
   var shapeProperty =$("#container").data("ejMap").model.layers[layerIndex].subLayers[subLayerIndex].shapeSettings.stroke;
   
   //Sets the stroke value 
   
   $("#container").data("ejMap").model.layers[layerIndex].subLayers[subLayersIndex].shapeSettings.stroke='#C1C1C1'; 

{% endhighlight %}


### layers.subLayers.shapeSettings.strokeThickness `number`
{:#members:layers-sublayers-shapesettings-strokethickness}

Specifies the shape stroke thickness value of the shape layer in map

#### Default Value

* "0.2"

#### Example

{% highlight js %}
 
//To set strokeThickness API value during initialization 
  $("#container").ejMap({layers:[{ subLayers: [{shapeSettings: {strokeThickness:'0.2'}}]}]});

{% endhighlight %}


{% highlight js %}
 
//Get or set the strokeThickness API, after initialization:
   
   //Gets the strokeThickness value 
   
   var shapeProperty =$("#container").data("ejMap").model.layers[layerIndex].subLayers[subLayerIndex].shapeSettings.strokeThickness;
  
   //Sets the strokeThickness value 
   
   $("#container").data("ejMap").model.layers[layerIndex].subLayers[subLayersIndex].shapeSettings.strokeThickness='0.2'; 

{% endhighlight %}


### layers.subLayers.shapeSettings.valuePath `string`
{:#members:layers-sublayers-shapesettings-valuepath}

Specifies the shape valuePath of the shape layer in map

#### Default Value

* null

#### Example

{% highlight js %}
 
//To set valuePath API value during initialization 
  $("#container").ejMap({layers:[{ subLayers: [{shapeSettings: {valuePath:'name'}}]}]});

{% endhighlight %}


{% highlight js %}
 
//Get or set the valuePath API, after initialization:
   
   //Gets the valuePath value 
   
   var shapeProperty =$("#container").data("ejMap").model.layers[layerIndex].subLayers[subLayerIndex].shapeSettings.valuePath;
        
   //Sets the valuePath value 
   
   $("#container").data("ejMap").model.layers[layerIndex].subLayers[subLayersIndex].shapeSettings.valuePath='name'; 

{% endhighlight %}


### layers.subLayers.showMapItems `boolean`
{:#members:layers-sublayers-showmapitems}

Shows or hides the map items.

#### Default Value

* false

#### Example

{% highlight js %}
  
// Set the showMapItems during initialization.                  
   $("#container").ejMap({layers: [{ subLayers: [{ showMapItems:false }]} ]});

{% endhighlight %}


{% highlight js %}
 
//Get or set the showMapItems after initialization:

  //Gets the showMapItems from map.

  var property =$("#container").data("ejMap").model.layers[layerIndex].subLayers[subLayerIndex].showMapItems;

  //Sets the showMapItems to map.

  $("#container").data("ejMap").model.layers[layerIndex].subLayers[subLayerIndex].showMapItems  = false;

{% endhighlight %}


### layers.subLayers.showTooltip `boolean`
{:#members:layers-sublayers-showtooltip}

Shows or hides the tooltip for shapes

#### Default Value

* false

#### Example

{% highlight js %}
  
// Set the showTooltip during initialization.                   
   $("#container").ejMap({layers: [{ subLayers: [{ showTooltip:false }]} ]});

{% endhighlight %}


{% highlight js %}
 
//Get or set the showTooltip after initialization:

  //Gets the showTooltip from map.

  var property =$("#container").data("ejMap").model.layers[layerIndex].subLayers[subLayerIndex].showTooltip;

  //Sets the showTooltip to map.

  $("#container").data("ejMap").model.layers[layerIndex].subLayers[subLayerIndex].showTooltip  = false;

{% endhighlight %}


### layers.subLayers.tooltipTemplate `string`
{:#members:layers-sublayers-tooltiptemplate}

Specifies the tooltip template for shapes.

#### Example

{% highlight js %}

// Set the tooltipTemplate of layer during initialization.                   
        $("#container").ejMap({layers: [{ subLayers: [{ layerType: "geometry", tooltipTemplate: "Template",  shapeData: mapShapeData }]} ]});

{% endhighlight %}


{% highlight js %}
 
//Get or set the tooltipTemplate after initialization:
   
   //Gets the tooltipTemplate from map.
   
   var tooltipTemplate =$("#container").data("ejMap").model.layers[layerIndex].subLayers[subLayerIndex].tooltipTemplate;
   
   //Sets the tooltipTemplate to map.
   
   $("#container").data("ejMap").model.layers[layerIndex].subLayers[subLayerIndex].tooltipTemplate  ="Template";

{% endhighlight %}


### layers.subLayers.urlTemplate `string`
{:#members:layers-sublayers-urltemplate}

Specifies the URL template for the OSM type map.

#### Default Value

* 'http://a.tile.openstreetmap.org/level/tileX/tileY.png'

#### Example

{% highlight js %}
  
// Set the urlTemplate during initialization.                   
   $("#container").ejMap({layers: [{ subLayers: [{ urlTemplate:'http://a.tile.openstreetmap.org/level/tileX/tileY.png' }]} ]});

{% endhighlight %}


{% highlight js %}
 
//Get or set the urlTemplate after initialization:
 
   //Gets the urlTemplate from map.
  
   var property =$("#container").data("ejMap").model.layers[layerIndex].subLayers[subLayerIndex].urlTemplate;
   
   //Sets the urlTemplate to map.
   
   $("#container").data("ejMap").model.layers[layerIndex].subLayers[subLayerIndex].urlTemplate  = 'http://a.tile.openstreetmap.org/level/tileX/tileY.png';

{% endhighlight %}




## Methods

### navigateTo(latitude, longitude, level)
{:#methods:navigateto}

Method for navigating to specific shape based on latitude, longitude and zoom level.

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
            <td class="name">{% highlight html %}latitude{% endhighlight %}</td>
            <td class="type"><span class="param-type">number</span></td>
            <td class="description last">Pass the latitude value for map</td>
        </tr>
        <tr>
            <td class="name">{% highlight html %}longitude{% endhighlight %}</td>
            <td class="type"><span class="param-type">number</span></td>
            <td class="description last">Pass the longitude value for map</td>
        </tr>
        <tr>
            <td class="name">{% highlight html %}level{% endhighlight %}</td>
            <td class="type"><span class="param-type">number</span></td>
            <td class="description last">Pass the zoom level for map</td>
        </tr>
    </tbody>
</table>


#### Returns: void


#### Example

{% highlight js %}
 
//navigateTo method for map
   $("#container").ejMap("navigateTo", latitude, longitude, level);
   
{% endhighlight %}


### pan(direction)
{:#methods:pan}

Method to perform map panning

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
            <td class="name">{% highlight html %}direction{% endhighlight %}</td>
            <td class="type"><span class="param-type">string</span></td>
            <td class="description last">Pass the direction in which map should be panned</td>
        </tr>
    </tbody>
</table>

#### Returns: void


#### Example

{% highlight js %}
 
//pan method for map
   $("#container").ejMap("pan", direction);

{% endhighlight %}


### refresh()
{:#methods:refresh}

Method to reload the map.


#### Returns: void

#### Example

{% highlight js %}
 
//refresh method for map
   $("#container").ejMap("refresh");

{% endhighlight %}


### refreshLayers()
{:#methods:refreshlayers}

Method to reload the shapeLayers with updated values


#### Returns: void


#### Example

{% highlight js %}
 
//refresh layers method for map
   $("#container").ejMap("refreshLayers");

{% endhighlight %}


### refreshNavigationControl(navigation)
{:#methods:refreshnavigationcontrol}

Method to reload the navigation control with updated values.

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
            <td class="name">{% highlight html %}navigation{% endhighlight %}</td>
            <td class="type"><span class="param-type">object</span></td>
            <td class="description last">Pass the navigation control instance</td>
        </tr>
    </tbody>
</table>


#### Returns: void


#### Example

{% highlight js %}
 
//Refresh navigation control method for map
   $("#container").ejMap("refreshNavigationControl",navigation);{% endhighlight %}


### zoom(level, isAnimate)
{:#methods:zoom}

Method to perform map zooming.

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
            <td class="name">{% highlight html %}level{% endhighlight %}</td>
            <td class="type"><span class="param-type">number</span></td>
            <td class="description last">Pass the zoom level for map to be zoomed</td>
        </tr>
        <tr>
            <td class="name">{% highlight html %}isAnimate{% endhighlight %}</td>
            <td class="type"><span class="param-type">boolean</span></td>
            <td class="description last">Pass the boolean value to enable or disable animation while zooming</td>
        </tr>
    </tbody>
</table>

#### Returns: void


#### Example

{% highlight js %}
 
//zoom method for map
   $("#container").ejMap("zoom",level,isAnimate);

{% endhighlight %}


### refreshLayer(layerIndex,sublayerIndex)
{:#methods:refreshlayer}

Method to reload the specified layer based on layer and sublayer index value.


#### Returns: void


#### Example

{% highlight js %}
 
//refresh layers method for map
   $("#container").ejMap("refreshLayer", layerIndex, sublayerIndex);

{% endhighlight %}


### addMarkers(layerIndex, sublayerIndex, markers)
{:#methods:addmarkers}

Add markers dynamically based on layer and sublayer index value.


#### Returns: void


#### Example

{% highlight js %}
 
//addMarkers method for map
   $("#container").ejMap("addMarkers", layerIndex, sublayerIndex, markers);

{% endhighlight %}



## Events

### markerSelected
{:#events:markerselected}

Triggered on selecting the map markers.

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
            <td class="name">{% highlight html %}originalEvent{% endhighlight %}</td>
            <td class="type"><span class="param-type">object</span></td>
            <td class="description last">Returns marker object.</td>
        </tr>
    </tbody>
</table>

#### Example

{% highlight js %}
 
//markerSelected event for map
  
  $("#container").ejMap({
   markerSelected: function (event) {}
  });

{% endhighlight %}


### legendItemRendering
{:#events:legenditemrendering}

Triggered while rendering the each legend in maps.

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
            <td class="name">{% highlight html %}originalEvent{% endhighlight %}</td>
            <td class="type"><span class="param-type">object</span></td>
            <td class="description last">Returns the legend item.</td>
        </tr>
    </tbody>
</table>

#### Example

{% highlight js %}
 
//legendItemRendering event for map
  
  $("#container").ejMap({
   legendItemRendering: function (event) {}
  });

{% endhighlight %}


### bubbleRendering
{:#events:bubblerendering}

Triggered while rendering the each bubbles in maps.

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
            <td class="name">{% highlight html %}originalEvent{% endhighlight %}</td>
            <td class="type"><span class="param-type">object</span></td>
            <td class="description last">Returns the bubble values.</td>
        </tr>
    </tbody>
</table>

#### Example

{% highlight js %}
 
//bubbleRendering event for map
  
  $("#container").ejMap({
   bubbleRendering: function (event) {}
  });

{% endhighlight %}


### shapeRendering
{:#events:shaperendering}

Triggered while rendering the each shapes in maps.

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
            <td class="name">{% highlight html %}originalEvent{% endhighlight %}</td>
            <td class="type"><span class="param-type">object</span></td>
            <td class="description last">Returns the shape values.</td>
        </tr>
    </tbody>
</table>

#### Example

{% highlight js %}
 
//shapeRendering event for map
  
  $("#container").ejMap({
   shapeRendering: function (event) {}
  });

{% endhighlight %}


### mouseleave
{:#events:mouseleave}

Triggers while leaving the hovered map shape

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
            <td class="name">{% highlight html %}originalEvent{% endhighlight %}</td>
            <td class="type"><span class="param-type">object</span></td>
            <td class="description last">Returns hovered map shape object.</td>
        </tr>
    </tbody>
</table>

#### Example

{% highlight js %}
 
//mouseleave  event for map
  $("#container").ejMap({
   mouseleave : function (event) {}
  });

{% endhighlight %}


### mouseover
{:#events:mouseover}

Triggers while hovering the map shape.

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
            <td class="name">{% highlight html %}originalEvent{% endhighlight %}</td>
            <td class="type"><span class="param-type">object</span></td>
            <td class="description last">Returns hovered map shape object.</td>
        </tr>
    </tbody>
</table>

#### Example

{% highlight js %}
 
//mouseover  event for map
  $("#container").ejMap({
   mouseover : function (event) {}
  });

{% endhighlight %}


### onRenderComplete
{:#events:onrendercomplete}

Triggers once map render completed.

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
            <td class="name">{% highlight html %}originalEvent{% endhighlight %}</td>
            <td class="type"><span class="param-type">Object</span></td>
            <td class="description last">Event parameters from map</td>
        </tr>
    </tbody>
</table>

#### Example

{% highlight js %}
 
//onRenderComplete event for map
  $("#container").ejMap({
   onRenderComplete: function () {}
  });
  
{% endhighlight %}


### panned
{:#events:panned}

Triggers when map panning ends.

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
            <td class="name">{% highlight html %}originalEvent{% endhighlight %}</td>
            <td class="type"><span class="param-type">Object</span></td>
            <td class="description last">Event parameters from map</td>
        </tr>
    </tbody>
</table>

#### Example

{% highlight js %}
 
//panned event for map
  $("#container").ejMap({
   panned: function (event) {}
  });
{% endhighlight %}


### shapeSelected
{:#events:shapeselected}

Triggered on selecting the map shapes.

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
            <td class="name">{% highlight html %}originalEvent{% endhighlight %}</td>
            <td class="type"><span class="param-type">object</span></td>
            <td class="description last">Returns selected shape object.</td>
        </tr>
    </tbody>
</table>

#### Example

{% highlight js %}
 
//shapeSelected event for map
  $("#container").ejMap({
   shapeSelected: function (event) {}
  });

{% endhighlight %}


### zoomedIn
{:#events:zoomedin}

Triggered when map is zoomed-in.

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
            <td class="name">{% highlight html %}originalEvent{% endhighlight %}</td>
            <td class="type"><span class="param-type">Object</span></td>
            <td class="description last">Event parameters from map</td>
        </tr>
        <tr>
            <td class="name">{% highlight html %}zoomLevel{% endhighlight %}</td>
            <td class="type"><span class="param-type">object</span></td>
            <td class="description last">Returns zoom level value for which the map is zoomed.</td>
        </tr>
    </tbody>
</table>

#### Example

{% highlight js %}
 
//zoomedIn event for map
  $("#container").ejMap({
   zoomedIn: function (event) {}
  });

{% endhighlight %}


### zoomedOut
{:#events:zoomedout}

Triggers when map is zoomed out.

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
            <td class="name">{% highlight html %}originalEvent{% endhighlight %}</td>
            <td class="type"><span class="param-type">Object</span></td>
            <td class="description last">Event parameters from map</td>
        </tr>
        <tr>
            <td class="name">{% highlight html %}zoomLevel{% endhighlight %}</td>
            <td class="type"><span class="param-type">object</span></td>
            <td class="description last">Returns zoom level value for which the map is zoomed.</td>
        </tr>
    </tbody>
</table>

Example
{:.example}


{% highlight js %}
 
//zoomedOut event for map
  $("#container").ejMap({
   zoomedOut: function () {}
  });

{% endhighlight %}

### Click
{:#events:click}




Fires, on clicking the map.



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
            <td class="name">{% highlight html %}originalEvent{% endhighlight %}</td>
            <td class="type"><span class="param-type">object</span></td>
            <td class="description last">Returns clicked shape object.</td>
        </tr>
    </tbody>
</table>

#### Example


{% highlight js %}
 
//Click event for map

$("#container").ejMap({

    click: function (args) {
              //Do something
    }
   
});

{% endhighlight %}


### legendItemClick
{:#events:legenditemclick}




Fires on clicking the legend item. 


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
<td class="description last">Instance of the map model object</td>
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
    <li>LegendItem - Instance of the legend item object that is about to be rendered</li>
    <li>style - Options to customize the legend item styles such as border, color, size, etc…,</li>    
    <li>symbolShape - Name of the legend item shape. Use this option to customize legend item shape before rendering</li>
    <li>map - Instance of the map object corresponding to the legend item</li>
</ul></td>
</tr>
</tbody>
</table>

#### Example


{% highlight js %}
 
//legendItem Click event for map.

$("#container").ejMap({

    legendItemClick: function (args) {
              //Do something
    }
   
});

{% endhighlight %}


### doubleClick
{:#events:doubleclick}




Fires, on double clicking the map.


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
            <td class="name">{% highlight html %}originalEvent{% endhighlight %}</td>
            <td class="type"><span class="param-type">object</span></td>
            <td class="description last">Returns double clicked shape object.</td>
        </tr>
    </tbody>
</table>

#### Example


{% highlight js %}
 
//DoubleClick event for map.

$("#container").ejMap({

    doubleClick: function (args) {
              //Do something
    }
   
});

{% endhighlight %}



### rightClick
{:#events:rightclick}




Fires, on right clicking the map.


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
            <td class="name">{% highlight html %}originalEvent{% endhighlight %}</td>
            <td class="type"><span class="param-type">object</span></td>
            <td class="description last">Returns right clicked shape object.</td>
        </tr>
    </tbody>
</table>

#### Example


{% highlight js %}
 
//RightClick event for map

$("#container").ejMap({
    rightClick: function (args) {
              //Do something
    }
   
});

{% endhighlight %}


### onLoad
{:#events:onload}

Fires before loading the map.

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
<td class="description last">Instance of the map model object</td>
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
 
//mouseover  event for map
  $("#container").ejMap({
   onLoad : function (event) {}
  });

{% endhighlight %}

### markerEnter
{:#events:markerenter}

Triggers while entering the hovered marker shape.

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
<td class="description last">Instance of the map model object</td>
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
 
//marker enter  event for map
  $("#container").ejMap({
   markerEnter : function (event) {}
  });

{% endhighlight %}

### markerLeave
{:#events:markerleave}

Triggers while leaving the hovered marker shape.

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
<td class="description last">Instance of the map model object</td>
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
 
//marker leave  event for map
  $("#container").ejMap({
   markerLeave : function (event) {}
  });

{% endhighlight %}

### refreshed
{:#events:refreshed}

Triggers after refreshing the map items.

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
            <td class="name">{% highlight html %}originalEvent{% endhighlight %}</td>
            <td class="type"><span class="param-type">object</span></td>
            <td class="description last">Refresh and load the map.</td>
        </tr>
    </tbody>
</table>

#### Example

{% highlight js %}
 
//refreshed  event for map
  $("#container").ejMap({
   refreshed : function (event) {}
  });

{% endhighlight %}

### displayTextRendering
{:#events:displaytextrendering}




Fires before rendering the data labels. This event is triggered for each data label in the layers. You can use this event to add custom text in data labels.


#### Example


{% highlight js %}
 
//displayTextRendering event for maps

$("#container").ejMap({

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
<td class="description last">Instance of the map model object.</td>
</tr>
<tr>
<td class="name">{% highlight js %}
type{% endhighlight %}</td>
<td class="type"><span class="param-type">string</span></td>
<td class="description last">Name of the event</td>
</tr>
</tbody>
</table>


<a class="" href="http://www.syncfusion.com/copyright" target="_blank">Copyright &copy; 2001 - 2015 Syncfusion Inc. All Rights Reserved</a>





