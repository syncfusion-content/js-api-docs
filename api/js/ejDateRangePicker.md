---
layout: post
title: Syncfusion Essential JS  DateRangePicker Widget
description: Properties, Methods & Events reference for ejDateRangePicker
documentation: ug
platform: js-api
keywords: dateRangePicker, ejDateRangePicker, syncfusion, dateRangePicker api 
---

# ejDateRangePicker

Input field that displays the two DatePicker type calendar in a single popup to select and set the different date ranges


#### Syntax

{% highlight javascript %}

$(element).ejDateRangePicker(options)

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
<td class="type"><span class="param-type">object</span></td>
<td class="description">settings for Date Range Picker.</td>
</tr>
</tbody>
</table>




#### Example



{% highlight html %}
 
<input type="text" id="daterangepicker" />
<script>
// Create DateRangePicker
$("#daterangepicker").ejDateRangePicker();
</script>

{% endhighlight %}





#### Requires



* module:jQuery

* module:ej.core.js

* module:ej.globalize.js

* module:ej.scroller.js

* module:ej.datepicker.js

* module:ej.timepicker.js

* module:ej.daterangepicker.js





## Members


### allowEdit `boolean`
{:#members:allowedit}


Used to allow or restrict the editing in DateRangePicker input field directly. By setting false to this API, You can only pick the date ranges from DateRangePicker popup.




#### Default Value







* true








#### Example



{% highlight html %}
 
<input type="text" id="daterangepicker" />
<script>
//To set allowEdit API during initialization to deny edit  
        $("#daterangepicker").ejDateRangePicker({   allowEdit : false });
</script>

{% endhighlight %}








### buttonText `object`
{:#members:buttontext}


Sets the specified text value to the available buttons (Reset, Cancel, Apply) in the DateRangePicker popup.




#### Default Value







* { reset: "Reset", cancel: "Cancel", apply: "Apply"}








#### Example



{% highlight html %}
 
<input type="text" id="daterangepicker" />
<script>
//To set buttonText API during initialization  
        $("#daterangepicker").ejDateRangePicker({  buttonText : {
            reset: "Reset",
            cancel: "Cancel",
            apply: "Apply"} });
            
</script>

{% endhighlight %}






### cssClass `string`
{:#members:cssclass}








Sets the root CSS class for DateRangePicker theme, which is used to customize.



#### Default Value







* ""








#### Example



{% highlight html %}
 
<input type="text" id="daterangepicker" />
<script>
//To set cssClass API during initialization  
        $("#daterangepicker").ejDateRangePicker({  cssClass: "gradient-lime" });
</script>

{% endhighlight %}







### dateFormat `string`
{:#members:dateformat}



Formats the date value of the DateRangePicker in to the specified date format. If this API is not specified, dateFormat will be set based on the current culture of DateRangePicker.




#### Default Value







* "MM/dd/yyyy"








#### Example



{% highlight html %}
 
<input type="text" id="daterangepicker" />
<script>
//To set dateFormat API during initialization  
        $("#daterangepicker").ejDateRangePicker({  dateFormat: "dd/MM/yyyy" });
</script>

{% endhighlight %}










### enableTimePicker `boolean`
{:#members:enableTimePicker}








Allows to embed the Timepicker align with the calendars in the page, two timepicker will be render, for selecting start and end date.




#### Default Value







* false








#### Example



{% highlight html %}
 
<input type="text" id="daterangepicker" />
<script>
//To set enableTimePicker API during initialization  
        $("#daterangepicker").ejDateRangePicker({  enableTimePicker: true });
</script>

{% endhighlight %}







### enabled `boolean`
{:#members:enabled}








Enable or disable the DateRangePicker control.




#### Default Value







* true








#### Example



{% highlight html %}
 
<input type="text" id="daterangepicker" />
<script>
//To set enabled API during initialization  
        $("#daterangepicker").ejDateRangePicker({  enabled: false });
</script>

{% endhighlight %}







### enablePersistence `boolean`
{:#members:enablepersistence}








Sustain the entire widget model of DateRangePicker even after form post or browser refresh 




#### Default Value







* false








#### Example



{% highlight html %}
 
<input type="text" id="daterangepicker" />
<script>
//To set enablePersistence API during initialization  
        $("#daterangepicker").ejDateRangePicker({  enablePersistence: true });
</script> 


{% endhighlight %}



### endDate `string | date`
{:#members:endDate}








Specifies the end date of the date ranges.




#### Default Value







* null








#### Example



{% highlight html %}
 
<input type="text" id="daterangepicker" />
<script>
//To set minDate value during initialization  
        $("#daterangepicker").ejDateRangePicker({  endDate: new Date("5/1/2013") });
</script>

{% endhighlight %}













### height `string | number`
{:#members:height}








Specifies the height of the DateRangePicker input.




#### Default Value







* "28px"








#### Example



{% highlight html %}
 
<input type="text" id="daterangepicker" />
<script>
//To set height API during initialization  
        $("#daterangepicker").ejDateRangePicker({  height: 35 });
</script> 

{% endhighlight %}


### locale `string`
{:#members:locale}


Change the DateRangePicker calendar and date format based on given culture.




#### Default Value







* "en-US"








#### Example



{% highlight html %}
 
<input type="text" id="daterangepicker" />
<script>
//To set locale API during initialization  
        $("#daterangepicker").ejDateRangePicker({  locale: "en-US" });
</script>

{% endhighlight %}


### maxDate `string | date`
{:#members:maxdate}


Specifies the maximum date in the calendar that the user can select as a startDate or endDate.


#### Default Value

* new Date(2099, 11, 31)

#### Example

{% highlight html %}
 
<input type="text" id="daterangepicker" />
<script>
//To set maxDate value during initialization  
        $("#daterangepicker").ejDateRangePicker({  maxDate : new Date("1/1/2018") });
</script>

{% endhighlight %}

### minDate `string | date`
{:#members:mindate}


Specifies the minimum date in the calendar that the user can select as a startDate or endDate.


#### Default Value

* new Date(1900, 00, 01)

#### Example

{% highlight html %}
 
<input type="text" id="daterangepicker" />
<script>
//To set minDate value during initialization  
        $("#daterangepicker").ejDateRangePicker({  minDate: new Date("1/1/2017") });
</script>

{% endhighlight %}


### ranges `object`
{:#members:ranges}


Used to add the preset ranges. Added ranges using this, will show in popup in right side for easy selection of different preset ranges.



#### Default Value:

* null

### ranges.label `string`

Set the name to preset range

### ranges.range `array`

Get and Set the startDate, end Date of predefined set ranges. The first argument to this field will consider as startDate, and second one will consider as endDate.

 
#### Example 

{% highlight html %}


	<input type="text" id="daterangepicker" />
<script>
//To set minDate value during initialization  
        $("#daterangepicker").ejDateRangePicker({  
ranges: [
            { label: "Today", range: [new Date(), new Date()] },
            { label: "Last 1 Week", range: [new Date(new Date().setDate(new Date().getDate() - 7)), new Date()] },
            { label: "Last 1 Month", range: [new Date(new Date().setMonth(new Date().getMonth() - 1)), new Date()] },
            { label: "Last 2 Month", range: [new Date(new Date().setMonth(new Date().getMonth() - 2)), new Date()] },


        ],
            });
</script>



{% endhighlight %}




### separator `string`
{:#members:separator}





Used to separate the two date strings of the value in the DateRangePicker popup.



#### Default Value





* "-"





#### Example



{% highlight html %}
 
<input type="text" id="daterangepicker" />
<script>
//To set different separator during initialization  
        $("#daterangepicker").ejDateRangePicker({  separator : "$" });
</script>

{% endhighlight %}


### startDate `string | date`
{:#members:startdate}








Specifies the start date of the date ranges



#### Default Value







* null








#### Example



{% highlight html %}
 
<input type="text" id="daterangepicker" />
<script>
//To set startDate value during initialization  
        $("#daterangepicker").ejDateRangePicker({  startDate : new Date("5/30/2015") });
</script>

{% endhighlight %}









### showPopupButton `boolean`
{:#members:showpopupbutton}







Shows/hides the date icon button at right side of textbox, which is used to open or close the DateRangePicker calendar popup.




#### Default Value







* true








#### Example



{% highlight html %}
 
<input type="text" id="daterangepicker" />
<script>
//To set showPopupButton API during initialization  
        $("#daterangepicker").ejDateRangePicker({  showPopupButton: false });
</script>

{% endhighlight %}







### showRoundedCorner `boolean`
{:#members:showroundedcorner}




DateRangePicker input and popup is displayed with rounded corner when this property is set to true.




#### Default Value







* false








#### Example



{% highlight html %}
 
<input type="text" id="daterangepicker" />
<script>
//To set showRoundedCorner API during initialization  
        $("#daterangepicker").ejDateRangePicker({  showRoundedCorner : true });
</script>

{% endhighlight %}




### timeFormat `string`
{:#members:timeformat}



Formats the date value of the DateRangePicker in to the specified time format. If this API is not specified, timeFormat will be set based on the current culture of DateRangePicker.




#### Default Value







* "HH:mm tt"








#### Example



{% highlight html %}
 
<input type="text" id="daterangepicker" />
<script>
//To set timeFormat API during initialization  
        $("#daterangepicker").ejDateRangePicker({  timeFormat: "HH:mm" });
</script>

{% endhighlight %}











### value `string`
{:#members:value}







Separated two date values in string format to sets the date ranges in calendars. 




#### Default Value







* null








#### Example



{% highlight html %}
 
<input type="text" id="daterangepicker" />
<script>
//To set the DateRangePicker value during initialization  
        $("#daterangepicker").ejDateRangePicker({  value: "5/5/2014 - 6/6/2018") });
</script>

{% endhighlight %}







### watermarkText `string`
{:#members:watermarktext}








Specifies the water mark text to be displayed in input text.




#### Default Value







* "Select Range"








#### Example



{% highlight html %}
 
<input type="text" id="daterangepicker" />
<script>
//To set watermarkText during initialization  
        $("#daterangepicker").ejDateRangePicker({  watermarkText: "Enter date" });
</script>

{% endhighlight %}







### width `string | number`
{:#members:width}



Specifies the width of the DateRangePicker input text.




#### Default Value


* "160px"


#### Example



{% highlight html %}
 
<input type="text" id="daterangepicker" />
<script>
//To set width API during initialization  
        $("#daterangepicker").ejDateRangePicker({  width: 200 });
</script> 

{% endhighlight %}





## Methods

### addRanges(label, range)
{:#methods:addRanges}




Add the preset ranges to DateRangePicker popup. 

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
label</td>
<td class="type"><span class="param-type">string</span></td>
<td class="description">Display name</td>
</tr>
<tr>
<td class="name">
range</td>
<td class="type"><span class="param-type">array</span></td>
<td class="description">StartDate and endDate of range.</td>
</tr>
</tbody>
</table>





#### Example



{% highlight html %}
 
<input type="text" id="daterangepicker" />
<script>
$("#daterangepicker").ejDateRangePicker();
// Create DateRangePicker instance
var dateObj = $("#daterangepicker").data("ejDateRangePicker");
dateObj.addRanges("new Range", [new Date("11/12/2019"),new Date("11/12/2021")] ); // Add the preset ranges to DateRangePicker
</script>

{% endhighlight %}

### clearRanges()
{:#methods:clearRanges}




Clears the all ranges selections in DateRangePicker popup





#### Example



{% highlight html %}
 
<input type="text" id="daterangepicker" />
<script>
$("#daterangepicker").ejDateRangePicker();
// create DateRangePicker instance
var dateObj = $("#daterangepicker").data("ejDateRangePicker");
dateObj.clearRanges(); // clear  the DateRangePicker ranges selection
</script>

{% endhighlight %}


{% highlight html %}
 
<input type="text" id="daterangepicker" />
<script>
$("#daterangepicker").ejDateRangePicker();
// clears the DateRangePicker selection
$("#daterangepicker").ejDateRangePicker("clearRanges");
</script>

{% endhighlight %}



### disable()
{:#methods:disable}


Disables the DateRangePicker control.

#### Example



{% highlight html %}
 
<input type="text" id="daterangepicker" />
<script>
$("#daterangepicker").ejDateRangePicker();
// Create DateRangePicker instance
var dateObj = $("#daterangepicker").data("ejDateRangePicker");
dateObj.disable(); // disables the daterangepicker
</script>

{% endhighlight %}


{% highlight html %}
 
<input type="text" id="daterangepicker" />
<script>
$("#daterangepicker").ejDateRangePicker();
// disables the daterangepicker
$("#daterangepicker").ejDateRangePicker("disable");
</script>

{% endhighlight %}







### enable()
{:#methods:enable}

Enable the DateRangePicker control, if it is in disabled state.





#### Example



{% highlight html %}
 
<input type="text" id="daterangepicker" />
<script>
$("#daterangepicker").ejDateRangePicker();
// Create DateRangePicker instance
var dateObj = $("#daterangepicker").data("ejDateRangePicker");
dateObj.enable(); // enables the daterangepicker
</script>{% endhighlight %}


{% highlight html %}
 
<input type="text" id="daterangepicker" />
<script>
$("#daterangepicker").ejDateRangePicker();
// enables the DateRangePicker
$("#daterangepicker").ejDateRangePicker("enable");
</script>

{% endhighlight %}






### getSelectedRange()
{:#methods:getSelectedRange}




Returns the startDate and endDate values in the selected ranges in the DateRangePicker control.





#### Returns:


Object


#### Example



{% highlight html %}
 
<input type="text" id="daterangepicker" />
<script>
$("#daterangepicker").ejDateRangePicker();
// Create DateRangePicker instance
var dateObj = $("#daterangepicker").data("ejDateRangePicker");
dateObj.getSelectedRange(); // returns the start and end date values
</script>

{% endhighlight %}


{% highlight html %}
 
<input type="text" id="daterangepicker" />
<script>
// returns the start and end date values
$("#daterangepicker").ejDateRangePicker();
$("#daterangepicker").ejDateRangePicker("getSelectedRange");
</script>

{% endhighlight %}







### popupHide()
{:#methods:popupHide}








Close the DateRangePicker popup, if it is in opened state.





#### Example



{% highlight html %}
 
<input type="text" id="daterangepicker" />
<script>
$("#daterangepicker").ejDateRangePicker();
// Create DateRangePicker instance
var dateObj = $("#daterangepicker").data("ejDateRangePicker");
dateObj.popupHide(); // hides the DateRangePicker popup
</script>

{% endhighlight %}


{% highlight html %}
 
<input type="text" id="daterangepicker" />
<script>
$("#daterangepicker").ejDateRangePicker();
// hides the DateRangePicker popup
$("#daterangepicker").ejDateRangePicker("popupHide");
</script>

{% endhighlight %}







### popupShow()
{:#methods:popupShow}








Opens the DateRangePicker popup.





#### Example



{% highlight html %}
 
<input type="text" id="daterangepicker" />
<script>
$("#daterangepicker").ejDateRangePicker();
// Create DateRangePicker instance
var dateObj = $("#daterangepicker").data("ejDateRangePicker");
dateObj.popupShow(); // shows the DateRangePicker popup
</script>

{% endhighlight %}


{% highlight html %}
 
<input type="text" id="daterangepicker" />
<script>
$("#daterangepicker").ejDateRangePicker();
// shows the DateRangePicker popup
$("#daterangepicker").ejDateRangePicker("popupShow");
</script>

{% endhighlight %}





### setRange()
{:#methods:setRange}




set the preset ranges to DateRangePicker popup. 

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
label</td>
<td class="type"><span class="param-type">string | array</span></td>
<td class="description">Display name | array of start date and end date</td>
</tr>

</tbody>
</table>





#### Example



{% highlight html %}
 
<input type="text" id="daterangepicker" />
<script>
$("#daterangepicker").ejDateRangePicker();
// Create DateRangePicker instance
var dateObj = $("#daterangepicker").data("ejDateRangePicker");
dateObj.setRange("new Range"); //set the preset ranges to DateRangePicker
</script>

{% endhighlight %}


{% highlight html %}
 
<input type="text" id="daterangepicker" />
<script>
$("#daterangepicker").ejDateRangePicker();
// Create DateRangePicker instance
var dateObj = $("#daterangepicker").data("ejDateRangePicker");
dateObj.setRange([new Date("11/12/2011"), new Date("11/12/2019")]); //set the predefined set of range DateRangePicker
</script>

{% endhighlight %}

## Events


### beforeClose
{:#events:beforeclose}


Fires before closing the DateRangePicker popup.

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
<td class="name">cancel</td>
<td class="type"><span class="param-type">boolean</span></td>
<td class="description">Set to true when the event has to be canceled, else false.</td>
</tr>
<tr>
<td class="name">
model</td>
<td class="type"><ts ref="ej.DateRangePicker.Model"/><span class="param-type">object</span></td>
<td class="description">returns the DateRangePicker model</td>
</tr>
<tr>
<td class="name">
type</td>
<td class="type"><span class="param-type">string</span></td>
<td class="description">returns the name of the event.</td>
</tr>
<tr>
<td class="name">
events</td>
<td class="type"><span class="param-type">object</span></td>
<td class="description">returns the event parameters from DateRangePicker.</td>
</tr>
<tr>
<td class="name">
element </td>
<td class="type"><span class="param-type">Element</span></td>
<td class="description">returns the DateRangePicker popup.</td>
</tr>
</tbody>
</table>




#### Example



{% highlight html %}
 
<input type="text" id="daterangepicker" />
<script>
//beforeClose event for DateRangePicker
$("#daterangepicker").ejDateRangePicker({
   beforeClose: function (args) {}
});  
</script>

{% endhighlight %}


### beforeOpen
{:#events:beforeopen}


Fires before opening the DateRangePicker popup.

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
<td class="description">Set to true when the event has to be canceled, else false.</td>
</tr>
<tr>
<td class="name">
model</td>
<td class="type"><ts ref="ej.DateRangePicker.Model"/><span class="param-type">object</span></td>
<td class="description">returns the DateRangePicker model.</td>
</tr>
<tr>
<td class="name">
type</td>
<td class="type"><span class="param-type">string</span></td>
<td class="description">returns the name of the event.</td>
</tr>
<tr>
<td class="name">
events</td>
<td class="type"><span class="param-type">object</span></td>
<td class="description">returns the event parameters from DateRangePicker.</td>
</tr>
<tr>
<td class="name">
element</td>
<td class="type"><span class="param-type">Element</span></td>
<td class="description">returns the DateRangePicker popup.</td>
</tr>
</tbody>
</table>




#### Example



{% highlight html %}
 
<input type="text" id="daterangepicker" />
<script>
//beforeOpen event for DateRangePicker
$("#daterangepicker").ejDateRangePicker({
   beforeOpen: function (args) {}
});  
</script>

{% endhighlight %}



### Change
{:#events:change}


Fires when the DateRangePicker values get changed.

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
model</td>
<td class="type"><ts ref="ej.DateRangePicker.Model"/><span class="param-type">object</span></td>
<td class="description">returns the DateRangePicker model.</td>
</tr>
<tr>
<td class="name">
type</td>
<td class="type"><span class="param-type">string</span></td>
<td class="description">returns the name of the event.</td>
</tr>
<tr>
<td class="name">
value</td>
<td class="type"><span class="param-type">string</span></td>
<td class="description">returns the DateRangePicker input value.</td>
</tr>
<tr>
<td class="name">
startDate</td>
<td class="type"><span class="param-type">object</span></td>
<td class="description">returns the startDate of DateRangePicker.</td>
</tr>
<tr>
<td class="name">
endDate</td>
<td class="type"><span class="param-type">object</span></td>
<td class="description">returns the endDate of the DateRangePicker popup.</td>
</tr>
</tbody>
</table>




#### Example



{% highlight html %}
 
<input type="text" id="daterangepicker" />
<script>
//Change event for DateRangePicker
$("#daterangepicker").ejDateRangePicker({
   change: function (args) {}
});  
</script> 

{% endhighlight %}







### close
{:#events:close}


Fires when DateRangePicker popup is closed.

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
date</td>
<td class="type"><span class="param-type">object</span></td>
<td class="description">returns the current date object.</td>
</tr>
<tr>
<td class="name">
model</td>
<td class="type"><ts ref="ej.DateRangePicker.Model"/><span class="param-type">object</span></td>
<td class="description">returns the DateRangePicker model.</td>
</tr>
<tr>
<td class="name">
type</td>
<td class="type"><span class="param-type">string</span></td>
<td class="description">returns the name of the event.</td>
</tr>
<tr>
<td class="name">
element</td>
<td class="type"><span class="param-type">Element</span></td>
<td class="description">returns the DateRangePicker popup.</td>
</tr>
</tbody>
</table>




#### Example



{% highlight html %}
 
<input type="text" id="daterangepicker" />
<script>
//close event for DateRangePicker
$("#daterangepicker").ejDateRangePicker({
   close: function (args) {}
});   
</script>

{% endhighlight %}







### create
{:#events:create}


Fires when the DateRangePicker is created successfully.

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
model</td>
<td class="type"><ts ref="ej.DateRangePicker.Model"/><span class="param-type">object</span></td>
<td class="description">returns the DateRangePicker model.</td>
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
 
<input type="text" id="daterangepicker" />
<script>
//create event for DateRangePicker
$("#daterangepicker").ejDateRangePicker({
   create: function (args) {}
});
</script>

{% endhighlight %}


### destroy
{:#events:destroy}


Fires when the DateRangePicker is destroyed successfully.

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
<td class="description">Set to true when the event has to be canceled, else false.</td>
</tr>
<tr>
<td class="name">
model</td>
<td class="type"><ts ref="ej.DateRangePicker.Model"/><span class="param-type">object</span></td>
<td class="description">returns the DateRangePicker model.</td>
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
 
<input type="text" id="daterangepicker" />
<script>
//destroy event for DateRangePicker
$("#daterangepicker").ejDateRangePicker({
   destroy: function (args) {}
}); 
</script>

{% endhighlight %}


### open
{:#events:open}


Fires when DateRangePicker popup is opened.

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
date</td>
<td class="type"><span class="param-type">object</span></td>
<td class="description">returns the current date object.</td>
</tr>
<tr>
<td class="name">
model</td>
<td class="type"><ts ref="ej.DateRangePicker.Model"/><span class="param-type">object</span></td>
<td class="description">returns the DateRangePicker model.</td>
</tr>
<tr>
<td class="name">
type</td>
<td class="type"><span class="param-type">string</span></td>
<td class="description">returns the name of the event</td>
</tr>
<tr>
<td class="name">
element</td>
<td class="type"><span class="param-type">Element</span></td>
<td class="description">returns the DateRangePicker popup.</td>
</tr>
</tbody>
</table>




#### Example



{% highlight html %}
 
<input type="text" id="daterangepicker" />
<script>
//open event for DateRangePicker
$("#daterangepicker").ejDateRangePicker({
   open: function (args) {}
});  
</script>

{% endhighlight %}







### select
{:#events:select}


Fires when a date ranges is selected from the DateRangePicker popup.

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
startDate</td>
<td class="type"><span class="param-type">object</span></td>
<td class="description">returns the selected date object.</td>
</tr>
<tr>
<td class="name">
model</td>
<td class="type"><ts ref="ej.DateRangePicker.Model"/><span class="param-type">object</span></td>
<td class="description">returns the DateRangePicker model.</td>
</tr>
<tr>
<td class="name">
type</td>
<td class="type"><span class="param-type">string</span></td>
<td class="description">returns the name of the event.</td>
</tr>
<tr>
<td class="name">
endDate</td>
<td class="type"><span class="param-type">object</span></td>
<td class="description">returns the current date value.</td>
</tr>
</tbody>
</table>




#### Example



{% highlight html %}
 
<input type="text" id="daterangepicker" />
<script>
//select event for DateRangePicker
$("#daterangepicker").ejDateRangePicker({
   select: function (args) {}
}); 
</script>


{% endhighlight %}




