---
layout: post
title: Properties, Methods and Events of ejNavigationDrawer Widget
description: API reference for ejNavigationDrawer
documentation: API
platform: js-api
keywords: NavigationDrawer, ejNavigationDrawer, syncfusion, NavigationDrawer api 
---

# ejNavigationDrawer




The Navigation Drawer is a sliding panel that displays the list of navigation options on demand. That is, by default, it is not visible but you can display it onto the left/right side of the screen by swiping or by clicking with desired target icon.




#### Syntax

{% highlight javascript %}

$(element).ejNavigationDrawer()

{% endhighlight %}













#### Example



{% highlight html %}
 
//create Navigation Drawer in Obtrusive way
<div id="home" class="navsubpage">
<div align="center" class="content">
<h2 class="title">
Home</h2>
<p>
Founded by industry experts in 2001,Syncfusion, Inc. provides the broadest range of enterprise-class software components and tools for the Microsoft .NET platform.
</p>
</div>
</div>
<style>
.list {
  border-bottom: 1px solid;
  line-height: 50px;
  text-align: center;
  width:200px;
  }
</style>
<div >
<div class="list"> Home </div>
<div class="list"> Communities </div>
</div>
<script>
$(function () {
$("#navigationPane").ejNavigationDrawer();     
});
</script>{% endhighlight %}







#### Requires



* module:jQuery


* module:ej.core.js


* module:ej.navigationdrawer.js


* module:ej.listview.js




## Members





### ajaxSettings  `Object`
{:#members:ajaxsettings}

Specifies the ajaxSettings option to load the content to the NavigationDrawer control.

#### Default Value

* null

#### Example

{% highlight html %}
 
    <div id="container"> </div>
    <div id="navigationPane">
    <ul>
        <li data-ej-text="Artwork"></li>
        <li data-ej-text="Abstract"></li>
        <li data-ej-text="2 Acrylic Mediums"></li>
        <li data-ej-text="Creative Acrylic"></li>
        <li data-ej-text="Modern Painting"></li>
    </ul>
    </div>
    <script>
    // Set the ajaxSettings options during initialization.                  
            $("#navigationPane").ejNavigationDrawer({  ajaxSettings: { type: 'GET', cache: false, data: {}, dataType: "html", contentType: "html", async: true } });
    </script>

{% endhighlight %}


### ajaxSettings.async `boolean`
{:#members:ajaxsettings-async}

It specifies, whether to enable or disable asynchronous request.

### ajaxSettings.cache `boolean`
{:#members:ajaxsettings-cache}

It specifies the page will be cached in the web browser.

### ajaxSettings.contentType `string`
{:#members:ajaxsettings-contenttype}

It specifies the type of data is send in the query string.

### ajaxSettings.data `Object`
{:#members:ajaxsettings-data}

It specifies the data as an object, will be passed in the query string.

### ajaxSettings.dataType `string`
{:#members:ajaxsettings-datatype}

It specifies the type of data that you're expecting back from the response.

### ajaxSettings.type `string`
{:#members:ajaxsettings-type}

It specifies the HTTP request type.


### contentId `string`
{:#members:contentid}








Specifies the contentId for navigation drawer, where the AJAX content need to updated




#### Default Value







* null








#### Example



{% highlight html %}
// Set Navigation Drawer contentId on initialization. 
//To set contentId API value 
<div id="container"> </div>
<div id="navigationPane">
<ul>
                <li data-ej-text="Artwork"></li>
                <li data-ej-text="Abstract"></li>
                <li data-ej-text="2 Acrylic Mediums"></li>
                <li data-ej-text="Creative Acrylic"></li>
                <li data-ej-text="Modern Painting"></li>
</ul>
</div>
<script>
$(function () {
$("#navigationPane").ejNavigationDrawer("contentId","container");      
});
</script>{% endhighlight %}


{% highlight html %}
 
<script>
//Get or set the Navigation Drawer contentId, after initialization:
$(function () {
// Gets the contentId API value.                
$("#navigationPane").ejNavigationDrawer("option", "contentId");       
// Sets the contentId API       
$("#navigationPane").ejNavigationDrawer ("option", "contentId", "container");  
});
</script>  {% endhighlight %}







### cssClass `string`
{:#members:cssclass}








Sets the root class for NavigationDrawer theme. This cssClass API helps to use custom skinning option for NavigationDrawer control. By defining the root class using this API, we need to include this root class in CSS.




#### Default Value







* ""








#### Example



{% highlight html %}
// Set Navigation Drawer direction on initialization. 
//To set direction API value 
<div id="home" class="navsubpage">
<div align="center" class="content">
<h2 class="title">
Home</h2>
<p>
Founded by industry experts in 2001,Syncfusion, Inc. provides the broadest range of enterprise-class software components and tools for the Microsoft .NET platform.
</p>
</div>            
<input id="target" type="button" text="target"/>
</div>
<style>
.list {
  border-bottom: 1px solid;
  line-height: 50px;
  text-align: center;
  width:200px;
  }
</style>
<div >
<div class="list"> Home </div>
<div class="list"> Communities </div>
</div>
<script>
$(function () {
$("#navigationPane").ejNavigationDrawer("cssClass","custom-class");     
});
</script>{% endhighlight %}


{% highlight html %}
 
<script>
//Get or set the Navigation Drawer cssClass, after initialization:
$(function () {
// Gets the cssClass API value.         
$("#navigationPane").ejNavigationDrawer("option", "cssClass"); 
// Sets the cssClass API        
$("#navigationPane").ejNavigationDrawer ("option", "cssClass", "custom-class");  
});
</script>  {% endhighlight %}







### direction `enum`
{:#members:direction}



<ts name="ej.Direction" />




Sets the Direction for the control. See <a href="global.html#Direction">Direction</a>



<table class="props">
<thead>
<tr>
<th>Name</th>
<th>Type</th>
<th>Default</th>
<th class="last">Description</th>
</tr>
</thead>
<tbody>
<tr>
<td class="name">
Left</td>
<td class="type">string</td>
<td class="default">left</td>
<td class="description">Used to set Direction as Left</td>
</tr>
<tr>
<td class="name">
None</td>
<td class="type">string</td>
<td class="default">none</td>
<td class="description">Used to set Direction as None</td>
</tr>
<tr>
<td class="name">
Right</td>
<td class="type">string</td>
<td class="default">right</td>
<td class="description">Used to set Direction as Right</td>
</tr>
</tbody>
</table>



#### Default Value







* left








#### Example



{% highlight html %}
// Set Navigation Drawer direction on initialization. 
//To set direction API value 
<div id="home" class="navsubpage">
<div align="center" class="content">
<h2 class="title">
Home</h2>
<p>
Founded by industry experts in 2001,Syncfusion, Inc. provides the broadest range of enterprise-class software components and tools for the Microsoft .NET platform.
</p>
</div>
</div>
<style>
.list {
  border-bottom: 1px solid;
  line-height: 50px;
  text-align: center;
  width:200px;
  }
</style>
<div >
<div class="list"> Home </div>
<div class="list"> Communities </div>
</div>
<script>
$(function () {
$("#navigationPane").ejNavigationDrawer("direction","left");   
});
</script>{% endhighlight %}


{% highlight html %}
 
<script>
//Get or set the Navigation Drawer direction, after initialization:
$(function () {
// Gets the direction API value.                
$("#navigationPane").ejNavigationDrawer("option", "direction");        
// Sets the direction API       
$("#navigationPane").ejNavigationDrawer ("option", "direction", "left");  
});
</script>  {% endhighlight %}







### enableListView `boolean`
{:#members:enablelistview}








Sets the listview to be enabled or not




#### Default Value







* false








#### Example



{% highlight html %}
// Set Navigation Drawer listview on initialization. 
//To set listview API value 
<div id="home" class="navsubpage">
<div align="center" class="content">
<h2 class="title">
Home</h2>
<p>
Founded by industry experts in 2001,Syncfusion, Inc. provides the broadest range of enterprise-class software components and tools for the Microsoft .NET platform.
</p>
</div>
</div>
<style>
.list {
  border-bottom: 1px solid;
  line-height: 50px;
  text-align: center;
  width:200px;
  }
</style>
<div >
<div class="list"> Home </div>
<div class="list"> Communities </div>
</div>
<script>
$(function () {
$("#navigationPane").ejNavigationDrawer("enableListView","false");     
});
</script>{% endhighlight %}


{% highlight html %}
 
<script>
//Get or set the Navigation Drawer listview, after initialization:
$(function () {
// Gets the listview API value.         
$("#navigationPane").ejNavigationDrawer("option", "enableListView");   
// Sets the listview API        
$("#navigationPane").ejNavigationDrawer ("option", "enableListView", "false");  
});
</script>  {% endhighlight %}







### items `Array`
{:#members:items}








Specifies the listview items as an array of object.




#### Default Value







* []








#### Example



{% highlight html %}
// Set Navigation Drawer listview items on initialization. 
//To set listview API value 
<div id="home" class="navsubpage">
<div align="center" class="content">
<h2 class="title">
Home</h2>
<p>
Founded by industry experts in 2001,Syncfusion, Inc. provides the broadest range of enterprise-class software components and tools for the Microsoft .NET platform.
</p>
</div>
</div>
<style>
.list {
  border-bottom: 1px solid;
  line-height: 50px;
  text-align: center;
  width:200px;
  }
</style>
<div >
<div class="list"> Home </div>
<div class="list"> Communities </div>
</div>
<script>
$(function () {
$("#navigationPane").ejNavigationDrawer({enableListview:true,items:[{text:"Item1"},{text:"Item2"},{text:"Item3"}]});   
});
</script>{% endhighlight %}


{% highlight html %}
 
<script>
//Get or set the Navigation Drawer listview items, after initialization:
$(function () {
// Gets the listViewSettings API value.         
$("#navigationPane").ejNavigationDrawer("option", "items");    
// Sets the listViewSettings API        
$("#navigationPane").ejNavigationDrawer ("option", "items", [{text:"Item1"},{text:"Item2"},{text:"Item3"}]);  
});
</script>  {% endhighlight %}







### listViewSettings `Object`
{:#members:listviewsettings}








Sets all the properties of listview to render in navigation drawer





#### Example



{% highlight html %}
// Set Navigation Drawer listview on initialization. 
//To set listview API value 
<div id="home" class="navsubpage">
<div align="center" class="content">
<h2 class="title">
Home</h2>
<p>
Founded by industry experts in 2001,Syncfusion, Inc. provides the broadest range of enterprise-class software components and tools for the Microsoft .NET platform.
</p>
</div>
</div>
<style>
.list {
  border-bottom: 1px solid;
  line-height: 50px;
  text-align: center;
  width:200px;
  }
</style>
<div >
<div class="list"> Home </div>
<div class="list"> Communities </div>
</div>
<script>
$(function () {
$("#navigationPane").ejNavigationDrawer({model.listViewSettings{width:200});   
});
</script>{% endhighlight %}


{% highlight html %}
 
<script>
//Get or set the Navigation Drawer listViewSettings, after initialization:
$(function () {
// Gets the listViewSettings API value.         
$("#navigationPane").ejNavigationDrawer("option", "listViewSettings.width");   
// Sets the listViewSettings API        
$("#navigationPane").ejNavigationDrawer ("option", "listViewSettings.width", "200");  
});
</script>  {% endhighlight %}







### position `string`
{:#members:position}








Specifies position whether it is in fixed or relative to the page. See <a href="global.html#Position">Position</a>




#### Default Value







* normal








#### Example



{% highlight html %}
// Set Navigation Drawer position on initialization. 
//To set position API value 
<div id="home" class="navsubpage">
<div align="center" class="content">
<h2 class="title">
Home</h2>
<p>
Founded by industry experts in 2001,Syncfusion, Inc. provides the broadest range of enterprise-class software components and tools for the Microsoft .NET platform.
</p>
</div>
</div>
<style>
.list {
  border-bottom: 1px solid;
  line-height: 50px;
  text-align: center;
  width:200px;
  }
</style>
<div >
<div class="list"> Home </div>
<div class="list"> Communities </div>
</div>
<script>
$(function () {
$("#navigationPane").ejNavigationDrawer("position","fixed");   
});
</script>{% endhighlight %}


{% highlight html %}
 
<script>
//Get or set the Navigation Drawer position, after initialization:
$(function () {
// Gets the position API value.         
$("#navigationPane").ejNavigationDrawer("option", "position"); 
// Sets the position API        
$("#navigationPane").ejNavigationDrawer ("option", "position", "fixed");  
});
</script>  {% endhighlight %}







### targetId `string`
{:#members:targetid}








Specifies the targetId for navigation drawer




#### Default Value







* ""








#### Example



{% highlight html %}
// Set Navigation Drawer direction on initialization. 
//To set direction API value 
<div id="home" class="navsubpage">
<div align="center" class="content">
<h2 class="title">
Home</h2>
<p>
Founded by industry experts in 2001,Syncfusion, Inc. provides the broadest range of enterprise-class software components and tools for the Microsoft .NET platform.
</p>
</div>            
<input id="target" type="button" text="target"/>
</div>
<style>
.list {
  border-bottom: 1px solid;
  line-height: 50px;
  text-align: center;
  width:200px;
  }
</style>
<div >
<div class="list"> Home </div>
<div class="list"> Communities </div>
</div>
<script>
$(function () {
$("#navigationPane").ejNavigationDrawer("targetId","target");  
});
</script>{% endhighlight %}


{% highlight html %}
 
<script>
//Get or set the Navigation Drawer targetId, after initialization:
$(function () {
// Gets the targetId API value.         
$("#navigationPane").ejNavigationDrawer("option", "targetId"); 
// Sets the targetId API        
$("#navigationPane").ejNavigationDrawer ("option", "targetId", "left");  
});
</script>  {% endhighlight %}


### type `string`
{:#members:type}








Sets the rendering type of the control. See Type




#### Default Value







* overlay








#### Example



{% highlight html %}
// Set Navigation Drawer type on initialization. 
//To set type API value 
<div id="home" class="navsubpage">
<div align="center" class="content">
<h2 class="title">
Home</h2>
<p>
Founded by industry experts in 2001,Syncfusion, Inc. provides the broadest range of enterprise-class software components and tools for the Microsoft .NET platform.
</p>
</div>
</div>
<style>
.list {
  border-bottom: 1px solid;
  line-height: 50px;
  text-align: center;
  width:200px;
  }
</style>
<div >
<div class="list"> Home </div>
<div class="list"> Communities </div>
</div>
<script>
$(function () {
$("#navigationPane").ejNavigationDrawer("type","overlay");     
});
</script>{% endhighlight %}


{% highlight html %}
 
<script>
//Get or set the Navigation Drawer type, after initialization:
$(function () {
// Gets the type API value.             
$("#navigationPane").ejNavigationDrawer("option", "type");     
// Sets the type API    
$("#navigationPane").ejNavigationDrawer ("option", "type", "overlay");  
});
</script>  {% endhighlight %}







### width `number`
{:#members:width}








Specifies the width of the control




#### Default Value







* auto








#### Example



{% highlight html %}
// Set Navigation Drawer width on initialization. 
//To set width API value 
<div id="home" class="navsubpage">
<div align="center" class="content">
<h2 class="title">
Home</h2>
<p>
Founded by industry experts in 2001,Syncfusion, Inc. provides the broadest range of enterprise-class software components and tools for the Microsoft .NET platform.
</p>
</div>
</div>
<style>
.list {
  border-bottom: 1px solid;
  line-height: 50px;
  text-align: center;
  width:200px;
  }
</style>
<div >
<div class="list"> Home </div>
<div class="list"> Communities </div>
</div>
<script>
$(function () {
$("#navigationPane").ejNavigationDrawer("width","200");        
});
</script>{% endhighlight %}


{% highlight html %}
 
<script>
//Get or set the Navigation Drawer width, after initialization:
$(function () {
// Gets the width API value.            
$("#navigationPane").ejNavigationDrawer("option", "width");    
// Sets the width API   
$("#navigationPane").ejNavigationDrawer ("option", "width", "overlay");  
});
</script>  {% endhighlight %}



### isPaneOpen `boolean`
{:#members:ispaneopen}


Navigation pane opened initially when isPaneOpen property is true.

#### Default Value

* false

#### Example


{% highlight html %}
// Set Navigation Drawer isPaneOpen on initialization. 
//To set isPaneOpen API value 
<div id="home" class="navsubpage">
<div align="center" class="content">
<h2 class="title">
Home</h2>
<p>
Founded by industry experts in 2001,Syncfusion, Inc. provides the broadest range of enterprise-class software components and tools for the Microsoft .NET platform.
</p>
</div>
</div>
<div >
<div class="list"> Home </div>
<div class="list"> Communities </div>
</div>
<script>
$(function () {
$("#navigationPane").ejNavigationDrawer({isPaneOpen:true});        
});
</script>{% endhighlight %}


{% highlight html %}
 
<script>
//Get or set the Navigation Drawer isPaneOpen, after initialization:
$(function () {
// Gets the isPaneOpen API value.            
$("#navigationPane").ejNavigationDrawer("option", "isPaneOpen");    
// Sets the isPaneOpen API   
$("#navigationPane").ejNavigationDrawer ("option", "isPaneOpen",false);  
});
</script>  {% endhighlight %}

## Methods








### close()
{:#methods:close}








To close the navigation drawer control





#### Example



{% highlight html %}
 
<div id="home" class="navsubpage">
<div align="center" class="content">
<h2 class="title">
Home</h2>
<p>
Founded by industry experts in 2001,Syncfusion, Inc. provides the broadest range of enterprise-class software components and tools for the Microsoft .NET platform.
</p>
</div>
</div>
<style>
.list {
  border-bottom: 1px solid;
  line-height: 50px;
  text-align: center;
  width:200px;
  }
</style>
<div id="navigationPane" >
<div class="list"> Home </div>
<div class="list"> Communities </div>
</div>
<script >
$(function(){
  $("#navigationPane").ejNavigationDrawer();
  $("#navigationPane").ejNavigationDrawer("close");
});
</script >{% endhighlight %}


### loadContent(id,url)
{:#methods:loadcontent}


To load AJAX content into NavigationDrawer container.


#### Example



{% highlight html %}

    <div class="e-header">
      <div id="buttonDrawer" class="drawericon e-icon"></div>
      <h2>Template Content</h2>
    </div>
    <div id="navigationPane">
      <div id="basicAccordion" class="control_frame">
        <h3><a href="#">Menu</a></h3>
        <div>
          <div class="selectedAccordion" data-url="#Home">Home</div>
          <div class="selectedAccordion" data-url="#People">People</div>
          <div class="selectedAccordion" data-url="#Profile">Profile</div>
        </div>
      </div>
    </div>
    <script >
    $(function(){
      $("#basicAccordion").ejAccordion({width:"100%",height:"100%"});
      $("#navigationPane").ejNavigationDrawer({ targetId: "buttonDrawer", contentId: "content_container", type: "overlay", direction: "left", position: "normal" });
      $(".selectedAccordion").click(function(e){
          var navigationObj = $("#navigationPane").ejNavigationDrawer("instance");
          navigationObj.loadContent($("#content_container") ,"/Content/NavigationDrawer/"+$(e.currentTarget).attr("data-url").replace("#","")+".html");
        });
    });
    </script >
    
{% endhighlight %}




### open()
{:#methods:open}








To open the navigation drawer control





#### Example



{% highlight html %}
 
<div id="home" class="navsubpage">
<div align="center" class="content">
<h2 class="title">
Home</h2>
<p>
Founded by industry experts in 2001,Syncfusion, Inc. provides the broadest range of enterprise-class software components and tools for the Microsoft .NET platform.
</p>
</div>
</div>
<style>
.list {
  border-bottom: 1px solid;
  line-height: 50px;
  text-align: center;
  width:200px;
  }
</style>
<div id="navigationPane" >
<div class="list"> Home </div>
<div class="list"> Communities </div>
</div>
<script >
$(function(){
        $("#navigationPane").ejNavigationDrawer();
  $("#navigationPane").ejNavigationDrawer("open");
});
</script >{% endhighlight %}







### toggle()
{:#methods:toggle}








To Toggle the navigation drawer control





#### Example



{% highlight html %}
 
<div id="home" class="navsubpage">
<div align="center" class="content">
<h2 class="title">
Home</h2>
<p>
Founded by industry experts in 2001,Syncfusion, Inc. provides the broadest range of enterprise-class software components and tools for the Microsoft .NET platform.
</p>
</div>
</div>
<style>
.list {
  border-bottom: 1px solid;
  line-height: 50px;
  text-align: center;
  width:200px;
  }
</style>
<div id="navigationPane" >
<div class="list"> Home </div>
<div class="list"> Communities </div>
</div>
<script >
$(function(){
        $("#navigationPane").ejNavigationDrawer();
  $("#navigationPane").ejNavigationDrawer("toggle");
});
</script >{% endhighlight %}





## Events





### ajaxComplete
{:#events:ajaxcomplete}




Event triggers after the AJAX content loaded completely.

<table>
<tr>
<th>
Name</th><th>
Type</th><th>
Description</th></tr>
<tr>
<td>
cancel</td><td>
boolean</td><td>
Set this option to true to cancel the event.</td></tr>
<tr>
<td>
model</td><td><ts ref="ej.NavigationDrawer.Model"/>
Object</td><td>
Instance of the navigation drawer model object.</td></tr>
<tr>
<td>
type</td><td>
string</td><td>
Name of the event.</td></tr>
<tr>
<td>
URL</td><td>
string</td><td>
URL of the content.</td></tr>
<tr>
<td>
data</td><td>
string</td><td>
Response content.</td></tr>
</table>


#### Example



{% highlight html %}

    <div id="home" class="navsubpage">
    <div align="center" class="content">
    <h2 class="title">
    Home</h2>
    <p>
    Founded by industry experts in 2001,Syncfusion, Inc. provides the broadest range of enterprise-class software components and tools for the Microsoft .NET platform.
    </p>
    </div>
    </div>
    <style>
    .list {
      border-bottom: 1px solid;
      line-height: 50px;
      text-align: center;
      width:200px;
      }
    </style>
    <div id="navigationPane" >
    <div class="list"> Home </div>
    <div class="list"> Communities </div>
    </div>
    <script >
    $(function(){
            $("#navigationPane").ejNavigationDrawer({
              ajaxComplete: function (args) { //handle the event }
            }
            });
    });
    </script >

{% endhighlight %}


### ajaxError
{:#events:ajaxerror}




Event triggers when the AJAX request failed.

<table>
<tr>
<th>
Name</th><th>
Type</th><th>
Description</th></tr>
<tr>
<td>
cancel</td><td>
boolean</td><td>
Set this option to true to cancel the event.</td></tr>
<tr>
<td>
model</td><td><ts ref="ej.NavigationDrawer.Model"/>
Object</td><td>
Instance of the navigation drawer model object.</td></tr>
<tr>
<td>
type</td><td>
string</td><td>
Name of the event.</td></tr>
<tr>
<td>
URL</td><td>
string</td><td>
URL of the content.</td></tr>
<tr>
<td class="name">data</td>
<td class="type"><ts ref="ej.NavigationDrawer.Model"/><span class="param-type">Object</span></td>
<td class="description last">
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
<td class="name">responseText</td>
<td class="type"><span class="param-type">string</span></td>
<td class="description last">Error page content.</td>
</tr>
<tr>
<td class="name">status</td>
<td class="type"><span class="param-type">number</span></td>
<td class="description last">Error code.</td>
</tr>
<tr>
<td class="name">statusText</td>
<td class="type"><span class="param-type">string</span></td>
<td class="description last">The corresponding error description.</td>
</tr>
</tbody>
</table>
</td>
</td>
</tr>
</table>


#### Example


{% highlight html %}

    <div id="home" class="navsubpage">
    <div align="center" class="content">
    <h2 class="title">
    Home</h2>
    <p>
    Founded by industry experts in 2001,Syncfusion, Inc. provides the broadest range of enterprise-class software components and tools for the Microsoft .NET platform.
    </p>
    </div>
    </div>
    <style>
    .list {
      border-bottom: 1px solid;
      line-height: 50px;
      text-align: center;
      width:200px;
      }
    </style>
    <div id="navigationPane" >
    <div class="list"> Home </div>
    <div class="list"> Communities </div>
    </div>
    <script >
    $(function(){
            $("#navigationPane").ejNavigationDrawer({
              ajaxError: function (args) { //handle the event }
            }
            });
    });
    </script >

{% endhighlight %}


### ajaxSuccess
{:#events:ajaxsuccess}




Event triggers after the AJAX content loaded successfully.

<table>
<tr>
<th>
Name</th><th>
Type</th><th>
Description</th></tr>
<tr>
<td>
cancel</td><td>
boolean</td><td>
Set this option to true to cancel the event.</td></tr>
<tr>
<td>
model</td><td><ts ref="ej.NavigationDrawer.Model"/>
Object</td><td>
Instance of the navigation drawer model object.</td></tr>
<tr>
<td>
type</td><td>
string</td><td>
Name of the event.</td></tr>
<tr>
<td>
URL</td><td>
string</td><td>
URL of the content.</td></tr>
<tr>
<td>
data</td><td>
string</td><td>
Response content.</td></tr>
</table>


#### Example


{% highlight html %}

    <div id="home" class="navsubpage">
    <div align="center" class="content">
    <h2 class="title">
    Home</h2>
    <p>
    Founded by industry experts in 2001,Syncfusion, Inc. provides the broadest range of enterprise-class software components and tools for the Microsoft .NET platform.
    </p>
    </div>
    </div>
    <style>
    .list {
      border-bottom: 1px solid;
      line-height: 50px;
      text-align: center;
      width:200px;
      }
    </style>
    <div id="navigationPane" >
    <div class="list"> Home </div>
    <div class="list"> Communities </div>
    </div>
    <script >
    $(function(){
            $("#navigationPane").ejNavigationDrawer({
              ajaxSuccess: function (args) { //handle the event }
            }
            });
    });
    </script >

{% endhighlight %}


### beforeClose
{:#events:beforeclose}








Event triggers before the control gets closed.

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
<td class="description">Event parameters from Navigation Drawer
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
<td class="type"><ts ref="ej.NavigationDrawer.Model"/><span class="param-type">Object</span></td>
<td class="description">returns the Navigation Drawer model</td>
</tr>
<tr>
<td class="name">
type</td>
<td class="type"><span class="param-type">string</span></td>
<td class="description">returns the name of the event</td>
</tr>
</tbody>
</table>
</td>
</tr>
</tbody>
</table>




#### Example



{% highlight html %}
 
//BeforeClose event for Navigation pane
<div id="home" class="navsubpage">
<div align="center" class="content">
<h2 class="title">
Home</h2>
<p>
Founded by industry experts in 2001,Syncfusion, Inc. provides the broadest range of enterprise-class software components and tools for the Microsoft .NET platform.
</p>
</div>
</div>
<style>
.list {
  border-bottom: 1px solid;
  line-height: 50px;
  text-align: center;
  width:200px;
  }
</style>
<div id="navigationPane" >
<div class="list"> Home </div>
<div class="list"> Communities </div>
</div>
<script>
$("#navigationPane").ejNavigationDrawer({
  beforeClose: function (args) { //handle the event
}
});   
$("#navigationPane").ejNavigationDrawer("close");
</script>{% endhighlight %}







### open
{:#events:open}








Event triggers when the control open.

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
<td class="description">Event parameters from Navigation Drawer
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
<td class="type"><ts ref="ej.NavigationDrawer.Model"/><span class="param-type">Object</span></td>
<td class="description">returns the Navigation Drawer model</td>
</tr>
<tr>
<td class="name">
type</td>
<td class="type"><span class="param-type">string</span></td>
<td class="description">returns the name of the event</td>
</tr>
</tbody>
</table>
</td>
</tr>
</tbody>
</table>




#### Example



{% highlight html %}
 
//Open event for Navigation pane
<div id="home" class="navsubpage">
<div align="center" class="content">
<h2 class="title">
Home</h2>
<p>
Founded by industry experts in 2001,Syncfusion, Inc. provides the broadest range of enterprise-class software components and tools for the Microsoft .NET platform.
</p>
</div>
</div>
<style>
.list {
  border-bottom: 1px solid;
  line-height: 50px;
  text-align: center;
  width:200px;
  }
</style>
<div id="navigationPane" >
<div class="list"> Home </div>
<div class="list"> Communities </div>
</div>
<script>
$("#navigationPane").ejNavigationDrawer({
  open: function (args) { //handle the event
}
});   
$("#navigationPane").ejNavigationDrawer("open");   
</script>{% endhighlight %}







### swipe
{:#events:swipe}








Event triggers when the Swipe happens.

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
<td class="description">Event parameters from Navigation Drawer
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
<td class="type"><ts ref="ej.NavigationDrawer.Model"/><span class="param-type">Object</span></td>
<td class="description">returns the Navigation Drawer model</td>
</tr>
<tr>
<td class="name">
type</td>
<td class="type"><span class="param-type">string</span></td>
<td class="description">returns the name of the event</td>
</tr>
</tbody>
</table>
</td>
</tr>
</tbody>
</table>




#### Example



{% highlight html %}
 
//Swipe event for Navigation pane
<div id="home" class="navsubpage">
<div align="center" class="content">
<h2 class="title">
Home</h2>
<p>
Founded by industry experts in 2001,Syncfusion, Inc. provides the broadest range of enterprise-class software components and tools for the Microsoft .NET platform.
</p>
</div>
</div>
<style>
.list {
  border-bottom: 1px solid;
  line-height: 50px;
  text-align: center;
  width:200px;
  }
</style>
<div id="navigationPane" >
<div class="list"> Home </div>
<div class="list"> Communities </div>
</div>
<script>
$("#navigationPane").ejNavigationDrawer({
  swipe: function (args) { //handle the event
}
});   
</script>{% endhighlight %}




