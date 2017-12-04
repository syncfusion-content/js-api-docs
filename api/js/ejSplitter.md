---
layout: post
title: Properties, Methods and Events of ejSplitter Widget
description: API reference for ejSplitter
documentation: API
platform: js-api
keywords: Splitter, ejSplitter, syncfusion, Splitter api  
---

# ejSplitter



The Splitter is a layout control that enables you to divide a Web page into distinct areas by inserting resizable panes. You can create any number of Splitter panes and place them inside the Splitter control. The split bars are inserted automatically in between the adjacent panes.



#### Syntax

{% highlight javascript %}

$(element).ejSplitter(options)

{% endhighlight %}



<table class="params">
<thead>
<tr>
<th>Name</th>
<th>Type</th>
<th>Description</th>
</tr>
</thead>
<tbody>
<tr>
<td class="name">
options</td>
<td class="type"><span class="param-type">Object</span></td>
<td class="description">settings for Splitter.</td>
</tr>
</tbody>
</table>




#### Example



{% highlight html %}
<div id="innerSplitter">
        <div>
                <div class="cont">Pane 1 </div>
        </div>
        <div>
                <div class="cont">Pane 2 </div>
        </div>
</div> 
<script>
// Create Splitter 
$('#innerSplitter').ejSplitter(); 
</script>{% endhighlight %}







#### Requires





* module:jQuery


* module:ej.core.js


* module:ej.splitter.js




## Members







### allowKeyboardNavigation `boolean`
{:#members:allowkeyboardnavigation}








Turns on keyboard interaction with the Splitter panes. You must set this property to true to access the keyboard shortcuts of ejSplitter.





#### Default Value







* true








#### Example



{% highlight html %}
<div id="innerSplitter">
<div>
<div class="cont">Pane 1 </div>
</div>
<div>
<div class="cont">Pane 2 </div>
</div>
</div> 
<script>
//To set allowKeyboardNavigation API value during initialization
        $("#innerSplitter").ejSplitter({allowKeyboardNavigation: false});
</script>{% endhighlight %}













### animationSpeed `number`
{:#members:animationspeed}








Specify animation speed for the Splitter pane movement, while collapsing and expanding.




#### Default Value







* 300








#### Example



{% highlight html %}
 
<div id="innerSplitter">
<div>
<div class="cont">Pane 1 </div>
</div>
<div>
<div class="cont">Pane 2 </div>
</div>
</div> 
<script>
//To set animationSpeed API value during initialization
$("#innerSplitter").ejSplitter({animationSpeed: 150 });
</script>{% endhighlight %}







### cssClass `string`
{:#members:cssclass}








Specify the CSS class to splitter control to achieve custom theme.




#### Default Value







* &ldquo;&rdquo;








#### Example



{% highlight html %}
<div id="innerSplitter">
        <div>
                <div class="cont">Pane 1 </div>
        </div>
        <div>
                <div class="cont">Pane 2 </div>
        </div>
</div> 
<script>
//To set cssClass API value during initialization
        $("#innerSplitter").ejSplitter({ cssClass: "gradient-lime"});
</script>{% endhighlight %}







### enableAnimation `boolean`
{:#members:enableanimation}








Specifies the animation behavior of the splitter.




#### Default Value







* true








#### Example



{% highlight html %}
 
<div id="innerSplitter">
        <div>
                <div class="cont">Pane 1 </div>
        </div>
        <div>
                <div class="cont">Pane 2 </div>
        </div>
</div> 
<script>
//To set enableAnimation API value during initialization  
        $("#innerSplitter").ejSplitter({ enableAnimation: false});
</script>{% endhighlight %}










### enableRTL `boolean`
{:#members:enablertl}






Specifies the splitter control to be displayed in right to left direction.





#### Default Value







* false








#### Example



{% highlight html %}
<div id="innerSplitter">
<div>
<div class="cont">Pane 1 </div>
</div>
<div>
<div class="cont">Pane 2 </div>
</div>
</div> 
<script>
//To set enableRTL API value during initialization  
        $("#innerSplitter").ejSplitter({enableRTL: true} );
</script>{% endhighlight %}



### expanderTemplate `string`
{:#members:expandertemplate}

Specifies HTML element string to replace the existing expand/collapse icons.


#### Default Value

* null


#### Example

{% highlight html %}
 
        <div id="innerSplitter">
        <div>
        <div class="cont">Pane 1 </div>
        </div>
        <div>
        <div class="cont">Pane 2 </div>
        </div>
        </div> 
        <script>
        //To set expanderTemplate API value during initialization
                $("#innerSplitter").ejSplitter({ expanderTemplate: '<img class="eimg" src="expander.png" alt="employee"/>', });
        </script>

{% endhighlight %}



### height `string`
{:#members:height}








Specify height for splitter control.




#### Default Value







* null








#### Example



{% highlight html %}
 
<div id="innerSplitter">
<div>
<div class="cont">Pane 1 </div>
</div>
<div>
<div class="cont">Pane 2 </div>
</div>
</div> 
<script>
//To set height API value during initialization
        $("#innerSplitter").ejSplitter({height: "100%" });
</script>{% endhighlight %}






### htmlAttributes `Object`
{:#members:htmlattributes}








Specifies the HTML Attributes of the Splitter.





#### Default Value







* {}








#### Example



{% highlight html %}
<div id="innerSplitter">
<div>
<div class="cont">Pane 1 </div>
</div>
<div>
<div class="cont">Pane 2 </div>
</div>
</div> 
<script>
//Set HtmlAttributes API during initialization
        $("#innerSplitter").ejSplitter({htmlAttributes: {class:"my-class"}});
</script>{% endhighlight %}










### isResponsive `boolean`
{:#members:isresponsive}








Specify window resizing behavior for splitter control.




#### Default Value







* false








#### Example



{% highlight html %}
<div id="innerSplitter">
<div>
<div class="cont">Pane 1 </div>
</div>
<div>
<div class="cont">Pane 2 </div>
</div>
</div> 
<script>
//To set isResponsive API value during initialization
        $("#innerSplitter").ejSplitter({isResponsive: true});
</script>{% endhighlight %}




N> We have renamed the API "enableAutoResize" to "isResponsive".






### orientation `enum`
{:#members:orientation}


<ts ref = "ej.Orientation"/>








Specify the orientation for splitter control. See orientation


<table class="params">
<thead>
<tr>
<th>Name</th>
<th>Description</th>
</tr>
</thead>
<tbody>
<tr>
<td class="name">
Horizontal</td>
<td class="description">To set the horizontal orientation for splitter control</td>
</tr>
<tr>
<td class="name">
Vertical</td>
<td class="description">To set the vertical orientation for splitter control</td>
</tr>
</tbody>
</table>




#### Default Value







* ej.orientation.Horizontal or &ldquo;horizontal&rdquo;








#### Example



{% highlight html %}
<div id="innerSplitter">
<div>
<div class="cont">Pane 1 </div>
</div>
<div>
<div class="cont">Pane 2 </div>
</div>
</div> 
<script>
//To set orientation API value during initialization  
$("#innerSplitter").ejSplitter({ orientation: ej.Orientation.Horizontal });
</script>{% endhighlight %}







### properties `Array`
{:#members:properties}








Specify properties for each pane like paneSize, minSize, maxSize, collapsible, expandable, resizable. 




#### Default Value







* []








#### Example



{% highlight html %}
 
<div id="innerSplitter">
<div>
<div class="cont">Pane 1 </div>
</div>
<div>
<div class="cont">Pane 2 </div>
</div>
</div> 
<script>
//To set properties API value during initialization  
        $("#innerSplitter").ejSplitter({properties: [{ paneSize: "100px", expandable:false }, { collapsible:false, paneSize: "50px"}]});
</script>{% endhighlight %}







### width `string`
{:#members:width}








Specify width for splitter control.




#### Default Value







* null








#### Example



{% highlight html %}
 
<div id="innerSplitter">
<div>
<div class="cont">Pane 1 </div>
</div>
<div>
<div class="cont">Pane 2 </div>
</div>
</div> 
<script>
//To set width API value during initialization  
        $("#innerSplitter").ejSplitter({width: 600} );
</script>{% endhighlight %}





## Methods








### addItem(content, property, index)
{:#methods:additem}








To add a new pane to splitter control.

<table class="params">
<thead>
<tr>
<th>Name</th>
<th>Type</th>
<th>Description</th>
</tr>
</thead>
<tbody>
<tr>
<td class="name">
content</td>
<td class="type"><span class="param-type">string</span></td>
<td class="description">content of pane.</td>
</tr>
<tr>
<td class="name">
property</td>
<td class="type"><span class="param-type">Object</span></td>
<td class="description">pane properties.</td>
</tr>
<tr>
<td class="name">
index</td>
<td class="type"><span class="param-type">number</span></td>
<td class="description">index of pane.</td>
</tr>
</tbody>
</table>


#### Returns:
Element

#### Example



{% highlight html %}
 
<div id="innerSplitter">
<div>
<div class="cont">Pane 1 </div>
</div>
<div>
<div class="cont">Pane 2 </div>
</div>
</div>
<script>
$("#innerSplitter").ejSplitter();
// Create splitter control
var splitterObj = $("#innerSplitter").data("ejSplitter");
splitterObj.addItem("New pane 0",{ paneSize:20, minSize:20, maxSize:100},0);
</script>{% endhighlight %}


{% highlight html %}
 
<div id="innerSplitter">
<div>
<div class="cont">Pane 1 </div>
</div>
<div>
<div class="cont">Pane 2 </div>
</div>
</div>
<script>
$("#innerSplitter").ejSplitter();
// expand the splitter control
$("#innerSplitter").ejSplitter("addItem","New pane 0",{ paneSize:20, minSize:20, maxSize:100},0);
</script>{% endhighlight %}







### collapse(paneIndex)
{:#methods:collapse}








To collapse the splitter control pane.



<table class="params">
<thead>
<tr>
<th>Name</th>
<th>Type</th>
<th>Description</th>
</tr>
</thead>
<tbody>
<tr>
<td class="name">
paneIndex</td>
<td class="type"><span class="param-type">number</span></td>
<td class="description">index number of pane.</td>
</tr>
</tbody>
</table>



#### Example



{% highlight html %}
 
<div id="innerSplitter">
<div>
<div class="cont">Pane 1 </div>
</div>
<div>
<div class="cont">Pane 2 </div>
</div>
</div>
<script>
$("#innerSplitter").ejSplitter();
// Create splitter control
var splitterObj = $("#innerSplitter").data("ejSplitter");
splitterObj.collapse(0); // collapse the splitter control pane.
</script>{% endhighlight %}


{% highlight html %}
 
<div id="innerSplitter">
<div>
<div class="cont">Pane 1 </div>
</div>
<div>
<div class="cont">Pane 2 </div>
</div>
</div>
<script>
$("#innerSplitter").ejSplitter();
// collapse the splitter control
$("#innerSplitter").ejSplitter("collapse", 0);
</script>{% endhighlight %}







### expand(paneIndex)
{:#methods:expand}








To expand the splitter control pane.




<table class="params">
<thead>
<tr>
<th>Name</th>
<th>Type</th>
<th>Description</th>
</tr>
</thead>
<tbody>
<tr>
<td class="name">
paneIndex</td>
<td class="type"><span class="param-type">number</span></td>
<td class="description">index number of pane.</td>
</tr>
</tbody>
</table>




#### Example



{% highlight html %}
 
<div id="innerSplitter">
<div>
<div class="cont">Pane 1 </div>
</div>
<div>
<div class="cont">Pane 2 </div>
</div>
</div>
<script>
$("#innerSplitter").ejSplitter();
// Create splitter control
var splitterObj = $("#innerSplitter").data("ejSplitter");
splitterObj.expand(0); // expand the splitter control pane.
</script>{% endhighlight %}


{% highlight html %}
 
<div id="innerSplitter">
<div>
<div class="cont">Pane 1 </div>
</div>
<div>
<div class="cont">Pane 2 </div>
</div>
</div>
<script>
$("#innerSplitter").ejSplitter();
// expand the splitter control
$("#innerSplitter").ejSplitter("expand", 0);
</script>{% endhighlight %}







### refresh()
{:#methods:refresh}








To refresh the splitter control pane resizing.





#### Example



{% highlight html %}
 
<div id="innerSplitter">
<div>
<div class="cont">Pane 1 </div>
</div>
<div>
<div class="cont">Pane 2 </div>
</div>
</div>
<script>
$("#innerSplitter").ejSplitter();
// Create splitter control
var splitterObj = $("#innerSplitter").data("ejSplitter");
splitterObj.refresh(); // refresh the splitter control pane resizing.
</script>{% endhighlight %}


{% highlight html %}
 
<div id="innerSplitter">
<div>
<div class="cont">Pane 1 </div>
</div>
<div>
<div class="cont">Pane 2 </div>
</div>
</div>
<script>
$("#innerSplitter").ejSplitter();
// refresh the splitter control
$("#innerSplitter").ejSplitter("refresh");
</script>{% endhighlight %}







### removeItem(index)
{:#methods:removeitem}








To remove a specified pane from the splitter control.

<table class="params">
<thead>
<tr>
<th>Name</th>
<th>Type</th>
<th>Description</th>
</tr>
</thead>
<tbody>
<tr>
<td class="name">
index</td>
<td class="type"><span class="param-type">number</span></td>
<td class="description">index of pane.</td>
</tr>
</tbody>
</table>


#### Example



{% highlight html %}
 
<div id="innerSplitter">
<div>
<div class="cont">Pane 1 </div>
</div>
<div>
<div class="cont">Pane 2 </div>
</div>
</div>
<script>
$("#innerSplitter").ejSplitter();
// Create splitter control
var splitterObj = $("#innerSplitter").data("ejSplitter");
splitterObj.removeItem(0); 
</script>{% endhighlight %}


{% highlight html %}
 
<div id="innerSplitter">
<div>
<div class="cont">Pane 1 </div>
</div>
<div>
<div class="cont">Pane 2 </div>
</div>
</div>
<script>
$("#innerSplitter").ejSplitter();
// expand the splitter control
$("#innerSplitter").ejSplitter("removeItem",0);
</script>{% endhighlight %}





## Events








### beforeExpandCollapse
{:#events:beforeexpandcollapse}








Fires before expanding / collapsing the split pane of splitter control.

<table class="params">
<thead>
<tr>
<th>Name</th>
<th>Type</th>
<th>Description</th>
</tr>
</thead>
<tbody>
<tr>
<td class="name">
argument</td>
<td class="type"><span class="param-type">Object</span></td>
<td class="description">Event parameters from splitter control
<table class="params">
<thead>
<tr>
<th>Name</th>
<th>Type</th>
<th>Description</th>
</tr>
</thead>
<tbody>
<tr>
<td class="name">
cancel</td>
<td class="type"><span class="param-type">boolean</span></td>
<td class="description">if the event should be canceled; otherwise, false.</td>
</tr>
<tr>
<td class="name">
collapsed</td>
<td class="type"><span class="param-type">Object</span></td>
<td class="description">returns collapsed pane details.</td>
</tr>
<tr>
<td class="name">
expanded</td>
<td class="type"><span class="param-type">Object</span></td>
<td class="description">returns expanded pane details.</td>
</tr>
<tr>
<td class="name">
model</td>
<td class="type"><ts ref="ej.Splitter.Model"/><span class="param-type">Object</span></td>
<td class="description">returns the splitter model.</td>
</tr>
<tr>
<td class="name">
splitbarIndex</td>
<td class="type"><span class="param-type">number</span></td>
<td class="description">returns the current split bar index.</td>
</tr>
<tr>
<td class="name">
type</td>
<td class="type"><span class="param-type">string</span></td>
<td class="description">returns the name of the event.</td>
</tr>
</tbody>
</table>
</td>
</tr>
</tbody>
</table>




#### Example



{% highlight html %}
 
<div id="innerSplitter">
<div>
<div class="cont">Pane 1 </div>
</div>
<div>
<div class="cont">Pane 2 </div>
</div>
</div> 
<script>
//beforeExpandCollapse event for splitter control
$("#innerSplitter").ejSplitter({
   beforeExpandCollapse: function (args) {}
});
</script>{% endhighlight %}



### clickOnExpander
{:#events:clickonexpander}

Triggered when we click on the template icon. (Note: This will work only when expanderTemplate is defined.)

<table class="params">
<thead>
<tr>
<th>Name</th>
<th>Type</th>
<th>Description</th>
</tr>
</thead>
<tbody>
<tr>
<td class="name">
argument</td>
<td class="type"><span class="param-type">Object</span></td>
<td class="description">Event parameters from splitter control
<table class="params">
<thead>
<tr>
<th>Name</th>
<th>Type</th>
<th>Description</th>
</tr>
</thead>
<tbody>
<tr>
<td class="name">
cancel</td>
<td class="type"><span class="param-type">boolean</span></td>
<td class="description">if the event should be canceled; otherwise, false.</td>
</tr>
<tr>
<td class="name">
model</td>
<td class="type"><ts ref="ej.Splitter.Model"/><span class="param-type">Object</span></td>
<td class="description">returns the splitter model.</td>
</tr>
<tr>
<td class="name">
type</td>
<td class="type"><span class="param-type">string</span></td>
<td class="description">returns the name of the event.</td>
</tr>
<tr>
<td class="name">
targetElement</td>
<td class="type"><span class="param-type">Object</span></td>
<td class="description">returns the target element from which click action is triggered.</td>
</tr>
</tbody>
</table>
</td>
</tr>
</tbody>
</table>




#### Example



{% highlight html %}

        <div id="innerSplitter">
        <div>
        <div class="cont">Pane 1 </div>
        </div>
        <div>
        <div class="cont">Pane 2 </div>
        </div>
        </div> 
        <script>
        //create event for splitter control
        $("#innerSplitter").ejSplitter({
                expanderTemplate: '<img class="eimg" src="expander.png" alt="employee"/>',
                clickOnExpander: function(args)
                { });
        </script>

{% endhighlight %}




### create
{:#events:create}








Fires when splitter control pane has been created.

<table class="params">
<thead>
<tr>
<th>Name</th>
<th>Type</th>
<th>Description</th>
</tr>
</thead>
<tbody>
<tr>
<td class="name">
argument</td>
<td class="type"><span class="param-type">Object</span></td>
<td class="description">Event parameters from splitter control
<table class="params">
<thead>
<tr>
<th>Name</th>
<th>Type</th>
<th>Description</th>
</tr>
</thead>
<tbody>
<tr>
<td class="name">
cancel</td>
<td class="type"><span class="param-type">boolean</span></td>
<td class="description">if the event should be canceled; otherwise, false.</td>
</tr>
<tr>
<td class="name">
model</td>
<td class="type"><ts ref="ej.Splitter.Model"/><span class="param-type">Object</span></td>
<td class="description">returns the splitter model.</td>
</tr>
<tr>
<td class="name">
type</td>
<td class="type"><span class="param-type">string</span></td>
<td class="description">returns the name of the event.</td>
</tr>
</tbody>
</table>
</td>
</tr>
</tbody>
</table>




#### Example



{% highlight html %}
<div id="innerSplitter">
<div>
<div class="cont">Pane 1 </div>
</div>
<div>
<div class="cont">Pane 2 </div>
</div>
</div> 
<script>
//create event for splitter control
$("#innerSplitter").ejSplitter({
   create: function (args) {}
});
</script>{% endhighlight %}







### destroy
{:#events:destroy}








Fires when splitter control pane has been destroyed.

<table class="params">
<thead>
<tr>
<th>Name</th>
<th>Type</th>
<th>Description</th>
</tr>
</thead>
<tbody>
<tr>
<td class="name">
argument</td>
<td class="type"><span class="param-type">Object</span></td>
<td class="description">Event parameters from splitter control
<table class="params">
<thead>
<tr>
<th>Name</th>
<th>Type</th>
<th>Description</th>
</tr>
</thead>
<tbody>
<tr>
<td class="name">
cancel</td>
<td class="type"><span class="param-type">boolean</span></td>
<td class="description">if the event should be canceled; otherwise, false.</td>
</tr>
<tr>
<td class="name">
model</td>
<td class="type"><ts ref="ej.Splitter.Model"/><span class="param-type">Object</span></td>
<td class="description">returns the splitter model.</td>
</tr>
<tr>
<td class="name">
type</td>
<td class="type"><span class="param-type">string</span></td>
<td class="description">returns the name of the event.</td>
</tr>
</tbody>
</table>
</td>
</tr>
</tbody>
</table>




#### Example



{% highlight html %}
<div id="innerSplitter">
<div>
<div class="cont">Pane 1 </div>
</div>
<div>
<div class="cont">Pane 2 </div>
</div>
</div> 
<script>
//destroy event for splitter control
$("#innerSplitter").ejSplitter({
   destroy: function (args) {}
});
</script>{% endhighlight %}







### expandCollapse
{:#events:expandcollapse}








Fires when expand / collapse operation in splitter control pane has been performed successfully.

<table class="params">
<thead>
<tr>
<th>Name</th>
<th>Type</th>
<th>Description</th>
</tr>
</thead>
<tbody>
<tr>
<td class="name">
argument</td>
<td class="type"><span class="param-type">Object</span></td>
<td class="description">Event parameters from splitter control
<table class="params">
<thead>
<tr>
<th>Name</th>
<th>Type</th>
<th>Description</th>
</tr>
</thead>
<tbody>
<tr>
<td class="name">
cancel</td>
<td class="type"><span class="param-type">boolean</span></td>
<td class="description">if the event should be canceled; otherwise, false.</td>
</tr>
<tr>
<td class="name">
collapsed</td>
<td class="type"><span class="param-type">Object</span></td>
<td class="description">returns collapsed pane details.</td>
</tr>
<tr>
<td class="name">
expanded</td>
<td class="type"><span class="param-type">Object</span></td>
<td class="description">returns expanded pane details.</td>
</tr>
<tr>
<td class="name">
model</td>
<td class="type"><ts ref="ej.Splitter.Model"/><span class="param-type">Object</span></td>
<td class="description">returns the splitter model.</td>
</tr>
<tr>
<td class="name">
splitbarIndex</td>
<td class="type"><span class="param-type">number</span></td>
<td class="description">returns the current split bar index.</td>
</tr>
<tr>
<td class="name">
type</td>
<td class="type"><span class="param-type">string</span></td>
<td class="description">returns the name of the event.</td>
</tr>
</tbody>
</table>
</td>
</tr>
</tbody>
</table>




#### Example



{% highlight html %}
 
<div id="innerSplitter">
<div>
<div class="cont">Pane 1 </div>
</div>
<div>
<div class="cont">Pane 2 </div>
</div>
</div> 
<script>
//expandCollapse event for splitter control
$("#innerSplitter").ejSplitter({
   expandCollapse: function (args) {}
});
</script>{% endhighlight %}







### resize
{:#events:resize}








Fires when resize in splitter control pane.

<table class="params">
<thead>
<tr>
<th>Name</th>
<th>Type</th>
<th>Description</th>
</tr>
</thead>
<tbody>
<tr>
<td class="name">
argument</td>
<td class="type"><span class="param-type">Object</span></td>
<td class="description">Event parameters from splitter control
<table class="params">
<thead>
<tr>
<th>Name</th>
<th>Type</th>
<th>Description</th>
</tr>
</thead>
<tbody>
<tr>
<td class="name">
cancel</td>
<td class="type"><span class="param-type">boolean</span></td>
<td class="description">if the event should be canceled; otherwise, false.</td>
</tr>
<tr>
<td class="name">
prevPane</td>
<td class="type"><span class="param-type">Object</span></td>
<td class="description">returns previous pane details.</td>
</tr>
<tr>
<td class="name">
nextPane</td>
<td class="type"><span class="param-type">Object</span></td>
<td class="description">returns next pane details.</td>
</tr>
<tr>
<td class="name">
model</td>
<td class="type"><ts ref="ej.Splitter.Model"/><span class="param-type">Object</span></td>
<td class="description">returns the splitter model.</td>
</tr>
<tr>
<td class="name">
splitbarIndex</td>
<td class="type"><span class="param-type">number</span></td>
<td class="description">returns the current split bar index.</td>
</tr>
<tr>
<td class="name">
type</td>
<td class="type"><span class="param-type">string</span></td>
<td class="description">returns the name of the event.</td>
</tr>
</tbody>
</table>
</td>
</tr>
</tbody>
</table>




#### Example



{% highlight html %}
<div id="innerSplitter">
<div>
<div class="cont">Pane 1 </div>
</div>
<div>
<div class="cont">Pane 2 </div>
</div>
</div> 
<script>
//resize event for splitter control
$("#innerSplitter").ejSplitter({
   resize: function (args) {}
});
</script>{% endhighlight %}




