---
layout: post
title: Properties,Methods and Events of Essential JS ejComboBox Widget
description: Methods, members, events available in ejComboBox
documentation: API
platform: js-api
keywords: ejComboBox, API, Essential JS ComboBox 
---

# ejComboBox

The ComboBox component allows the user to type a value or choose an option from the list of predefined options.

#### Syntax

{% highlight javascript %}
		
	$(element).ejComboBox()

{% endhighlight %}

#### Example

{% highlight html %}
		
	<input type="text" id="combobox" /> 
	<script> 
	// Create ComboBox 
	$('#ComboBox').ejComboBox({ 
		dataSource: window.carList,
		value:"Austin-Healey" 
	}); 
	</script>

{% endhighlight %}

#### Requires

* module:jQuery

* module:ej.core.js

* module:ej.data.js

* module:ej.globalize.js

* module:ej.combobox.js


## Members

### actionFailureTemplate `string`
{:#members:actionfailuretemplate}

Accepts the template and assigns it to the popup list content of the component when the data fetch request from the remote server fails.

#### Default Value:

* "The Request Failed"

#### Example

{% highlight javascript %}

	$("#combobox").ejComboBox({ 
		dataSource: window.carList,  
		actionFailureTemplate:"Data Not Load" 
	});

{% endhighlight %}

### allowCustom `boolean`
{:#members:allowcustom}

Specifies whether the component allows user defined value which does not exist in data source.

#### Default Value: 
* true

#### Example 

{% highlight javascript %}

	$("#combobox").ejComboBox({ 
		allowCustom: false 
	});

{% endhighlight %}

### allowFiltering `boolean`
{:#members:allowfiltering}

When allowFiltering is set to true, show the filter bar (search box) of the component. The filter action retrieves matched items through the filtering event based on the characters typed in the search TextBox. If no match is found, the value of the noRecordsTemplate property will be displayed. 

#### Default Value: 

* false

#### Example 
{% highlight html %}

	<input type="text" tabindex="1" id="list"> </input>

{% endhighlight %}

{% highlight javascript %}
var searchData = [ {id: 's1', country: 'California'}, {id: 's2', country: 'India'},
{id: 's3', country: 'USA'}, {id: 's4', country: 'England'}]
  $("#list").ejComboBox({ 
     dataSource: searchData,
     fields: { text: "country", value: "id" },
     allowFiltering: true,
     filtering: function (e) {
         let query = new Query();
         query = (e.text != "") ? query.where("country", "startswith", e.text, true) : query;
         e.updateData(searchData, query);
     }
  });

{% endhighlight %}

### autofill `boolean`
{:#members:autofill}

Specifies whether suggest a first matched item in input when searching. No action happens when no matches found.

#### Default Value: 

* false

#### Example 

{% highlight javascript %}

	$("#combobox").ejComboBox({ 
		autofill: true
	});

{% endhighlight %}

### cssClass `string`
{:#members:cssclass}

Sets CSS classes to the root element of the component that helps customize the UI styles. 

#### Default Value: 

* null

#### Example 

{% highlight javascript %}
<style type="text/css">
   .gradient-green {
       font-family: cursive;
   }
</style>
</script>
	$("#combobox").ejComboBox({ 
		cssClass: 'gradient-lime' 
	});
</script>
{% endhighlight %}

### dataSource `Object|Array`
{:#members:datasource}

Accepts the list items either through local or remote service and binds it to the component. It can be an array of JSON objects or an instance of DataManager.

#### Default Value: 

* []

#### Example 

{% highlight javascript %}

	$("#combobox").ejComboBox({ 
		dataSource: window.carList, 
		value: "Austin-Healey" 
	});

{% endhighlight %}

### enableRtl `boolean`
{:#members:enablertl}

When set to true, enables RTL mode of the component that displays the content in the right-to-left direction.

#### Default Value: 

* false

#### Example 

{% highlight javascript %}

	$("#combobox").ejComboBox({
		enableRtl: true 
	});

{% endhighlight %}

### enabled `boolean`
{:#members:enabled}

Specifies a value that indicates whether the component is enabled or not.

#### Default Value: 

* true

#### Example 

{% highlight javascript %}

	$("#combobox").ejComboBox({
		enabled: false 
	});

{% endhighlight %}

### fields `Object`
{:#members:fields}

The fields property maps the columns of the data table and binds the data to the component.


### fields.groupBy `string`
{:#members:fields-groupby}

Used to group the popup list items.

#### Default Value:

* null

### fields.iconCss `string`
{:#members:fields-iconcss}

Defines class for the item.

#### Default Value:

* null

### fields.value `string`
{:#members:fields-value}

Defines the specific field name which contains unique values for the list items.

#### Default Value:

* null

### fields.text `string`
{:#members:fields-text}

Defines the specific field name in the data source to load the popup list with data.

#### Default Value:

* null

#### Example 

{% highlight javascript %}

	$("#combobox").ejComboBox({ 
		fields: { 
			text: "name", 
			value: "id" 
		} 
	});

{% endhighlight %}


### footerTemplate `string`
{:#members:footertemplate}

Accepts the template design and assigns it to the footer container of the popup list.

#### Default Value:  

* null

#### Example  

{% highlight javascript %}

	$("#combobox").ejComboBox({
		footerTemplate: '<div class="Foot"> Total Items Count: 5 </div>'
	});

{% endhighlight %}

### groupTemplate `string`
{:#members:grouptemplate}

Accepts the template design and assigns it to the group headers present in the popup list.

#### Default Value:  

* null

#### Example  

{% highlight javascript %}

	$("#combobox").ejComboBox({
		groupTemplate: '<div class="group"> Contact Info </div>'
	});

{% endhighlight %}

### headerTemplate `string`
{:#members:headertemplate}

Accepts the template design and assigns it to the header container of the popup list.

#### Default Value:  

* null

#### Example  

{% highlight javascript %}

	$("#combobox").ejComboBox({ 
		headerTemplate: '<div class="head">  Photo  <span style="padding-left:42px"> Contact Info </span></div>'
	});

{% endhighlight %}

### htmlAttributes `object`
{:#members:htmlattributes}

Allows additional HTML attributes such as title, name, etc., and accepts n number of attributes in a key-value pair format.

#### Default Value:  

* {}

#### Example  

{% highlight javascript %}

	$("#combobox").ejComboBox({ 
		htmlAttributes: { title: 'List of games available here.' }
	});

{% endhighlight %}

### index `number`
{:#members:index}

Gets or sets the index of the selected item in the component.

#### Default Value:  

* null

#### Example 

{% highlight javascript %}

    $("#combobox").ejComboBox({index: 1});

{% endhighlight %}

### itemTemplate `string`
{:#members:itemtemplate}

Accepts the template design and assigns it to each list item present in the popup.

#### Default Value:  

* null

#### Example  

{% highlight javascript %}

	$("#combobox").ejComboBox({ 
		itemTemplate: '<div><img class="eimg" src="${eimg}.png" alt="employee"/>' +
                    '<div class="ename"> ${text} </div><div class="temp"> ${country} </div></div>'
	});

{% endhighlight %}

### locale `string`
{:#members:locale}

Overrides the global culture and localization value for this component. Default global culture is 'en-US'.

#### Default Value:  

* "en-US"

#### Example 

{% highlight javascript %}

    $("#combobox").ejComboBox({ 
		locale: "es-ES"
	});

{% endhighlight %}

### noRecordsTemplate `string`
{:#members:norecordstemplate}

Accepts the template design and assigns it to popup list of component when no data is available on the component.

#### Default Value:

* No Records Found


#### Example 

{% highlight javascript %}

	$("#combobox").ejComboBox({ 
		noRecordsTemplate:"Data Not Found"
	});

{% endhighlight %}

### placeholder `string`
{:#members:placeholder}

Accepts the value to be displayed as a watermark text on the component input.

#### Default Value:

* null


#### Example 

{% highlight javascript %}

	$("#combobox").ejComboBox({ 
		placeholder:"Select text"
	});

{% endhighlight %}

### popupHeight `string|number`
{:#members:popupheight}

Specifies the height of the popup list.

#### Default Value:

* "300px"

#### Example 

{% highlight javascript %}

	$("#combobox").ejComboBox({ 
		popupHeight: "400px"
	});

{% endhighlight %}

### popupWidth `string|number`
{:#members:popupwidth}

Specifies the width of the popup list. By default, the popup width sets based on the width of the component.

#### Default Value:

* "100%"

#### Example 

{% highlight javascript %}

	$("#combobox").ejComboBox({ 
		popupWidth: "300px"
	});

{% endhighlight %}

### query `ej.Query`
{:#members:query}

The query to retrieve the data from the data source.

#### Default Value:   

* null

#### Example  

{% highlight javascript %}

	var dataManger = ej.DataManager({ 
		url: "http://mvc.syncfusion.com/Services/Northwnd.svc/" 
	});
	
	var query = ej.Query().from("Suppliers").select("ContactName");
	
	$("#combobox").ejComboBox({ 
		dataSource: dataManger, 
		query: query, 
		fields: { 
			text: "ContactName" 
		}
	});

{% endhighlight %}

### readonly `boolean`
{:#members:readonly}

When set to true, the user interactions on the component are disabled.

#### Default Value:
* false

#### Example 

{% highlight javascript %}

	$("#combobox").ejComboBox({ 
    	readonly: true
	});

{% endhighlight %}


### showClearButton `boolean`
{:#members:showClearButton}

Specifies whether to show or hide the clear button. When the clear button is clicked, value, text, and index properties are reset to null. 

#### Default Value:
* true

#### Example
{:.example}


{% highlight html %}
 $("#combobox").ejComboBox({ 
	 	showClearButton:true
	});
{% endhighlight %}

### sortOrder `enum`
{:#members:sortorder}

<ts name = "ej.ComboBox.SortOrder"/>

Specifies the sortOrder to sort the data source. The available type of sort orders are 

<table>
<tr>
<th>Name<br/></th>
<th>Description<br/></th>
</tr>
<tr>
<td>None<br/></td>
<td>The data source is not sorting.<br/></td>
</tr>
<tr>
<td>Ascending<br/></td>
<td>The data source is sorting with ascending order.<br/></td>
</tr>
<tr>
<td>Descending<br/></td>
<td>The data source is sorting with descending order.<br/></td>
</tr>
</table>


#### Default Value:  

* ej.SortOrder.None

#### Example  

{% highlight javascript %}

	$("#combobox").ejComboBox({ 
		sortOrder: ej.SortOrder.Decending 
	});

{% endhighlight %}

### text `string`
{:#members:text}

Gets or sets the display text of the selected item in the component.

#### Default Value:  
* null

#### Example 

{% highlight javascript %}

	$("#combobox").ejComboBox({ 
		dataSource: window.carList, 
		text: "Austin-Healey"
	});

{% endhighlight %}

### value `number|string`
{:#members:value}

Gets or sets the value of the selected item in the component.

#### Default Value:
* null

#### Example 

{% highlight javascript %}

	$("#combobox").ejComboBox({ 
		dataSource: window.carList, 
		value: "Austin-Healey"
	});

{% endhighlight %}

### width `number|string`
{:#members:width}

Specifies the width of the component. By default, the component width sets based on the width of its parent container. You can also set the width in pixel values.

#### Default Value:
* "100%"

#### Example 

{% highlight javascript %}

	$("#combobox").ejComboBox({ 
		width: "300px"
	});

{% endhighlight %}


## Methods

### addItem()
{:#methods:additem}

Adds a new item to the popup list. By default, new item appends to the list as the last item, but you can insert based on the index parameter.

<table>
<tr>
<th>Name<br/></th>
<th>Type<br/></th>
<th>Description<br/></th>
</tr>
<tr>
<td>items<br/></td>
<td>[] | Object<br/></td>
<td>Specifies an array of JSON data or a JSON data.<br/></td>
</tr>
<tr>
<td>itemIndex (optional)<br/></td>
<td>number<br/></td>
<td>Specifies the index to place the newly added item in the popup list.<br/></td>
</tr>
</table>

#### Returns: void

#### Example  

{% highlight javascript %}

	$("#combobox").ejComboBox("addItem",{ id: 'level11', sports: 'cricket' });

{% endhighlight %}

### focusIn()
{:#methods:focusin}

Sets the focus to the component for interaction.

#### Returns: void

#### Example  

{% highlight javascript %}

	$("#combobox").ejComboBox("focusIn");

{% endhighlight %}

### focusOut()
{:#methods:focusout}

Moves the focus from the component if the component is already focused.

#### Returns: void

#### Example  

{% highlight javascript %}

	$("#combobox").ejComboBox("focusOut");

{% endhighlight %}

### getDataByValue()
{:#methods:getdatabyvalue}

Gets the data object that matches the given value.

<table>
<tr>
<th>Name<br/></th>
<th>Type<br/></th>
<th>Description<br/></th>
</tr>
<tr>
<td>value<br/></td>
<td>string | number<br/></td>
<td>Specifies the value of the list item.<br/></td>
</tr>
</table>

#### Returns: object

#### Example  

{% highlight javascript %}

	$("#combobox").ejComboBox("getDataByValue","value");

{% endhighlight %}

### getItems()
{:#methods:getitems}

Gets all the list items bound on this component.

#### Returns: Element[]

#### Example  

{% highlight javascript %}

	$("#combobox").ejComboBox("getItems");

{% endhighlight %}

### hidePopup()
{:#methods:hidepopup}

Hides the popup if it is in open state.

#### Returns: void

#### Example  

{% highlight javascript %}

	$("#combobox").ejComboBox("hidePopup");

{% endhighlight %}

### showPopup()
{:#methods:showpopup}

Opens the popup that displays the list of items.

#### Returns: void

#### Example  

{% highlight javascript %}

	$("#combobox").ejComboBox("showPopup");

{% endhighlight %}


## Events

### actionBegin
{:#events:actionBegin}

Triggers before fetching data from the remote server.

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
<td class="name">cancel</td>
<td class="type"><span class="param-type">boolean</span></td>
<td class="description last">if the event should be canceled; otherwise, false.</td>
</tr>
<tr>
<td class="name">model</td>
<td class="type"><span class="param-type">object</span></td>
<td class="description last">returns the ComboBox model</td>
</tr>
<tr>
<td class="name">type</td>
<td class="type"><span class="param-type">string</span></td>
<td class="description last">returns the name of the event</td>
</tr>
</tbody>
</table>

 N>  It internally uses jQuery ajaxStart event. For details refer [here](http://api.jquery.com/ajaxStart/#).

#### Example

{% highlight javascript %}

	$("#combobox").ejComboBox({
		actionBegin:function(arg){
			//Action Success Code
		} 
	});

{% endhighlight %}


### actionComplete
{:#events:actioncomplete}

Triggers after data is fetched successfully from the remote server.

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
<td class="description">if the event should be canceled; otherwise, false.</td>
</tr>
<tr>
<td class="name">model</td>
<td class="type"><span class="param-type">object</span></td>
<td class="description">returns the Autocomplete model</td>
</tr>
<tr>
<td class="name">e</td>
<td class="type"><span class="param-type">object</span></td>
<td class="description">Returns the query for data retrieval from the Database </td>
</tr>
<tr>
<td class="name">type</td>
<td class="type"><span class="param-type">string</span></td>
<td class="description">returns the name of the event</td>
</tr>
</tbody>
</table>

N> It internally uses jQuery ajaxComplete event. For details refer [here](http://api.jquery.com/ajaxcomplete/#).

#### Example

{% highlight javascript %}

	$("#combobox").ejComboBox({
		actionComplete:function(arg){
			//Action Complete Code
		} 
	});

{% endhighlight %}

### actionFailure
{:#events:actionfailure}

Triggers when the data fetch request from the remote server fails.

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
<td class="description">if the event should be canceled; otherwise, false.</td>
</tr>
<tr>
<td class="name">e</td>
<td class="type"><span class="param-type">object</span></td>
<td class="description">Returns the error message</td>
</tr>
<tr>
<td class="name">model</td>
<td class="type"><span class="param-type">object</span></td>
<td class="description">returns the Autocomplete model</td>
</tr>
<tr>
<td class="name">type</td>
<td class="type"><span class="param-type">string</span></td>
<td class="description">returns the name of the event</td>
</tr>
</tbody>
</table>

 N>  It internally uses jQuery ajaxError event. For details refer [here](http://api.jquery.com/ajaxerror/#).

#### Example

{% highlight javascript %}

	$("#combobox").ejComboBox({
		actionFailure:function(arg){
			//Action Failure Code
		} 
	});

{% endhighlight %}

### change
{:#events:change}

Triggers when an item in a popup is selected or when the model value is changed.

<table>
<tr>
<th>Name<br/></th>
<th>Type<br/></th>
<th>Description<br/></th>
</tr>
<tr>
<td>cancel<br/></td>
<td>boolean<br/></td>
<td>Set this option to true to cancel the event.<br/></td>
</tr>
<tr>
<td>model<br/></td>
<td><ts ref="ej.ComboBox.Model"/>Object<br/></td>
<td>Instance of the combobox model object.<br/></td>
</tr>
<tr>
<td>type<br/></td>
<td>string<br/></td>
<td>Name of the event.<br/></td>
</tr>
<tr>
<td>value<br/></td>
<td>string|number<br/></td>
<td>Value of the combobox textbox.<br/></td>
</tr>
<td>itemData<br/></td>
<td><ts ref="ej.ComboBox.Model"/>Object<br/></td>
<td>Data object of the selected item.<br/></td
></tr>
<tr>
<td>Item<br/></td>
<td>Object<br/></td>
<td>Li element of the selected item.<br/></td>
</tr>
<tr>
<td>e<br/></td>
<td>Object<br/></td>
<td>Event argument.<br/></td>
</tr>
<tr>
<td>isInteracted<br/></td>
<td>boolean<br/></td>
<td>value of the interaction<br/></td>
</tr>
</table>

#### Example  

{% highlight javascript %}

	$("#combobox").ejComboBox({
		change: function (argument) {
			//do something
		}
	}); 

{% endhighlight %}

### close
{:#events:close}

Triggers when the popup is closed.

<table>
<tr>
<th>Name<br/></th>
<th>Type<br/></th>
<th>Description<br/></th>
</tr>
<tr>
<td>popup<br/></td>
<td>object<br/></td>
<td>Element of the combobox popup list<br/></td>
</tr>
</table>

#### Example  

{% highlight javascript %}

	$("#combobox").ejComboBox({ 
		close: function (argument) {
			//do something
		}
	});

{% endhighlight %}

### create
{:#events:create}

Triggers when ComboBox widget is created.

<table>
<tr>
<th>Name<br/></th>
<th>Type<br/></th>
<th>Description<br/></th>
</tr>
<tr>
<td>cancel<br/></td>
<td>boolean<br/></td>
<td>Set this option to true to cancel the event.<br/></td>
</tr>
<tr>
<td>model<br/></td>
<td><ts ref="ej.ComboBox.Model"/>Object<br/></td>
<td>Instance of the combobox model object.<br/></td>
</tr>
<tr>
<td>type<br/></td>
<td>string<br/></td>
<td>Name of the event.<br/></td>
</tr>
</table>

#### Example  

{% highlight javascript %}

	$("#combobox").ejComboBox({
		create: function (argument) {
			//do something
		}
	});

{% endhighlight %}

### customValueSpecifier
{:#events:customvaluespecifier}

Triggers on set a custom value to this component.

<table>
<tr>
<th>Name<br/></th>
<th>Type<br/></th>
<th>Description<br/></th>
</tr>
<tr>
<td>model<br/></td>
<td><ts ref="ej.ComboBox.Model"/>Object<br/></td>
<td>Instance of the combobox model object.<br/></td>
</tr>
<tr>
<td>type<br/></td>
<td>string<br/></td>
<td>Name of the event.<br/></td>
</tr>
<tr>
<td>text<br/></td>
<td>string<br/></td>
<td>text of the combobox.<br/></td>
</tr>
</table>

#### Example  

{% highlight javascript %}

	$("#combobox").ejComboBox({
		customValueSpecifier: function (argument) {
			//do something
		}
	});

{% endhighlight %}

### filtering
{:#events:filtering}

Triggers on typing a character in the component.

<table>
<tr>
<th>Name<br/></th>
<th>Type<br/></th>
<th>Description<br/></th>
</tr>
<tr>
<td>model<br/></td>
<td><ts ref="ej.ComboBox.Model"/>Object<br/></td>
<td>Instance of the combobox model object.<br/></td>
</tr>
<tr>
<td>type<br/></td>
<td>string<br/></td>
<td>Name of the event.<br/></td>
</tr>
<tr>
<td>text<br/></td>
<td>string<br/></td>
<td>text of the combobox.<br/></td>
</tr>
<tr>
<td>updateData<br/></td>
<td>function<br/></td>
<td>Function used to update the filtering value.<br/></td>
</tr>
</table>

#### Example  

{% highlight javascript %}

	$("#combobox").ejComboBox({
		filtering: function (argument) {
			//do something
		}
	});

{% endhighlight %}

### focus
{:#events:focus}

Triggers when the component is focused.

<table>
<tr>
<th>Name<br/></th>
<th>Type<br/></th>
<th>Description<br/></th>
</tr>
<tr>
<td>cancel<br/></td>
<td>boolean<br/></td>
<td>Set this option to true to cancel the event.<br/></td>
</tr>
<tr>
<td>model<br/></td>
<td><ts ref="ej.ComboBox.Model"/>Object<br/></td>
<td>Instance of the combobox model object.<br/></td>
</tr>
<tr>
<td>type<br/></td>
<td>string<br/></td>
<td>Name of the event.<br/></td>
</tr>
</table>

#### Example  

{% highlight javascript %}

	$("#combobox").ejComboBox({
		focus: function () {
			//do something
		}
	});

{% endhighlight %}

### open
{:#events:open}

Triggers after the suggestion list is opened.

<table>
<tr>
<th>Name<br/></th>
<th>Type<br/></th>
<th>Description<br/></th>
</tr>
<tr>
<td>popup<br/></td>
<td>object<br/></td>
<td>Element of the combobox popup list<br/></td>
</tr>
</table>

#### Example  

{% highlight javascript %}

	$("#combobox").ejComboBox({  
		open: function (argument) {
			//do something
		}
	});

{% endhighlight %}

### select
{:#events:select}

Triggers when an item in the popup is selected.

<table>
<tr>
<th>Name<br/></th>
<th>Type<br/></th>
<th>Description<br/></th>
</tr>
<tr>
<td>cancel<br/></td>
<td>boolean<br/></td>
<td>Set this option to true to cancel the event.<br/></td>
</tr>
<tr>
<td>model<br/></td>
<td><ts ref="ej.ComboBox.Model"/>Object<br/></td>
<td>Instance of the combobox model object.<br/></td>
</tr>
<tr>
<td>type<br/></td>
<td>string<br/></td>
<td>Name of the event.<br/></td>
</tr>
<tr>
<td>value<br/></td>
<td>string|number<br/></td>
<td>Value of the combobox textbox.<br/></td>
</tr>
<tr>
<td>text<br/></td>
<td>string<br/></td>
<td>Text of the selected item.<br/></td>
</tr>
<tr>
<td>itemData<br/></td>
<td><ts ref="ej.ComboBox.Model"/>Object<br/></td>
<td>Data object of the selected item.<br/></td
></tr>
<tr>
<td>Item<br/></td>
<td>Object<br/></td>
<td>Li element of the selected item.<br/></td>
</tr>
<tr>
<td>e<br/></td>
<td>Object<br/></td>
<td>Event argument.<br/></td>
</tr>
<tr>
<td>isInteracted<br/></td>
<td>boolean<br/></td>
<td>value of the interaction<br/></td>
</tr>
</table>

#### Example  

{% highlight javascript %}

	$("#combobox").ejComboBox({
		select: function (argument) {
			//do something
		}
	});

{% endhighlight %}