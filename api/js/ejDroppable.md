---
layout: post
title: Properties, Methods and Events of ejDroppable Widget
description: API reference for ejDroppable
documentation: API
platform: js-api
keywords: Droppable, ejDroppable, syncfusion, Droppable api
---

# ejDroppable

Plugin to make any DOM element Droppable.  


#### Syntax

{% highlight javascript %}

$(element).ejDroppable()

{% endhighlight %}



#### Example



{% highlight html %}
 
<div  id="droppable" />
 
{% endhighlight %}

{% highlight javascript %}

<script>
// Create Draggable
$('#droppable').ejDroppable();   
</script>

{% endhighlight %}



#### Requires


* module:jQuery


* module:ej.core


* module:ej.droppable

## Members


### accept `object`
{:#members:accept}



Used to accept the specified draggable items.




#### Default Value



* null



#### Example



{% highlight javascript %}
 
//To set scope API value during initialization  
        $("#droppable").ejDroppable({ accept: null });                          
        
{% endhighlight %}


{% highlight javascript %}
 
//Get or set the accept API, after initialization:
        //Gets the accept value  
        $("#droppable").ejDroppable('option', 'accept');
                    
{% endhighlight %}




### scope `string`
{:#members:scope}


Used to group sets of droppable items, in addition to droppable's accept option. A draggable with the same scope value as a droppable will be accepted by the droppable.


#### Default Value



* 'default'




#### Example



{% highlight javascript %}
 
//To set scope API value during initialization  
        $("#droppable").ejDroppable({ scope: 'default' });                             
                
{% endhighlight %}


{% highlight javascript %}
 
//Get or set the scope API, after initialization:
        //Gets the scope value  
        $("#droppable").ejDroppable('option', 'scope');
                     
{% endhighlight %}





## Methods



### destroy()
{:#methods:destroy}

destroy in the Droppable.


#### Example


{% highlight html %}
 
<div  id="droppable"> </div > 
 
{% endhighlight %}


{% highlight javascript %}

<script>
// Create droppableObj
var droppableObj  = $("#droppable").data("ejDroppable");
droppableObj.destroy(); 
</script>

{% endhighlight %}



## Events



### drop
{:#events:drop}



This event is triggered when the mouse up is moved during the dragging.

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
<td class="type"><ts ref="ej.Droppable.Model"/><span class="param-type">object</span></td>
<td class="description">returns the autocomplete model</td>
</tr>
<tr>
<td class="name">
type</td>
<td class="type"><span class="param-type">string</span></td>
<td class="description">returns the name of the event</td>
</tr>
<tr>
<td class="name">
target</td>
<td class="type"><span class="param-type">object</span></td>
<td class="description">returns the element which accepts the droppable element.</td>
</tr>
</tbody>
</table>




#### Example



{% highlight html %}
 
//drop event for Droppable
$("#droppable").ejDroppable({ 
        drop: function(args) {}
});      

{% endhighlight %}





### out
{:#events:out}


This event is triggered when the mouse is moved out.

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
<td class="type"><ts ref="ej.Droppable.Model"/><span class="param-type">object</span></td>
<td class="description">returns the autocomplete model</td>
</tr>
<tr>
<td class="name">
type</td>
<td class="type"><span class="param-type">string</span></td>
<td class="description">returns the name of the event</td>
</tr>
<tr>
<td class="name">
target</td>
<td class="type"><span class="param-type">object</span></td>
<td class="description">returns the mouse out over the element</td>
</tr>
<tr>
</tbody>
</table>




#### Example



{% highlight html %}
 
//drop event for Droppable
$("#droppable").ejDroppable({ 
        out: function(args) {}
});      

{% endhighlight %}







### over
{:#events:over}


This event is triggered when the mouse is moved over.

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
<td class="type"><ts ref="ej.Droppable.Model"/><span class="param-type">object</span></td>
<td class="description">returns the autocomplete model</td>
</tr>
<tr>
<td class="name">
type</td>
<td class="type"><span class="param-type">string</span></td>
<td class="description">returns the name of the event</td>
</tr>
<tr>
<td class="name">
target</td>
<td class="type"><span class="param-type">object</span></td>
<td class="description">returns the mouse over the element</td>
</tr>
</tbody>
</table>




#### Example



{% highlight html %}
 
//drop event for Droppable
$("#droppable").ejDroppable({ 
        over: function(args) {}
});     

 {% endhighlight %}



