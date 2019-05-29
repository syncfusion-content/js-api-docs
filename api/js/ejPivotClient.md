---
layout: post
title: Properties, Methods and Events of Syncfusion ejPivotClient Widget
description: Methods,members and events available in ejPivotClient
documentation: UG
platform: js-api
keywords: ejPivotClient, API, Essential JS PivotClient
metaname: API reference for ejPivotClient
metacontent: ejPivotClient, API, Essential JS PivotClient
---

# Pivot client

The pivot client is an ad hoc analysis tool that can be easily bound to any OLAP and relational datasources to provide a visual presentation of the information retrieved from the database.

#### Syntax

{% highlight javascript %}

    $(element).ejPivotClient()
{% endhighlight %}

#### Example

{% highlight html %}
 
    <div id="PivotClient1"></div>
 
    <script>
        //Create PivotClient
        $("#PivotClient1").ejPivotClient(...);     
    </script>
{% endhighlight %}

#### Requires

* module: jQuery-3.0.0.min.js
* module: ej.core.js
* module: ej.data.js
* module: ej.globalize.js
* module: ej.touch.js
* module: ej.draggable.js
* module: ej.scroller.js
* module: ej.chart.js
* module: ej.synchart.js
* module: ej.rangescrollbar.js
* module: ej.tooltip.js
* module: ej.button.js
* module: ej.checkbox.js
* module: ej.dropdownlist.js
* module: ej.dialog.js
* module: ej.togglebutton.js
* module: ej.toolbar.js
* module: ej.maskedit.js
* module: ej.waitingpopup.js
* module: ej.menu.js
* module: ej.treeview.js
* module: ej.tab.js
* module: ej.pivot.common.js
* module: ej.pivotanalysis.base.js
* module: ej.olap.base.js
* module: ej.pivotchart.js
* module: ej.pivottreemap.js
* module: ej.pivotpager.js
* module: ej.pivotgrid.js
* module: ej.pivotschemadesigner.js
* module: ej.pivotclient.js

## Members

### analysisMode `enum`
{:#members:analysisMode}

<ts ref = "ej.Pivot.AnalysisMode"/>

Sets the mode for the pivot client widget for binding the OLAP or relational data sources.

#### Default Value: ej.Pivot.AnalysisMode.Pivot

<table class="params">
    <thead>
        <tr>
            <th>Name</th>
            <th>Description</th>
        </tr>
    </thead>
    <tbody>
        <tr>
            <td class="name">Pivot</td>
            <td class="description">To bind Relational datasource to PivotClient widget</td>
        </tr>
        <tr>
            <td class="name">OLAP</td>
            <td class="description">To bind OLAP datasource to PivotClient widget</td>
        </tr>
    </tbody>
</table>

**Example:**

{% highlight javascript %}
 
    $("#PivotClient1").ejPivotClient({ analysisMode: ej.Pivot.AnalysisMode.Olap });
{% endhighlight %}

### chartType `enum`
{:#members:charttype}

<ts ref = "ej.PivotChart.ChartTypes"/>

Allows you to set the specific chart type for the pivot chart in the pivot client widget.

#### Default Value: ej.PivotChart.ChartTypes.Column

<table class="params">
    <thead>
        <tr>
            <th>Name</th>
            <th>Description</th>
        </tr>
    </thead>
    <tbody>
        <tr>
            <td class="name">Line</td>
            <td class="description">To render a Line type for PivotChart.</td>
        </tr>
        <tr>
            <td class="name">Spline</td>
            <td class="description">To render a Spline type for PivotChart.</td>
        </tr>
        <tr>
            <td class="name">Column</td>
            <td class="description">To render a Column type for PivotChart.</td>
        </tr>
        <tr>
            <td class="name">Area</td>
            <td class="description">To render an Area type for PivotChart.</td>
        </tr>
        <tr>
            <td class="name">SplineArea</td>
            <td class="description">To render a SplineArea type for PivotChart.</td>
        </tr>
        <tr>
            <td class="name">StepLine</td>
            <td class="description">To render a StepLine type for PivotChart.</td>
        </tr>
        <tr>
            <td class="name">StepArea</td>
            <td class="description">To render a StepArea type for PivotChart.</td>
        </tr>
        <tr>
            <td class="name">Pie</td>
            <td class="description">To render a Pie type for PivotChart.</td>
        </tr>
        <tr>
            <td class="name">Bar</td>
            <td class="description">To render a Bar type for PivotChart.</td>
        </tr>
        <tr>
            <td class="name">StackingArea</td>
            <td class="description">To render a StackingArea type for PivotChart.</td>
        </tr>
        <tr>
            <td class="name">StackingColumn</td>
            <td class="description">To render a StackingColumn type for PivotChart.</td>
        </tr>
        <tr>
            <td class="name">StackingBar</td>
            <td class="description">To render a StackingBar type for PivotChart.</td>
        </tr>
        <tr>
            <td class="name">Pyramid</td>
            <td class="description">To render a Pyramid type for PivotChart.</td>
        </tr>
        <tr>
            <td class="name">Funnel</td>
            <td class="description">To render a Funnel type for PivotChart.</td>
        </tr>
        <tr>
            <td class="name">Doughnut</td>
            <td class="description">To render a Doughnut type for PivotChart.</td>
        </tr>
        <tr>
            <td class="name">Scatter</td>
            <td class="description">To render a Scatter type for PivotChart.</td>
        </tr>
        <tr>
            <td class="name">Bubble</td>
            <td class="description">To render a Bubble type for PivotChart.</td>
        </tr>
    </tbody>
</table>


**Example:**

{% highlight javascript %}
 
    $("#PivotClient1").ejPivotClient({ chartType: ej.PivotChart.ChartTypes.Spline });
{% endhighlight %}

### clientExportMode `enum`
{:#members:clientExportMode}

<ts name = "ej.PivotClient.ClientExportMode"/>

Allows you to set the content for exporting the pivot client widget.

#### Default Value: ej.PivotClient.ClientExportMode.ChartAndGrid

<table class="params">
    <thead>
        <tr>
            <th>Name</th>
            <th>Description</th>
        </tr>
    </thead>
    <tbody>
        <tr>
            <td class="name">ChartAndGrid</td>
            <td class="description">Exports both the PivotChart and PivotGrid on exporting.</td>
        </tr>
        <tr>
            <td class="name">ChartOnly</td>
            <td class="description">Exports the PivotChart control alone on exporting.</td>
        </tr>
        <tr>
            <td class="name">GridOnly</td>
            <td class="description">Exports the PivotGrid control alone on exporting.</td>
        </tr>
    </tbody>
</table>


**Example:**

{% highlight javascript %}
 
    $("#PivotClient1").ejPivotClient({ clientExportMode: ej.PivotClient.ClientExportMode.ChartOnly });
{% endhighlight %}

### cssClass `string`
{:#members:cssclass}

Specifies the CSS class to the pivot client for achieving the custom theme.

#### Default Value: “”

**Example:**

{% highlight javascript %}
 
    $("#PivotClient1").ejPivotClient({ cssClass: "Olive" });
{% endhighlight %}

### customObject `object`
{:#members:customobject}

An object is utilized to pass the additional information between the client-end and the service-end when the control functions are present in the server-mode.

#### Default Value: {}

**Example:**

{% highlight javascript %}
 
    $("#PivotClient1").ejPivotClient({ customObject: { "MyMessage": "Hi Syncfusion!!" } });
{% endhighlight %}

### dataSource `object`
{:#members:datasource}

Initializes the data source for the pivot client widget, when it functions completely on the client-side.

#### Default Value: {}

**Example:**

{% highlight javascript %}
 
    $("#PivotClient1").ejPivotClient( { dataSource: { data: value } });
{% endhighlight %}

### dataSource.columns `array`
{:#members:datasource-columns}

Lists out the items to be arranged in the columns section of the pivot client.

#### Default Value: []

**Example:**

{% highlight javascript %}
 
    $("#PivotClient1").ejPivotClient({ dataSource: { columns: itemsArray } });
{% endhighlight %}


### dataSource.columns.fieldName `string`
{:#members:datasource-columns-fieldname}

Allows you to bind the item by using its unique name as field name.

#### Default Value: ""

**Example:**

{% highlight javascript %}
 
    $("#PivotClient1").ejPivotClient({ dataSource: { columns: [{ fieldName : "MyFieldName" }] } });
{% endhighlight %}

### dataSource.columns.fieldCaption `string`
{:#members:datasource-columns-fieldcaption}

Allows you to set the display caption for an item.

#### Default Value: ""

**Example:**

{% highlight javascript %}
 
    $("#PivotClient1").ejPivotClient({ dataSource: { columns: [{ fieldCaption : "MyFieldCaption" }] } });
{% endhighlight %}

### dataSource.columns.advancedFilter `array`
{:#members:datasource-columns-advancedfilter}

Allows you to filter the report by default using the advanced filtering (e.g., Microsoft Excel) option for the OLAP data source in the client-mode.

#### Default Value: []

**Example:**

{% highlight javascript %}
 
    $("#PivotClient1").ejPivotClient({ dataSource: { columns: [{ advancedFilter : itemArray }] } });
{% endhighlight %}

### dataSource.columns.advancedFilter.name `string`
{:#members:datasource-columns-advancedfilter-name}

Allows you to provide a level unique name to perform the advanced filtering.

#### Default Value: ""

**Example:**

{% highlight javascript %}
 
    $("#PivotClient1").ejPivotClient({ dataSource: { columns: [{ advancedFilter : [{ name: "levelUniqueName" }] }] } });
{% endhighlight %}

### dataSource.columns.advancedFilter.labelFilterOperator `string`
{:#members:datasource-columns-advancedfilter-labelfilteroperator}

Allows you to set the operator to perform label filtering.

#### Default Value: "none"

**Example:**

{% highlight javascript %}
 
    $("#PivotClient1").ejPivotClient({ dataSource: { columns: [{ advancedFilter : [{ labelFilterOperator: ej.olap.LabelFilterOptions.EndsWith }] }] } });
{% endhighlight %}

### dataSource.columns.advancedFilter.valueFilterOperator `string`
{:#members:datasource-columns-advancedfilter-valuefilteroperator}

Allows you to set the operator to perform value filtering.

#### Default Value: "none"

**Example:**

{% highlight javascript %}
 
    $("#PivotClient1").ejPivotClient({ dataSource: { columns: [{ advancedFilter : [{ valueFilterOperator: ej.olap.ValueFilterOptions.Between }] }] } });
{% endhighlight %}

### dataSource.columns.advancedFilter.advancedFilterType `string`
{:#members:datasource-columns-advancedfilter-advancedfiltertype}

Allows you to set the filtering type while performing the advanced filtering.

#### Default Value: ""

**Example:**

{% highlight javascript %}
 
    $("#PivotClient1").ejPivotClient({ dataSource: { columns: [{ advancedFilter : [{ advancedFilterType:  ej.olap.AdvancedFilterType.LabelFilter }] }] } });
{% endhighlight %}

### dataSource.columns.advancedFilter.measure `string`
{:#members:datasource-columns-advancedfilter-measure}

In value filtering, this property contains the measure name to which the filter is applied.

#### Default Value: ""

**Example:**

{% highlight javascript %}
 
    $("#PivotClient1").ejPivotClient({ dataSource: { columns: [{ advancedFilter : [{ measure: "measureUniqueName", advancedFilterType: ej.olap.AdvancedFilterType.ValueFilter }] }] } });
{% endhighlight %}

### dataSource.columns.advancedFilter.values `array`
{:#members:datasource-columns-advancedfilter-values}

Allows you to hold the filter operand values in the advanced filtering.

#### Default Value: ""

**Example:**

{% highlight javascript %}
    
    //For Label Filters
    $("#PivotClient1").ejPivotClient({ dataSource: { columns: [{ advancedFilter : [{ labelFilterOperator: ej.olap.LabelFilterOptions.EndsWith, values:  ["002"] }] }] } });
    
    //For Value Filters
    $("#PivotClient1").ejPivotClient({ dataSource: { columns: [{ advancedFilter : [{ valueFilterOperator: ej.olap.ValueFilterOptions.GreaterThan, values:  ["200"] }] }] } });
{% endhighlight %}


### dataSource.columns.isNamedSets `boolean`
{:#members:datasource-columns-isnamedsets}

Allows you to indicate whether the added item is a named set or not.

> **Note**: This is applicable only for the OLAP data source.

#### Default Value: false

**Example:**

{% highlight javascript %}
 
    $("#PivotClient1").ejPivotClient({ dataSource: { columns: [{ fieldName: "[Core Product Group]", isNamedSets : true }] } });
{% endhighlight %}

### dataSource.columns.showSubTotal `boolean`
{:#members:datasource-columns-showsubtotal}

Shows/hides the sub-total of the field in the pivot grid.

>**Note**: This is applicable only for the relational data source.

#### Default Value: true

**Example:**

{% highlight javascript %}
 
    $("#PivotClient1").ejPivotClient({ dataSource: { columns: [{ fieldName: "Country", showSubTotal : false }] } });
{% endhighlight %}

### dataSource.columns.format `string`
{:#members:datasource-columns-format}

Allows to set the format for the column headers.

>**Note**: This is applicable only for the relational data source.

#### Default Value: ""

**Example:**

{% highlight javascript %}
 
    $("#PivotClient1").ejPivotClient({ dataSource: { columns: [{ format : "date" }] } });
{% endhighlight %}

### dataSource.columns.formatString `string`
{:#members:datasource-columns-formatstring}

This property is set to display the formatted values with format types in the pivot grid.

#### Default Value: ""

**Example:**

{% highlight javascript %}
 
    $("#PivotClient1").ejPivotClient({ dataSource: { columns: [{ formatString : "MM/DD/YYYY" }] } });
{% endhighlight %}

### dataSource.columns.cssClass `string`
{:#members:datasource-columns-cssclass}

Allows you to set the custom theme for the column headers.

>**Note**: This is applicable only for the relational data source.

#### Default Value: ""

**Example:**

{% highlight javascript %}
 
    $("#PivotClient1").ejPivotClient({ dataSource: { columns: [{ cssClass : "className" }] } });
{% endhighlight %}

### dataSource.columns.sortOrder `enum`
{:#members:datasource-columns-sortorder}

<ts ref = "ej.PivotAnalysis.SortOrder"/>

Allows you to set the sorting order of members of the field.

>**Note**: This is applicable only for the relational data source.

#### Default Value: ej.PivotAnalysis.SortOrder.Ascending

<table class="params">
    <thead>
        <tr>
            <th>Name</th>
            <th>Description</th>
        </tr>
    </thead>
    <tbody>
        <tr>
            <td class="name">Ascending</td>
            <td class="description">Sorts the members of the field in ascending order.</td>
        </tr>
        <tr>
            <td class="name">Descending</td>
            <td class="description">Sorts the members of the field in descending order.</td>
        </tr>
        <tr>
            <td class="name">None</td>
            <td class="description">Displays the members without sorting in any order.</td>
        </tr>
    </tbody>
</table>

**Example:**

{% highlight javascript %}
 
    $("#PivotClient1").ejPivotClient({ dataSource: { columns: [{ fieldName: "Country", sortOrder : ej.PivotAnalysis.SortOrder.Descending }] } });
{% endhighlight %}

### dataSource.columns.drilledItems `array`
{:#members:datasource-columns-drilleditems}

Contains the list of members need to be drilled down by default in the field.

#### Default Value: []

**Example:**

{% highlight javascript %}
 
    $("#PivotClient1").ejPivotClient({ dataSource: { columns: [{ fieldName: "Country", drilledItems : ["Canada", "France"] }] } });
{% endhighlight %}

### dataSource.columns.filterItems `object`
{:#members:datasource-columns-filteritems}

Applies the filter to field members.

#### Default Value: null

**Example:**

{% highlight javascript %}
 
    $("#PivotClient1").ejPivotClient({ dataSource: { columns: [{ fieldName: "Country", filterItems : { filterType: ej.PivotAnalysis.FilterType.Exclude, values: ["Canada", "France"] } }] } });
{% endhighlight %}

### dataSource.columns.filterItems.filterType `enum`
{:#members:datasource-columns-filteritems-filtertype}

<ts ref = "ej.PivotAnalysis.FilterType"/>

Sets the type of filter whether to include/exclude the mentioned values.

>**Note**: This is applicable only for the relational data source.

#### Default Value: ej.PivotAnalysis.FilterType.Exclude

<table class="params">
    <thead>
        <tr>
            <th>Name</th>
            <th>Description</th>
        </tr>
    </thead>
    <tbody>
        <tr>
            <td class="name">Exclude</td>
            <td class="description">Excludes the specified values among the members of the field.</td>
        </tr>
        <tr>
            <td class="name">Include</td>
            <td class="description">Includes the specified values alone among the members of the field.</td>
        </tr>
    </tbody>
</table>

**Example:**

{% highlight javascript %}
 
    $("#PivotClient1").ejPivotClient({ dataSource: { columns: [{ fieldName: "Country", filterItems : { filterType: ej.PivotAnalysis.FilterType.Include, values: valueArray } }] } });
{% endhighlight %}

### dataSource.columns.filterItems.values `array`
{:#members:datasource-columns-filteritems-values}

Contains the collection of items to be included/excluded among the field members.

#### Default Value: []

**Example:**

{% highlight javascript %}
 
    $("#PivotClient1").ejPivotClient({ dataSource: { columns: [{ fieldName: "Country", filterItems : { filterType: ej.PivotAnalysis.FilterType.Exclude, values: ["Canada", "France"] } }] } });
{% endhighlight %}

### dataSource.rows `array`
{:#members:datasource-rows}

Lists out the items to be arranged in the rows section of the pivot client.

#### Default Value: []

**Example:**

{% highlight javascript %}
 
    $("#PivotClient1").ejPivotClient({ dataSource: { rows: itemsArray } });
{% endhighlight %}


### dataSource.rows.fieldName `string`
{:#members:datasource-rows-fieldname}

Allows you to bind the item by using its unique name as field name.

#### Default Value: ""

**Example:**

{% highlight javascript %}
 
    $("#PivotClient1").ejPivotClient({ dataSource: { rows: [{ fieldName : "MyFieldName" }] } });
{% endhighlight %}

### dataSource.rows.fieldCaption `string`
{:#members:datasource-rows-fieldcaption}

Allows you to set the display caption for an item.

#### Default Value: ""

**Example:**

{% highlight javascript %}
 
    $("#PivotClient1").ejPivotClient({ dataSource: { rows: [{ fieldCaption : "MyFieldCaption" }] } });
{% endhighlight %}

### dataSource.rows.advancedFilter `array`
{:#members:datasource-rows-advancedfilter}

Allows you to filter the report by using the advanced filtering (e.g., Microsoft Excel) option for the OLAP data source in the client-mode.

#### Default Value: []

**Example:**

{% highlight javascript %}
 
    $("#PivotClient1").ejPivotClient({ dataSource: { rows: [{ advancedFilter : itemArray }] } });
{% endhighlight %}

### dataSource.rows.advancedFilter.name `string`
{:#members:datasource-rows-advancedfilter-name}

Allows you to provide a level unique name to perform the advanced filtering.

#### Default Value: ""

**Example:**

{% highlight javascript %}
 
    $("#PivotClient1").ejPivotClient({ dataSource: { rows: [{ advancedFilter : [{ name: "levelUniqueName" }] }] } });
{% endhighlight %}

### dataSource.rows.advancedFilter.labelFilterOperator `string`
{:#members:datasource-rows-advancedfilter-labelfilteroperator}

Allows you to set the operator to perform the label filtering.

#### Default Value: "none"

**Example:**

{% highlight javascript %}
 
    $("#PivotClient1").ejPivotClient({ dataSource: { rows: [{ advancedFilter : [{ labelFilterOperator: ej.olap.LabelFilterOptions.EndsWith }] }] } });
{% endhighlight %}

### dataSource.rows.advancedFilter.valueFilterOperator `string`
{:#members:datasource-rows-advancedfilter-valuefilteroperator}

Allows you to set the operator to perform the value filtering.

#### Default Value: "none"

**Example:**

{% highlight javascript %}
 
    $("#PivotClient1").ejPivotClient({ dataSource: { rows: [{ advancedFilter : [{ valueFilterOperator: ej.olap.ValueFilterOptions.Between }] }] } });
{% endhighlight %}

### dataSource.rows.advancedFilter.advancedFilterType `string`
{:#members:datasource-rows-advancedfilter-advancedfiltertype}

Allows you to set the filtering type while performing the advanced filtering.

#### Default Value: ""

**Example:**

{% highlight javascript %}
 
    $("#PivotClient1").ejPivotClient({ dataSource: { rows: [{ advancedFilter : [{ advancedFilterType:  ej.olap.AdvancedFilterType.LabelFilter }] }] } });
{% endhighlight %}

### dataSource.rows.advancedFilter.measure `string`
{:#members:datasource-rows-advancedfilter-measure}

In value filtering, this property contains the measure name to which the filter is applied.

#### Default Value: ""

**Example:**

{% highlight javascript %}
 
    $("#PivotClient1").ejPivotClient({ dataSource: { rows: [{ advancedFilter : [{ measure: "measureUniqueName", advancedFilterType: ej.olap.AdvancedFilterType.ValueFilter }] }] } });
{% endhighlight %}

### dataSource.rows.advancedFilter.values `array`
{:#members:datasource-rows-advancedfilter-values}

Allows you to hold the filter operand values in the advanced filtering.

#### Default Value: ""

**Example:**

{% highlight javascript %}
    
    //For Label Filters
    $("#PivotClient1").ejPivotClient({ dataSource: { rows: [{ advancedFilter : [{ labelFilterOperator: ej.olap.LabelFilterOptions.EndsWith, values:  ["002"] }] }] } });
    
    //For Value Filters
    $("#PivotClient1").ejPivotClient({ dataSource: { rows: [{ advancedFilter : [{ valueFilterOperator: ej.olap.ValueFilterOptions.GreaterThan, values:  ["200"] }] }] } });
{% endhighlight %}


### dataSource.rows.isNamedSets `boolean`
{:#members:datasource-rows-isnamedsets}

Allows you to indicate whether the added item is a named set or not. 

> **Note**: This is applicable only for the OLAP data source.

#### Default Value: false

**Example:**

{% highlight javascript %}
 
    $("#PivotClient1").ejPivotClient({ dataSource: { rows: [{ fieldName: "[Core Product Group]", isNamedSets : true }] } });
{% endhighlight %}

### dataSource.rows.showSubTotal `boolean`
{:#members:datasource-rows-showsubtotal}

Shows/hides the sub-total of the field.

>**Note**: This is applicable only for the relational data source.

#### Default Value: true

**Example:**

{% highlight javascript %}
 
    $("#PivotClient1").ejPivotClient({ dataSource: { rows: [{ fieldName: "Country", showSubTotal : false }] } });
{% endhighlight %}

### dataSource.rows.format `string`
{:#members:datasource-rows-format}

Allows to set the format for row headers.

>**Note**: This is applicable only for the relational data source.

#### Default Value: ""

**Example:**

{% highlight javascript %}
 
    $("#PivotClient1").ejPivotClient({ dataSource: { rows: [{ format : "date" }] } });
{% endhighlight %}

### dataSource.rows.formatString `string`
{:#members:datasource-rows-formatstring}

This property is set to display the formatted values with format types in the pivot grid.

#### Default Value: ""

**Example:**

{% highlight javascript %}
 
    $("#PivotClient1").ejPivotClient({ dataSource: { rows: [{ formatString : "MM/DD/YYYY" }] } });
{% endhighlight %}

### dataSource.rows.cssClass `string`
{:#members:datasource-rows-cssclass}

Allows to set the custom theme for row headers.

>**Note**: This is applicable only for the relational data source.

#### Default Value: ""

**Example:**

{% highlight javascript %}
 
    $("#PivotClient1").ejPivotClient({ dataSource: { rows: [{ cssClass : "className" }] } });
{% endhighlight %}

### dataSource.rows.sortOrder `enum`
{:#members:datasource-rows-sortorder}

<ts ref = "ej.PivotAnalysis.SortOrder"/>

Allows you to set the sorting order for the field members.

>**Note**: This is applicable only for the relational data source.

#### Default Value: ej.PivotAnalysis.SortOrder.Ascending

<table class="params">
    <thead>
        <tr>
            <th>Name</th>
            <th>Description</th>
        </tr>
    </thead>
    <tbody>
        <tr>
            <td class="name">Ascending</td>
            <td class="description">Sorts the members of the field in ascending order.</td>
        </tr>
        <tr>
            <td class="name">Descending</td>
            <td class="description">Sorts the members of the field in descending order.</td>
        </tr>
        <tr>
            <td class="name">None</td>
            <td class="description">Displays the members without sorting in any order.</td>
        </tr>
    </tbody>
</table>

**Example:**

{% highlight javascript %}
 
    $("#PivotClient1").ejPivotClient({ dataSource: { rows: [{ fieldName: "Country", sortOrder : ej.PivotAnalysis.SortOrder.Descending }] } });
{% endhighlight %}

### dataSource.rows.drilledItems `array`
{:#members:datasource-rows-drilleditems}

Contains the list of members need to be drilled down by default in the field.

#### Default Value: []

**Example:**

{% highlight javascript %}
 
    $("#PivotClient1").ejPivotClient({ dataSource: { rows: [{ fieldName: "Country", drilledItems : ["Canada", "France"] }] } });
{% endhighlight %}

### dataSource.rows.filterItems `object`
{:#members:datasource-rows-filteritems}

Applies the filter to the field members.

#### Default Value: null

**Example:**

{% highlight javascript %}
 
    $("#PivotClient1").ejPivotClient({ dataSource: { rows: [{ fieldName: "Country", filterItems : { filterType: ej.PivotAnalysis.FilterType.Exclude, values: ["Canada", "France"] } }] } });
{% endhighlight %}

### dataSource.rows.filterItems.filterType `enum`
{:#members:datasource-rows-filteritems-filtertype}

<ts ref = "ej.PivotAnalysis.FilterType"/>

Sets the type of filter whether to include/exclude the mentioned values.

>**Note**: This is applicable only for the relational data source.

#### Default Value: ej.PivotAnalysis.FilterType.Exclude

<table class="params">
    <thead>
        <tr>
            <th>Name</th>
            <th>Description</th>
        </tr>
    </thead>
    <tbody>
        <tr>
            <td class="name">Exclude</td>
            <td class="description">Excludes the specified values among the members of the field.</td>
        </tr>
        <tr>
            <td class="name">Include</td>
            <td class="description">Includes the specified values alone among the members of the field.</td>
        </tr>
    </tbody>
</table>

**Example:**

{% highlight javascript %}
 
    $("#PivotClient1").ejPivotClient({ dataSource: { rows: [{ fieldName: "Country", filterItems : { filterType: ej.PivotAnalysis.FilterType.Include, values: valueArray } }] } });
{% endhighlight %}

### dataSource.rows.filterItems.values `array`
{:#members:datasource-rows-filteritems-values}

Contains the collection of items to be included/excluded among the field members.

#### Default Value: []

**Example:**

{% highlight javascript %}
 
    $("#PivotClient1").ejPivotClient({ dataSource: { rows: [{ fieldName: "Country", filterItems : { filterType: ej.PivotAnalysis.FilterType.Exclude, values: ["Canada", "France"] } }] } });
{% endhighlight %}

### dataSource.values `array`
{:#members:datasource-values}

Lists out the items which supports calculation in the pivot client.

#### Default Value: []

**Example:**

{% highlight javascript %}
 
    $("#PivotClient1").ejPivotClient({ dataSource: { values: itemsArray } });
{% endhighlight %}

### dataSource.values.fieldName `string`
{:#members:datasource-values-fieldname}

Allows you to bind the item by using its unique name as field name for the relational data source.

>**Note**: This is applicable only for the relational data source.

#### Default Value: ""

**Example:**

{% highlight javascript %}
 
    $("#PivotClient1").ejPivotClient({ dataSource: { values: [{ fieldName : "MyFieldName" }] } });
{% endhighlight %}

### dataSource.values.fieldCaption `string`
{:#members:datasource-values-fieldcaption}

Allows you to set the display caption for an item for the relational data source.

>**Note**: This is applicable only for the relational data source.

#### Default Value: ""

**Example:**

{% highlight javascript %}
 
    $("#PivotClient1").ejPivotClient({ dataSource: { values: [{ fieldCaption : "MyFieldCaption" }] } });
{% endhighlight %}

### dataSource.values.measures `array`
{:#members:datasource-values-measures}

This holds the list of unique names of measures to bind them from the OLAP cube.

#### Default Value: []

**Example:**

{% highlight javascript %}
 
    $("#PivotClient1").ejPivotClient({ dataSource: { values: [{ measures : itemsArray }] } });
{% endhighlight %}

### dataSource.values.measures.fieldName `string`
{:#members:datasource-values-measures-fieldName}

Allows you to bind the measure from the OLAP data source by using its unique name as field name.

#### Default Value: ""

**Example:**

{% highlight javascript %}
 
    $("#PivotClient1").ejPivotClient({ dataSource: { values: [{ measures : [{ fieldName: "MeasureUniqueName" }] }] } });
{% endhighlight %}

### dataSource.values.axis `string`
{:#members:datasource-values-axis}

Allows to set the axis name to place the measures items.

>**Note**: This is applicable only for the OLAP data source.

#### Default Value: "rows"

**Example:**

{% highlight javascript %}
 
    $("#PivotClient1").ejPivotClient({ dataSource: { values: [{ axis : ej.olap.AxisName.Row }] } });
{% endhighlight %}

### dataSource.values.isCalculatedField `boolean`
{:#members:datasource-values-iscalculatedfield}

Indicates whether the field is a calculated field or not with the relational data source.

#### Default Value: false

**Example:**

{% highlight javascript %}
 
    $("#PivotClient1").ejPivotClient({ dataSource: { values: [{ isCalculatedField : true }] } });
{% endhighlight %}

### dataSource.values.summaryType `enum`
{:#members:datasource-values-summarytype}

<ts ref = "ej.PivotAnalysis.SummaryType"/>

Allows to set the type of the pivot grid summary calculation for the value field with the relational data source.

#### Default Value: ej.PivotAnalysis.SummaryType.Sum

**Example:**

<table class="params">
    <thead>
        <tr>
            <th>Name</th>
            <th>Description</th>
        </tr>
    </thead>
    <tbody>
        <tr>
            <td class="name">Sum</td>
            <td class="description">Calculates the summary as the total of all values.</td>
        </tr>
        <tr>
            <td class="name">Average</td>
            <td class="description">Displays the average of all values as the summaries.</td>
        </tr>
        <tr>
            <td class="name">Count</td>
            <td class="description">Displays the count of items in summaries.</td>
        </tr>
        <tr>
            <td class="name">Min</td>
            <td class="description">Displays the minimum value of all the items in the summary.</td>
        </tr>
        <tr>
            <td class="name">Max</td>
            <td class="description">Displays the maximum value of all the items in the summary.</td>
        </tr>
    </tbody>
</table>

{% highlight javascript %}
 
    $("#PivotClient1").ejPivotClient({ dataSource: { values: [{ summaryType : ej.PivotAnalysis.SummaryType.Average }] } });
{% endhighlight %}

### dataSource.values.format `string`
{:#members:datasource-values-format}

Allows to set the format of the values.

#### Default Value: ""

**Example:**

{% highlight javascript %}
 
    $("#PivotClient1").ejPivotClient({ dataSource: { values: [{ format : "percentage" }] } });
{% endhighlight %}

### dataSource.values.formatString `string`
{:#members:datasource-values-formatstring}

This property is set to display the formatted values with format types in the pivot grid.

#### Default Value: ""

**Example:**

{% highlight javascript %}
 
    $("#PivotClient1").ejPivotClient({ dataSource: { values: [{ formatString : "MM/DD/YYYY" }] } });
{% endhighlight %}

### dataSource.values.cssClass `string`
{:#members:datasource-values-cssclass}

Allows to set the custom theme for the values.

>**Note**: This is applicable only for the relational data source.

#### Default Value: ""

**Example:**

{% highlight javascript %}
 
    $("#PivotClient1").ejPivotClient({ dataSource: { values: [{ cssClass : "className" }] } });
{% endhighlight %}

### dataSource.values.formula `string`
{:#members:datasource-values-formula}

Allows to set the formula for calculation of members values in the relational data source.

#### Default Value: ""

**Example:**

{% highlight javascript %}
 
    $("#PivotClient1").ejPivotClient({ dataSource: { values: [{ formula : "Quantity*10" }] } });
{% endhighlight %}

### dataSource.filters `array`
{:#members:datasource-filters}

Lists out the items which supports filtering of values without displaying the members in UI of the pivot client.

#### Default Value: []

**Example:**

{% highlight javascript %}
 
    $("#PivotClient1").ejPivotClient({ dataSource: { filters: itemsArray } });
{% endhighlight %}


### dataSource.filters.fieldName `string`
{:#members:datasource-filters-fieldname}

Allows you to bind the item by using its unique name as field name.

#### Default Value: ""

**Example:**

{% highlight javascript %}
 
    $("#PivotClient1").ejPivotClient({ dataSource: { filters: [{ fieldName : "MyFieldName" }] } });
{% endhighlight %}

### dataSource.filters.fieldCaption `string`
{:#members:datasource-filters-fieldcaption}

Allows you to set the display name for an item.

#### Default Value: ""

**Example:**

{% highlight javascript %}
 
    $("#PivotClient1").ejPivotClient({ dataSource: { filters: [{ fieldCaption : "MyFieldCaption" }] } });
{% endhighlight %}

### dataSource.filters.filterItems `object`
{:#members:datasource-filters-filteritems}

Applies filter to the field members.

#### Default Value: null

**Example:**

{% highlight javascript %}
 
    $("#PivotClient1").ejPivotClient({ dataSource: { filters: [{ fieldName: "Country", filterItems : { filterType: ej.PivotAnalysis.FilterType.Exclude, values: ["Canada", "France"] } }] } });
{% endhighlight %}

### dataSource.filters.filterItems.filterType `enum`
{:#members:datasource-filters-filteritems-filtertype}

<ts ref = "ej.PivotAnalysis.FilterType"/>

Sets the type of filter whether to include/exclude the mentioned values.

>**Note**: This is applicable only for the relational data source.

#### Default Value: ej.PivotAnalysis.FilterType.Exclude

<table class="params">
    <thead>
        <tr>
            <th>Name</th>
            <th>Description</th>
        </tr>
    </thead>
    <tbody>
        <tr>
            <td class="name">Exclude</td>
            <td class="description">Excludes the specified values among the members of the field.</td>
        </tr>
        <tr>
            <td class="name">Include</td>
            <td class="description">Includes the specified values alone among the members of the field.</td>
        </tr>
    </tbody>
</table>

**Example:**

{% highlight javascript %}
 
    $("#PivotClient1").ejPivotClient({ dataSource: { filters: [{ fieldName: "Country", filterItems : { filterType: ej.PivotAnalysis.FilterType.Include, values: valueArray } }] } });
{% endhighlight %}

### dataSource.filters.filterItems.values `array`
{:#members:datasource-filters-filteritems-values}

Contains the collection of items to be included/excluded among the field members.

#### Default Value: []

**Example:**

{% highlight javascript %}
 
    $("#PivotClient1").ejPivotClient({ dataSource: { filters: [{ fieldName: "Country", filterItems : { filterType: ej.PivotAnalysis.FilterType.Exclude, values: ["Canada", "France"] } }] } });
{% endhighlight %}

### dataSource.cube `string`
{:#members:datasource-cube}

Contains the respective cube name from the OLAP database as string type.

#### Default Value: “”

**Example:**

{% highlight javascript %}
 
    $("#PivotClient1").ejPivotClient({ dataSource: { cube: "Adventure Works" } });
{% endhighlight %}

### dataSource.sourceInfo `string`
{:#members:datasource-sourceinfo}

Allows to set the data source name to fetch the data from that.

>**Note**: This is applicable only for the Mondrian connection.

#### Default Value: “”

**Example:**

{% highlight javascript %}
 
    $("#PivotClient1").ejPivotClient({ dataSource: { sourceInfo: "Provider Mondrian" } });
{% endhighlight %}

### dataSource.providerName `string`
{:#members:datasource-providername}

Sets the provider name for the pivot client to identify whether the provider is SSAS or Mondrian.

>**Note**: This is applicable only for the client side OLAP data.

#### Default Value: "ssas"

<table class="params">
    <thead>
        <tr>
            <th>Name</th>
            <th>Description</th>
        </tr>
    </thead>
    <tbody>
        <tr>
            <td class="name">ssas</td>
            <td class="description">To bind an OLAP data source to PivotClient through SSAS provider.</td>
        </tr>
        <tr>
            <td class="name">mondrian</td>
            <td class="description">To bind a relational data source to PivotClient through Mondrian provider.</td>
        </tr>
    </tbody>
</table>

**Example:**

{% highlight javascript %}
 
    $("#PivotClient1").ejPivotClient({ dataSource: { providerName: "mondrian" } });
{% endhighlight %}

### dataSource.data `object`
{:#members:datasource-data}

Provides the raw data source for the pivot client.

#### Default Value: null

**Example:**

{% highlight javascript %}
 
    $("#PivotClient1").ejPivotClient({ dataSource: { data: value } });
{% endhighlight %}

### dataSource.catalog `string`
{:#members:datasource-catalog}

In connection with an OLAP database, this property contains the database name as string to fetch the data from the given connection string.

#### Default Value: “”

**Example:**

{% highlight javascript %}
 
    $("#PivotClient1").ejPivotClient( { dataSource: { catalog: "databaseName" } } );
{% endhighlight %}

### dataSource.enableAdvancedFilter `boolean`
{:#members:datasource-enableadvancedfilter}

Allows you to filter the members (by its name and values) through the advanced filtering (e.g., Microsoft Excel) option in the client-mode.

#### Default Value: false

**Example:**

{% highlight javascript %}
 
    $("#PivotClient1").ejPivotClient({ dataSource: { enableAdvancedFilter: true } });
{% endhighlight %}

### dataSource.reportName `string`
{:#members:datasource-reportName}

Sets a name to the report bound to the control.

#### Default Value: ""

**Example:**

{% highlight javascript %}
 
    $("#PivotClient1").ejPivotClient({ dataSource: { reportName: "Default Report" } });
{% endhighlight %}

### dataSource.pagerOptions `object`
{:#members:datasource-pageroptions}

Allows to set the page size and current page number for each axis on applying the paging.

> **Note**: This is applicable only for binding the OLAP data from the client-side.

#### Default Value: {}

**Example:**

{% highlight javascript %}
 
    $("#PivotClient1").ejPivotClient({ dataSource: { pagerOptions: pagerSettings } }); 
{% endhighlight %}

### dataSource.pagerOptions.categoricalPageSize `number`
{:#members:datasource-pageroptions-categoricalpagesize}

Allows to set the number of categorical columns to be displayed in each page on applying the paging.

#### Default Value: 0

**Example:**

{% highlight javascript %}
 
    $("#PivotClient1").ejPivotClient({ dataSource: { pagerOptions: { categoricalPageSize: 10 } } }); 
{% endhighlight %}

### dataSource.pagerOptions.seriesPageSize `number`
{:#members:datasource-pageroptions-seriespagesize}

Allows to set the number of series rows to be displayed in each page on applying the paging.

#### Default Value: 0

**Example:**

{% highlight javascript %}
 
    $("#PivotClient1").ejPivotClient({ dataSource: { pagerOptions: { seriesPageSize: 5 } } }); 
{% endhighlight %}

### dataSource.pagerOptions.categoricalCurrentPage `number`
{:#members:datasource-pageroptions-categoricalcurrentpage}

Allows to set the page number in the categorical axis to be loaded by default.

> **Note**: This is applicable only for binding the OLAP data from the client-side.

#### Default Value: 1

**Example:**

{% highlight javascript %}
 
    $("#PivotClient1").ejPivotClient({ dataSource: { pagerOptions: { categoricalCurrentPage: 3 } } }); 
{% endhighlight %}

### dataSource.pagerOptions.seriesCurrentPage `number`
{:#members:datasource-pageroptions-seriescurrentpage}

Allows to set the page number in the series axis to be loaded by default.

#### Default Value: 1

**Example:**

{% highlight javascript %}
 
    $("#PivotClient1").ejPivotClient({ dataSource: { pagerOptions: { seriesCurrentPage: 7 } } }); 
{% endhighlight %}

### enableDrillThrough `boolean`
{:#members:enabledrillthrough}

Enables the drill-through feature which retrieves the raw items that are used to create a specific cell in the pivot grid.

#### Default Value: false

**Example:**

{% highlight javascript %}
 
    $("#PivotClient1").ejPivotClient({ enableDrillThrough: true });
{% endhighlight %}

### displaySettings `object`
{:#members:displaysettings}

Allows you to customize the layout and appearance of the widget.

#### Default Value: {}

**Example:**

{% highlight javascript %}
 
    $("#PivotClient1").ejPivotClient({ displaySettings: settingsObject });
{% endhighlight %}

### displaySettings.controlPlacement `enum`
{:#members:displaysettings-controlplacement}

<ts name = "ej.PivotClient.ControlPlacement"/>

Allows you to customize the display of the pivot chart and pivot grid widgets in the tabs or tiles.

#### Default Value: ej.PivotClient.ControlPlacement.Tab

<table class="params">
    <thead>
        <tr>
            <th>Name</th>
            <th>Description</th>
        </tr>
    </thead>
    <tbody>
        <tr>
            <td class="name">Tab</td>
            <td class="description">Displays PivotChart and PivotGrid widgets in separate tabs.</td>
        </tr>
        <tr>
            <td class="name">Tile</td>
            <td class="description">Displays PivotChart and PivotGrid widgets one above the other.</td>
        </tr>
    </tbody>
</table>


**Example:**

{% highlight javascript %}
 
    $("#PivotClient1").ejPivotClient({ displaySettings: { controlPlacement: ej.PivotClient.ControlPlacement.Tile } });
{% endhighlight %}

### displaySettings.defaultView `enum`
{:#members:displaysettings-defaultview}

<ts name = "ej.PivotClient.DefaultView"/>

Allows you to set either the chart or grid as the start-up widget.

#### Default Value: ej.PivotClient.DefaultView.Grid

<table class="params">
    <thead>
        <tr>
            <th>Name</th>
            <th>Description</th>
        </tr>
    </thead>
    <tbody>
        <tr>
            <td class="name">Chart</td>
            <td class="description">To set PivotChart as a default control in view.</td>
        </tr>
        <tr>
            <td class="name">Grid</td>
            <td class="description">To set PivotGrid as a default control in view.</td>
        </tr>
    </tbody>
</table>


**Example:**

{% highlight javascript %}
 
    $("#PivotClient1").ejPivotClient({ displaySettings: { defaultView: ej.PivotClient.DefaultView.Chart } });
{% endhighlight %}

### displaySettings.enableFullScreen `boolean`
{:#members:displaysettings-enablefullscreen}

Allows you to switch to full screen view of the pivot chart and the pivot grid from default view in the pivot client.

#### Default Value: false

**Example:**

{% highlight javascript %}
 
    $("#PivotClient1").ejPivotClient({ displaySettings: { enableFullScreen: true } });
{% endhighlight %}

### displaySettings.enableTogglePanel `boolean`
{:#members:displaysettings-enabletogglepanel}

Enables an option to enhance the space for the pivot grid and pivot chart by hiding the cube browser and the axis element builder.

#### Default Value: false

**Example:**

{% highlight javascript %}
 
    $("#PivotClient1").ejPivotClient({ displaySettings: { enableTogglePanel: true } });
{% endhighlight %}

### displaySettings.mode `enum`
{:#members:displaysettings-mode}

<ts name = "ej.PivotClient.DisplayMode"/>

Sets the display mode (only chart/only grid/both) in the pivot client.

#### Default Value: ej.PivotClient.DisplayMode.ChartAndGrid

<table class="params">
    <thead>
        <tr>
            <th>Name</th>
            <th>Description</th>
        </tr>
    </thead>
    <tbody>
        <tr>
            <td class="name">ChartOnly</td>
            <td class="description">To display only PivotChart widget.</td>
        </tr>
        <tr>
            <td class="name">GridOnly</td>
            <td class="description">To display only PivotGrid widget.</td>
        </tr>
        <tr>
            <td class="name">ChartAndGrid</td>
            <td class="description">To display both PivotChart and PivotGrid widgets.</td>
        </tr>
    </tbody>
</table>


**Example:**

{% highlight javascript %}
 
    $("#PivotClient1").ejPivotClient({ displaySettings: { mode: ej.PivotClient.DisplayMode.ChartOnly } });
{% endhighlight %}

### toolbarIconSettings `object`
{:#members:toolbariconsettings}

Allows you to set the visibility of icons in the toolbar panel.

#### Default Value: {}

**Example:**

{% highlight javascript %}
 
    $("#PivotClient1").ejPivotClient({ toolbarIconSettings: settingsObject });
{% endhighlight %}

### toolbarIconSettings.enableAddReport `boolean`
{:#members:toolbariconsettings-enableaddreport}

Allows you to set the visibility of `Add Report` icon in the toolbar panel.

#### Default Value: true

**Example:**

{% highlight javascript %}
 
    $("#PivotClient1").ejPivotClient({ toolbarIconSettings: {enableAddReport : true} });
{% endhighlight %}

### toolbarIconSettings.enableNewReport `boolean`
{:#members:toolbariconsettings-enablenewreport}

Allows you to set the visibility of `New Report` icon in the toolbar panel.

#### Default Value: true

**Example:**

{% highlight javascript %}
 
    $("#PivotClient1").ejPivotClient({ toolbarIconSettings: {enableNewReport : true} });
{% endhighlight %}

### toolbarIconSettings.enableRenameReport `boolean`
{:#members:toolbariconsettings-enablerenamereport}

Allows you to set the visibility of `Rename Report` icon in the toolbar panel.

#### Default Value: true

**Example:**

{% highlight javascript %}
 
    $("#PivotClient1").ejPivotClient({ toolbarIconSettings: {enableRenameReport : true} });
{% endhighlight %}

### toolbarIconSettings.enableDBManipulation `boolean`
{:#members:toolbariconsettings-enabledbmanipulation}

Allows you to set the visibility of `DB Manipulation` icon in the toolbar panel.

#### Default Value: true

**Example:**

{% highlight javascript %}
 
    $("#PivotClient1").ejPivotClient({ toolbarIconSettings: {enableDBManipulation : true} });
{% endhighlight %}

### toolbarIconSettings.enableWordExport `boolean`
{:#members:toolbariconsettings-enablewordexport}

Allows you to set the visibility of `Word Export` icon in the toolbar panel.

#### Default Value: true

**Example:**

{% highlight javascript %}
 
    $("#PivotClient1").ejPivotClient({ toolbarIconSettings: {enableWordExport : true} });
{% endhighlight %}

### toolbarIconSettings.enableExcelExport `boolean`
{:#members:toolbariconsettings-enableexcelexport}

Allows you to set the visibility of `Excel Export` icon in the toolbar panel.

#### Default Value: true

**Example:**

{% highlight javascript %}
 
    $("#PivotClient1").ejPivotClient({ toolbarIconSettings: {enableExcelExport : true} });
{% endhighlight %}

### toolbarIconSettings.enablePdfExport `boolean`
{:#members:toolbariconsettings-enablepdfexport}

Allows you to set the visibility of `PDF Export` icon in the toolbar panel.

#### Default Value: true

**Example:**

{% highlight javascript %}
 
    $("#PivotClient1").ejPivotClient({ toolbarIconSettings: {enablePdfExport : true} });
{% endhighlight %}

### toolbarIconSettings.enableMDXQuery `boolean`
{:#members:toolbariconsettings-enablemdxquery}

Allows you to set the visibility of `MDX Query` icon in the toolbar panel.

>**Note**: This is not applicable for the relational data source.

#### Default Value: true

**Example:**

{% highlight javascript %}
 
    $("#PivotClient1").ejPivotClient({ toolbarIconSettings: {enableMDXQuery : true} });
{% endhighlight %}

### toolbarIconSettings.enableDeferUpdate `boolean`
{:#members:toolbariconsettings-enabledeferupdate}

Allows to set the visibility of `Defer Update` icon in the toolbar panel.

#### Default Value: false

**Example:**

{% highlight javascript %}
 
    $("#PivotClient1").ejPivotClient({ toolbarIconSettings: {enableDeferUpdate : true} });
{% endhighlight %}

### toolbarIconSettings.enableFullScreen `boolean`
{:#members:toolbariconsettings-enablefullscreen}

Allows to set the visibility of `Full Screen` icon in the toolbar panel.

#### Default Value: false

**Example:**

{% highlight javascript %}
 
    $("#PivotClient1").ejPivotClient({ toolbarIconSettings: {enableFullScreen : true} });
{% endhighlight %}

### toolbarIconSettings.enableSortOrFilterColumn `boolean`
{:#members:toolbariconsettings-enablesortorfiltercolumn}

Allows you to set the visibility of `Sort/Filter Column` icon in the toolbar panel.

>**Note**: This is only applicable for the OLAP data bound from the server-side.

#### Default Value: true

**Example:**

{% highlight javascript %}
 
    $("#PivotClient1").ejPivotClient({ toolbarIconSettings: {enableSortOrFilterColumn : true} });
{% endhighlight %}

### toolbarIconSettings.enableSortOrFilterRow `boolean`
{:#members:toolbariconsettings-enablesortorfilterrow}

Allows you to set the visibility of `Sort/Filter Row` icon in the toolbar panel.

>**Note**: This is only applicable for the OLAP data bound from the server-side.

#### Default Value: true

**Example:**

{% highlight javascript %}
 
    $("#PivotClient1").ejPivotClient({ toolbarIconSettings: {enableSortOrFilterRow : true} });
{% endhighlight %}

### toolbarIconSettings.enableToggleAxis `boolean`
{:#members:toolbariconsettings-enabletoggleaxis}

Allows you to set the visibility of `Toggle Axis` icon in the toolbar panel.

#### Default Value: true

**Example:**

{% highlight javascript %}
 
    $("#PivotClient1").ejPivotClient({ toolbarIconSettings: {enableToggleAxis : true} });
{% endhighlight %}

### toolbarIconSettings.enableChartTypes `boolean`
{:#members:toolbariconsettings-enablecharttypes}

Allows you to set the visibility of `Chart Types` icon in the toolbar panel.

#### Default Value: true

**Example:**

{% highlight javascript %}
 
    $("#PivotClient1").ejPivotClient({ toolbarIconSettings: {enableChartTypes : true} });
{% endhighlight %}

### toolbarIconSettings.enableRemoveReport `boolean`
{:#members:toolbariconsettings-enableremovereport}

Allows you to set the visibility of `Remove Report` icon in the toolbar panel.

#### Default Value: true

**Example:**

{% highlight javascript %}
 
    $("#PivotClient1").ejPivotClient({ toolbarIconSettings: {enableRemoveReport : true} });
{% endhighlight %}

### toolbarIconSettings.enableCalculatedMember `boolean`
{:#members:toolbariconsettings-enablecalculatedmember}

Allows you to set the visibility of `Calculated Member` icon in the toolbar panel.

>**Note**: This is applicable only for the OLAP data bound from the server-side.

#### Default Value: false

**Example:**

{% highlight javascript %}
 
    $("#PivotClient1").ejPivotClient({ toolbarIconSettings: {enableCalculatedMember : true} });
{% endhighlight %}

### showUniqueNameOnPivotButton `boolean`
{:#members:showuniquenameonpivotbutton}

Allows you to show a unique name on the pivot button.

>**Note**: This is only applicable for the OLAP data source.

#### Default Value: false

**Example:**

{% highlight javascript %}
 
    $("#PivotClient1").ejPivotClient({ showUniqueNameOnPivotButton: true });
{% endhighlight %}

### showReportCollection `boolean`
{:#members:showreportcollection}

Allows you to load the saved report collection from the database.

#### Default Value: false

**Example:**

{% highlight javascript %}
 
    $("#PivotClient1").ejPivotClient({ showReportCollection: true });
{% endhighlight %}

### enableSplitter `boolean`
{:#members:enableSplitter}

Enables the splitter option for resizing the elements in the control.

>**Note**: This is not applicable for the OLAP data bound from the server-side.

#### Default Value: false

**Example:**

{% highlight javascript %}
 
    $("#PivotClient1").ejPivotClient({ enableSplitter: true });
{% endhighlight %}


### enableAdvancedFilter `boolean`
{:#members:enableadvancedfilter}

Enables the advanced filtering options such as value filtering, label filtering, and sorting for each dimensions when binding the OLAP data in the server mode.

#### Default Value: false

**Example:**

{% highlight javascript %}
 
    $("#PivotClient1").ejPivotClient({ enableAdvancedFilter: true });
{% endhighlight %}

### enableDeferUpdate `boolean`
{:#members:enabledeferupdate}

Allows you to refresh the control on-demand and not during the every UI operation.

> **Note**: This property is applicable for OLAP data bound from the server-side alone.

#### Default Value: false

**Example:**

{% highlight javascript %}
 
    $("#PivotClient1").ejPivotClient({ enableDeferUpdate: true });
{% endhighlight %}

### enableLocalStorage `boolean`
{:#members:enablelocalstorage}

Allows to save and load the reports in a customized way with the help of events. 

#### Default Value: false

**Example:**

{% highlight javascript %}
 
    $("#PivotClient1").ejPivotClient({ enableLocalStorage: true });
{% endhighlight %}

### enablePaging `boolean`
{:#members:enablepaging}

Allows you to enable the paging for both the pivot chart and the pivot grid components for viewing the large data.

> **Note**: This property is applicable only for the OLAP data bound from the client-side.

#### Default Value: false

**Example:**

{% highlight javascript %}
 
    $("#PivotClient1").ejPivotClient({ enablePaging: true });
{% endhighlight %}

### enablePivotTreeMap `boolean`
{:#members:enablepivottreemap}

Allows you to include the pivot tree map component as one of the chart types.

> **Note**: This property is applicable only for the OLAP data bound from the server-side.

#### Default Value: false

**Example:**

{% highlight javascript %}
 
    $("#PivotClient1").ejPivotClient({ enablePivotTreeMap: true });
{% endhighlight %}

### enableRTL `boolean`
{:#members:enablertl}

Allows you to view the layout of the pivot client from right to left.

#### Default Value: false

**Example:**

{% highlight javascript %}
 
    $("#PivotClient1").ejPivotClient({ enableRTL: true });
{% endhighlight %}

### enableMeasureGroups `boolean`
{:#members:enablemeasuregroups}

Enables/disables the visibility of measure group selector drop-down in the cube browser.

> **Note**: This property is applicable only for the OLAP data source bound from the server-side.

#### Default Value: false

**Example:**

{% highlight javascript %}
 
    $("#PivotClient1").ejPivotClient({ enableMeasureGroups : true });
{% endhighlight %}


### enableCellClick `boolean`
{:#members:enablecellclick}

Allows you to get cell details in JSON format by clicking the value cell.

#### Default Value: false

**Example:**

{% highlight javascript %}
 
    $("#PivotClient1").ejPivotClient({ enableCellClick: true });
{% endhighlight %}

### enableCellDoubleClick `boolean`
{:#members:enablecelldoubleclick}

Allows you to get cell details in JSON format by double-clicking the value cell.

#### Default Value: false

**Example:**

{% highlight javascript %}
 
    $("#PivotClient1").ejPivotClient({ enableCellDoubleClick: true });
{% endhighlight %}

### enableVirtualScrolling `boolean`
{:#members:enablevirtualscrolling}

Allows you to enable the virtual scrolling for both the pivot chart and pivot grid components for viewing the large data.

> **Note**: This is applicable only for the OLAP data.

#### Default Value: false

**Example:**

{% highlight javascript %}
 
    $("#PivotClient1").ejPivotClient({ enableVirtualScrolling: true });
{% endhighlight %}

### maxNodeLimitInMemberEditor `number`
{:#members:maxNodeLimitInMemberEditor}

Allows you to set the maximum number of nodes as well as child nodes to be displayed in the member editor.

#### Default Value: 1000

**Example:**

{% highlight javascript %}
 
    $("#PivotClient1").ejPivotClient({ maxNodeLimitInMemberEditor: 1500 });
{% endhighlight %}

### enableMemberEditorPaging `boolean`
{:#members:enablemembereditorpaging}

Enables/disables paging in the member editor for viewing the large count of members in the pages.

#### Default Value: false

**Example:**

{% highlight javascript %}
 
    $("#PivotClient1").ejPivotClient({ enableMemberEditorPaging: true });
{% endhighlight %}

### memberEditorPageSize `number`
{:#members:membereditorpagesize}

Allows you to set the number of members to be displayed in each page of the member editor on applying the paging in it.

#### Default Value: 100

**Example:**

{% highlight javascript %}
 
    $("#PivotClient1").ejPivotClient({ memberEditorPageSize: 50 });
{% endhighlight %}

### enableMemberEditorSorting `boolean`
{:#members:enablemembereditorsorting}

Enables/Disables sorting option in member editor dialog for the members of the respective field.

#### Default Value: false

**Example:**

{% highlight javascript %}

    $("#PivotClient1").ejPivotClient({ enableMemberEditorSorting: true });
{% endhighlight %}

### gridLayout `enum`
{:#members:gridlayout}

<ts ref = "ej.PivotGrid.Layout"/>

Sets the summary layout for the pivot grid. Following are the ways in which the summary can be positioned: normal summary (bottom), top summary, no summary, and Microsoft Excel summary.

> **Note**: This property is applicable only for the OLAP data bound from the server-side.

#### Default Value: ej.PivotGrid.Layout.Normal

<table class="params">
    <thead>
        <tr>
            <th>Name</th>
            <th>Description</th>
        </tr>
    </thead>
    <tbody>
        <tr>
            <td class="name">Normal</td>
            <td class="description">To set normal summary layout in PivotGrid.</td>
        </tr>
        <tr>
            <td class="name">NormalTopSummary</td>
            <td class="description">To set layout with summaries at the top in PivotGrid.</td>
        </tr>
        <tr>
            <td class="name">NoSummaries</td>
            <td class="description">To set layout without summaries in PivotGrid.</td>
        </tr>
        <tr>
            <td class="name">ExcelLikeLayout</td>
            <td class="description">To set excel-like layout in PivotGrid.</td>
        </tr>
    </tbody>
</table>

**Example:** 

{% highlight javascript %}
 
    $("#PivotClient1").ejPivotClient({ gridLayout: ej.PivotGrid.Layout.NoSummaries });
{% endhighlight %}

### collapseCubeBrowserByDefault `boolean`
{:#members:collapsecubebrowserbydefault}

Allows you to hide the cube browser and the axis element builder of the pivot client while initiating the widget.

#### Default Value: false

**Example:**

{% highlight javascript %}
 
    $("#PivotClient1").ejPivotClient({ collapseCubeBrowserByDefault: true });
{% endhighlight %}

### enableKPI `boolean`
{:#members:enablekpi}

Allows you to view the KPI elements in tree-view of the pivot client's cube browser.

> **Note**: This property is applicable only for the OLAP data.

#### Default Value: false

**Example:**

{% highlight javascript %}
 
    $("#PivotClient1").ejPivotClient({ enableKPI: true });
{% endhighlight %}

### isResponsive `boolean`
{:#members:isresponsive}

Allows you to enable the pivot client’s responsiveness in the browser layout.

#### Default Value: false

**Example:**

{% highlight javascript %}
 
    $("#PivotClient1").ejPivotClient({ isResponsive: true });
{% endhighlight %}

### size `object`
{:#members:size}

Options to customize the size of the pivot client control.

#### Default Value: { height: "685px", width: "1000px" }

**Example:**

{% highlight javascript %}
 
    $("#PivotClient1").ejPivotClient({ size: { width: "50%" , height: "80%" } });
{% endhighlight %}

### locale `string`
{:#members:locale}

Allows you to set the localized language for the widget.

#### Default Value: "en-US"

**Example:** 

{% highlight javascript %}
 
    $("#PivotClient1").ejPivotClient({ locale: "fr-FR" });
{% endhighlight %}

### operationalMode `enum`
{:#members:operationalmode}

<ts ref = "ej.Pivot.OperationalMode"/>

Sets the mode for the pivot client widget to bind the data source in the server-side or the client-side.

<table class="params">
    <thead>
        <tr>
            <th>Name</th>
            <th>Description</th>
        </tr>
    </thead>
    <tbody>
        <tr>
            <td class="name">ClientMode</td>
            <td class="description">To bind data source completely from client-side.</td>
        </tr>
        <tr>
            <td class="name">ServerMode</td>
            <td class="description">To bind data source completely from server-side.</td>
        </tr>
    </tbody>
</table>

#### Default Value: ej.Pivot.OperationalMode.ClientMode

**Example:**

{% highlight javascript %}
 
    $("#PivotClient1").ejPivotClient({ operationalMode: ej.Pivot.OperationalMode.ServerMode });
{% endhighlight %}

### serviceMethodSettings `object`
{:#members:servicemethodsettings}

Allows you to set the custom name for methods at service-end, and it is communicated during the AJAX post.

> **Note**: This property is applicable only for operating the control from the server-side.

#### Default Value: {}

**Example:**

{% highlight javascript %}
 
    $("#PivotClient1").ejPivotClient({ serviceMethodSettings: value });
{% endhighlight %}

### serviceMethodSettings.cubeChanged `string`
{:#members:servicemethodsettings-cubechanged}

Allows you to set the custom name for the service method that is responsible for updating the entire report and widget, while changing the cube.

#### Default Value: "CubeChanged"

**Example:**

{% highlight javascript %}
 
    $("#PivotClient1").ejPivotClient({ serviceMethodSettings: { cubeChanged: "CubeChangedMyMethod" } });
{% endhighlight %}

### serviceMethodSettings.exportPivotClient `string`
{:#members:servicemethodsettings-exportpivotclient}

Allows to set the custom name for the service method responsible for exporting.

#### Default Value: "Export"

**Example:**

{% highlight javascript %}
 
    $("#PivotClient1").ejPivotClient({ serviceMethodSettings: { exportPivotClient: "ExportMyMethod" } }); 
{% endhighlight %}

### serviceMethodSettings.fetchMemberTreeNodes `string`
{:#members:servicemethodsettings-fetchmembertreenodes}

Allows you to set the custom name for the service method that is responsible to get the members for tree-view in the member-editor dialog.

#### Default Value: "FetchMemberTreeNodes"

**Example:**

{% highlight javascript %}
 
    $("#PivotClient1").ejPivotClient({ serviceMethodSettings: { fetchMemberTreeNodes: "FetchMemberTreeNodesMyMethod" } }); 
{% endhighlight %}

### serviceMethodSettings.fetchReportList `string`
{:#members:servicemethodsettings-fetchreportlist}

Allows you to set the custom name for the service method that is responsible for fetching the report names from the database.

#### Default Value: "FetchReportListFromDB"

**Example:**

{% highlight javascript %}
                     
    $("#PivotClient1").ejPivotClient({ serviceMethodSettings: { fetchReportList: "FetchReportListFromDBMyMethod" } }); 
{% endhighlight %}

### serviceMethodSettings.filterElement `string`
{:#members:servicemethodsettings-filterelement}

Allows you to set the custom name for the service method that is responsible for updating the report while filtering the members.

#### Default Value: "FilterElement"

**Example:**

{% highlight javascript %}
 
    $("#PivotClient1").ejPivotClient({ serviceMethodSettings: { filterElement: "filterElementMyMethod" } }); 
{% endhighlight %}

### serviceMethodSettings.initialize `string`
{:#members:servicemethodsettings-initialize}

Allows you to set the custom name for the service method that is responsible for initializing the pivot client.

#### Default Value: "InitializeClient"

**Example:**

{% highlight javascript %}
 
    $("#PivotClient1").ejPivotClient({ serviceMethodSettings: { initialize: "InitializeClientMyMethod" } }); 
{% endhighlight %}

### serviceMethodSettings.loadReport `string`
{:#members:servicemethodsettings-loadreport}

Allows you to set the custom name for the service method that is responsible for loading a report collection from the database.

#### Default Value: "LoadReportFromDB"

**Example:**

{% highlight javascript %}
 
    $("#PivotClient1").ejPivotClient({ serviceMethodSettings: { loadReport: "LoadReportFromDBMyMethod" } }); 
{% endhighlight %}

### serviceMethodSettings.removeDBReport `string`
{:#members:servicemethodsettings-removedbreport}

Allows you to set the custom name for the service method that is responsible to remove a report collection from the database.

#### Default Value: "RemoveReportFromDB"

**Example:**

{% highlight javascript %}
 
    $("#PivotClient1").ejPivotClient({ serviceMethodSettings: { removeDBReport: "RemoveReportFromMyDBMethod" } }); 
{% endhighlight %}

### serviceMethodSettings.renameDBReport `string`
{:#members:servicemethodsettings-renamedbreport}

Allows you to set the custom name for the service method that is responsible for renaming the report collection in the database.

#### Default Value: "RenameReportInDB"

**Example:**

{% highlight javascript %}
 
    $("#PivotClient1").ejPivotClient({ serviceMethodSettings: { renameDBReport: "RenameReportInMyDBMethod" } }); 
{% endhighlight %}

### serviceMethodSettings.mdxQuery `string`
{:#members:servicemethodsettings-mdxquery}

Allows you to set the custom name for the service method that is responsible for retrieving the MDX query for the current report.

>**Note**: This is applicable only with the bounded OLAP data.

#### Default Value: "GetMDXQuery"

**Example:**

{% highlight javascript %}
 
    $("#PivotClient1").ejPivotClient({ serviceMethodSettings: { mdxQuery: "GetMDXQueryMyMethod" } });
{% endhighlight %}

### serviceMethodSettings.measureGroupChanged `string`
{:#members:servicemethodsettings-measuregroupchanged}

Allows you to set the custom name for the service method that is responsible for updating the tree-view in the cube browser, while changing the measure group.

#### Default Value: "MeasureGroupChanged"

**Example:**

{% highlight javascript %}
 
    $("#PivotClient1").ejPivotClient({ serviceMethodSettings: { measureGroupChanged: "MeasureGroupChangedMyMethod" } }); 
{% endhighlight %}

### serviceMethodSettings.memberExpand `string`
{:#members:servicemethodsettings-memberexpand}

Allows you to set the custom name for the service method that is responsible to get the child members, on tree-view node expansion.

#### Default Value: "MemberExpanded"

**Example:**

{% highlight javascript %}
 
    $("#PivotClient1").ejPivotClient({ serviceMethodSettings: { memberExpand: "MemberExpandedMyMethod" } });
{% endhighlight %}

### serviceMethodSettings.nodeDropped `string`
{:#members:servicemethodsettings-nodedropped}

Allows you to set the custom name for the service method that is responsible for updating the report while dropping a node/split button in the axis element builder.

#### Default Value: "NodeDropped"

**Example:**

{% highlight javascript %}
 
    $("#PivotClient1").ejPivotClient({ serviceMethodSettings: { nodeDropped: "NodeDroppedMyMethod" } }); 
{% endhighlight %}

### serviceMethodSettings.removeSplitButton `string`
{:#members:servicemethodsettings-removesplitbutton}

Allows you to set the custom name for the service method that is responsible to update the report while removing the split button from the axis element builder.

#### Default Value: "RemoveSplitButton"

**Example:**

{% highlight javascript %}
 
    $("#PivotClient1").ejPivotClient({ serviceMethodSettings: { removeSplitButton: "RemoveSplitButtonMyMethod" } }); 
{% endhighlight %}

### serviceMethodSettings.saveReport `string`
{:#members:servicemethodsettings-savereport}

Allows you to set the custom name for the service method that is responsible for saving the report collection in the database.

#### Default Value: "SaveReportToDB"

**Example:**

{% highlight javascript %}
 
    $("#PivotClient1").ejPivotClient({ serviceMethodSettings: { saveReport: "SaveReportToDBMyMethod" } }); 
{% endhighlight %}

### serviceMethodSettings.toggleAxis `string`
{:#members:servicemethodsettings-toggleaxis}

Allows you to set the custom name for the service method that is responsible for toggling the elements in the row and column axes.

#### Default Value: "ToggleAxis"

**Example:**

{% highlight javascript %}
 
    $("#PivotClient1").ejPivotClient({ serviceMethodSettings: { toggleAxis: "ToggleAxisMyMethod" } });
{% endhighlight %}

### serviceMethodSettings.toolbarServices `string`
{:#members:servicemethodsettings-toolbarservices}

Allows you to set the custom name for the service method that is responsible for all the toolbar operations.

#### Default Value: "ToolbarOperations"

**Example:**

{% highlight javascript %}
 
    $("#PivotClient1").ejPivotClient({ serviceMethodSettings: { toolbarServices: "ToolbarOperationsMyMethod" } }); 
{% endhighlight %}

### serviceMethodSettings.updateReport `string`
{:#members:servicemethodsettings-updatereport}

Allows you to set the custom name for the service method that is responsible for updating the report collection.

#### Default Value: "UpdateReport"

**Example:**

{% highlight javascript %}
 
    $("#PivotClient1").ejPivotClient({  serviceMethodSettings: { updateReport: "UpdateReportFromMyMethod" } }); 
{% endhighlight %}

### serviceMethodSettings.paging `string`
{:#members:servicemethodsettings-paging}

Allows you to set the custom name for the service method while navigating between the pages in the paged pivot client.

#### Default Value: "Paging"

**Example:**

{% highlight javascript %}
 
    $("#PivotClient1").ejPivotClient({  serviceMethodSettings: { calculatedMember: "CalculatedMember" } }); 
{% endhighlight %}

### serviceMethodSettings.calculatedMember `string`
{:#members:servicemethodsettings-calculatedmember}

Allows you to set the custom name for the service method that is responsible for updating the report with the calculated member.

#### Default Value: "CalculatedMember"

**Example:**

{% highlight javascript %}
 
    $("#PivotClient1").ejPivotClient({  serviceMethodSettings: { paging: "PagingMyMethod" } }); 
{% endhighlight %}

### serviceMethodSettings.valueSorting `string`
{:#members:servicemethodsettings-valuesorting}

Allows you to set the custom name for the service method that is responsible for performing value sorting operation in the PivotClient.

#### Default Value: "ValueSorting"

**Example:**

{% highlight javascript %}
 
    $("#PivotClient1").ejPivotClient({ serviceMethodSettings: { valueSorting: "MyValueSorting" } });
{% endhighlight %}

### serviceMethodSettings.drillThroughHierarchies `string`
{:#members:servicemethodsettings-drillthroughhierarchies}

Allows you to set the custom name for the service method that is responsible for performing the drill through operation.

#### Default Value: "DrillThroughHierarchies"

**Example:**

{% highlight javascript %}
 
    $("#PivotClient1").ejPivotClient({ serviceMethodSettings: { drillThroughHierarchies: "MyDrillThroughHierarchiesMethod" } });
{% endhighlight %}

### serviceMethodSettings.drillThroughDataTable `string`
{:#members:servicemethodsettings-drillthroughdatatable}

Allows you to set the custom name for the service method that is responsible for performing the drill through operation in the data table.

#### Default Value: "DrillThroughDataTable"

**Example:**

{% highlight javascript %}
 
    $("#PivotClient1").ejPivotClient({ serviceMethodSettings: { drillThroughDataTable: "MyDrillThroughDataTableMethod" } });
{% endhighlight %}

### valueSortSettings `object`
{:#members:valueSortSettings}

Holds the necessary properties for value sorting.

>**Note**: This is applicable only for the relational datasource.

#### Default Value: {}

{% highlight javascript %}
 
    $("#PivotClient1").ejPivotClient({ valueSortSettings: { } }); 
{% endhighlight %}

### valueSortSettings.headerText `string`
{:#members:valueSortSettings-headerText}

Contains the header of the specific column to which value sorting is applied.

>**Note**: This is applicable only for the relational datasource.

#### Default Value: ""

{% highlight javascript %}
 
    $("#PivotClient1").ejPivotClient({ valueSortSettings: { headerText: "Bike##Amount" } });
{% endhighlight %}

### valueSortSettings.headerDelimiters `string`
{:#members:valueSortSettings-headerDelimiters}

Allows you to set the string for separating column headers provided in the **headerText** property.

>**Note**: This is applicable only for the relational datasource.

#### Default Value: ""

{% highlight javascript %}
 
    $("#PivotClient1").ejPivotClient({ valueSortSettings: { headerDelimiters: "##" } });
{% endhighlight %}

### valueSortSettings.sortOrder `enum`
{:#members:valueSortSettings-sortOrder}

<ts ref = "ej.PivotAnalysis.SortOrder"/>

Allows you to set the sorting order of values of the field.

>**Note**: This is applicable only for the relational datasource.

#### Default Value: ej.PivotAnalysis.SortOrder.Ascending

<table class="params">
    <thead>
        <tr>
            <th>Name</th>
            <th>Description</th>
        </tr>
    </thead>
    <tbody>
        <tr>
            <td class="name">Ascending</td>
            <td class="description">Sorts the members of the field in ascending order.</td>
        </tr>
        <tr>
            <td class="name">Descending</td>
            <td class="description">Sorts the members of the field in descending order.</td>
        </tr>
        <tr>
            <td class="name">None</td>
            <td class="description">Displays the members without sorting in default order.</td>
        </tr>
    </tbody>
</table>

{% highlight javascript %}
 
    $("#PivotClient1").ejPivotClient({ valueSortSettings: { sortOrder: ej.PivotAnalysis.SortOrder.Descending } });
{% endhighlight %}

### title `string`
{:#members:title}

Sets the title for the pivot client widget.

#### Default Value: ""

**Example:**

{% highlight javascript %}
 
    $("#PivotClient1").ejPivotClient({ title: "OLAP Browser" });
{% endhighlight %}

### url `string`
{:#members:url}

Connects the service using the specified URL for any server updates.

#### Default Value: ""

**Example:**

{% highlight javascript %}
 
    $("#PivotClient1").ejPivotClient({ url: "/wcf/OlapService" });
{% endhighlight %}

### enableCompleteDataExport `boolean`
{:#members:enableCompleteDataExport}

Allows you to export entire data instead of current page data, while paging option is enabled.

#### Default Value: false

**Example:**

{% highlight javascript %}
 
    $("#PivotClient1").ejPivotClient({ enableCompleteDataExport: true });
{% endhighlight %}

### enableXHRCredentials `boolean`
{:#members:enableXHRCredentials}

Allows you to enable "withCredentials" property inside XMLHttpRequest object for CORS(Cross-Origin Resource Sharing) request.

#### Default Value: false

**Example:**

{% highlight javascript %}
 
    $("#PivotClient1").ejPivotClient({ enableXHRCredentials: true });
{% endhighlight %}

## Methods

### doAjaxPost()
{:#methods:doajaxpost}

Performs an asynchronous HTTP (AJAX) request.

**Example:**

{% highlight javascript %}
 
    var clientObj = $("#PivotClient1").data("ejPivotClient");
    clientObj.doAjaxPost("POST", "/OlapService/Initialize", { "key", "Hello World" }, "renderControlSuccess", null);
{% endhighlight %}

### doPostBack()
{:#methods:dopostback}

Performs an asynchronous HTTP (full post) submit.

**Example:**

{% highlight javascript %}

    var clientObj = $("#PivotClient1").data("ejPivotClient");
    clientObj.doPostBack("/OlapService/Initialize", { "key", "Hello World" });
{% endhighlight %}

### refreshPagedPivotClient()
{:#methods:refreshpagedpivotclient}

Navigates to a specified page in the specified axis.

**Example:**

{% highlight javascript %}
 
    var clientObj = $("#PivotClient1").data("ejPivotClient");
    clientObj.refreshPagedPivotClient("series", 24);//Loads the 24th page in series axis
{% endhighlight %}

### refreshPagedPivotClientSuccess()
{:#methods:refreshpagedpivotclientsuccess}

Updates the pivot client component with the JSON data that is fetched from the service while navigating between the pages.

**Example:**

{% highlight javascript %}
 
    var clientObj = $("#PivotClient1").data("ejPivotClient");
    clientObj.refreshPagedPivotClientSuccess(jsonData); //jsonData object holds the JSON data required to render a specific page of the control.
{% endhighlight %}

### generateJSON()
{:#methods:generatejson}

Renders the pivot chart and the pivot grid with the provided JSON data.

**Example:**

{% highlight javascript %}
 
    var clientObj = $("#PivotClient1").data("ejPivotClient");
    clientObj.generateJSON(jsonData);//jsonData object holds the data in JSON format required to render the control
{% endhighlight %}

### refreshControl()
{:#methods:refreshcontrol}

Re-renders the control with the report at that instant.

> **Note**: This method can be used only for the client-side operation.

**Example:**

{% highlight javascript %}
 
    var clientObj = $("#PivotClient1").data("ejPivotClient");
    clientObj.refreshControl();
{% endhighlight %}

### getActiveTab()
{:#methods:getactivetab}

Returns the control tab string that displays currently in the pivot client.

**Example:**

{% highlight javascript %}
 
    var clientObj = $("#PivotClient1").data("ejPivotClient");
    var report = clientObj.getActiveTab();
{% endhighlight %}

### destroy()
{:#methods:destroy}

This function destroys all events of the pivot client widget bound using "this._on" and bring the control to pre-init state.

**Example:**

{% highlight javascript %}
 
    var clientObj = $("#PivotClient1").data("ejPivotClient");
    clientObj.destroy();
{% endhighlight %}

### getOlapReport()
{:#methods:getolapreport}

Returns the OLAP report string that is maintained along with the axis elements information.

#### Returns:

string

**Example:**

{% highlight javascript %}
 
    var clientObj = $("#PivotClient1").data("ejPivotClient");
    var report = clientObj.getOlapReport();
{% endhighlight %}

### setOlapReport()
{:#methods:setolapreport}

Sets the OLAP report string along with the axis information and maintains it in a property.

**Example:**

{% highlight javascript %}
 
    var clientObj = $("#PivotClient1").data("ejPivotClient");
    clientObj.setOlapReport(olapReportObj);
{% endhighlight %}

### getJSONRecords()
{:#methods:getjsonrecords}

Returns the formed JSON records to render the control.

#### Returns:

array

**Example:**

{% highlight javascript %}
 
    var clientObj = $("#PivotClient1").data("ejPivotClient");
    var jsonRecords = clientObj.getJSONRecords();
{% endhighlight %}

### setJSONRecords()
{:#methods:setjsonrecords}

Sets the formed JSON records to render the control to a property.

**Example:**

{% highlight javascript %}
 
    var clientObj = $("#PivotClient1").data("ejPivotClient");
    clientObj.setJSONRecords(jsonRecords);
{% endhighlight %}

## Events

### afterServiceInvoke
{:#events:afterserviceinvoke}

Triggers when it reaches the client-side after any AJAX request.

<table class="params">
<thead>
<tr>
<th colspan="3">Event Parameters</th>
</tr>
<tr>
<th>Name</th>
<th>Type</th>
<th>Description</th>
</tr>
</thead>
<tbody>
<tr>
<td class="name">action</td>
<td class="type">string</td>
<td class="description last">returns the current action of PivotClient control.</td>
</tr>
<tr>
<td class="name">customObject</td>
<td class="type">object</td>
<td class="description last">returns the custom object bounds with PivotClient control.</td>
</tr>
<tr>
<td class="name">element</td>
<td class="type">object</td>
<td class="description last">returns the HTML element of PivotClient control.</td>
</tr>
</tbody>
</table>

**Example:**

{% highlight javascript %}
 
    $("#PivotClient1").ejPivotClient({
        afterServiceInvoke: function(args) { }
    });
{% endhighlight %}



### beforeServiceInvoke
{:#events:beforeserviceinvoke}

Triggers before any AJAX request is passed from the client-side to the service methods.

<table class="params">
<thead>
<tr>
<th colspan="3">Event Parameters</th>
</tr>
<tr>
<th>Name</th>
<th>Type</th>
<th>Description</th>
</tr>
</thead>
<tbody>
<tr>
<td class="name">action</td>
<td class="type">string</td>
<td class="description last">returns the current action of PivotClient control.</td>
</tr>
<tr>
<td class="name">customObject</td>
<td class="type">object</td>
<td class="description last">returns the custom object bounds with PivotClient control.</td>
</tr>
<tr>
<td class="name">element</td>
<td class="type">object</td>
<td class="description last">returns the HTML element of PivotClient control.</td>
</tr>
</tbody>
</table>

**Example:**

{% highlight javascript %}
 
    $("#PivotClient1").ejPivotClient({
        beforeServiceInvoke: function(args) { }
    });
{% endhighlight %}

### saveReport
{:#events:savereport}

Triggers before saving the current collection of reports.

<table class="params">
<thead>
<tr>
<th colspan="3">Event Parameters</th>
</tr>
<tr>
<th>Name</th>
<th>Type</th>
<th>Description</th>
</tr>
</thead>
<tbody>
<tr>
<td class="name">targetControl</td>
<td class="type">object</td>
<td class="description last">returns the current instance of PivotClient control.</td>
</tr>
<tr>
<td class="name">saveReportSetting</td>
<td class="type">object</td>
<td class="description last">returns the object which holds the necessary parameters required for saving the report collection.</td>
</tr>
</tbody>
</table>

**Example:**

{% highlight javascript %}
 
    $("#PivotClient1").ejPivotClient({
        saveReport: function(args) { }
    });
{% endhighlight %}

### loadReport
{:#events:loadreport}

Triggers before loading the saved collection of reports.

<table class="params">
<thead>
<tr>
<th colspan="3">Event Parameters</th>
</tr>
<tr>
<th>Name</th>
<th>Type</th>
<th>Description</th>
</tr>
</thead>
<tbody>
<tr>
<td class="name">targetControl</td>
<td class="type">object</td>
<td class="description last">returns the current instance of PivotClient control.</td>
</tr>
<tr>
<td class="name">loadReportSetting</td>
<td class="type">object</td>
<td class="description last">returns the object which holds the necessary parameters required for loading a report collection from database.</td>
</tr>
</tbody>
</table>

**Example:**

{% highlight javascript %}
 
    $("#PivotClient1").ejPivotClient({
        loadReport: function(args) { }
    });

{% endhighlight %}

### fetchReport
{:#events:fetchreport}

Triggers before fetching the report collection from the storage.

<table class="params">
<thead>
<tr>
<th colspan="3">Event Parameters</th>
</tr>
<tr>
<th>Name</th>
<th>Type</th>
<th>Description</th>
</tr>
</thead>
<tbody>
<tr>
<td class="name">targetControl</td>
<td class="type">object</td>
<td class="description last">returns the current instance of PivotClient control.</td>
</tr>
<tr>
<td class="name">fetchReportSetting</td>
<td class="type">object</td>
<td class="description last">returns the object which holds the necessary parameters required for fetching the report names stored in database.</td>
</tr>
</tbody>
</table>

**Example:**

{% highlight javascript %}
 
    $("#PivotClient1").ejPivotClient({
        fetchReport: function(args) { }
    });

{% endhighlight %}

### beforeExport
{:#events:beforeexport}

Triggers before exporting the control.

<table class="params">
<thead>
<tr>
<th colspan="3">Event Parameters</th>
</tr>
<tr>
<th>Name</th>
<th>Type</th>
<th>Description</th>
</tr>
</thead>
<tbody>
<tr>
<td class="name">url</td>
<td class="type">string</td>
<td class="description last">holds the url of the service method responsible for exporting the PivotClient control.</td>
</tr>
<tr>
<td class="name">fileName</td>
<td class="type">string</td>
<td class="description last">holds the name of the file to be exported.</td>
</tr>
</tbody>
</table>

**Example:**

{% highlight javascript %}
 
    $("#PivotClient1").ejPivotClient({
        beforeExport: function(args) { }
    });
{% endhighlight %}

### chartLoad
{:#events:chartload}

Triggers before rendering the pivot chart.

<table class="params">
<thead>
<tr>
<th colspan="3">Event Parameters</th>
</tr>
<tr>
<th>Name</th>
<th>Type</th>
<th>Description</th>
</tr>
</thead>
<tbody>
<tr>
<td class="name">action</td>
<td class="type">string</td>
<td class="description last">returns the current action of PivotChart control.</td>
</tr>
<tr>
<td class="name">customObject</td>
<td class="type">object</td>
<td class="description last">returns the custom object bound with PivotChart control.</td>
</tr>
<tr>
<td class="name">element</td>
<td class="type">object</td>
<td class="description last">returns the HTML element of PivotChart control.</td>
</tr>
</tbody>
</table>
</td>
</tr>
</tbody>
</table>

**Example:**

{% highlight javascript %}
 
    $("#PivotClient1").ejPivotClient({
        chartLoad: function (args) { }
    });      

{% endhighlight %}

### schemaLoad
{:#events:schemaload}

Triggers before rendering the pivot schema designer.

<table class="params">
<thead>
<tr>
<th colspan="3">Event Parameters</th>
</tr>
<tr>
<th>Name</th>
<th>Type</th>
<th>Description</th>
</tr>
</thead>
<tbody>
<tr>
<td class="name">action</td>
<td class="type">string</td>
<td class="description last">returns the current action of PivotSchemaDesigner control.</td>
</tr>
</thead>
<tbody>
<tr>
<td class="name">element</td>
<td class="type">object</td>
<td class="description last">returns the HTML element of PivotSchemaDesigner control.</td>
</tr>
</tbody>
</table>
</td>
</tr>
</tbody>
</table>

**Example:**

{% highlight javascript %}
 
    $("#PivotClient1").ejPivotClient({
        schemaLoad: function (args) { }
    });      

{% endhighlight %}

### treeMapLoad
{:#events:treemapload}

Triggers before rendering the pivot tree map.

<table class="params">
<thead>
<tr>
<th colspan="3">Event Parameters</th>
</tr>
<tr>
<th>Name</th>
<th>Type</th>
<th>Description</th>
</tr>
</thead>
<tbody>
<tr>
<td class="name">action</td>
<td class="type">string</td>
<td class="description last">returns the current action of PivotTreeMap control.</td>
</tr>
<tr>
<td class="name">customObject</td>
<td class="type">object</td>
<td class="description last">returns the custom object bound with PivotTreeMap control.</td>
</tr>
<tr>
<td class="name">element</td>
<td class="type">object</td>
<td class="description last">returns the HTML element of PivotTreeMap control.</td>
</tr>
</tbody>
</table>

**Example:**

{% highlight javascript %}
 
    $("#PivotClient1").ejPivotClient({
        treeMapLoad: function (args) { }
    });
{% endhighlight %}

## gridDrillSuccess
{:#events:griddrillsuccess}

Triggers when performing the drill up/down operation on the row/columns headers.

<table class="params">
<thead>
<tr>
<th colspan="3">Event Parameters</th>
</tr>
<tr>
<th>Name</th>
<th>Type</th>
<th>Description</th>
</tr>
</thead>
<tbody>
<tr>
<td class="name">type</td>
<td class="type">string</td>
<td class="description last">returns the current action of PivotClient control.</td>
</tr>
<tr>
<td class="name">axis</td>
<td class="type">string</td>
<td class="description last">returns the axis class name of the drilled cell in PivotGrid.</td>
</tr>
<tr>
<td class="name">cellPosition</td>
<td class="type">string</td>
<td class="description last">returns the position of the drilled cell.</td>
</tr>
<tr>
<td class="name">drillAction</td>
<td class="type">string</td>
<td class="description last">returns the drill action name.</td>
</tr>
<tr>
<td class="name">drilledMember</td>
<td class="type">string</td>
<td class="description last">returns the drilled cell string.</td>
</tr>
<tr>
<td class="name">fieldName</td>
<td class="type">string</td>
<td class="description last">returns the field/item name of the drilled cell.</td>
</tr>
<tr>
<td class="name">model</td>
<td class="type">object</td>
<td class="description last">returns the model object bound with PivotClient control.</td>
</tr>
<tr>
<td class="name">gridObj</td>
<td class="type">object</td>
<td class="description last">returns the object bound with PivotGrid control.</td>
</tr>
</tbody>
</table>

**Example:**

{% highlight javascript %}
 
    $("#PivotClient1").ejPivotClient({
        gridDrillSuccess: function (args) { }
    });

{% endhighlight %}

## chartDrillSuccess
{:#events:chartdrillsuccess}

Triggers when performing the drill operation on the chart series.

<table class="params">
<thead>
<tr>
<th colspan="3">Event Parameters</th>
</tr>
<tr>
<th>Name</th>
<th>Type</th>
<th>Description</th>
</tr>
</thead>
<tbody>
<tr>
<td class="name">type</td>
<td class="type">string</td>
<td class="description last">returns the current action of PivotClient control.</td>
</tr>
<tr>
<td class="name">element</td>
<td class="type">object</td>
<td class="description last">returns the HTML element of PivotChart control.</td>
</tr>
<tr>
<td class="name">model</td>
<td class="type">object</td>
<td class="description last">returns the model object bound with PivotClient control.</td>
</tr>
</tbody>
</table>

**Example:**

{% highlight javascript %}
 
    $("#PivotClient1").ejPivotClient({
        chartDrillSuccess: function (args) { }
    });

{% endhighlight %}

## treeMapDrillSuccess
{:#events:treemapdrillsuccess}

Triggers when performing the drill operation on the tree map.
<table class="params">
<thead>
<tr>
<th colspan="3">Event Parameters</th>
</tr>
<tr>
<th>Name</th>
<th>Type</th>
<th>Description</th>
</tr>
</thead>
<tbody>
<tr>
<td class="name">type</td>
<td class="type">string</td>
<td class="description last">returns the current action of PivotClient control.</td>
</tr>
<tr>
<td class="name">element</td>
<td class="type">object</td>
<td class="description last">returns the HTML element of PivotTreeMap control.</td>
</tr>
<tr>
<td class="name">model</td>
<td class="type">object</td>
<td class="description last">returns the model object bound with PivotTreeMap control.</td>
</tr>
</tbody>
</table>

**Example:**

{% highlight javascript %}
 
    $("#PivotClient1").ejPivotClient({
        treeMapDrillSuccess: function (args) { }
    });

{% endhighlight %}

### valueCellHyperlinkClick
{:#events:valuecellhyperlinkclick}

Triggers when clicking any value cell in the pivot grid.

<table class="params">
<thead>
<tr>
<th colspan="3">Event Parameters</th>
</tr>
<tr>
<th>Name</th>
<th>Type</th>
<th>Description</th>
</tr>
</thead>
<tbody>
<tr>
<td class="name">type</td>
<td class="type">string</td>
<td class="description last">returns the current action of PivotClient control.</td>
</tr>
<tr>
<td class="name">args</td>
<td class="type">object</td>
<td class="description last">returns the clicked cell information.</td>
</tr>
<tr>
<td class="name">customerObject</td>
<td class="type">object</td>
<td class="description last">returns the custom object bounds with PivotClient control.</td>
</tr>
<tr>
<td class="name">element</td>
<td class="type">object</td>
<td class="description last">returns the HTML element of PivotGrid control.</td>
</tr>
<tr>
<td class="name">model</td>
<td class="type">object</td>
<td class="description last">returns the model object bound with PivotClient control.</td>
</tr>
</tbody>
</table>

**Example:**

{% highlight javascript %}
 
    $("#PivotClient1").ejPivotClient({
        valueCellHyperlinkClick: function (args) { }
    });

{% endhighlight %}
 
## rowHeaderHyperlinkClick
{:#events:rowheaderhyperlinkclick}

Triggers when clicking any row header cell in the pivot grid.

<table class="params">
<thead>
<tr>
<th colspan="3">Event Parameters</th>
</tr>
<tr>
<th>Name</th>
<th>Type</th>
<th>Description</th>
</tr>
</thead>
<tbody>
<tr>
<td class="name">type</td>
<td class="type">string</td>
<td class="description last">returns the current action of PivotClient control.</td>
</tr>
<tr>
<td class="name">args</td>
<td class="type">object</td>
<td class="description last">returns the clicked cell information.</td>
</tr>
<tr>
<td class="name">customerObject</td>
<td class="type">object</td>
<td class="description last">returns the custom object bounds with PivotClient control.</td>
</tr>
<tr>
<td class="name">element</td>
<td class="type">object</td>
<td class="description last">returns the HTML element of PivotGrid control.</td>
</tr>
<tr>
<td class="name">model</td>
<td class="type">object</td>
<td class="description last">returns the model object bound with PivotClient control.</td>
</tr>
</tbody>
</table>

**Example:**

{% highlight javascript %}
 
    $("#PivotClient1").ejPivotClient({
        rowHeaderHyperlinkClick: function (args) { }
    });

{% endhighlight %}
 
## columnHeaderHyperlinkClick
{:#events:columnheaderhyperlinkclick}

Triggers when clicking any column header cell in the pivot grid.

<table class="params">
<thead>
<tr>
<th colspan="3">Event Parameters</th>
</tr>
<tr>
<th>Name</th>
<th>Type</th>
<th>Description</th>
</tr>
</thead>
<tbody>
<tr>
<td class="name">type</td>
<td class="type">string</td>
<td class="description last">returns the current action of PivotClient control.</td>
</tr>
<tr>
<td class="name">args</td>
<td class="type">object</td>
<td class="description last">returns the clicked cell information.</td>
</tr>
<tr>
<td class="name">customerObject</td>
<td class="type">object</td>
<td class="description last">returns the custom object bounds with PivotClient control.</td>
</tr>
<tr>
<td class="name">element</td>
<td class="type">object</td>
<td class="description last">returns the HTML element of PivotGrid control.</td>
</tr>
<tr>
<td class="name">model</td>
<td class="type">object</td>
<td class="description last">returns the model object bound with PivotClient control.</td>
</tr>
</tbody>
</table>

**Example:**

{% highlight javascript %}
 
    $("#PivotClient1").ejPivotClient({
        columnHeaderHyperlinkClick: function (args) { }
    });

{% endhighlight %}
 
## summaryCellHyperlinkClick
{:#events:summarycellhyperlinkclick}

Triggers when clicking any summary cell in the pivot grid.

<table class="params">
<thead>
<tr>
<th colspan="3">Event Parameters</th>
</tr>
<tr>
<th>Name</th>
<th>Type</th>
<th>Description</th>
</tr>
</thead>
<tbody>
<tr>
<td class="name">type</td>
<td class="type">string</td>
<td class="description last">returns the current action of PivotClient control.</td>
</tr>
<tr>
<td class="name">args</td>
<td class="type">object</td>
<td class="description last">returns the clicked cell information.</td>
</tr>
<tr>
<td class="name">customerObject</td>
<td class="type">object</td>
<td class="description last">returns the custom object bounds with PivotClient control.</td>
</tr>
<tr>
<td class="name">element</td>
<td class="type">object</td>
<td class="description last">returns the HTML element of PivotGrid control.</td>
</tr>
<tr>
<td class="name">model</td>
<td class="type">object</td>
<td class="description last">returns the model object bound with PivotClient control.</td>
</tr>
</tbody>
</table>

**Example:**

{% highlight javascript %}
 
    $("#PivotClient1").ejPivotClient({
        summaryCellHyperlinkClick: function (args) { }
    });

{% endhighlight %}
 
## cellContext
{:#events:cellcontext}

Triggers when right-clicking a cell in the pivot grid.

<table class="params">
<thead>
<tr>
<th colspan="3">Event Parameters</th>
</tr>
<tr>
<th>Name</th>
<th>Type</th>
<th>Description</th>
</tr>
</thead>
<tbody>
<tr>
<td class="name">type</td>
<td class="type">string</td>
<td class="description last">returns the current action of PivotClient control.</td>
</tr>
<tr>
<td class="name">cellType</td>
<td class="type">string</td>
<td class="description last">returns the clicked cell type in PivotGrid.</td>
</tr>
<tr>
<td class="name">cellPosition</td>
<td class="type">string</td>
<td class="description last">returns the position of the clicked cell.</td>
</tr>
<tr>
<td class="name">cellValue</td>
<td class="type">string</td>
<td class="description last">returns the HTML string of the clicked cell.</td>
</tr>
<tr>
<td class="name">rawdata</td>
<td class="type">string</td>
<td class="description last">returns the clicked cell string.</td>
</tr>
<tr>
<td class="name">role</td>
<td class="type">string</td>
<td class="description last">returns the role of the clicked cell.</td>
</tr>
<tr>
<td class="name">uniqueName</td>
<td class="type">string</td>
<td class="description last">returns the unique name of the clicked cell.</td>
</tr>
<tr>
<td class="name">model</td>
<td class="type">object</td>
<td class="description last">returns the model object bound with PivotClient control.</td>
</tr>
</tbody>
</table>

**Example:**

{% highlight javascript %}
 
    $("#PivotClient1").ejPivotClient({
        cellContext: function (args) { }
    });

{% endhighlight %}
 
## cellSelection
{:#events:cellselection}

Triggers when select/click any of the cell in the pivot grid.

<table class="params">
<thead>
<tr>
<th colspan="3">Event Parameters</th>
</tr>
<tr>
<th>Name</th>
<th>Type</th>
<th>Description</th>
</tr>
</thead>
<tbody>
<tr>
<td class="name">type</td>
<td class="type">string</td>
<td class="description last">returns the current action of PivotClient control.</td>
</tr>
<tr>
<td class="name">JSONRecords</td>
<td class="type">array</td>
<td class="description last">returns the JSON information of the clicked cell.</td>
</tr>
<tr>
<td class="name">model</td>
<td class="type">object</td>
<td class="description last">returns the model object bound with PivotClient control.</td>
</tr>
</tbody>
</table>

**Example:**

{% highlight javascript %}
 
    $("#PivotClient1").ejPivotClient({
        cellSelection: function (args) { }
    });

{% endhighlight %}
 
## cellEdit
{:#events:celledit}

Triggers when any of the value cell is edited in the pivot grid.

<table class="params">
<thead>
<tr>
<th colspan="3">Event Parameters</th>
</tr>
<tr>
<th>Name</th>
<th>Type</th>
<th>Description</th>
</tr>
</thead>
<tbody>
<tr>
<td class="name">type</td>
<td class="type">string</td>
<td class="description last">returns the current action of PivotClient control.</td>
</tr>
<tr>
<td class="name">editCellsInfo</td>
<td class="type">object</td>
<td class="description last">returns the edited cell information.</td>
</tr>
<tr>
<td class="name">model</td>
<td class="type">object</td>
<td class="description last">returns the model object bound with PivotClient control.</td>
</tr>
</tbody>
</table>

**Example:**

{% highlight javascript %}
 
    $("#PivotClient1").ejPivotClient({
        cellEdit: function (args) { }
    });

{% endhighlight %}

### cellClick
{:#events:cellclick}

Triggers when click action is performed over a grid value cell.

<table class="params">
<thead>
<tr>
<th colspan="3">Event Parameters</th>
</tr>
<tr>
<th>Name</th>
<th>Type</th>
<th>Description</th>
</tr>
</thead>
<tbody>
<tr>
<td class="name">selectedData</td>
<td class="type">array</td>
<td class="description last">returns the JSON details of the respective on cell.</td>
</tr>
<tr>
<td class="name">customObject</td>
<td class="type">object</td>
<td class="description last">returns the custom object bound with PivotClient control.</td>
</tr>
<tr>
<td class="name">element</td>
<td class="type">object</td>
<td class="description last">returns the HTML element of PivotGrid control.</td>
</tr>
</tbody>
</table>

**Example:**

{% highlight javascript %}
 
    $("#PivotClient1").ejPivotClient({
        cellClick: function (args) {}
    });
{% endhighlight %}

## cellDoubleClick
{:#events:celldoubleclick}

Triggers when double-click on any of the value cell in the pivot grid.

<table class="params">
<thead>
<tr>
<th colspan="3">Event Parameters</th>
</tr>
<tr>
<th>Name</th>
<th>Type</th>
<th>Description</th>
</tr>
</thead>
<tbody>
<tr>
<td class="name">type</td>
<td class="type">string</td>
<td class="description last">returns the current action of PivotClient control.</td>
</tr>
<tr>
<td class="name">customerObject</td>
<td class="type">object</td>
<td class="description last">returns the custom object bounds with PivotClient control.</td>
</tr>
<tr>
<td class="name">element</td>
<td class="type">object</td>
<td class="description last">returns the HTML element of PivotGrid control.</td>
</tr>
<tr>
<td class="name">model</td>
<td class="type">object</td>
<td class="description last">returns the model object bound with PivotClient control.</td>
</tr>
<tr>
<td class="name">selectedData</td>
<td class="type">array</td>
<td class="description last">returns the array of selected data source object for the clicked value cell.</td>
</tr>
</tbody>
</table>

**Example:**

{% highlight javascript %}
 
    $("#PivotClient1").ejPivotClient({
        cellDoubleClick: function (args) { }
    });

{% endhighlight %}
 
### pointRegionClick
{:#events:pointregionclick}

Triggers when clicking on any chart series points in the pivot chart.

<table class="params">
<thead>
<tr>
<th colspan="3">Event Parameters</th>
</tr>
<tr>
<th>Name</th>
<th>Type</th>
<th>Description</th>
</tr>
</thead>
<tbody>
<tr>
<td class="name">type</td>
<td class="type">string</td>
<td class="description last">returns the current action of PivotClient control.</td>
</tr>
<tr>
<td class="name">data</td>
<td class="type">object</td>
<td class="description last">returns the clicked Chart series points information.</td>
</tr>
<tr>
<td class="name">model</td>
<td class="type">object</td>
<td class="description last">returns the model object bound with PivotClient control.</td>
</tr>
</tbody>
</table>

**Example:**

{% highlight javascript %}
 
    $("#PivotClient1").ejPivotClient({
        pointRegionClick: function (args) { }
    });

{% endhighlight %}
  
### axesLabelRendering
{:#events:axeslabelrendering}

Triggers before the chart label is rendered in the pivot chart.

<table class="params">
<thead>
<tr>
<th colspan="3">Event Parameters</th>
</tr>
<tr>
<th>Name</th>
<th>Type</th>
<th>Description</th>
</tr>
</thead>
<tbody>
<tr>
<td class="name">type</td>
<td class="type">string</td>
<td class="description last">returns the current action of PivotClient control.</td>
</tr>
<tr>
<td class="name">data</td>
<td class="type">object</td>
<td class="description last">returns the Chart label information.</td>
</tr>
<tr>
<td class="name">model</td>
<td class="type">object</td>
<td class="description last">returns the model object bound with PivotClient control.</td>
</tr>
</tbody>
</table>

**Example:**

{% highlight javascript %}
 
    $("#PivotClient1").ejPivotClient({
        axesLabelRendering: function (args) { }
    });

{% endhighlight %}
 
### drillThrough
{:#events:drillthrough}

Triggers while clicking the value cells in the pivot grid.

<table class="params">
<thead>
<tr>
<th colspan="3">Event Parameters</th>
</tr>
<tr>
<th>Name</th>
<th>Type</th>
<th>Description</th>
</tr>
</thead>
<tbody>
<tr>
<td class="name">data</td>
<td class="type">object</td>
<td class="description last">return the JSON records of the generated cells on drill-through operation.</td>
</tr>
<tr>
<td class="name">element</td>
<td class="type">object</td>
<td class="description last">returns the HTML element of PivotClient.</td>
</tr>
</tbody>
</table>

**Example:**

{% highlight javascript %}
 
    $("#PivotClient1").ejPivotClient({
        drillThrough: function (args) {}
    });
{% endhighlight %}

### load
{:#events:load}

Triggers while initiating the loading of the widget.

<table class="params">
<thead>
<tr>
<th colspan="3">Event Parameters</th>
</tr>
<tr>
<th>Name</th>
<th>Type</th>
<th>Description</th>
</tr>
</thead>
<tbody>
<tr>
<td class="name">element</td>
<td class="type">object</td>
<td class="description last">returns the HTML element of PivotClient component.</td>
</tr>
<tr>
<td class="name">customObject</td>
<td class="type">object</td>
<td class="description last">returns the custom object bound with PivotTreeMap control.</td>
</tr>
</tbody>
</table>

**Example:**

{% highlight javascript %}
 
    $("#PivotClient1").ejPivotClient({
        load: function (args) { }
    });
{% endhighlight %}


### renderComplete
{:#events:rendercomplete}

Triggers when the pivot client widget completes all operations at client-end after any AJAX request.

<table class="params">
<thead>
<tr>
<th colspan="3">Event Parameters</th>
</tr>
<tr>
<th>Name</th>
<th>Type</th>
<th>Description</th>
</tr>
</thead>
<tbody>
<tr>
<td class="name">element</td>
<td class="type">object</td>
<td class="description last">returns the HTML element of PivotClient component.</td>
</tr>
<tr>
<td class="name">customObject</td>
<td class="type">object</td>
<td class="description last">returns the custom object bound with PivotTreeMap control.</td>
</tr>
</tbody>
</table>

**Example:**

{% highlight javascript %}
 
    $("#PivotClient1").ejPivotClient({
        renderComplete: function (args) { }
    });
{% endhighlight %}

### renderFailure
{:#events:renderfailure}

Triggers when any error is occurred during the AJAX request.

<table class="params">
<thead>
<tr>
<th colspan="3">Event Parameters</th>
</tr>
<tr>
<th>Name</th>
<th>Type</th>
<th>Description</th>
</tr>
</thead>
<tbody>
<tr>
<td class="name">customObject</td>
<td class="type">object</td>
<td class="description last">returns the custom object bound with the control.</td>
</tr>
<tr>
<td class="name">element</td>
<td class="type">object</td>
<td class="description last">returns the HTML element of PivotClient control.</td>
</tr>
<tr>
<td class="name">message</td>
<td class="type">string</td>
<td class="description last">returns the error message with error code.</td>
</tr>
</tbody>
</table>

**Example:**

{% highlight javascript %}
 
    $("#PivotClient1").ejPivotClient({
        renderFailure: function (args) { }
    });     

{% endhighlight %}

### renderSuccess
{:#events:rendersuccess}

Triggers when the pivot client is completely rendered.

<table class="params">
<thead>
<tr>
<th colspan="3">Event Parameters</th>
</tr>
<tr>
<th>Name</th>
<th>Type</th>
<th>Description</th>
</tr>
</thead>
<tbody>
<tr>
<td class="name">args</td>
<td class="type">object</td>
<td class="description last">returns the object of PivotClient control at that instant.</td>
</tr>
</tbody>
</table>

**Example:**

{% highlight javascript %}
 
    $("#PivotClient1").ejPivotClient({
        renderSuccess: function (args) { }
    });      

{% endhighlight %}

