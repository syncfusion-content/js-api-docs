---
layout: post
title: Properties, Methods and Events of ejScroller Widget
description: API reference for ejScroller
documentation: API
platform: js-api
keywords: Scroller, ejScroller, syncfusion, Scroller api 
---

# ejScroller




The Scroller control has a sliding document whose position corresponds to a value. The document has text, HTML content or images. You can also customize the Scroller control by resizing the scrolling bar and changing the theme.



#### Syntax

{% highlight javascript %}

$(element).ejScroller()

{% endhighlight %}








#### Example



{% highlight html %}
 
<div id="scrollContent" style="width:900px;">
<div>
<p>Model view controller (MVC) is a software architecture pattern which separates the
representation of information from the user's interaction with it.
The model consists of application data, business rules, logic, and functions. A view can be any
output representation of data, such as a chart or a diagram. Multiple views of the same data 
are possible, such as a bar chart for management and a tabular view for accountants. 
The controller mediates input, converting it to commands for the model or view.The central 
ideas behind MVC are code reusable and in addition to dividing the application into three 
kinds of components, the MVC design defines the interactions between them.

<ul>
<li>
<b>A controller</b>  can send commands to its associated view to change the view's presentation of the model (e.g., by scrolling through a document). 
         It can also send commands to the model to update the model's state (e.g., editing a document).
</li>
</ul>
</div>     
</div> 
 
<script>
// Create Scroller
$('#scrollContent').ejScroller();       
</script>

{% endhighlight %}




#### Requires


* module:jQuery

* module:ej.core.js

* module:ej.draggable.js

* module:ej.touch.js

* module:ej.scroller.js


## Members



### animationSpeed `number`
{:#members:animationspeed}




Specifies the swipe scrolling speed(in millisecond).


#### Default Value




* 600




#### Example



{% highlight html %}
 
<div id="scrollContent" style="width:900px;" >
<div>
<p>Model view controller (MVC) is a software architecture pattern which separates the
representation of information from the user's interaction with it.
The model consists of application data, business rules, logic, and functions. A view can be any
output representation of data, such as a chart or a diagram. Multiple views of the same data 
are possible, such as a bar chart for management and a tabular view for accountants. 
The controller mediates input, converting it to commands for the model or view.The central 
ideas behind MVC are code reusable and in addition to dividing the application into three 
kinds of components, the MVC design defines the interactions between them.

<ul>
<li>
<b>A controller</b>can send commands to its associated view to change the view's presentation of the model (e.g., by scrolling through a document). 
It can also send commands to the model to update the model's state (e.g., editing a document).
</li>
</ul> 
</div>
</div> 
 
<script>
//To set the animationSpeed property of Scroller during initialization
        $("#scrollContent").ejScroller({animationSpeed: 1000 });      
</script> 
{% endhighlight %}






### autoHide `boolean`
{:#members:autohide}




Set true to hides the scrollbar, when mouseout the content area.


#### Default Value




* false




#### Example



{% highlight html %}
 
<div id="scrollContent" style="width:900px;" >
<div>
<p>Model view controller (MVC) is a software architecture pattern which separates the
representation of information from the user's interaction with it.
The model consists of application data, business rules, logic, and functions. A view can be any
output representation of data, such as a chart or a diagram. Multiple views of the same data 
are possible, such as a bar chart for management and a tabular view for accountants. 
The controller mediates input, converting it to commands for the model or view.The central 
ideas behind MVC are code reusable and in addition to dividing the application into three 
kinds of components, the MVC design defines the interactions between them.

<ul>
<li>
<b>A controller</b>can send commands to its associated view to change the view's presentation of the model (e.g., by scrolling through a document). 
It can also send commands to the model to update the model's state (e.g., editing a document).
</li>
</ul> 
</div>
</div> 
 
<script>
//To enable the autoHide property of Scroller during initialization
        $("#scrollContent").ejScroller({autoHide: true });      
</script> 
{% endhighlight %}





### buttonSize `number`
{:#members:buttonsize}




Specifies the height and width of button in the scrollbar.



#### Default Value




* 18




#### Example



{% highlight html %}
 
<div id="scrollContent" style="width:900px;" >
<div>
<p>Model view controller (MVC) is a software architecture pattern which separates the
representation of information from the user's interaction with it.
The model consists of application data, business rules, logic, and functions. A view can be any
output representation of data, such as a chart or a diagram. Multiple views of the same data 
are possible, such as a bar chart for management and a tabular view for accountants. 
The controller mediates input, converting it to commands for the model or view.The central 
ideas behind MVC are code reusable and in addition to dividing the application into three 
kinds of components, the MVC design defines the interactions between them.

<ul>
<li>
<b>A controller </b>can send commands to its associated view to change the view's presentation of the model (e.g., by scrolling through a document). 
It can also send commands to the model to update the model's state (e.g., editing a document).
</li>
</ul> 
</div>
</div> 
 
<script>
//To set Button Size of Scroller during initialization
        $("#scrollContent").ejScroller({buttonSize: 20 });      
</script>{% endhighlight %}




### enabled `boolean`
{:#members:enabled}




Specifies to enable or disable the scroller


#### Default Value




* true




#### Example



{% highlight html %}
 
<div id="scrollContent" style="width:900px;" >
<div>
<p>Model view controller (MVC) is a software architecture pattern which separates the
representation of information from the user's interaction with it.
The model consists of application data, business rules, logic, and functions. A view can be any
output representation of data, such as a chart or a diagram. Multiple views of the same data 
are possible, such as a bar chart for management and a tabular view for accountants. 
The controller mediates input, converting it to commands for the model or view.The central 
ideas behind MVC are code reusable and in addition to dividing the application into three 
kinds of components, the MVC design defines the interactions between them.

<ul>
<li>
<b>A controller </b>can send commands to its associated view to change the view's presentation of the model (e.g., by scrolling through a document). 
It can also send commands to the model to update the model's state (e.g., editing a document).
</li>
</ul> 
</div>
</div> 
 
<script>
//Enable or disable scroller API on initialization
        $("#scrollContent").ejScroller({enabled: true });       
</script> {% endhighlight %}




### enablePersistence `boolean`
{:#members:enablepersistence}




Save current model value to browser cookies for state maintenance. While refresh the page Rating control values are retained.


#### Default Value




* false




#### Example



{% highlight html %}
 
<div id="scrollContent" style="width:900px;" >
<div>
<p>Model view controller (MVC) is a software architecture pattern which separates the
representation of information from the user's interaction with it.
The model consists of application data, business rules, logic, and functions. A view can be any
output representation of data, such as a chart or a diagram. Multiple views of the same data 
are possible, such as a bar chart for management and a tabular view for accountants. 
The controller mediates input, converting it to commands for the model or view.The central 
ideas behind MVC are code reusable and in addition to dividing the application into three 
kinds of components, the MVC design defines the interactions between them.

<ul>
<li>
<b>A controller </b>can send commands to its associated view to change the view's presentation of the model (e.g., by scrolling through a document). 
It can also send commands to the model to update the model's state (e.g., editing a document).
</li>
</ul> 
</div>
</div> 
 
<script>
//Enable enablePersistence API on initialization
        $("#scrollContent").ejScroller({enablePersistence: true });
</script>
 {% endhighlight %}




### enableRTL `boolean`
{:#members:enablertl}




Indicates the Right to Left direction to scroller


#### Default Value




* undefined




#### Example



{% highlight html %}
 
<div id="scrollContent" style="width:900px;" >
<div>
<p>Model view controller (MVC) is a software architecture pattern which separates the
representation of information from the user's interaction with it.
The model consists of application data, business rules, logic, and functions. A view can be any
output representation of data, such as a chart or a diagram. Multiple views of the same data 
are possible, such as a bar chart for management and a tabular view for accountants. 
The controller mediates input, converting it to commands for the model or view.The central 
ideas behind MVC are code reusable and in addition to dividing the application into three 
kinds of components, the MVC design defines the interactions between them.

<ul>
<li>
<b>A controller </b>can send commands to its associated view to change the view's presentation of the model (e.g., by scrolling through a document). 
It can also send commands to the model to update the model's state (e.g., editing a document).
</li>
</ul> 
</div>
</div> 
 
<script>
//Enable enableRTL API on initialization
        $("#scrollContent").ejScroller({enableRTL: true });     
</script> {% endhighlight %}




### enableTouchScroll `boolean`
{:#members:enabletouchscroll}




Enables or Disable the touch Scroll


#### Default Value




* true




#### Example



{% highlight html %}
 
<div id="scrollContent" style="width:900px;" >
<div>
<p>Model view controller (MVC) is a software architecture pattern which separates the
representation of information from the user's interaction with it.
The model consists of application data, business rules, logic, and functions. A view can be any
output representation of data, such as a chart or a diagram. Multiple views of the same data 
are possible, such as a bar chart for management and a tabular view for accountants. 
The controller mediates input, converting it to commands for the model or view.The central 
ideas behind MVC are code reusable and in addition to dividing the application into three 
kinds of components, the MVC design defines the interactions between them.

<ul>
<li>
<b>A controller </b>can send commands to its associated view to change the view's presentation of the model (e.g., by scrolling through a document). 
It can also send commands to the model to update the model's state (e.g., editing a document).
</li>
</ul> 
</div>
</div> 
 
<script>
//Disable Touch Scroll API on initialization
        $("#scrollContent").ejScroller({enableTouchScroll: false });    
</script> {% endhighlight %}




### height `number|string`
{:#members:height}




Specifies the height of Scroll panel and scrollbars.


#### Default Value




* 250




#### Example



{% highlight html %}
 
<div id="scrollContent" style="width:900px;" >
<div>
<p>Model view controller (MVC) is a software architecture pattern which separates the
representation of information from the user's interaction with it.
The model consists of application data, business rules, logic, and functions. A view can be any
output representation of data, such as a chart or a diagram. Multiple views of the same data 
are possible, such as a bar chart for management and a tabular view for accountants. 
The controller mediates input, converting it to commands for the model or view.The central 
ideas behind MVC are code reusable and in addition to dividing the application into three 
kinds of components, the MVC design defines the interactions between them.

<ul>
<li>
<b>A controller </b>can send commands to its associated view to change the view's presentation of the model (e.g., by scrolling through a document). 
It can also send commands to the model to update the model's state (e.g., editing a document).
</li>
</ul> 
</div>
</div> 
 
<script>
//To set height API value during initialization  
        $("#scrollContent").ejScroller({height: 200 }); 
</script>{% endhighlight %}




### scrollerSize `number`
{:#members:scrollersize}



If the scrollbar has vertical it set as width, else it will set as height of the handler.


#### Default Value




* 18




#### Example



{% highlight html %}
 
<div id="scrollContent" style="width:900px;" >
<div>
<p>Model view controller (MVC) is a software architecture pattern which separates the
representation of information from the user's interaction with it.
The model consists of application data, business rules, logic, and functions. A view can be any
output representation of data, such as a chart or a diagram. Multiple views of the same data 
are possible, such as a bar chart for management and a tabular view for accountants. 
The controller mediates input, converting it to commands for the model or view.The central 
ideas behind MVC are code reusable and in addition to dividing the application into three 
kinds of components, the MVC design defines the interactions between them.

<ul>
<li>
<b>A controller </b>can send commands to its associated view to change the view's presentation of the model (e.g., by scrolling through a document). 
It can also send commands to the model to update the model's state (e.g., editing a document).
</li>
</ul> 
</div>
</div> 
 
<script>
//Enable scrollerSize on initialization 
        //To set scroller Size API value 
        $("#scrollContent").ejScroller({scrollerSize: 20 });    
</script>{% endhighlight %}




### scrollLeft `number`
{:#members:scrollleft}




The Scroller content and scrollbars move left with given value.


#### Default Value




* 0




#### Example



{% highlight html %}
 
<div id="scrollContent" style="width:900px;" >
<div>
<p>Model view controller (MVC) is a software architecture pattern which separates the
representation of information from the user's interaction with it.
The model consists of application data, business rules, logic, and functions. A view can be any
output representation of data, such as a chart or a diagram. Multiple views of the same data 
are possible, such as a bar chart for management and a tabular view for accountants. 
The controller mediates input, converting it to commands for the model or view.The central 
ideas behind MVC are code reusable and in addition to dividing the application into three 
kinds of components, the MVC design defines the interactions between them.

<ul>
<li>
<b>A controller </b>can send commands to its associated view to change the view's presentation of the model (e.g., by scrolling through a document). 
It can also send commands to the model to update the model's state (e.g., editing a document).
</li>
</ul> 
</div>
</div> 
 
<script>
//To set Scroll left API during initialization
        $("#scrollContent").ejScroller({scrollLeft: 40 });      
</script>{% endhighlight %}




### scrollOneStepBy `number`
{:#members:scrollonestepby}




While press on the arrow key the scrollbar position added to the given pixel value.


#### Default Value




* 57




#### Example



{% highlight html %}
 
<div id="scrollContent" style="width:900px;" >
<div>
<p>Model view controller (MVC) is a software architecture pattern which separates the
representation of information from the user's interaction with it.
The model consists of application data, business rules, logic, and functions. A view can be any
output representation of data, such as a chart or a diagram. Multiple views of the same data 
are possible, such as a bar chart for management and a tabular view for accountants. 
The controller mediates input, converting it to commands for the model or view.The central 
ideas behind MVC are code reusable and in addition to dividing the application into three 
kinds of components, the MVC design defines the interactions between them.

<ul>
<li>
<b>A controller </b>can send commands to its associated view to change the view's presentation of the model (e.g., by scrolling through a document). 
It can also send commands to the model to update the model's state (e.g., editing a document).
</li>
</ul> 
</div>
</div> 
 
<script>
//To set scrollOneStepBy API value during initialization
        $("#scrollContent").ejScroller({scrollOneStepBy: 40 }); 
</script>{% endhighlight %}




### scrollTop `number`
{:#members:scrolltop}




The Scroller content and scrollbars move to top position with specified value.


#### Default Value




* 0




#### Example



{% highlight html %}
 
<div id="scrollContent" style="width:900px;" >
<div>
<p>Model view controller (MVC) is a software architecture pattern which separates the
representation of information from the user's interaction with it.
The model consists of application data, business rules, logic, and functions. A view can be any
output representation of data, such as a chart or a diagram. Multiple views of the same data 
are possible, such as a bar chart for management and a tabular view for accountants. 
The controller mediates input, converting it to commands for the model or view.The central 
ideas behind MVC are code reusable and in addition to dividing the application into three 
kinds of components, the MVC design defines the interactions between them.

<ul>
<li>
<b>A controller </b>can send commands to its associated view to change the view's presentation of the model (e.g., by scrolling through a document). 
It can also send commands to the model to update the model's state (e.g., editing a document).
</li>
</ul> 
</div>
</div> 
 
<script>
//To set Scroll top API during initialization
        $("#scrollContent").ejScroller({scrollTop: 40 });       
</script>{% endhighlight %}




### targetPane `string`
{:#members:targetpane}




Indicates the target area to which scroller have to appear.


#### Default Value




* null




#### Example



{% highlight html %}
 
<div id="scrollContent" style="width:900px;" >
<div>
<p>Model view controller (MVC) is a software architecture pattern which separates the
representation of information from the user's interaction with it.
The model consists of application data, business rules, logic, and functions. A view can be any
output representation of data, such as a chart or a diagram. Multiple views of the same data 
are possible, such as a bar chart for management and a tabular view for accountants. 
The controller mediates input, converting it to commands for the model or view.The central 
ideas behind MVC are code reusable and in addition to dividing the application into three 
kinds of components, the MVC design defines the interactions between them.

<ul>
<li>
<b>A controller </b>can send commands to its associated view to change the view's presentation of the model (e.g., by scrolling through a document). 
It can also send commands to the model to update the model's state (e.g., editing a document).
</li>
</ul> 
</div>
</div> 
 
<script>
//To set Scroller for the specified target panel during initialization
        $("#scrollContent").ejScroller({targetPane: "contentArea" });   
</script>{% endhighlight %}




### width `number|string`
{:#members:width}




Specifies the width of Scroll panel and scrollbars.


#### Default Value




* 0




#### Example



{% highlight html %}
 
<div id="scrollContent" style="width:900px;" >
<div>
<p>Model view controller (MVC) is a software architecture pattern which separates the
representation of information from the user's interaction with it.
The model consists of application data, business rules, logic, and functions. A view can be any
output representation of data, such as a chart or a diagram. Multiple views of the same data 
are possible, such as a bar chart for management and a tabular view for accountants. 
The controller mediates input, converting it to commands for the model or view.The central 
ideas behind MVC are code reusable and in addition to dividing the application into three 
kinds of components, the MVC design defines the interactions between them.

<ul>
<li>
<b>A controller </b>can send commands to its associated view to change the view's presentation of the model (e.g., by scrolling through a document). 
It can also send commands to the model to update the model's state (e.g., editing a document).
</li>
</ul> 
</div>
</div> 
 
<script>
//To set width API value during initialization
        $("#scrollContent").ejScroller({width: 500 });  
</script>{% endhighlight %}



## Methods




### destroy()
{:#methods:destroy}




destroy the Scroller control, unbind the all ej control related events automatically and bring the control to pre-init state.



#### Example



{% highlight html %}
 
<div id="scrollContent" style="width:900px;" >
<div>
<p>Model view controller (MVC) is a software architecture pattern which separates the
representation of information from the user's interaction with it.
The model consists of application data, business rules, logic, and functions. A view can be any
output representation of data, such as a chart or a diagram. Multiple views of the same data 
are possible, such as a bar chart for management and a tabular view for accountants. 
The controller mediates input, converting it to commands for the model or view.The central 
ideas behind MVC are code reusable and in addition to dividing the application into three 
kinds of components, the MVC design defines the interactions between them.

<ul><li>
<b>A controller</b>can send commands to its associated view to change the view's presentation of the model (e.g., by scrolling through a document). 
It can also send commands to the model to update the model's state (e.g., editing a document).
</li>
</ul> 
</div>
</div> 
 
<script>
$('#scrollContent').ejScroller();       
// Destroy Scroller
var scrollerObj  = $("#scrollContent").data("ejScroller");
scrollerObj.destroy(); // destroy the scroller
</script>{% endhighlight %}


{% highlight html %}
 
<div id="scrollContent" style="width:900px;" >
<div>
<p>Model view controller (MVC) is a software architecture pattern which separates the
representation of information from the user's interaction with it.
The model consists of application data, business rules, logic, and functions. A view can be any
output representation of data, such as a chart or a diagram. Multiple views of the same data 
are possible, such as a bar chart for management and a tabular view for accountants. 
The controller mediates input, converting it to commands for the model or view.The central 
ideas behind MVC are code reusable and in addition to dividing the application into three 
kinds of components, the MVC design defines the interactions between them.

<ul><li>
<b>A controller </b>can send commands to its associated view to change the view's presentation of the model (e.g., by scrolling through a document). 
It can also send commands to the model to update the model's state (e.g., editing a document).
</li>
</ul> 
</div>
</div> 
 
<script>
$('#scrollContent').ejScroller();       
// destroy the scroller
$("#scrollContent").ejScroller("destroy");      
</script>{% endhighlight %}




### disable()
{:#methods:disable}




User disables the Scroller control at any time.



#### Example



{% highlight html %}
 
<div id="scrollContent" style="width:900px;" >
<div>
<p>Model view controller (MVC) is a software architecture pattern which separates the
representation of information from the user's interaction with it.
The model consists of application data, business rules, logic, and functions. A view can be any
output representation of data, such as a chart or a diagram. Multiple views of the same data 
are possible, such as a bar chart for management and a tabular view for accountants. 
The controller mediates input, converting it to commands for the model or view.The central 
ideas behind MVC are code reusable and in addition to dividing the application into three 
kinds of components, the MVC design defines the interactions between them.

<ul>
<li>
<b>A controller </b>can send commands to its associated view to change the view's presentation of the model (e.g., by scrolling through a document). 
It can also send commands to the model to update the model's state (e.g., editing a document).
</li>
</ul> 
</div>
</div> 
 
<script>
$('#scrollContent').ejScroller();       
// To disable the Scroller control at any time.
var scrollerObj  = $("#scrollContent").data("ejScroller");
scrollerObj.disable(); // disable the Scroller control at any time
</script>{% endhighlight %}


{% highlight html %}
 
<div id="scrollContent" style="width:900px;" >
<div>
<p>Model view controller (MVC) is a software architecture pattern which separates the
representation of information from the user's interaction with it.
The model consists of application data, business rules, logic, and functions. A view can be any
output representation of data, such as a chart or a diagram. Multiple views of the same data 
are possible, such as a bar chart for management and a tabular view for accountants. 
The controller mediates input, converting it to commands for the model or view.The central 
ideas behind MVC are code reusable and in addition to dividing the application into three 
kinds of components, the MVC design defines the interactions between them.

<ul>
<li>
<b>A controller </b>can send commands to its associated view to change the view's presentation of the model (e.g., by scrolling through a document). 
It can also send commands to the model to update the model's state (e.g., editing a document).
</li>
</ul> 
</div>
</div> 
 
<script>
$('#scrollContent').ejScroller();       
// disable the scroller control
$("#scrollContent").ejScroller("disable");      
</script>{% endhighlight %}




### enable()
{:#methods:enable}




User enables the Scroller control at any time.



#### Example



{% highlight html %}
 
<div id="scrollContent" style="width:900px;" >
<div>
<p>Model view controller (MVC) is a software architecture pattern which separates the
representation of information from the user's interaction with it.
The model consists of application data, business rules, logic, and functions. A view can be any
output representation of data, such as a chart or a diagram. Multiple views of the same data 
are possible, such as a bar chart for management and a tabular view for accountants. 
The controller mediates input, converting it to commands for the model or view.The central 
ideas behind MVC are code reusable and in addition to dividing the application into three 
kinds of components, the MVC design defines the interactions between them.

<ul>
<li>
<b>A controller </b>can send commands to its associated view to change the view's presentation of the model (e.g., by scrolling through a document). 
It can also send commands to the model to update the model's state (e.g., editing a document).
</li>
</ul> 
</div>
</div> 
 
<script>
$('#scrollContent').ejScroller();       
// To enable the Scroller control at any time.
var scrollerObj  = $("#scrollContent").data("ejScroller");
scrollerObj.enable(); // enable the Scroller control at any time
</script>{% endhighlight %}


{% highlight html %}
 
<div id="scrollContent" style="width:900px;" >
<div>
<p>Model view controller (MVC) is a software architecture pattern which separates the
representation of information from the user's interaction with it.
The model consists of application data, business rules, logic, and functions. A view can be any
output representation of data, such as a chart or a diagram. Multiple views of the same data 
are possible, such as a bar chart for management and a tabular view for accountants. 
The controller mediates input, converting it to commands for the model or view.The central 
ideas behind MVC are code reusable and in addition to dividing the application into three 
kinds of components, the MVC design defines the interactions between them.

<ul>
<li>
<b>A controller </b>can send commands to its associated view to change the view's presentation of the model (e.g., by scrolling through a document). 
It can also send commands to the model to update the model's state (e.g., editing a document).
</li>
</ul> 
</div>
</div> 
 
<script>
$('#scrollContent').ejScroller();       
// enables the scroller control
$("#scrollContent").ejScroller("enable");       
</script>{% endhighlight %}




### isHScroll()
{:#methods:ishscroll}




Returns true if horizontal scrollbar is shown, else return false.



#### Returns:
{:#methods:returns:}

boolean

#### Example



{% highlight html %}
 
<div id="scrollContent" style="width:900px;" >
<div>
<p>Model view controller (MVC) is a software architecture pattern which separates the
representation of information from the user's interaction with it.
The model consists of application data, business rules, logic, and functions. A view can be any
output representation of data, such as a chart or a diagram. Multiple views of the same data 
are possible, such as a bar chart for management and a tabular view for accountants. 
The controller mediates input, converting it to commands for the model or view.The central 
ideas behind MVC are code reusable and in addition to dividing the application into three 
kinds of components, the MVC design defines the interactions between them.

<ul>
<li>
<b>A controller </b>can send commands to its associated view to change the view's presentation of the model (e.g., by scrolling through a document). 
It can also send commands to the model to update the model's state (e.g., editing a document).
</li>
</ul> 
</div>
</div> 
 
<script>
// To check horizontal scrollbar is rendered or not
var scrollerObj  = $("#scrollContent").data("ejScroller");
scrollerObj.isHScroll(); // Returns horizontal scrollbar is shown or not.
</script>{% endhighlight %}


{% highlight html %}
 
<div id="scrollContent" style="width:900px;" >
<div>
<p>Model view controller (MVC) is a software architecture pattern which separates the
representation of information from the user's interaction with it.
The model consists of application data, business rules, logic, and functions. A view can be any
output representation of data, such as a chart or a diagram. Multiple views of the same data 
are possible, such as a bar chart for management and a tabular view for accountants. 
The controller mediates input, converting it to commands for the model or view.The central 
ideas behind MVC are code reusable and in addition to dividing the application into three 
kinds of components, the MVC design defines the interactions between them.

<ul>
<li>
<b>A controller </b>can send commands to its associated view to change the view's presentation of the model (e.g., by scrolling through a document). 
It can also send commands to the model to update the model's state (e.g., editing a document).
</li>
</ul> 
</div>
</div> 
 
<script>
// To check horizontal scrollbar is rendered or not
$("#scrollContent").ejScroller("isHScroll");    
</script>{% endhighlight %}




### isVScroll()
{:#methods:isvscroll}




Returns true if vertical scrollbar is shown, else return false.



#### Returns:
{:#methods:returns:}

boolean

#### Example



{% highlight html %}
 
<div id="scrollContent" style="width:900px;" >
<div>
<p>Model view controller (MVC) is a software architecture pattern which separates the
representation of information from the user's interaction with it.
The model consists of application data, business rules, logic, and functions. A view can be any
output representation of data, such as a chart or a diagram. Multiple views of the same data 
are possible, such as a bar chart for management and a tabular view for accountants. 
The controller mediates input, converting it to commands for the model or view.The central 
ideas behind MVC are code reusable and in addition to dividing the application into three 
kinds of components, the MVC design defines the interactions between them.

<ul>
<li>
<b>A controller </b>can send commands to its associated view to change the view's presentation of the model (e.g., by scrolling through a document). 
It can also send commands to the model to update the model's state (e.g., editing a document).
</li>
</ul> 
</div>
</div> 
 
<script>
$('#scrollContent').ejScroller();       
// To check vertical scrollbar is rendered or not
var scrollerObj  = $("#scrollContent").data("ejScroller");
scrollerObj.isVScroll(); // Returns vertical scrollbar is shown or not.
</script>{% endhighlight %}


{% highlight html %}
 
<div id="scrollContent" style="width:900px;">
<div>
<p>Model view controller (MVC) is a software architecture pattern which separates the
representation of information from the user's interaction with it.
The model consists of application data, business rules, logic, and functions. A view can be any
output representation of data, such as a chart or a diagram. Multiple views of the same data 
are possible, such as a bar chart for management and a tabular view for accountants. 
The controller mediates input, converting it to commands for the model or view.The central 
ideas behind MVC are code reusable and in addition to dividing the application into three 
kinds of components, the MVC design defines the interactions between them.

<ul>
<li>
<b>A controller </b>can send commands to its associated view to change the view's presentation of the model (e.g., by scrolling through a document). 
It can also send commands to the model to update the model's state (e.g., editing a document).
</li>
</ul> 
</div>
</div> 
 
<script>
$('#scrollContent').ejScroller();       
// To check vertical scrollbar is rendered or not
$("#scrollContent").ejScrollBar("isVScroll");   
</script>{% endhighlight %}




### refresh()
{:#methods:refresh}




User refreshes the Scroller control at any time.



#### Example



{% highlight html %}
 
<div id="scrollContent" style="width:900px;" >
<div>
<p>Model view controller (MVC) is a software architecture pattern which separates the
representation of information from the user's interaction with it.
The model consists of application data, business rules, logic, and functions. A view can be any
output representation of data, such as a chart or a diagram. Multiple views of the same data 
are possible, such as a bar chart for management and a tabular view for accountants. 
The controller mediates input, converting it to commands for the model or view.The central 
ideas behind MVC are code reusable and in addition to dividing the application into three 
kinds of components, the MVC design defines the interactions between them.

<ul>
<li>
<b>A controller </b>can send commands to its associated view to change the view's presentation of the model (e.g., by scrolling through a document). 
It can also send commands to the model to update the model's state (e.g., editing a document).
</li>
</ul> 
</div>
</div> 
 
<script>
$('#scrollContent').ejScroller();       
// To refresh the Scroller control at any time.
var scrollerObj  = $("#scrollContent").data("ejScroller");
scrollerObj.refresh(); // refreshes the Scroller control at any time
</script>{% endhighlight %}


{% highlight html %}
 
<div id="scrollContent" style="width:900px;" >
<div>
<p>Model view controller (MVC) is a software architecture pattern which separates the
representation of information from the user's interaction with it.
The model consists of application data, business rules, logic, and functions. A view can be any
output representation of data, such as a chart or a diagram. Multiple views of the same data 
are possible, such as a bar chart for management and a tabular view for accountants. 
The controller mediates input, converting it to commands for the model or view.The central 
ideas behind MVC are code reusable and in addition to dividing the application into three 
kinds of components, the MVC design defines the interactions between them.

<ul>
<li>
<b>A controller </b>can send commands to its associated view to change the view's presentation of the model (e.g., by scrolling through a document). 
It can also send commands to the model to update the model's state (e.g., editing a document).
</li>
</ul> 
</div>
</div> 
 
<script>
$('#scrollContent').ejScroller();       
// Refresh the scroller control
$("#scrollContent").ejScroller("refresh");      
</script>{% endhighlight %}




### scrollX(pixel, disableAnimation, animationSpeed)
{:#methods:scrollx}


Horizontal scroller moves to given pixel from its origin position. We can also specify the animation speed,in which the scroller has to move while re-positioning it.

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
pixel </td>
<td class="type"><span class="param-type">number|string</span></td>
<td class="description">Horizontal scroller moves to the specified pixel.</td>
</tr>
<tr>
<td class="name"> 
disableAnimation </td>
<td class="type"><span class="param-type">boolean</span></td>
<td class="description">Specifies to enable/disable the animation.</td>
</tr>
<tr>
<td class="name"> 
animationSpeed </td>
<td class="type"><span class="param-type">number</span></td>
<td class="description">Specifies the animation speed when scrolling, if animation is enabled.</td>
</tr>
</tbody>
</table>


#### Example



{% highlight html %}
 
<div id="scrollContent" style="width:900px;" >
<div>
<p>Model view controller (MVC) is a software architecture pattern which separates the
representation of information from the user's interaction with it.
The model consists of application data, business rules, logic, and functions. A view can be any
output representation of data, such as a chart or a diagram. Multiple views of the same data 
are possible, such as a bar chart for management and a tabular view for accountants. 
The controller mediates input, converting it to commands for the model or view.The central 
ideas behind MVC are code reusable and in addition to dividing the application into three 
kinds of components, the MVC design defines the interactions between them.

<ul>
<li>
<b>A controller </b>can send commands to its associated view to change the view's presentation of the model (e.g., by scrolling through a document). 
It can also send commands to the model to update the model's state (e.g., editing a document).
</li>
</ul> 
</div>
</div> 
 
<script>
$('#scrollContent').ejScroller();       
// Moves scroller to given pixel in X (left) position.
var scrollerObj  = $("#scrollContent").data("ejScroller");
scrollerObj.scrollX(25); // call scrollX method(with animation disabled)
scrollObj.scrollX(25,false,1000); // call scrollX method(with animation enabled. the third parameter "1000" indicates the animation speed while re-positioning the scroller)
</script>{% endhighlight %}


{% highlight html %}
 
<div id="scrollContent" style="width:900px;" >
<div>
<p>Model view controller (MVC) is a software architecture pattern which separates the
representation of information from the user's interaction with it.
The model consists of application data, business rules, logic, and functions. A view can be any
output representation of data, such as a chart or a diagram. Multiple views of the same data 
are possible, such as a bar chart for management and a tabular view for accountants. 
The controller mediates input, converting it to commands for the model or view.The central 
ideas behind MVC are code reusable and in addition to dividing the application into three 
kinds of components, the MVC design defines the interactions between them.

<ul>
<li>
<b>A controller </b>can send commands to its associated view to change the view's presentation of the model (e.g., by scrolling through a document). 
It can also send commands to the model to update the model's state (e.g., editing a document).
</li>
</ul> 
</div>
</div> 
 
<script>
$('#scrollContent').ejScroller();       
//Moves scroller to given pixel in X (left) position.
$("#scrollContent").ejScroller("scrollX", 25, true);    // call scrollX method(with animation disabled. "true" indicates animation is off)
$("#scrollContent").ejScroller("scrollX", 25,false,1000);       // call scrollX method(with animation enabled. Here, the fourth parameter "1000" indicates the animation speed while re-positioning the scroller)
</script>{% endhighlight %}




### scrollY(pixel, disableAnimation, animationSpeed)
{:#methods:scrolly}

Vertical scroller moves to given pixel from its origin position. We can also specify the animation speed,in which the scroller has to move while re-positioning it.

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
pixel </td>
<td class="type"><span class="param-type">number|string</span></td>
<td class="description">Vertical scroller moves to the specified pixel.</td>
</tr>
<tr>
<td class="name"> 
disableAnimation </td>
<td class="type"><span class="param-type">boolean</span></td>
<td class="description">Specifies to enable/disable the animation.</td>
</tr>
<tr>
<td class="name"> 
animationSpeed </td>
<td class="type"><span class="param-type">number</span></td>
<td class="description">Specifies the animation speed when scrolling, if animation is enabled.</td>
</tr>
</tbody>
</table>

#### Example



{% highlight html %}
 
<div id="scrollContent" style="width:900px;" >
<div>
<p>Model view controller (MVC) is a software architecture pattern which separates the
representation of information from the user's interaction with it.
The model consists of application data, business rules, logic, and functions. A view can be any
output representation of data, such as a chart or a diagram. Multiple views of the same data 
are possible, such as a bar chart for management and a tabular view for accountants. 
The controller mediates input, converting it to commands for the model or view.The central 
ideas behind MVC are code reusable and in addition to dividing the application into three 
kinds of components, the MVC design defines the interactions between them.

<ul>
<li>
<b>A controller </b>can send commands to its associated view to change the view's presentation of the model (e.g., by scrolling through a document). 
It can also send commands to the model to update the model's state (e.g., editing a document).
</li>
</ul> 
</div>
</div> 
 
<script>
$('#scrollContent').ejScroller();       
// Moves scroller to given pixel in Y (top) position.
var scrollerObj  = $("#scrollContent").data("ejScroller");
scrollerObj.scrollY(25); // call scrollY method(with animation disabled)
scrollObj.scrollY(25,false,1000); // call scrollY method(with animation enabled. the third parameter "1000" indicates the animation speed while re-positioning the scroller)
</script>{% endhighlight %}


{% highlight html %}
 
<div id="scrollContent" style="width:900px;" >
<div>
<p>Model view controller (MVC) is a software architecture pattern which separates the
representation of information from the user's interaction with it.
The model consists of application data, business rules, logic, and functions. A view can be any
output representation of data, such as a chart or a diagram. Multiple views of the same data 
are possible, such as a bar chart for management and a tabular view for accountants. 
The controller mediates input, converting it to commands for the model or view.The central 
ideas behind MVC are code reusable and in addition to dividing the application into three 
kinds of components, the MVC design defines the interactions between them.

<ul>
<li>
<b>A controller</b>can send commands to its associated view to change the view's presentation of the model (e.g., by scrolling through a document). 
It can also send commands to the model to update the model's state (e.g., editing a document).
</li>
</ul> 
</div>
</div> 
 
<script>
$('#scrollContent').ejScroller();       
//Moves scroller to given pixel in Y (top) position.
$("#scrollContent").ejScroller("scrollY", 25, true);    // call scrollY method(with animation disabled. "true" indicates animation is off)
$("#scrollContent").ejScroller("scrollY", 25,false,1000);       // call scrollY method(with animation enabled. Here, fourth parameter "1000" indicates the animation speed while re-positioning the scroller)
</script>{% endhighlight %}



## Events




### create
{:#events:create}




Fires when Scroller control is created.

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
<td class="type"><ts ref="ej.Scroller.Model"/><span class="param-type">object</span></td>
<td class="description">returns the scroller model</td>
</tr>
<tr>
<td class="name">
type</td>
<td class="type"><span class="param-type">string</span></td>
<td class="description">returns the name of the event.</td>
</tr>
</tbody>
</table>



#### Example



{% highlight html %}
 
<div id="scrollContent" style="width:900px;" >
<div>
<p>Model view controller (MVC) is a software architecture pattern which separates the
representation of information from the user's interaction with it.
The model consists of application data, business rules, logic, and functions. A view can be any
output representation of data, such as a chart or a diagram. Multiple views of the same data 
are possible, such as a bar chart for management and a tabular view for accountants. 
The controller mediates input, converting it to commands for the model or view.The central 
ideas behind MVC are code reusable and in addition to dividing the application into three 
kinds of components, the MVC design defines the interactions between them.

<ul>
<li>
<b>A controller</b>can send commands to its associated view to change the view's presentation of the model (e.g., by scrolling through a document). 
It can also send commands to the model to update the model's state (e.g., editing a document).
</li>
</ul> 
</div>
</div> 
 
<script>
//create event for scroller
$("#scrollContent").ejScroller({
   create: function (args) {}
});   
</script>   {% endhighlight %}




### destroy
{:#events:destroy}




Fires when Scroller control is destroyed.

<table class="params">
<thead>
<tr>
<th>Name</th>
<th>Type</th>
<th>Description</th>
</tr>
</thead>
<tr>
<td class="name">
cancel</td>
<td class="type"><span class="param-type">boolean</span></td>
<td class="description">if the event should be canceled; otherwise, false.</td>
</tr>
<tr>
<td class="name">
model</td>
<td class="type"><ts ref="ej.Scroller.Model"/><span class="param-type">object</span></td>
<td class="description">returns the scroller model</td>
</tr>
<tr>
<td class="name">
type</td>
<td class="type"><span class="param-type">string</span></td>
<td class="description">returns the name of the event.</td>
</tr>
</tbody>
</table>



#### Example



{% highlight html %}
 
<div id="scrollContent" style="width:900px;" >
<div>
<p>Model view controller (MVC) is a software architecture pattern which separates the
representation of information from the user's interaction with it.
The model consists of application data, business rules, logic, and functions. A view can be any
output representation of data, such as a chart or a diagram. Multiple views of the same data 
are possible, such as a bar chart for management and a tabular view for accountants. 
The controller mediates input, converting it to commands for the model or view.The central 
ideas behind MVC are code reusable and in addition to dividing the application into three 
kinds of components, the MVC design defines the interactions between them.

<ul>
<li>
<b>A controller</b>can send commands to its associated view to change the view's presentation of the model (e.g., by scrolling through a document). 
It can also send commands to the model to update the model's state (e.g., editing a document).
</li>
</ul> 
</div>
</div> 
 
<script>
//destroy event for scroller
$("#scrollContent").ejScroller({
   destroy: function (args) {}
});  
</script>     {% endhighlight %}



### thumbMove
{:#events:thumbmove}


Fires when a thumb point is moved along the touch surface.

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
<td class="type"><ts ref="ej.Scroller.Model"/><span class="param-type">object</span></td>
<td class="description">returns the scroller model</td>
</tr>
<tr>
<td class="name">
originalEvent</td>
<td class="type"><span class="param-type">object</span></td>
<td class="description">returns the original event name and its event properties of the current event.</td>
</tr>
<tr>
<td class="name">
scrollData</td>
<td class="type"><span class="param-type">object</span></td>
<td class="description">returns the current data related to the event.</td>
</tr>
<tr>
<td class="name">
type</td>
<td class="type"><span class="param-type">string</span></td>
<td class="description">returns the name of the event.</td>
</tr>
</tbody>
</table>



#### Example



{% highlight html %}
 
<div id="scrollContent" style="width:900px;" >
<div>
<p>Model view controller (MVC) is a software architecture pattern which separates the
representation of information from the user's interaction with it.
The model consists of application data, business rules, logic, and functions. A view can be any
output representation of data, such as a chart or a diagram. Multiple views of the same data 
are possible, such as a bar chart for management and a tabular view for accountants. 
The controller mediates input, converting it to commands for the model or view.The central 
ideas behind MVC are code reusable and in addition to dividing the application into three 
kinds of components, the MVC design defines the interactions between them.

<ul>
<li>
<b>A controller</b>can send commands to its associated view to change the view's presentation of the model (e.g., by scrolling through a document). 
It can also send commands to the model to update the model's state (e.g., editing a document).
</li>
</ul> 
</div>
</div> 
 
<script>
//thumbMove event for scroller
$("#scrollContent").ejScroller({
   thumbMove: function (args) {}
});  
</script>     
{% endhighlight %}


### thumbStart
{:#events:thumbstart}


Fires when a thumb point is placed on the touch surface.

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
<td class="type"><ts ref="ej.Scroller.Model"/><span class="param-type">object</span></td>
<td class="description">returns the scroller model</td>
</tr>
<tr>
<td class="name">
originalEvent</td>
<td class="type"><span class="param-type">object</span></td>
<td class="description">returns the original event name and its event properties of the current event.</td>
</tr>
<tr>
<td class="name">
scrollData</td>
<td class="type"><span class="param-type">object</span></td>
<td class="description">returns the current data related to the event.</td>
</tr>
<tr>
<td class="name">
type</td>
<td class="type"><span class="param-type">string</span></td>
<td class="description">returns the name of the event.</td>
</tr>
</tbody>
</table>



#### Example



{% highlight html %}
 
<div id="scrollContent" style="width:900px;" >
<div>
<p>Model view controller (MVC) is a software architecture pattern which separates the
representation of information from the user's interaction with it.
The model consists of application data, business rules, logic, and functions. A view can be any
output representation of data, such as a chart or a diagram. Multiple views of the same data 
are possible, such as a bar chart for management and a tabular view for accountants. 
The controller mediates input, converting it to commands for the model or view.The central 
ideas behind MVC are code reusable and in addition to dividing the application into three 
kinds of components, the MVC design defines the interactions between them.

<ul>
<li>
<b>A controller</b>can send commands to its associated view to change the view's presentation of the model (e.g., by scrolling through a document). 
It can also send commands to the model to update the model's state (e.g., editing a document).
</li>
</ul> 
</div>
</div> 
 
<script>
//thumbStart event for scroller
$("#scrollContent").ejScroller({
   thumbStart: function (args) {}
});  
</script>     
{% endhighlight %}



### thumbEnd
{:#events:thumbend}


Fires when a thumb point is removed from the touch surface.

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
<td class="type"><ts ref="ej.Scroller.Model"/><span class="param-type">object</span></td>
<td class="description">returns the scroller model</td>
</tr>
<tr>
<td class="name">
originalEvent</td>
<td class="type"><span class="param-type">object</span></td>
<td class="description">returns the original event name and its event properties of the current event.</td>
</tr>
<tr>
<td class="name">
scrollData</td>
<td class="type"><span class="param-type">object</span></td>
<td class="description">returns the current data related to the event.</td>
</tr>
<tr>
<td class="name">
type</td>
<td class="type"><span class="param-type">string</span></td>
<td class="description">returns the name of the event.</td>
</tr>
</tbody>
</table>



#### Example



{% highlight html %}
 
<div id="scrollContent" style="width:900px;" >
<div>
<p>Model view controller (MVC) is a software architecture pattern which separates the
representation of information from the user's interaction with it.
The model consists of application data, business rules, logic, and functions. A view can be any
output representation of data, such as a chart or a diagram. Multiple views of the same data 
are possible, such as a bar chart for management and a tabular view for accountants. 
The controller mediates input, converting it to commands for the model or view.The central 
ideas behind MVC are code reusable and in addition to dividing the application into three 
kinds of components, the MVC design defines the interactions between them.

<ul>
<li>
<b>A controller</b>can send commands to its associated view to change the view's presentation of the model (e.g., by scrolling through a document). 
It can also send commands to the model to update the model's state (e.g., editing a document).
</li>
</ul> 
</div>
</div> 
 
<script>
//thumbEnd event for scroller
$("#scrollContent").ejScroller({
   thumbEnd: function (args) {}
});  
</script>     
{% endhighlight %}





### wheelMove
{:#events:wheelmove}




It fires whenever the mouse wheel is rotated either in upwards or downwards.

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
<td class="type"><ts ref="ej.Scroller.Model"/><span class="param-type">object</span></td>
<td class="description">returns the scroller model</td>
</tr>
<tr>
<td class="name">
originalEvent</td>
<td class="type"><span class="param-type">object</span></td>
<td class="description">returns the original event name and its event properties of the current event.</td>
</tr>
<td class="name">
direction</td>
<td class="type"><span class="param-type">number</span></td>
<td class="description">returns the trackball scrolling direction. If it returns 1, the wheel moved top to bottom direction. or if it returns -1, the wheel moved bottom to top direction.</td>
</tr>
<tr>
<tr>
<td class="name">
scrollData</td>
<td class="type"><span class="param-type">object</span></td>
<td class="description">returns the current data related to the event.</td>
</tr>
<tr>
<td class="name">
type</td>
<td class="type"><span class="param-type">string</span></td>
<td class="description">returns the name of the event.</td>
</tr>
</tbody>
</table>



#### Example



{% highlight html %}
 
<div id="scrollContent" style="width:900px;" >
<div>
<p>Model view controller (MVC) is a software architecture pattern which separates the
representation of information from the user's interaction with it.
The model consists of application data, business rules, logic, and functions. A view can be any
output representation of data, such as a chart or a diagram. Multiple views of the same data 
are possible, such as a bar chart for management and a tabular view for accountants. 
The controller mediates input, converting it to commands for the model or view.The central 
ideas behind MVC are code reusable and in addition to dividing the application into three 
kinds of components, the MVC design defines the interactions between them.

<ul>
<li>
<b>A controller</b>can send commands to its associated view to change the view's presentation of the model (e.g., by scrolling through a document). 
It can also send commands to the model to update the model's state (e.g., editing a document).
</li>
</ul> 
</div>
</div> 
 
<script>
//wheelMove event for scroller
$("#scrollContent").ejScroller({
   wheelMove: function (args) {}
});  
</script>    
 {% endhighlight %}



### wheelStart
{:#events:wheelstart}




It will fire when mouse trackball has been start to wheel.

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
<td class="type"><ts ref="ej.Scroller.Model"/><span class="param-type">object</span></td>
<td class="description">returns the scroller model</td>
</tr>
<tr>
<td class="name">
originalEvent</td>
<td class="type"><span class="param-type">object</span></td>
<td class="description">returns the original event name and its event properties of the current event.</td>
</tr>
<tr>
<td class="name">
scrollData</td>
<td class="type"><span class="param-type">object</span></td>
<td class="description">returns the current data related to the event.</td>
</tr>
<tr>
<td class="name">
type</td>
<td class="type"><span class="param-type">string</span></td>
<td class="description">returns the name of the event.</td>
</tr>
</tbody>
</table>



#### Example



{% highlight html %}
 
<div id="scrollContent" style="width:900px;" >
<div>
<p>Model view controller (MVC) is a software architecture pattern which separates the
representation of information from the user's interaction with it.
The model consists of application data, business rules, logic, and functions. A view can be any
output representation of data, such as a chart or a diagram. Multiple views of the same data 
are possible, such as a bar chart for management and a tabular view for accountants. 
The controller mediates input, converting it to commands for the model or view.The central 
ideas behind MVC are code reusable and in addition to dividing the application into three 
kinds of components, the MVC design defines the interactions between them.

<ul>
<li>
<b>A controller</b>can send commands to its associated view to change the view's presentation of the model (e.g., by scrolling through a document). 
It can also send commands to the model to update the model's state (e.g., editing a document).
</li>
</ul> 
</div>
</div> 
 
<script>
//wheelStart event for scroller
$("#scrollContent").ejScroller({
   wheelStart: function (args) {}
});  
</script>     
{% endhighlight %}





### wheelStop
{:#events:wheelstop}




It will fire when mouse trackball has been stop to wheel.

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
<td class="type"><ts ref="ej.Scroller.Model"/><span class="param-type">object</span></td>
<td class="description">returns the scroller model</td>
</tr>
<tr>
<td class="name">
type</td>
<td class="type"><span class="param-type">string</span></td>
<td class="description">returns the name of the event.</td>
</tr>
<tr>
<td class="name">
originalEvent</td>
<td class="type"><span class="param-type">object</span></td>
<td class="description">returns the original event name and its event properties of the current event.</td>
</tr>
<td class="name">
direction</td>
<td class="type"><span class="param-type">number</span></td>
<td class="description">returns the trackball scrolling direction. If it returns 1, the wheel moved top to bottom direction. or if it returns -1, the wheel moved bottom to top direction.</td>
</tr>
<tr>
<tr>
<td class="name">
scrollData</td>
<td class="type"><span class="param-type">object</span></td>
<td class="description">returns the current data related to the event.</td>
</tr>
<tr>
</tbody>
</table>


#### Example



{% highlight html %}
 
<div id="scrollContent" style="width:900px;" >
<div>
<p>Model view controller (MVC) is a software architecture pattern which separates the
representation of information from the user's interaction with it.
The model consists of application data, business rules, logic, and functions. A view can be any
output representation of data, such as a chart or a diagram. Multiple views of the same data 
are possible, such as a bar chart for management and a tabular view for accountants. 
The controller mediates input, converting it to commands for the model or view.The central 
ideas behind MVC are code reusable and in addition to dividing the application into three 
kinds of components, the MVC design defines the interactions between them.

<ul>
<li>
<b>A controller</b>can send commands to its associated view to change the view's presentation of the model (e.g., by scrolling through a document). 
It can also send commands to the model to update the model's state (e.g., editing a document).
</li>
</ul> 
</div>
</div> 
 
<script>
//wheelStop event for scroller
$("#scrollContent").ejScroller({
   wheelStop: function (args) {}
});  
</script>     
{% endhighlight %}