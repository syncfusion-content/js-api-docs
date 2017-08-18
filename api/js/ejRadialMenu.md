---
layout: post
title: Properties, Methods and Events of ejRadialMenu Widget
documentation: API
platform: js-api
metaname: 
metacontent: 
---

# ejRadialMenu

The RadialMenu control is a context that represents the menu items are arranged in a circular order with a centric button element in it. By default, only the center button is visible. The Radial Menu displays the root level menu item with rotational animation effects on clicking the center menu button. 

#### Syntax

{% highlight js %}

      $(element).ejRadialMenu()

{% endhighlight %}




Example
{:.example}


{% highlight html %}
// Create radialmenu in obtrusive way
<script> 
$(function(){
$("#defaultRadialMenu").ejRadialMenu(); 
});
</script>
<div >
<br />
<p>
Model-view-controller (MVC) is a software architecture pattern which separates the representation of information from the user's interaction with it.
</p>
</div>  
<div id="defaultRadialMenu">
<ul>
<li data-ej-imageurl="../themes/sample/radialmenu/social.png"
data-ej-text="social"></li>
<li data-ej-imageurl="../themes/sample/radialmenu/music.png" 
data-ej-text="music"></li>
<li data-ej-imageurl="../themes/sample/radialmenu/direction.png" 
data-ej-text="direction"></li>
<li data-ej-imageurl="../themes/sample/radialmenu/message.png" 
data-ej-text="message"></li>
<li data-ej-imageurl="../themes/sample/radialmenu/browser.png" 
data-ej-text="browser"></li>
</ul>
</div>{% endhighlight %}




Requires
{:.require}


* module:jQuery

* module:ej.core

* module:ej.unobtrusive

* module:ej.data

* module:ej.touch

* module:ej.radialmenu


## Members




### autoOpen `boolean`
{:#members:autoopen}




To show the Radial in initial render.


Default Value:
{:.param}



* false




Example
{:.example}


{% highlight html %}
 
// Set Radialmenu autoOpen on initialization. 
//To set autoOpen API 
<div >
<br />
<p>
Model-view-controller (MVC) is a software architecture pattern which separates the representation of information from the user's interaction with it.
</p>
</div>  
<div id="defaultRadialMenu">
<ul>
<li data-ej-imageurl="../themes/sample/radialmenu/social.png"
data-ej-text="social"></li>
<li data-ej-imageurl="../themes/sample/radialmenu/music.png" 
data-ej-text="music"></li>
<li data-ej-imageurl="../themes/sample/radialmenu/direction.png" 
data-ej-text="direction"></li>
<li data-ej-imageurl="../themes/sample/radialmenu/message.png" 
data-ej-text="message"></li>
<li data-ej-imageurl="../themes/sample/radialmenu/browser.png" 
data-ej-text="browser"></li>
</ul>
</div>
<script>
$(function () {
$("#defaultRadialMenu").ejRadialMenu({ "autoOpen":true });      
});
</script>{% endhighlight %}


{% highlight html %}
 
//Get or set the Radialmenu autoOpen, after initialization:
<script>
// Gets the autoOpen API.               
$("#defaultRadialMenu").ejRadialMenu ("option", "autoOpen");                    
// Sets the autoOpen API
$("#defaultRadialMenu").ejRadialMenu ("option", "autoOpen", true);            
</script>{% endhighlight %}




### backImageClass `string`
{:#members:backimageclass}




Renders the back button Image for Radial using class.


Default Value:
{:.param}



* e-backimage




Example
{:.example}


{% highlight html %}
 
// Set Radialmenu back button Image on initialization. 
//To set back button image API 
<div >
<br />
<p>
Model-view-controller (MVC) is a software architecture pattern which separates the representation of information from the user's interaction with it.
</p>
</div>  
<div id="defaultRadialMenu">
<ul>
<li data-ej-imageurl="../themes/sample/radialmenu/social.png"
data-ej-text="social"></li>
<li data-ej-imageurl="../themes/sample/radialmenu/music.png" 
data-ej-text="music"></li>
<li data-ej-imageurl="../themes/sample/radialmenu/direction.png" 
data-ej-text="direction"></li>
<li data-ej-imageurl="../themes/sample/radialmenu/message.png" 
data-ej-text="message"></li>
<li data-ej-imageurl="../themes/sample/radialmenu/browser.png" 
data-ej-text="browser"></li>
</ul>
</div>
<script>
$(function () {
$("#defaultRadialMenu").ejRadialMenu({ "backImageClass":"e-backimage" });       
});
</script>{% endhighlight %}


{% highlight html %}
 
//Get or set the Radialmenu backImageClass, after initialization:
<script>
// Gets the backImageClass API.         
$("#defaultRadialMenu").ejRadialMenu ("option", "backImageClass");                      
// Sets the backImageClass API
$("#defaultRadialMenu").ejRadialMenu ("option", "backImageClass", "e-backimage");            
</script>{% endhighlight %}




### cssClass `string`
{:#members:cssclass}




Sets the root class for RadialMenu theme. This cssClass API helps to use custom skinning option for RadialMenu control. By defining the root class using this API, we need to include this root class in CSS.


Default Value:
{:.param}



* ""




Example
{:.example}


{% highlight html %}
 
// Set Radialmenu cssClass on initialization. 
//To set cssClass API 
<div >
<br />
<p>
Model-view-controller (MVC) is a software architecture pattern which separates the representation of information from the user's interaction with it.
</p>
</div>  
<div id="defaultRadialMenu">
<ul>
<li data-ej-imageurl="../themes/sample/radialmenu/social.png"
data-ej-text="social"></li>
<li data-ej-imageurl="../themes/sample/radialmenu/music.png" 
data-ej-text="music"></li>
<li data-ej-imageurl="../themes/sample/radialmenu/direction.png" 
data-ej-text="direction"></li>
<li data-ej-imageurl="../themes/sample/radialmenu/message.png" 
data-ej-text="message"></li>
<li data-ej-imageurl="../themes/sample/radialmenu/browser.png" 
data-ej-text="browser"></li>
</ul>
</div>
<script>
$(function () {
$("#defaultRadialMenu").ejRadialMenu({ "cssClass":"custom-class" });     
});
</script>{% endhighlight %}


{% highlight html %}
 
//Get or set the Radialmenu cssClass, after initialization:
<script>
// Gets the cssClass API.               
$("#defaultRadialMenu").ejRadialMenu ("option", "cssClass");                    
// Sets the cssClass API
$("#defaultRadialMenu").ejRadialMenu ("option", "cssClass", "custom-class");            
</script>{% endhighlight %}




### enableAnimation `boolean`
{:#members:enableanimation}




To enable Animation for Radial Menu.


Default Value:
{:.param}



* true




Example
{:.example}


{% highlight html %}
 
// Set Radialmenu enableAnimation on initialization. 
//To set enableAnimation API 
<div >
<br />
<p>
Model-view-controller (MVC) is a software architecture pattern which separates the representation of information from the user's interaction with it.
</p>
</div>  
<div id="defaultRadialMenu">
<ul>
<li data-ej-imageurl="../themes/sample/radialmenu/social.png"
data-ej-text="social"></li>
<li data-ej-imageurl="../themes/sample/radialmenu/music.png" 
data-ej-text="music"></li>
<li data-ej-imageurl="../themes/sample/radialmenu/direction.png" 
data-ej-text="direction"></li>
<li data-ej-imageurl="../themes/sample/radialmenu/message.png" 
data-ej-text="message"></li>
<li data-ej-imageurl="../themes/sample/radialmenu/browser.png" 
data-ej-text="browser"></li>
</ul>
</div>
<script>
$(function () {
$("#defaultRadialMenu").ejRadialMenu({ "enableAnimation":true });       
});
</script>{% endhighlight %}


{% highlight html %}
 
//Get or set the Radialmenu enableAnimation, after initialization:
<script>
// Gets the enableAnimation API.                
$("#defaultRadialMenu").ejRadialMenu ("option", "enableAnimation");                     
// Sets the enableAnimation API
$("#defaultRadialMenu").ejRadialMenu ("option", "enableAnimation", true);            
</script>{% endhighlight %}




### imageClass `string`
{:#members:imageclass}




Renders the Image for Radial using Class.


Default Value:
{:.param}



* e-radialimage




Example
{:.example}


{% highlight html %}
 
// Set Radialmenu Image on initialization. 
//To set image API  
<div >
<br />
<p>
Model-view-controller (MVC) is a software architecture pattern which separates the representation of information from the user's interaction with it.
</p>
</div>  
<div id="defaultRadialMenu">
<ul>
<li data-ej-imageurl="../themes/sample/radialmenu/social.png"
data-ej-text="social"></li>
<li data-ej-imageurl="../themes/sample/radialmenu/music.png" 
data-ej-text="music"></li>
<li data-ej-imageurl="../themes/sample/radialmenu/direction.png" 
data-ej-text="direction"></li>
<li data-ej-imageurl="../themes/sample/radialmenu/message.png" 
data-ej-text="message"></li>
<li data-ej-imageurl="../themes/sample/radialmenu/browser.png" 
data-ej-text="browser"></li>
</ul>
</div>
<script>
$(function () {
$("#defaultRadialMenu").ejRadialMenu({ "imageClass":"e-radialimage" }); 
});
</script>{% endhighlight %}


{% highlight html %}
 
//Get or set the Radialmenu Image, after initialization:
<script>
// Gets the Image API.          
 $("#radialmenu").ejRadialMenu ("option", "imageClass");                        
// Sets the imageClass API
$("#radialmenu").ejRadialMenu ("option", "imageClass", "e-radialimage");            
</script>

{% endhighlight %}





### items `Array`
{:#members:items}




Specify the items of radial menu




Example
{:.example}


{% highlight html %}
 
<div id="defaultRadialMenu">
</div>
 
<script>
$(function () {
$("#defaultRadialMenu").ejRadialMenu({ items:[{ text:"textField", imageUrl:"/Bold.jpg"}] }); 
});
</script>{% endhighlight %}






### items.imageUrl `string`
{:#members:items-imageUrl}




Specify the URL of the frame background image for radial menu item.




Example
{:.example}


{% highlight html %}
 
<div id="defaultRadialMenu">
</div>
 
<script>
$(function () {
$("#defaultRadialMenu").ejRadialMenu({ items:[{ imageUrl:"/Bold.jpg"}] }); 
});
</script>{% endhighlight %}


### items.prependTo `string`
{:#members:items-prependTo}


Specifies the template property of RadialMenu for SVG icon.


Example
{:.example}

{% highlight html %}
 
<div id="defaultRadialMenu">
</div>
 
<script>
$(function () {
$("#defaultRadialMenu").ejRadialMenu({ items:[{ prependTo:"#template"}] }); 
});
</script> {% endhighlight %}


### items.text `string`
{:#members:items-text}


Specifies the text of RadialMenu item. 




#### Example


{% highlight html %}
 
<div id="defaultRadialMenu">
</div>
 
<script>
$(function () {
$("#defaultRadialMenu").ejRadialMenu({ items:[{ text:"textField" }] }); 
});
</script>{% endhighlight %}



### items.enabled `boolean`
{:#members:items-enabled}


Specifies the enable state of RadialMenu item. 



Example
{:.example}


{% highlight html %}
 
<div id="defaultRadialMenu">
</div>
 
<script>
$(function () {
$("#defaultRadialMenu").ejRadialMenu({ items:[{ enabled:false }] }); 
});
</script>{% endhighlight %}


### items.click `string`
{:#members:items-click}


specify the click event to corresponding image/text for performing some specific action.


Example
{:.example}



{% highlight html %}

<div id="radialmenu" ></div>
<script>
$("#radialmenu").ejRadialMenu({ items:[{imageUrl:"themes/sample/tile/font.png", text:"Bold", click:"bold" }]});
function bold(e){
  //do some actions
}
</script>{% endhighlight %}


### items.badge `Object`
{:#members:items-badge}


Specifies radialmenu item badges.


Example
{:.example}



{% highlight html %}

<div id="radialmenu" ></div>
<script>
$("#radialmenu").ejRadialMenu({ items:[{text:"Bold", enabled: true, badge.enabled:true }]});

</script>{% endhighlight %}


### items.badge.enabled `boolean`
{:#members:items-badge-enabled}


Specifies whether to enable radialmenu item badge or not.


Example
{:.example}



{% highlight html %}

<div id="radialmenu" ></div>
<script>
$("#radialmenu").ejRadialMenu({ items:[{text:"Bold", enabled: true, badge.enabled:true }]});

</script>{% endhighlight %}



### items.badge.value `number`
{:#members:items-badge-value}


Specifies the value of radial menu item badge.


Example
{:.example}



{% highlight html %}

<div id="radialmenu" ></div>
<script>
$("#radialmenu").ejRadialMenu({ items:[{ badge.enabled:true, badge.value:3 }]});

</script>{% endhighlight %}



### items.type `string`
{:#members:items-type}


Specifies the type of nested radial menu item.


Example
{:.example}



{% highlight html %}

<div id="radialmenu" ></div>
<script>
$("#radialmenu").ejRadialMenu({ items:[{badge.enabled:true, badge.value:"3", type:"slider" }]});

</script>{% endhighlight %}


### items.sliderSettings `Object`

{:#members:items-sliderSettings}


Specifies the sliderSettings ticks for nested radial menu items.


Example
{:.example}



{% highlight html %}

<div id="radialmenu" ></div>
<script>
$("#radialmenu").ejRadialMenu({ items:[{ badge.enabled:true, badge.value:3, type:"slider", sliderSettings.ticks:[0,2,4,6,8,10] }]});

</script>{% endhighlight %}




### items.sliderSettings.ticks `Array`
{:#members:items-sliderSettings-ticks}


Specifies the sliderSettings ticks values of nested radial menu items.


Example
{:.example}



{% highlight html %}

<div id="radialmenu" ></div>
<script>
$("#radialmenu").ejRadialMenu({ items:[{ badge.enabled:true, badge.value:3, type:"slider", sliderSettings.ticks:[0,2,4,6,8,10] }]});

</script>{% endhighlight %}




### items.sliderSettings.strokeWidth `number`
{:#members:items-sliderSettings-strokeWidth}


Specifies the sliderSettings stroke Width value.


Example
{:.example}



{% highlight html %}

<div id="radialmenu" ></div>
<script>
$("#radialmenu").ejRadialMenu({ items:[{badge.value:3, type:"slider", sliderSettings.ticks:[0,2,4,6,8,10], sliderSettings.strokeWidth:3 }]});

</script>{% endhighlight %}






### items.sliderSettings.labelSpace `number`
{:#members:items-sliderSettings-labelSpace}


Specifies the value of sliderSettings labelSpace .


Example
{:.example}



{% highlight html %}

<div id="radialmenu" ></div>
<script>
$("#radialmenu").ejRadialMenu({ items:[{ type:"slider", sliderSettings.ticks:[0,2,4,6,8,10], sliderSettings.labelSpace:15 }]});

</script>{% endhighlight %}


### items.items `Array`
{:#members:items-items}


Specifies to add sub level items .

### radius `number`
{:#members:radius}




Specifies the radius of radial menu


Default Value:
{:.param}



* 150




Example
{:.example}


{% highlight html %}
 
// Set Radialmenu radius on initialization. 
//To set radius API  
<div >
<br />
<p>
Model-view-controller (MVC) is a software architecture pattern which separates the representation of information from the user's interaction with it.
</p>
</div>  
<div id="defaultRadialMenu">
<ul>
<li data-ej-imageurl="../themes/sample/radialmenu/social.png"
data-ej-text="social"></li>
<li data-ej-imageurl="../themes/sample/radialmenu/music.png" 
data-ej-text="music"></li>
<li data-ej-imageurl="../themes/sample/radialmenu/direction.png" 
data-ej-text="direction"></li>
<li data-ej-imageurl="../themes/sample/radialmenu/message.png" 
data-ej-text="message"></li>
<li data-ej-imageurl="../themes/sample/radialmenu/browser.png" 
data-ej-text="browser"></li>
</ul>
</div>
<script>
$(function () {
$("#defaultRadialMenu").ejRadialMenu({ "radius":150});  
});
</script>{% endhighlight %}


{% highlight html %}
 
//Get or set the Radialmenu radius, after initialization:
<script>
// Gets the radius API.         
 $("#radialmenu").ejRadialMenu ("option", "radius");                    
// Sets the radius API
$("#radialmenu").ejRadialMenu ("option", "radius", 150);            
</script>{% endhighlight %}




### targetElementId `string`
{:#members:targetelementid}




To show the Radial while clicking given target element.


Default Value:
{:.param}



* null




Example
{:.example}


{% highlight html %}
 
// Set Radialmenu targetElementId on initialization. 
//To set targetElementId API 
<div >
<br />
<p>
Model-view-controller (MVC) is a software architecture pattern which separates the representation of information from the user's interaction with it.
</p>
</div>  
<div id="defaultRadialMenu">
<ul>
<li data-ej-imageurl="../themes/sample/radialmenu/social.png"
data-ej-text="social"></li>
<li data-ej-imageurl="../themes/sample/radialmenu/music.png" 
data-ej-text="music"></li>
<li data-ej-imageurl="../themes/sample/radialmenu/direction.png" 
data-ej-text="direction"></li>
<li data-ej-imageurl="../themes/sample/radialmenu/message.png" 
data-ej-text="message"></li>
<li data-ej-imageurl="../themes/sample/radialmenu/browser.png" 
data-ej-text="browser"></li>
</ul>
</div>
<script>
$(function () {
$("#defaultRadialMenu").ejRadialMenu({ "targetElementId":"target" });   
});
</script>{% endhighlight %}


{% highlight html %}
 
//Get or set the Radialmenu targetElementId, after initialization:
<script>
// Gets the targetElementId API.                
$("#defaultRadialMenu").ejRadialMenu ("option", "targetElementId");                     
// Sets the targetElementId API
$("#defaultRadialMenu").ejRadialMenu ("option", "targetElementId", "target");            
</script>{% endhighlight %}




### position `Object`
{:#members:position}


To set radial render position.



Default Value:
{:.param}



* null




Example
{:.example}


{% highlight html %}
 
// Set Radialmenu position on initialization. 
//To set position API 
<div >
<br />
<p>
Model-view-controller (MVC) is a software architecture pattern which separates the representation of information from the user's interaction with it.
</p>
</div>  
<div id="defaultRadialMenu">
<ul>
<li data-ej-imageurl="../themes/sample/radialmenu/social.png"
data-ej-text="social"></li>
<li data-ej-imageurl="../themes/sample/radialmenu/music.png" 
data-ej-text="music"></li>
<li data-ej-imageurl="../themes/sample/radialmenu/direction.png" 
data-ej-text="direction"></li>
<li data-ej-imageurl="../themes/sample/radialmenu/message.png" 
data-ej-text="message"></li>
<li data-ej-imageurl="../themes/sample/radialmenu/browser.png" 
data-ej-text="browser"></li>
</ul>
</div>
<script>
$(function () {
$("#defaultRadialMenu").ejRadialMenu({ position:{x:10,y:10} });   
});
</script>{% endhighlight %}


{% highlight html %}
 
//Get or set the Radialmenu position, after initialization:
<script>
// Gets the position API.                
$("#defaultRadialMenu").ejRadialMenu ("option", "position");                     
// Sets the position API
$("#defaultRadialMenu").ejRadialMenu ("option", "position");            
</script>{% endhighlight %}




## Methods




### hide()
{:#methods:hide}




To hide the radialmenu



Example
{:.example}


{% highlight html %}
 
<div >
<br />
<p>
Model-view-controller (MVC) is a software architecture pattern which separates the representation of information from the user's interaction with it.
</p>
</div>  
<div id="defaultRadialMenu">
<ul>
<li data-ej-imageurl="../themes/sample/radialmenu/social.png"
data-ej-text="social"></li>
<li data-ej-imageurl="../themes/sample/radialmenu/music.png" 
data-ej-text="music"></li>
<li data-ej-imageurl="../themes/sample/radialmenu/direction.png" 
data-ej-text="direction"></li>
<li data-ej-imageurl="../themes/sample/radialmenu/message.png" 
data-ej-text="message"></li>
<li data-ej-imageurl="../themes/sample/radialmenu/browser.png" 
data-ej-text="browser"></li>
</ul>
</div>{% endhighlight %}


{% highlight html %}
 
<script>
$("#defaultRadialMenu").ejRadialMenu ("hide");
</script>{% endhighlight %}




### menuHide()[Deprecated]
{:#methods:menuhidedeprecated}




To hide the radialmenu items

N>Since it is deprecated use the method “[hideMenu](#methods:hideMenu)”

Example
{:.example}


{% highlight html %}
 
<div >
<br />
<p>
Model-view-controller (MVC) is a software architecture pattern which separates the representation of information from the user's interaction with it.
</p>
</div>  
<div id="defaultRadialMenu">
<ul>
<li data-ej-imageurl="../themes/sample/radialmenu/social.png"
data-ej-text="social"></li>
<li data-ej-imageurl="../themes/sample/radialmenu/music.png" 
data-ej-text="music"></li>
<li data-ej-imageurl="../themes/sample/radialmenu/direction.png" 
data-ej-text="direction"></li>
<li data-ej-imageurl="../themes/sample/radialmenu/message.png" 
data-ej-text="message"></li>
<li data-ej-imageurl="../themes/sample/radialmenu/browser.png" 
data-ej-text="browser"></li>
</ul>
</div>{% endhighlight %}


{% highlight html %}
 
<script>
$("#defaultRadialMenu").ejRadialMenu ("menuHide");
</script>{% endhighlight %}




### hideMenu()
{:#methods:hidemenu}




To hide the radialmenu items



Example
{:.example}


{% highlight html %}
 
<div >
<br />
<p>
Model-view-controller (MVC) is a software architecture pattern which separates the representation of information from the user's interaction with it.
</p>
</div>  
<div id="defaultRadialMenu">
<ul>
<li data-ej-imageurl="../themes/sample/radialmenu/social.png"
data-ej-text="social"></li>
<li data-ej-imageurl="../themes/sample/radialmenu/music.png" 
data-ej-text="music"></li>
<li data-ej-imageurl="../themes/sample/radialmenu/direction.png" 
data-ej-text="direction"></li>
<li data-ej-imageurl="../themes/sample/radialmenu/message.png" 
data-ej-text="message"></li>
<li data-ej-imageurl="../themes/sample/radialmenu/browser.png" 
data-ej-text="browser"></li>
</ul>
</div>{% endhighlight %}


{% highlight html %}
 
<script>
$("#defaultRadialMenu").ejRadialMenu ("hideMenu");
</script>{% endhighlight %}




### show()
{:#methods:show}




To Show the radial menu



Example
{:.example}


{% highlight html %}
 
<div >
<br />
<p>
Model-view-controller (MVC) is a software architecture pattern which separates the representation of information from the user's interaction with it.
</p>
</div>  
<div id="defaultRadialMenu">
<ul>
<li data-ej-imageurl="../themes/sample/radialmenu/social.png"
data-ej-text="social"></li>
<li data-ej-imageurl="../themes/sample/radialmenu/music.png" 
data-ej-text="music"></li>
<li data-ej-imageurl="../themes/sample/radialmenu/direction.png" 
data-ej-text="direction"></li>
<li data-ej-imageurl="../themes/sample/radialmenu/message.png" 
data-ej-text="message"></li>
<li data-ej-imageurl="../themes/sample/radialmenu/browser.png" 
data-ej-text="browser"></li>
</ul>
</div>{% endhighlight %}


{% highlight html %}
 
<script>
$("#defaultRadialMenu").ejRadialMenu ("show");
</script>{% endhighlight %}



### showMenu()
{:#methods:showmenu}




To show menu items



Example
{:.example}


{% highlight html %}
 
<div >
<br />
<p>
Model-view-controller (MVC) is a software architecture pattern which separates the representation of information from the user's interaction with it.
</p>
</div>  
<div id="defaultRadialMenu">
<ul>
<li data-ej-imageurl="../themes/sample/radialmenu/social.png"
data-ej-text="social"></li>
<li data-ej-imageurl="../themes/sample/radialmenu/music.png" 
data-ej-text="music"></li>
<li data-ej-imageurl="../themes/sample/radialmenu/direction.png" 
data-ej-text="direction"></li>
<li data-ej-imageurl="../themes/sample/radialmenu/message.png" 
data-ej-text="message"></li>
<li data-ej-imageurl="../themes/sample/radialmenu/browser.png" 
data-ej-text="browser"></li>
</ul>
</div>{% endhighlight %}


{% highlight html %}
 
<script>
$("#defaultRadialMenu").ejRadialMenu ("showMenu");
</script>{% endhighlight %}




### enableItemByIndex(itemIndex)
{:#methods:enableitembyindex}


To enable menu item using index

<table>
<tr>
<td>
<b>Parameters</b></td><td>
<b>Type</b></td><td>
<b>Description</b></td></tr>
<tr>
<td>
itemIndex</td><td>
number</td><td>
Index of the Radialmenu to be enabled.</td></tr>
</table>



Example
{:.example}


{% highlight html %}
 
<div >
<br />
<p>
Model-view-controller (MVC) is a software architecture pattern which separates the representation of information from the user's interaction with it.
</p>
</div>  
<div id="defaultRadialMenu">
<ul>
<li data-ej-imageurl="../themes/sample/radialmenu/social.png"
data-ej-text="social" data-ej-enabled="false"></li>
<li data-ej-imageurl="../themes/sample/radialmenu/music.png" 
data-ej-text="music"></li>
<li data-ej-imageurl="../themes/sample/radialmenu/direction.png" 
data-ej-text="direction"></li>
<li data-ej-imageurl="../themes/sample/radialmenu/message.png" 
data-ej-text="message"></li>
<li data-ej-imageurl="../themes/sample/radialmenu/browser.png" 
data-ej-text="browser"></li>
</ul>
</div>{% endhighlight %}


{% highlight html %}
 
<script>
$("#defaultRadialMenu").ejRadialMenu ({ "autoOpen":true});
var obj=$("#defaultRadialMenu").ejRadialMenu("instance");
obj.enableItemByIndex(0);
</script>{% endhighlight %}




### enableItemsByIndices(itemIndices)
{:#methods:enableItemsByIndices}


To enable menu items using indices

<table>
<tr>
<td>
<b>Parameters</b></td><td>
<b>Type</b></td><td>
<b>Description</b></td></tr>
<tr>
<td>
itemIndices</td><td>
Array</td><td>
Index of the Radialmenu to be enabled.</td></tr>
</table>



Example
{:.example}


{% highlight html %}
 
<div >
<br />
<p>
Model-view-controller (MVC) is a software architecture pattern which separates the representation of information from the user's interaction with it.
</p>
</div>  
<div id="defaultRadialMenu">
<ul>
<li data-ej-imageurl="../themes/sample/radialmenu/social.png"
data-ej-text="social" data-ej-enabled="false"></li>
<li data-ej-imageurl="../themes/sample/radialmenu/music.png" 
data-ej-text="music"></li>
<li data-ej-imageurl="../themes/sample/radialmenu/direction.png" 
data-ej-text="direction" data-ej-enabled="false"></li>
<li data-ej-imageurl="../themes/sample/radialmenu/message.png" 
data-ej-text="message"></li>
<li data-ej-imageurl="../themes/sample/radialmenu/browser.png" 
data-ej-text="browser"></li>
</ul>
</div>{% endhighlight %}


{% highlight html %}
 
<script>
$("#defaultRadialMenu").ejRadialMenu ({ "autoOpen":true});
var obj=$("#defaultRadialMenu").ejRadialMenu("instance");
obj.enableItemsByIndices([0,2]);
</script>{% endhighlight %}




### disableItemByIndex(itemIndex)
{:#methods:disableitembyindex}

To disable menu item using index

<table>
<tr>
<td>
<b>Parameters</b></td><td>
<b>Type</b></td><td>
<b>Description</b></td></tr>
<tr>
<td>
itemIndex</td><td>
number</td><td>
Index of the Radialmenu to be disabled.</td></tr>
</table>



Example
{:.example}


{% highlight html %}
 
<div >
<br />
<p>
Model-view-controller (MVC) is a software architecture pattern which separates the representation of information from the user's interaction with it.
</p>
</div>  
<div id="defaultRadialMenu">
<ul>
<li data-ej-imageurl="../themes/sample/radialmenu/social.png"
data-ej-text="social"></li>
<li data-ej-imageurl="../themes/sample/radialmenu/music.png" 
data-ej-text="music"></li>
<li data-ej-imageurl="../themes/sample/radialmenu/direction.png" 
data-ej-text="direction"></li>
<li data-ej-imageurl="../themes/sample/radialmenu/message.png" 
data-ej-text="message"></li>
<li data-ej-imageurl="../themes/sample/radialmenu/browser.png" 
data-ej-text="browser"></li>
</ul>
</div>{% endhighlight %}


{% highlight html %}
 
<script>
$("#defaultRadialMenu").ejRadialMenu({ "autoOpen":true});  
var obj=$("#defaultRadialMenu").ejRadialMenu("instance");
obj.disableItemByIndex(0);
</script>{% endhighlight %}




### disableItemsByIndices(itemIndices)
{:#methods:disableitemsbyindices}

To disable menu items using indices


<table>
<tr>
<td>
<b>Parameters</b></td><td>
<b>Type</b></td><td>
<b>Description</b></td></tr>
<tr>
<td>
itemIndices</td><td>
Array</td><td>
items of the Radialmenu to disable.</td></tr>
</table>

Example
{:.example}


{% highlight html %}
 
<div >
<br />
<p>
Model-view-controller (MVC) is a software architecture pattern which separates the representation of information from the user's interaction with it.
</p>
</div>  
<div id="defaultRadialMenu">
<ul>
<li data-ej-imageurl="../themes/sample/radialmenu/social.png"
data-ej-text="social"></li>
<li data-ej-imageurl="../themes/sample/radialmenu/music.png" 
data-ej-text="music"></li>
<li data-ej-imageurl="../themes/sample/radialmenu/direction.png" 
data-ej-text="direction"></li>
<li data-ej-imageurl="../themes/sample/radialmenu/message.png" 
data-ej-text="message"></li>
<li data-ej-imageurl="../themes/sample/radialmenu/browser.png" 
data-ej-text="browser"></li>
</ul>
</div>{% endhighlight %}


{% highlight html %}
 
<script>
$("#defaultRadialMenu").ejRadialMenu({ "autoOpen":true});  
var obj=$("#defaultRadialMenu").ejRadialMenu("instance");
obj.disableItemsByIndices([1,3]);
</script>{% endhighlight %}




### enableItem(item)
{:#methods:enableitem}


To enable menu item using item text

<table>
<tr>
<td>
<b>Parameters</b></td><td>
<b>Type</b></td><td>
<b>Description</b></td></tr>
<tr>
<td>
item</td><td>
String</td><td>
item of the Radialmenu item to enable.</td></tr>
</table>



Example
{:.example}


{% highlight html %}
 
<div >
<br />
<p>
Model-view-controller (MVC) is a software architecture pattern which separates the representation of information from the user's interaction with it.
</p>
</div>  
<div id="defaultRadialMenu">
<ul>
<li data-ej-imageurl="../themes/sample/radialmenu/social.png"
data-ej-text="social" data-ej-enabled="false"></li>
<li data-ej-imageurl="../themes/sample/radialmenu/music.png" 
data-ej-text="music"></li>
<li data-ej-imageurl="../themes/sample/radialmenu/direction.png" 
data-ej-text="direction"></li>
<li data-ej-imageurl="../themes/sample/radialmenu/message.png" 
data-ej-text="message"></li>
<li data-ej-imageurl="../themes/sample/radialmenu/browser.png" 
data-ej-text="browser"></li>
</ul>
</div>{% endhighlight %}


{% highlight html %}
 
<script>
$("#defaultRadialMenu").ejRadialMenu({ "autoOpen":true});  
var obj=$("#defaultRadialMenu").ejRadialMenu("instance");
obj.enableItem("social");
</script>{% endhighlight %}




### disableItem(item)
{:#methods:disableitem}

To disable menu item using item text

<table>
<tr>
<td>
<b>Parameters</b></td><td>
<b>Type</b></td><td>
<b>Description</b></td></tr>
<tr>
<td>
item</td><td>
String</td><td>
item of the Radialmenu item to disable.</td></tr>
</table>




Example
{:.example}


{% highlight html %}
 
<div >
<br />
<p>
Model-view-controller (MVC) is a software architecture pattern which separates the representation of information from the user's interaction with it.
</p>
</div>  
<div id="defaultRadialMenu">
<ul>
<li data-ej-imageurl="../themes/sample/radialmenu/social.png"
data-ej-text="social"></li>
<li data-ej-imageurl="../themes/sample/radialmenu/music.png" 
data-ej-text="music"></li>
<li data-ej-imageurl="../themes/sample/radialmenu/direction.png" 
data-ej-text="direction"></li>
<li data-ej-imageurl="../themes/sample/radialmenu/message.png" 
data-ej-text="message"></li>
<li data-ej-imageurl="../themes/sample/radialmenu/browser.png" 
data-ej-text="browser"></li>
</ul>
</div>{% endhighlight %}


{% highlight html %}
 
<script>
$("#defaultRadialMenu").ejRadialMenu({ "autoOpen":true});  
var obj=$("#defaultRadialMenu").ejRadialMenu("instance");
obj.disableItem("social");
</script>{% endhighlight %}




### enableItems(items)
{:#methods:enableitems}


To enable menu items using item texts

<table>
<tr>
<td>
<b>Parameters</b></td><td>
<b>Type</b></td><td>
<b>Description</b></td></tr>
<tr>
<td>
items</td><td>
Array</td><td>
items of the Radialmenu item to enable.</td></tr>
</table>




Example
{:.example}


{% highlight html %}
 
<div >
<br />
<p>
Model-view-controller (MVC) is a software architecture pattern which separates the representation of information from the user's interaction with it.
</p>
</div>  
<div id="defaultRadialMenu">
<ul>
<li data-ej-imageurl="../themes/sample/radialmenu/social.png"
data-ej-text="social" data-ej-enabled="false"></li>
<li data-ej-imageurl="../themes/sample/radialmenu/music.png" 
data-ej-text="music"></li>
<li data-ej-imageurl="../themes/sample/radialmenu/direction.png" 
data-ej-text="direction" data-ej-enabled="false"></li>
<li data-ej-imageurl="../themes/sample/radialmenu/message.png" 
data-ej-text="message"></li>
<li data-ej-imageurl="../themes/sample/radialmenu/browser.png" 
data-ej-text="browser"></li>
</ul>
</div>{% endhighlight %}


{% highlight html %}
 
<script>
$("#defaultRadialMenu").ejRadialMenu({ "autoOpen":true});  
var obj=$("#defaultRadialMenu").ejRadialMenu("instance");
obj.enableItems(["social","direction"]);
</script>{% endhighlight %}




### disableItems(items)
{:#methods:disableitems}


To disable menu items using item texts

<table>
<tr>
<td>
<b>Parameters</b></td><td>
<b>Type</b></td><td>
<b>Description</b></td></tr>
<tr>
<td>
items</td><td>
Array</td><td>
items of the Radialmenu item to disable.</td></tr>
</table>



Example
{:.example}


{% highlight html %}
 
<div >
<br />
<p>
Model-view-controller (MVC) is a software architecture pattern which separates the representation of information from the user's interaction with it.
</p>
</div>  
<div id="defaultRadialMenu">
<ul>
<li data-ej-imageurl="../themes/sample/radialmenu/social.png"
data-ej-text="social"></li>
<li data-ej-imageurl="../themes/sample/radialmenu/music.png" 
data-ej-text="music"></li>
<li data-ej-imageurl="../themes/sample/radialmenu/direction.png" 
data-ej-text="direction"></li>
<li data-ej-imageurl="../themes/sample/radialmenu/message.png" 
data-ej-text="message"></li>
<li data-ej-imageurl="../themes/sample/radialmenu/browser.png" 
data-ej-text="browser"></li>
</ul>
</div>{% endhighlight %}


{% highlight html %}
 
<script>
$("#defaultRadialMenu").ejRadialMenu({ "autoOpen":true});  
var obj=$("#defaultRadialMenu").ejRadialMenu("instance");
obj.disableItems(["social","direction"]);
</script>{% endhighlight %}




### updateBadgeValue(index, value)
{:#methods:updatebadgevalue}


To update menu item badge value

<table>
<tr>
<td>
<b>Parameters</b></td><td>
<b>Type</b></td><td>
<b>Description</b></td></tr>
<tr>
<td>
index</td><td>
number</td><td>
The index value to add the given items at the specified index. If index is not specified, the given value will not be updated.</td></tr>
<tr>
<td>
value</td><td>
number</td><td>
The Value to be updated in the badge. It will be updated based on the given index</td></tr>
</table>


Example
{:.example}


{% highlight html %}
 
<div >
<br />
<p>
Model-view-controller (MVC) is a software architecture pattern which separates the representation of information from the user's interaction with it.
</p>
</div>  
<div id="defaultRadialMenu">
<ul>
<li data-ej-imageurl="../themes/sample/radialmenu/social.png"
data-ej-text="social" data-ej-badge-enabled="true" data-ej-badge-value="3"></li>
<li data-ej-imageurl="../themes/sample/radialmenu/music.png" 
data-ej-text="music"></li>
<li data-ej-imageurl="../themes/sample/radialmenu/direction.png" 
data-ej-text="direction"></li>
<li data-ej-imageurl="../themes/sample/radialmenu/message.png" 
data-ej-text="message"></li>
<li data-ej-imageurl="../themes/sample/radialmenu/browser.png" 
data-ej-text="browser"></li>
</ul>
</div>{% endhighlight %}


{% highlight html %}
 
<script>
$("#defaultRadialMenu").ejRadialMenu({ "autoOpen":true});  
var obj=$("#defaultRadialMenu").ejRadialMenu("instance");
obj.updateBadgeValue(0,4);
</script>{% endhighlight %}




### showBadge(index)
{:#methods:showbadge}


To show menu item badge 

<table>
<tr>
<td>
<b>Parameters</b></td><td>
<b>Type</b></td><td>
<b>Description</b></td></tr>
<tr>
<td>
index</td><td>
number</td><td>
Index of the Radialmenu item to be shown badge.</td></tr>
</table>





Example
{:.example}


{% highlight html %}
 
<div >
<br />
<p>
Model-view-controller (MVC) is a software architecture pattern which separates the representation of information from the user's interaction with it.
</p>
</div>  
<div id="defaultRadialMenu">
<ul>
<li data-ej-imageurl="../themes/sample/radialmenu/social.png"
data-ej-text="social" data-ej-badge-enabled="true" data-ej-badge-value="3"></li>
<li data-ej-imageurl="../themes/sample/radialmenu/music.png" 
data-ej-text="music"></li>
<li data-ej-imageurl="../themes/sample/radialmenu/direction.png" 
data-ej-text="direction"></li>
<li data-ej-imageurl="../themes/sample/radialmenu/message.png" 
data-ej-text="message"></li>
<li data-ej-imageurl="../themes/sample/radialmenu/browser.png" 
data-ej-text="browser"></li>
</ul>
</div>{% endhighlight %}


{% highlight html %}
 
<script>
$("#defaultRadialMenu").ejRadialMenu({ "autoOpen":true});  
var obj=$("#defaultRadialMenu").ejRadialMenu("instance");
obj.showBadge(0);
</script>{% endhighlight %}




### hideBadge(index)
{:#methods:hidebadge}


To hide menu item badge 

<table>
<tr>
<td>
<b>Parameters</b></td><td>
<b>Type</b></td><td>
<b>Description</b></td></tr>
<tr>
<td>
index</td><td>
number</td><td>
Index of the Radialmenu item to hide the badge.</td></tr>
</table>



Example
{:.example}


{% highlight html %}
 
<div >
<br />
<p>
Model-view-controller (MVC) is a software architecture pattern which separates the representation of information from the user's interaction with it.
</p>
</div>  
<div id="defaultRadialMenu">
<ul>
<li data-ej-imageurl="../themes/sample/radialmenu/social.png"
data-ej-text="social" data-ej-badge-enabled="true" data-ej-badge-value="3"></li>
<li data-ej-imageurl="../themes/sample/radialmenu/music.png" 
data-ej-text="music"></li>
<li data-ej-imageurl="../themes/sample/radialmenu/direction.png" 
data-ej-text="direction"></li>
<li data-ej-imageurl="../themes/sample/radialmenu/message.png" 
data-ej-text="message"></li>
<li data-ej-imageurl="../themes/sample/radialmenu/browser.png" 
data-ej-text="browser"></li>
</ul>
</div>{% endhighlight %}


{% highlight html %}
 
<script>
$("#defaultRadialMenu").ejRadialMenu({ "autoOpen":true});  
var obj=$("#defaultRadialMenu").ejRadialMenu("instance");
obj.hideBadge(0);
</script>{% endhighlight %}




## Events



### select[Deprecated]
{:#events:selectdeprecated}




Event triggers when we select an item.

N>Since it is deprecated use the method “[click](#events:click)”

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
<td class="name">{% highlight html %}
argument{% endhighlight %}</td>
<td class="type"><span class="param-type">Object</span></td>
<td class="description last">Event parameters from Radialmenu
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
<td class="name">{% highlight html %}
cancel{% endhighlight %}</td>
<td class="type"><span class="param-type">boolean</span></td>
<td class="description last">if the event should be canceled; otherwise, false.</td>
</tr>
<tr>
<td class="name">{% highlight html %}
model{% endhighlight %}</td>
<td class="type"><span class="param-type">Object</span></td>
<td class="description last">returns the Radialmenu model</td>
</tr>
<tr>
<td class="name">{% highlight html %}
type{% endhighlight %}</td>
<td class="type"><span class="param-type">string</span></td>
<td class="description last">returns the name of the event</td>
</tr>
<tr>
<td class="name">{% highlight html %}
item{% endhighlight %}</td>
<td class="type"><span class="param-type">Object</span></td>
<td class="description last">returns the item of element</td>
</tr>
<tr>
<td class="name">{% highlight html %}
itemName{% endhighlight %}</td>
<td class="type"><span class="param-type">String</span></td>
<td class="description last">returns the name of item</td>
</tr>
</tbody>
</table>
</td>
</tr>
</tbody>
</table>


Example
{:.example}


{% highlight html %}
 
//select event for Radialmenu
<div >
<br />
<p>
Syncfusion is the enterprise technology partner of choice for Windows development
</p>
</div>  
<div id="defaultRadialMenu">
<ul>
<li data-ej-imageurl="../themes/sample/radialmenu/social.png"
data-ej-text="social"></li>
<li data-ej-imageurl="../themes/sample/radialmenu/music.png" 
data-ej-text="music"></li>
<li data-ej-imageurl="../themes/sample/radialmenu/direction.png" 
data-ej-text="direction"></li>
<li data-ej-imageurl="../themes/sample/radialmenu/message.png" 
data-ej-text="message"></li>
<li data-ej-imageurl="../themes/sample/radialmenu/browser.png" 
data-ej-text="browser"></li>
</ul>
</div>
<script>
$("#defaultRadialMenu").ejRadialMenu({
  select: function (args) { //handle the event
}
});         
</script>{% endhighlight %}



### click
{:#events:click}




Event triggers when we click an item.



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
<td class="name">{% highlight html %}
argument{% endhighlight %}</td>
<td class="type"><span class="param-type">Object</span></td>
<td class="description last">Event parameters from Radialmenu
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
<td class="name">{% highlight html %}
cancel{% endhighlight %}</td>
<td class="type"><span class="param-type">boolean</span></td>
<td class="description last">if the event should be canceled; otherwise, false.</td>
</tr>
<tr>
<td class="name">{% highlight html %}
model{% endhighlight %}</td>
<td class="type"><span class="param-type">Object</span></td>
<td class="description last">returns the Radialmenu model</td>
</tr>
<tr>
<td class="name">{% highlight html %}
type{% endhighlight %}</td>
<td class="type"><span class="param-type">string</span></td>
<td class="description last">returns the name of the event</td>
</tr>
<tr>
<td class="name">{% highlight html %}
item{% endhighlight %}</td>
<td class="type"><span class="param-type">Object</span></td>
<td class="description last">returns the item of element</td>
</tr>
<tr>
<td class="name">{% highlight html %}
itemName{% endhighlight %}</td>
<td class="type"><span class="param-type">String</span></td>
<td class="description last">returns the name of item</td>
</tr>
</tbody>
</table>
</td>
</tr>
</tbody>
</table>


Example
{:.example}


{% highlight html %}
 
//click event for Radialmenu
<div >
<br />
<p>
Model-view-controller (MVC) is a software architecture pattern which separates the representation of information from the user's interaction with it.
</p>
</div>  
<div id="defaultRadialMenu">
<ul>
<li data-ej-imageurl="../themes/sample/radialmenu/social.png"
data-ej-text="social"></li>
<li data-ej-imageurl="../themes/sample/radialmenu/music.png" 
data-ej-text="music"></li>
<li data-ej-imageurl="../themes/sample/radialmenu/direction.png" 
data-ej-text="direction"></li>
<li data-ej-imageurl="../themes/sample/radialmenu/message.png" 
data-ej-text="message"></li>
<li data-ej-imageurl="../themes/sample/radialmenu/browser.png" 
data-ej-text="browser"></li>
</ul>
</div>
<script>
$("#defaultRadialMenu").ejRadialMenu({
  click: function (args) { //handle the event
}
});         
</script>{% endhighlight %}




### open 
{:#events:open}




Event triggers when the menu is opened.

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
<td class="name">{% highlight html %}
argument{% endhighlight %}</td>
<td class="type"><span class="param-type">Object</span></td>
<td class="description last">Event parameters from Radialmenu
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
<td class="name">{% highlight html %}
cancel{% endhighlight %}</td>
<td class="type"><span class="param-type">boolean</span></td>
<td class="description last">if the event should be canceled; otherwise, false.</td>
</tr>
<tr>
<td class="name">{% highlight html %}
model{% endhighlight %}</td>
<td class="type"><span class="param-type">Object</span></td>
<td class="description last">returns the Radialmenu model</td>
</tr>
<tr>
<td class="name">{% highlight html %}
type{% endhighlight %}</td>
<td class="type"><span class="param-type">string</span></td>
<td class="description last">returns the name of the event</td>
</tr>
</tbody>
</table>
</td>
</tr>
</tbody>
</table>


Example
{:.example}


{% highlight html %}
 
//open event for Radialmenu
<div >
<br />
<p>
Model-view-controller (MVC) is a software architecture pattern which separates the representation of information from the user's interaction with it.
</p>
</div>  
<div id="defaultRadialMenu">
<ul>
<li data-ej-imageurl="../themes/sample/radialmenu/social.png"
data-ej-text="social"></li>
<li data-ej-imageurl="../themes/sample/radialmenu/music.png" 
data-ej-text="music"></li>
<li data-ej-imageurl="../themes/sample/radialmenu/direction.png" 
data-ej-text="direction"></li>
<li data-ej-imageurl="../themes/sample/radialmenu/message.png" 
data-ej-text="message"></li>
<li data-ej-imageurl="../themes/sample/radialmenu/browser.png" 
data-ej-text="browser"></li>
</ul>
</div>
<script>
$("#defaultRadialMenu").ejRadialMenu({
  open: function (args) { //handle the event
}
});         
</script>{% endhighlight %}




### close 
{:#events:close}




Event triggers when the menu is closed.

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
<td class="name">{% highlight html %}
argument{% endhighlight %}</td>
<td class="type"><span class="param-type">Object</span></td>
<td class="description last">Event parameters from Radialmenu
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
<td class="name">{% highlight html %}
cancel{% endhighlight %}</td>
<td class="type"><span class="param-type">boolean</span></td>
<td class="description last">if the event should be canceled; otherwise, false.</td>
</tr>
<tr>
<td class="name">{% highlight html %}
model{% endhighlight %}</td>
<td class="type"><span class="param-type">Object</span></td>
<td class="description last">returns the Radialmenu model</td>
</tr>
<tr>
<td class="name">{% highlight html %}
type{% endhighlight %}</td>
<td class="type"><span class="param-type">string</span></td>
<td class="description last">returns the name of the event</td>
</tr>
</tbody>
</table>
</td>
</tr>
</tbody>
</table>


Example
{:.example}


{% highlight html %}
 
//close event for Radialmenu
<div >
<br />
<p>
Model-view-controller (MVC) is a software architecture pattern which separates the representation of information from the user's interaction with it.
</p>
</div>  
<div id="defaultRadialMenu">
<ul>
<li data-ej-imageurl="../themes/sample/radialmenu/social.png"
data-ej-text="social"></li>
<li data-ej-imageurl="../themes/sample/radialmenu/music.png" 
data-ej-text="music"></li>
<li data-ej-imageurl="../themes/sample/radialmenu/direction.png" 
data-ej-text="direction"></li>
<li data-ej-imageurl="../themes/sample/radialmenu/message.png" 
data-ej-text="message"></li>
<li data-ej-imageurl="../themes/sample/radialmenu/browser.png" 
data-ej-text="browser"></li>
</ul>
</div>
<script>
$("#defaultRadialMenu").ejRadialMenu({
  close: function (args) { //handle the event
}
});         
</script>{% endhighlight %}




