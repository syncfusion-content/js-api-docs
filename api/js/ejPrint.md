---
layout: post
title: ejPrint
documentation: API
platform: js
keywords: ejPrint, API, Essential JS Print
---

# ejPrint

 A flexible widget that allows the user to print a complete page or a particular element in it with the required customizations. 

#### Syntax

{% highlight js %}
 
    $(element).ejPrint();

{% endhighlight %}


#### Example

{% highlight html %}

   <div id="Grid"></div>
 
    <script>
    $("#Grid").ejPrint();
    </script>  
   
{% endhighlight %}


#### Requires

* module:jQuery
* module:ej.core
* module:ej.print

## Members

### append  `string`
{:#members:append}

Append the custom HTML after the selected content.

#### Default Value:

* null

#### Example

{% highlight html %}

    <div id="control">
        <div id="Grid"></div>
        <br />
        Print the Grid :
        <button class="button" id="print">Print</button>
    </div>
    <script>
        $(function () {
            $("#Grid").ejGrid({
                dataSource: window.gridData,
                allowPaging: true,
                columns: ["OrderID", "EmployeeID", "ShipCity", "ShipCountry", "Freight"]
            });

            $("#print").ejButton({
                size: "normal", width: "113px", click: "onPrint"
            });
        })
    </script>

    //To make use of append - 
    
    <script>
    function onPrint(e) {
            var gridElement = $("#Grid");
            if (!gridElement.hasClass("e-print")) {
                $("#Grid").ejPrint(
                 {
                     append: "#Grid"
                 });
            } else {
                var obj = $("#Grid").ejPrint("instance")
                obj.option("append", "#Grid");
                obj.print();
            }
        }
    </script>

{% endhighlight %}


### excludeSelector `string`
{:#members:excludeselector}

A selector that specifies a particular element to be excluded from printing.

#### Default Value:

* null

#### Example

{% highlight html %}
 
    //To set excludeSelector 
    <div id="Grid"></div>
    <script>
      function onPrint(e) {
            var gridElement = $("#Grid");
            if (!gridElement.hasClass("e-print")) {
                $("#Grid").ejPrint(
            {
                excludeSelector: "#Grid"
            });

            } else {
                var obj = $("#Grid").ejPrint("instance");
                obj.option("excludeSelector", "#Grid");
                obj.print();
            }
        }
   </script>
    
{% endhighlight %}

### externalStyles `string`
{:#members:externalstyles}

Specifies whether the URL of an external stylesheet can be included to customize and print that page.

#### Default Value:

* null

#### Example 

{% highlight html %}
 
    //To set externalStyles API 
    <div id="Grid"></div>
    <script>
          function onPrint(e) {
            var gridElement = $("#Grid");
            if (!gridElement.hasClass("e-print")) {
                $("#Grid").ejPrint(
                 {
                     globalStyles: false,
                     externalStyles: "http://cdn.syncfusion.com/{{ site.releaseversion }}/js/web/flat-azure/ej.web.all.min.css"
                 });
            } else {
                var obj = $("#Grid").ejPrint("instance")
                obj.option("globalStyles", false);
                obj.option("externalStyles", "http://cdn.syncfusion.com/{{ site.releaseversion }}/js/web/flat-azure/ej.web.all.min.css");
                obj.print();
            }
        }
    </script>

{% endhighlight %}

### docType `string`
{:#members:doctype}

Prepend a docType to the document frame.

#### Default Value:

* <!doctype html>


#### Example

{% highlight html %}
 
    //To set docType API 
    <div id="Grid"></div>
    <script>
     function onPrint(e) {
            var gridElement = $("#Grid");
            if (!gridElement.hasClass("e-print")) {
                $("#Grid").ejPrint(
                 {
                     docType: "<!doctype html>"
                 });
            } else {
                var obj = $("#Grid").ejPrint("instance")
                obj.option("docType", "<!DOCTYPE html>");
                obj.print();
            }
        }
    </script>

{% endhighlight %}



### globalStyles `boolean`
{:#members:globalstyles}

Specifies whether the global styles can be applied to the element to be printed.


#### Default Value:

* true

#### Example

{% highlight html %}

    <script>
        function onPrint(e) {
            var gridElement = $("#Grid");
            if (!gridElement.hasClass("e-print")) {
                $("#Grid").ejPrint(
                 {
                     globalStyles: false
                 });
            } else {
                var obj = $("#Grid").ejPrint("instance")
                obj.option("globalStyles", false);
                obj.print();
            }
        }
    </script>

    
{% endhighlight %}

### height `number`
{:#members:height}

Sets the height of the print window.


#### Default Value:

* 454

#### Example

{% highlight html %}

    //To set the height of the print window
   
    <script>
        function onPrint(e) {
            var gridElement = $("#Grid");
            if (!gridElement.hasClass("e-print")) {
                $("#Grid").ejPrint(
                 {
                     height: 500
                 });
            } else {
                var obj = $("#Grid").ejPrint("instance")
                obj.option("height", 500);
                obj.print();
            }
        }
    </script>

    
{% endhighlight %}

### prepend  `string`
{:#members:prepend}

Prepends the custom HTML before the selected content.


#### Default Value:

* null

#### Example

{% highlight html %}

    <div id="Grid"></div>
    <script>
    function onPrint(e) {
            var gridElement = $("#Grid");
            if (!gridElement.hasClass("e-print")) {
                $("#Grid").ejPrint(
                 {
                     prepend: "#Grid"
                 });
            } else {
                var obj = $("#Grid").ejPrint("instance")
                obj.option("prepend", "#Grid");
                obj.print();
            }
        }
    </script>

{% endhighlight %}

### printInNewWindow `boolean`
{:#members:printInNewWindow}

Allows printing the content in a new window.


#### Default Value:

* false

#### Example

{% highlight html %}
 
    <div id="Grid"></div>
    <script>
     function onPrint(e) {
            var gridElement = $("#Grid");
            if (!gridElement.hasClass("e-print")) {
                $("#Grid").ejPrint(
                 {
                     printInNewWindow:true
                 });
            } else {
                var obj = $("#Grid").ejPrint("instance")
                obj.option("printInNewWindow",true);
                obj.print();
            }
        }
    </script>

{% endhighlight %}

### timeOutPeriod `number`
{:#members:timeOutPeriod}

Sets the period of time to wait before printing the content.


#### Default Value:

* 1000

#### Example


{% highlight html %}

    <div id="Grid"></div>
    <script>
    function onPrint(e) {
            var gridElement = $("#Grid");
            if (!gridElement.hasClass("e-print")) {
                $("#Grid").ejPrint(
                 {
                     timeOutPeriod: 1200
                 });
            } else {
                var obj = $("#Grid").ejPrint("instance")
                obj.option("timeOutPeriod", 1200);
                obj.print();
            }
        }
    </script>

{% endhighlight %}


### title  `string`
{:#members:title}

Sets the title of the print document.

#### Default Value:

* null

#### Example

{% highlight html %}
 
    <div id="Grid"></div>
    <script>
    function onPrint(e) {
            var gridElement = $("#Grid");
            if (!gridElement.hasClass("e-print")) {
                $("#Grid").ejPrint(
                 {
                     title: "Print Grid"
                 });
            } else {
                var obj = $("#Grid").ejPrint("instance")
                obj.option("title", "Print Grid");
                obj.print();
            }
        }
    </script>

{% endhighlight %}

### width  `number`
{:#members:width}

Defines the width of the print window.

#### Default Value:

* 1024

#### Example

{% highlight html %}
 
    <div id="Grid"></div>
    <script>
    function onPrint(e) {
            var gridElement = $("#Grid");
            if (!gridElement.hasClass("e-print")) {
                $("#Grid").ejPrint(
                 {
                     width: 1500
                 });
            } else {
                var obj = $("#Grid").ejPrint("instance")
                obj.option("width", 1500);
                obj.print();
            }
        }
    </script>

{% endhighlight %}


## Methods

### print()
{:#methods:print}

Print the specific page or an element.

#### Returns:
{:#methods:returns:}

void

#### Example

{% highlight html %}
 
    <div id="Grid"></div>
 
    <script>
    //Print the particular element
        function onPrint(e) {
            var gridElement = $("#Grid");
            if (!gridElement.hasClass("e-print")) {
                $("#Grid").ejPrint();
                $("#Grid").ejPrint("print","#print");  
            } else {
                var obj = $("#Grid").ejPrint("instance")
                obj.print("#print");
            }
        }
        //Print the current page
          function onPrint (e) {
            var gridElement = $(document.body);
            if (!gridElement.hasClass("e-print")) {
                $(document.body).ejPrint();
            } else {
                obj = $(document.body).ejPrint("instance");
                obj.print();

            }
        }

    </script>

{% endhighlight %}


## Events

### beforeStart
{:#events:beforeStart}

Event triggers before the document page or an element in it gets printed.

<table class="params" border="1">
<thead>
<tr>
<th> Name </th>
<th> Type </th>
<th> Description </th>
</tr>
</thead>

<tbody>
<tr>
<td> cancel </td>
<td> boolean </td>
<td> Set this option as true to cancel the event.</td>
</tr>

<tr>
<td> model </td>
<td><ts ref="ej.Print.Model"/><span class="param-type">Object</span></td>
<td> Returns the Print model </td>
</tr>
<tr>
<td> type </td>
<td> string </td>
<td> Returns the name of an event </td>
</tr>
<tr>
<td> content</td>
<td> Object </td>
<td> Returns the printed element</td>
</tr>
</tbody>
</table>

#### Example

{% highlight html %}
 
    //beforeStart event for Print

    <div id="Grid"></div>

    <script>
    $("#Grid").ejPrint ({
    beforeStart: function (args) 
    { 
    //handle the event
    }
    });         
    </script>
    
    
{% endhighlight %}