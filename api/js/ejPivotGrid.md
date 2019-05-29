---
layout: post
title: Properties, Methods and Events of Syncfusion ejPivotGrid Widget
description: Methods,members and events available in ejPivotGrid
documentation: UG
platform: js-api
keywords: ejPivotGrid, API, Essential JS PivotGrid
metaname: API reference for ejPivotGrid
metacontent: ejPivotGrid, API, Essential JS PivotGrid
---

# PivotGrid

The PivotGrid control is easily configurable, presentation-quality business control that reads OLAP data from a Microsoft SQL Server Analysis Services database, an offline cube, XML/A, or relational datasource.

#### Syntax

{% highlight javascript %}

    $(element).ejPivotGrid()
{% endhighlight %}

#### Example

{% highlight html %}
 
    <div id="PivotGrid1"> </div> 
    
    <script>
        //Create PivotGrid
        $("#PivotGrid1").ejPivotGrid(...);       
    </script>

{% endhighlight %}

#### Requires

* module:jQuery-3.0.0.min.js
* module:ej.core.js
* module:ej.data.js
* module:ej.touch.js
* module:ej.waitingpopup.js
* module:ej.pivot.common.js
* module:ej.pivotanalysis.base.js
* module:ej.olap.base.js
* module:ej.pivotgrid.js
* module:ej.pivotpager.js


## Members

### analysisMode `enum`
{:#members:analysismode}

<ts name = "ej.Pivot.AnalysisMode"/>

Sets the mode for the PivotGrid widget to bind either OLAP or relational data source.

<table class="params">
    <thead>
        <tr>
            <th>Name</th>
            <th>Description</th>
        </tr>
    </thead>
    <tbody>
        <tr>
            <td class="name">OLAP</td>
            <td class="description">To bind an OLAP data source to PivotGrid.</td>
        </tr>
        <tr>
            <td class="name">Pivot</td>
            <td class="description">To bind a relational data source to PivotGrid.</td>
        </tr>
    </tbody>
</table>

#### Default Value: ej.Pivot.AnalysisMode.Pivot

**Example:**

{% highlight javascript %}
 
    $("#PivotGrid1").ejPivotGrid({ analysisMode: ej.Pivot.AnalysisMode.Olap });
{% endhighlight %}


### cssClass `string`
{:#members:cssclass}

Specifies the CSS class to the PivotGrid for achieving the custom theme.

#### Default Value: “”

**Example:**

{% highlight javascript %}
 
    $("#PivotGrid1").ejPivotGrid({ cssClass: "gradient-lime" });
{% endhighlight %}

### pivotTableFieldListID `string`
{:#members:pivottablefieldlistid}

Connects the PivotSchemaDesigner with specified ID to the PivotGrid control.

#### Default Value: “”

**Example:**

{% highlight javascript %}
 
    $("#PivotGrid1").ejPivotGrid({ pivotTableFieldListID: "PivotTableFieldListID" });
{% endhighlight %}

### dataSource `object`
{:#members:datasource}

Initializes the data source for the PivotGrid widget, when it functions completely on client-side.

#### Default Value: {}

**Example:**

{% highlight javascript %}
 
    $("#PivotGrid1").ejPivotGrid( { dataSource: { data: value } });
{% endhighlight %}

### dataSource.columns `array`
{:#members:datasource-columns}

Lists out the items to be arranged in the columns section of the PivotGrid.

#### Default Value: []

**Example:**

{% highlight javascript %}
 
    $("#PivotGrid1").ejPivotGrid({ dataSource: { columns: itemsArray } });
{% endhighlight %}


### dataSource.columns.fieldName `string`
{:#members:datasource-columns-fieldname}

Allows you to bind the item by using its unique name as field name.

#### Default Value: ""

**Example:**

{% highlight javascript %}
 
    $("#PivotGrid1").ejPivotGrid({ dataSource: { columns: [{ fieldName : "MyFieldName" }] } });
{% endhighlight %}

### dataSource.columns.fieldCaption `string`
{:#members:datasource-columns-fieldcaption}

Allows you to set the display caption for an item.

#### Default Value: ""

**Example:**

{% highlight javascript %}
 
    $("#PivotGrid1").ejPivotGrid({ dataSource: { columns: [{ fieldCaption : "MyFieldCaption" }] } });
{% endhighlight %}

### dataSource.columns.advancedFilter `array`
{:#members:datasource-columns-advancedfilter}

Allows you to filter the report by using advanced filtering (e.g., Microsoft Excel) option for the OLAP data source in client-mode.

#### Default Value: []

**Example:**

{% highlight javascript %}
 
    $("#PivotGrid1").ejPivotGrid({ dataSource: { columns: [{ advancedFilter : itemArray }] } });
{% endhighlight %}

### dataSource.columns.advancedFilter.name `string`
{:#members:datasource-columns-advancedfilter-name}

Allows you to provide a level unique name to perform the advanced filtering.

#### Default Value: ""

**Example:**

{% highlight javascript %}
 
    $("#PivotGrid1").ejPivotGrid({ dataSource: { columns: [{ advancedFilter : [{ name: "levelUniqueName" }] }] } });
{% endhighlight %}

### dataSource.columns.advancedFilter.labelFilterOperator `string`
{:#members:datasource-columns-advancedfilter-labelfilteroperator}

Allows you to set the operator to perform the label filtering.

#### Default Value: "none"

**Example:**

{% highlight javascript %}
 
    $("#PivotGrid1").ejPivotGrid({ dataSource: { columns: [{ advancedFilter : [{ labelFilterOperator: ej.olap.LabelFilterOptions.EndsWith }] }] } });
{% endhighlight %}

### dataSource.columns.advancedFilter.valueFilterOperator `string`
{:#members:datasource-columns-advancedfilter-valuefilteroperator}

Allows you to set the operator to perform the value filtering.

#### Default Value: "none"

**Example:**

{% highlight javascript %}
 
    $("#PivotGrid1").ejPivotGrid({ dataSource: { columns: [{ advancedFilter : [{ valueFilterOperator: ej.olap.ValueFilterOptions.Between }] }] } });
{% endhighlight %}

### dataSource.columns.advancedFilter.advancedFilterType `string`
{:#members:datasource-columns-advancedfilter-advancedfiltertype}

Allows you to set the filtering type while performing the advanced filtering.

#### Default Value: ""

**Example:**

{% highlight javascript %}
 
    $("#PivotGrid1").ejPivotGrid({ dataSource: { columns: [{ advancedFilter : [{ advancedFilterType:  ej.olap.AdvancedFilterType.LabelFilter }] }] } });
{% endhighlight %}

### dataSource.columns.advancedFilter.measure `string`
{:#members:datasource-columns-advancedfilter-measure}

In value filtering, this property contains the measure name to which the filter is applied.

#### Default Value: ""

**Example:**

{% highlight javascript %}
 
    $("#PivotGrid1").ejPivotGrid({ dataSource: { columns: [{ advancedFilter : [{ measure: "measureUniqueName", advancedFilterType: ej.olap.AdvancedFilterType.ValueFilter }] }] } });
{% endhighlight %}

### dataSource.columns.advancedFilter.values `array`
{:#members:datasource-columns-advancedfilter-values}

Allows you to hold filter operand values in the advanced filtering.

#### Default Value: ""

**Example:**

{% highlight javascript %}
    
    //For Label Filters
    $("#PivotGrid1").ejPivotGrid({ dataSource: { columns: [{ advancedFilter : [{ labelFilterOperator: ej.olap.LabelFilterOptions.EndsWith, values:  ["002"] }] }] } });
    
    //For Value Filters
    $("#PivotGrid1").ejPivotGrid({ dataSource: { columns: [{ advancedFilter : [{ valueFilterOperator: ej.olap.ValueFilterOptions.GreaterThan, values:  ["200"] }] }] } });
{% endhighlight %}


### dataSource.columns.isNamedSets `boolean`
{:#members:datasource-columns-isnamedsets}

Allows you to indicate whether the added item is a named set or not. 

> **Note**: This is only applicable for the OLAP datasource.

#### Default Value: false

**Example:**

{% highlight javascript %}
 
    $("#PivotGrid1").ejPivotGrid({ dataSource: { columns: [{ fieldName: "[Core Product Group]", isNamedSets : true }] } });
{% endhighlight %}

### dataSource.columns.showSubTotal `boolean`
{:#members:datasource-columns-showsubtotal}

Shows/hides the sub-total of the field in PivotGrid.

>**Note**: This is applicable only for the relational datasource.

#### Default Value: true

**Example:**

{% highlight javascript %}
 
    $("#PivotGrid1").ejPivotGrid({ dataSource: { columns: [{ fieldName: "Country", showSubTotal : false }] } });
{% endhighlight %}

### dataSource.columns.format `string`
{:#members:datasource-columns-format}

Allows you to set the format for column headers.

>**Note**: This is applicable only for the relational datasource.

#### Default Value: ""

**Example:**

{% highlight javascript %}
 
    $("#PivotGrid1").ejPivotGrid({ dataSource: { columns: [{ format : "date" }] } });
{% endhighlight %}

### dataSource.columns.formatString `string`
{:#members:datasource-columns-formatstring}

This property is set to display the formatted values with format types in the PivotGrid.

#### Default Value: ""

**Example:**

{% highlight javascript %}
 
    $("#PivotGrid1").ejPivotGrid({ dataSource: { columns: [{ formatString : "MM/DD/YYYY" }] } });
{% endhighlight %}

### dataSource.columns.cssClass `string`
{:#members:datasource-columns-cssclass}

Allows you to set the custom theme for column headers.

>**Note**: This is applicable only for the relational datasource.

#### Default Value: ""

**Example:**

{% highlight javascript %}
 
    $("#PivotGrid1").ejPivotGrid({ dataSource: { columns: [{ cssClass : "className" }] } });
{% endhighlight %}

### dataSource.columns.delimiter `string`
{:#members:datasource-columns-delimiter}

Allows you to set the delimiter for date type format in the **formatString**. This is applicable for the **groupByDate** of row/column headers.

>**Note**: This is applicable only for the relational datasource with ClientMode.

#### Default Value: ""

**Example:**

{% highlight javascript %}
 
    $("#PivotGrid1").ejPivotGrid({ dataSource: { columns: [{ delimiter : "-" }] } });
{% endhighlight %}

### dataSource.columns.sortOrder `enum`
{:#members:datasource-columns-sortorder}

<ts name = "ej.PivotAnalysis.SortOrder"/>

Allows you to set the sorting order of members of the field.

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

**Example:**

{% highlight javascript %}
 
    $("#PivotGrid1").ejPivotGrid({ dataSource: { columns: [{ fieldName: "Country", sortOrder: ej.PivotAnalysis.SortOrder.Descending }] } });
{% endhighlight %}

### dataSource.columns.drilledItems `array`
{:#members:datasource-columns-drilleditems}

Contains the list of members need to be drilled down by default in the field.

#### Default Value: []

**Example:**

{% highlight javascript %}
 
    $("#PivotGrid1").ejPivotGrid({ dataSource: { columns: [{ fieldName: "Country", drilledItems: ["Canada", "France"] }] } });
{% endhighlight %}

### dataSource.columns.filterItems `object`
{:#members:datasource-columns-filteritems}

Applies the filter to field members.

#### Default Value: null

**Example:**

{% highlight javascript %}
 
    $("#PivotGrid1").ejPivotGrid({ dataSource: { columns: [{ fieldName: "Country", filterItems: { filterType: ej.PivotAnalysis.FilterType.Exclude, values: ["Canada", "France"] } }] } });
{% endhighlight %}

### dataSource.columns.filterItems.filterType `enum`
{:#members:datasource-columns-filteritems-filtertype}

<ts name = "ej.PivotAnalysis.FilterType"/>

Sets the type of filter to include/exclude the mentioned values.

>**Note**: This is applicable only for the relational datasource.

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
 
    $("#PivotGrid1").ejPivotGrid({ dataSource: { columns: [{ fieldName: "Country", filterItems: { filterType: ej.PivotAnalysis.FilterType.Include, values: valueArray } }] } });
{% endhighlight %}

### dataSource.columns.filterItems.values `array`
{:#members:datasource-columns-filteritems-values}

Contains the collection of items to be included/excluded among the field members.

#### Default Value: []

**Example:**

{% highlight javascript %}
 
    $("#PivotGrid1").ejPivotGrid({ dataSource: { columns: [{ fieldName: "Country", filterItems: { filterType: ej.PivotAnalysis.FilterType.Exclude, values: ["Canada", "France"] } }] } });
{% endhighlight %}

### dataSource.rows `array`
{:#members:datasource-rows}

Lists out the items to be arranged in the rows section of PivotGrid.

#### Default Value: []

**Example:**

{% highlight javascript %}
 
    $("#PivotGrid1").ejPivotGrid({ dataSource: { rows: itemsArray } });
{% endhighlight %}


### dataSource.rows.fieldName `string`
{:#members:datasource-rows-fieldname}

Allows you to bind the item by using its unique name as field name.

#### Default Value: ""

**Example:**

{% highlight javascript %}
 
    $("#PivotGrid1").ejPivotGrid({ dataSource: { rows: [{ fieldName : "MyFieldName" }] } });
{% endhighlight %}

### dataSource.rows.fieldCaption `string`
{:#members:datasource-rows-fieldcaption}

Allows you to set the display caption for the item.

#### Default Value: ""

**Example:**

{% highlight javascript %}
 
    $("#PivotGrid1").ejPivotGrid({ dataSource: { rows: [{ fieldCaption : "MyFieldCaption" }] } });
{% endhighlight %}

### dataSource.rows.advancedFilter `array`
{:#members:datasource-rows-advancedfilter}

Allows you to filter the report by using the advanced filtering (e.g., Microsoft Excel) option for the OLAP data source in client-mode.

#### Default Value: []

**Example:**

{% highlight javascript %}
 
    $("#PivotGrid1").ejPivotGrid({ dataSource: { rows: [{ advancedFilter : itemArray }] } });
{% endhighlight %}

### dataSource.rows.advancedFilter.name `string`
{:#members:datasource-rows-advancedfilter-name}

Allows you to provide the level unique name to perform the advanced filtering.

#### Default Value: ""

**Example:**

{% highlight javascript %}
 
    $("#PivotGrid1").ejPivotGrid({ dataSource: { rows: [{ advancedFilter : [{ name: "levelUniqueName" }] }] } });
{% endhighlight %}

### dataSource.rows.advancedFilter.labelFilterOperator `string`
{:#members:datasource-rows-advancedfilter-labelfilteroperator}

Allows you to set the operator to perform the label filtering.

#### Default Value: "none"

**Example:**

{% highlight javascript %}
 
    $("#PivotGrid1").ejPivotGrid({ dataSource: { rows: [{ advancedFilter : [{ labelFilterOperator: ej.olap.LabelFilterOptions.EndsWith }] }] } });
{% endhighlight %}

### dataSource.rows.advancedFilter.valueFilterOperator `string`
{:#members:datasource-rows-advancedfilter-valuefilteroperator}

Allows you to set the operator to perform the value filtering.

#### Default Value: "none"

**Example:**

{% highlight javascript %}
 
    $("#PivotGrid1").ejPivotGrid({ dataSource: { rows: [{ advancedFilter : [{ valueFilterOperator: ej.olap.ValueFilterOptions.Between }] }] } });
{% endhighlight %}

### dataSource.rows.advancedFilter.advancedFilterType `string`
{:#members:datasource-rows-advancedfilter-advancedfiltertype}

Allows you to set the filtering type while performing the advanced filtering.

#### Default Value: ""

**Example:**

{% highlight javascript %}
 
    $("#PivotGrid1").ejPivotGrid({ dataSource: { rows: [{ advancedFilter : [{ advancedFilterType:  ej.olap.AdvancedFilterType.LabelFilter }] }] } });
{% endhighlight %}

### dataSource.rows.advancedFilter.measure `string`
{:#members:datasource-rows-advancedfilter-measure}

In value filtering, this property contains the measure name to which the filter is applied.

#### Default Value: ""

**Example:**

{% highlight javascript %}
 
    $("#PivotGrid1").ejPivotGrid({ dataSource: { rows: [{ advancedFilter : [{ measure: "measureUniqueName", advancedFilterType: ej.olap.AdvancedFilterType.ValueFilter }] }] } });
{% endhighlight %}

### dataSource.rows.advancedFilter.values `array`
{:#members:datasource-rows-advancedfilter-values}

Allows you to hold the filter operand values in the advanced filtering.

#### Default Value: ""

**Example:**

{% highlight javascript %}
    
    //For Label Filters
    $("#PivotGrid1").ejPivotGrid({ dataSource: { rows: [{ advancedFilter : [{ labelFilterOperator: ej.olap.LabelFilterOptions.EndsWith, values:  ["002"] }] }] } });
    
    //For Value Filters
    $("#PivotGrid1").ejPivotGrid({ dataSource: { rows: [{ advancedFilter : [{ valueFilterOperator: ej.olap.ValueFilterOptions.GreaterThan, values:  ["200"] }] }] } });
{% endhighlight %}


### dataSource.rows.isNamedSets `boolean`
{:#members:datasource-rows-isnamedsets}

Allows you to indicate whether the added item is a named set or not.

> **Note**: This is only applicable for the OLAP datasource.

#### Default Value: false

**Example:**

{% highlight javascript %}
 
    $("#PivotGrid1").ejPivotGrid({ dataSource: { rows: [{ fieldName: "[Core Product Group]", isNamedSets : true }] } });
{% endhighlight %}

### dataSource.rows.showSubTotal `boolean`
{:#members:datasource-rows-showsubtotal}

Shows/hides the sub-total of the field.

>**Note**: This is applicable only for the relational datasource.

#### Default Value: true

**Example:**

{% highlight javascript %}
 
    $("#PivotGrid1").ejPivotGrid({ dataSource: { rows: [{ fieldName: "Country", showSubTotal : false }] } });
{% endhighlight %}

### dataSource.rows.format `string`
{:#members:datasource-rows-format}

Allows you to set the format for row headers.

>**Note**: This is applicable only for the relational datasource.

#### Default Value: ""

**Example:**

{% highlight javascript %}
 
    $("#PivotGrid1").ejPivotGrid({ dataSource: { rows: [{ format : "date" }] } });
{% endhighlight %}

### dataSource.rows.formatString `string`
{:#members:datasource-rows-formatstring}

This property is set to display the formatted values with format types in the PivotGrid.

#### Default Value: ""

**Example:**

{% highlight javascript %}
 
    $("#PivotGrid1").ejPivotGrid({ dataSource: { rows: [{ formatString : "MM/DD/YYYY" }] } });
{% endhighlight %}

### dataSource.rows.cssClass `string`
{:#members:datasource-rows-cssclass}

Allows you to set the custom theme for row headers.

>**Note**: This is applicable only for the relational datasource.

#### Default Value: ""

**Example:**

{% highlight javascript %}
 
    $("#PivotGrid1").ejPivotGrid({ dataSource: { rows: [{ cssClass : "className" }] } });
{% endhighlight %}

### dataSource.rows.delimiter `string`
{:#members:datasource-rows-delimiter}

Allows you to set the delimiter for date type format in the **formatString**. This is applicable for the **groupByDate** in row/column headers.

>**Note**: This is applicable only for the relational datasource with ClientMode.

#### Default Value: ""

**Example:**

{% highlight javascript %}
 
    $("#PivotGrid1").ejPivotGrid({ dataSource: { rows: [{ delimiter : "-" }] } });
{% endhighlight %}

### dataSource.rows.sortOrder `enum`
{:#members:datasource-rows-sortorder}

<ts ref = "ej.PivotAnalysis.SortOrder"/>

Allows you to set the sorting order of members of the field.

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
            <td class="description">Displays the members without sorting in any order.</td>
        </tr>
    </tbody>
</table>

**Example:**

{% highlight javascript %}
 
    $("#PivotGrid1").ejPivotGrid({ dataSource: { rows: [{ fieldName: "Country", sortOrder : ej.PivotAnalysis.SortOrder.Descending }] } });
{% endhighlight %}

### dataSource.rows.drilledItems `array`
{:#members:datasource-rows-drilleditems}

Contains the list of members need to be drilled down by default in the field.

#### Default Value: []

**Example:**

{% highlight javascript %}
 
    $("#PivotGrid1").ejPivotGrid({ dataSource: { rows: [{ fieldName: "Country", drilledItems : ["Canada", "France"] }] } });
{% endhighlight %}

### dataSource.rows.filterItems `object`
{:#members:datasource-rows-filteritems}

Applies the filter to field members.

#### Default Value: null

**Example:**

{% highlight javascript %}
 
    $("#PivotGrid1").ejPivotGrid({ dataSource: { rows: [{ fieldName: "Country", filterItems : { filterType: ej.PivotAnalysis.FilterType.Exclude, values: ["Canada", "France"] } }] } });
{% endhighlight %}

### dataSource.rows.filterItems.filterType `enum`
{:#members:datasource-rows-filteritems-filtertype}

<ts ref = "ej.PivotAnalysis.FilterType"/>

Sets the type of filter to include/exclude the mentioned values.

>**Note**: This is applicable only for the relational datasource.

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
 
    $("#PivotGrid1").ejPivotGrid({ dataSource: { rows: [{ fieldName: "Country", filterItems : { filterType: ej.PivotAnalysis.FilterType.Include, values: valueArray } }] } });
{% endhighlight %}

### dataSource.rows.filterItems.values `array`
{:#members:datasource-rows-filteritems-values}

Contains the collection of items to be included/excluded among the field members.

#### Default Value: []

**Example:**

{% highlight javascript %}
 
    $("#PivotGrid1").ejPivotGrid({ dataSource: { rows: [{ fieldName: "Country", filterItems : { filterType: ej.PivotAnalysis.FilterType.Exclude, values: ["Canada", "France"] } }] } });
{% endhighlight %}

### dataSource.values `array`
{:#members:datasource-values}

Lists out the items that support calculation in the PivotGrid.

#### Default Value: []

**Example:**

{% highlight javascript %}
 
    $("#PivotGrid1").ejPivotGrid({ dataSource: { values: itemsArray } });
{% endhighlight %}

### dataSource.values.fieldName `string`
{:#members:datasource-values-fieldname}

Allows you to bind the item by using its unique name as field name for the relational datasource.

#### Default Value: ""

**Example:**

{% highlight javascript %}
 
    $("#PivotGrid1").ejPivotGrid({ dataSource: { values: [{ fieldName : "MyFieldName" }] } });
{% endhighlight %}

### dataSource.values.fieldCaption `string`
{:#members:datasource-values-fieldcaption}

Allows you to set the display caption for the item in the relational datasource.

#### Default Value: ""

**Example:**

{% highlight javascript %}
 
    $("#PivotGrid1").ejPivotGrid({ dataSource: { values: [{ fieldCaption : "MyFieldCaption" }] } });
{% endhighlight %}

### dataSource.values.measures `array`
{:#members:datasource-values-measures}

This holds the list of unique names of measures to bind them from the OLAP cube.

#### Default Value: []

**Example:**

{% highlight javascript %}
 
    $("#PivotGrid1").ejPivotGrid({ dataSource: { values: [{ measures : itemsArray }] } });
{% endhighlight %}

### dataSource.values.measures.fieldName `string`
{:#members:datasource-values-measures-fieldName}

Allows you to bind the measure from the OLAP datasource by using its unique name as field name.

#### Default Value: ""

**Example:**

{% highlight javascript %}
 
    $("#PivotGrid1").ejPivotGrid({ dataSource: { values: [{ measures : [{ fieldName: "MeasureUniqueName" }] }] } });
{% endhighlight %}

### dataSource.values.axis `string`
{:#members:datasource-values-axis}

Allows you to set the axis name to place measures items.

>**Note**: This is applicable only for the OLAP datasource.

#### Default Value: "rows"

**Example:**

{% highlight javascript %}
 
    $("#PivotGrid1").ejPivotGrid({ dataSource: { values: [{ axis : ej.olap.AxisName.Row }] } });
{% endhighlight %}

### dataSource.values.isCalculatedField `boolean`
{:#members:datasource-values-iscalculatedfield}

Indicates whether the field is a calculated field with the relational datasource or not.

#### Default Value: false

**Example:**

{% highlight javascript %}
 
    $("#PivotGrid1").ejPivotGrid({ dataSource: { values: [{ isCalculatedField : true }] } });
{% endhighlight %}

### dataSource.values.summaryType `enum`
{:#members:datasource-values-summarytype}

<ts name = "ej.PivotAnalysis.SummaryType"/>

Allows to set the type of PivotGrid summary calculation in the value field with the relational datasource.

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
 
    $("#PivotGrid1").ejPivotGrid({ dataSource: { values: [{ summaryType : ej.PivotAnalysis.SummaryType.Average }] } });
{% endhighlight %}

### dataSource.values.format `string`
{:#members:datasource-values-format}

Allows to set the format for values.

>**Note**: This is applicable only for the relational datasource.

#### Default Value: ""

**Example:**

{% highlight javascript %}
 
    $("#PivotGrid1").ejPivotGrid({ dataSource: { values: [{ format : "percentage" }] } });
{% endhighlight %}

### dataSource.values.formatString `string`
{:#members:datasource-values-formatstring}

This property is set to display the formatted values with format types in the PivotGrid.

#### Default Value: ""

**Example:**

{% highlight javascript %}
 
    $("#PivotGrid1").ejPivotGrid({ dataSource: { values: [{ formatString : "MM/DD/YYYY" }] } });
{% endhighlight %}

### dataSource.values.formula `string`
{:#members:datasource-values-formula}

Allows to set the formula for calculation of values for calculated members in the relational datasource.

#### Default Value: ""

**Example:**

{% highlight javascript %}
 
    $("#PivotGrid1").ejPivotGrid({ dataSource: { values: [{ formula : "Quantity*10" }] } });
{% endhighlight %}

### dataSource.values.cssClass `string`
{:#members:datasource-values-cssclass}

Allows to set the custom theme for values.

>**Note**: This is applicable only for the relational datasource.

#### Default Value: ""

**Example:**

{% highlight javascript %}
 
    $("#PivotGrid1").ejPivotGrid({ dataSource: { values: [{ cssClass : "className" }] } });
{% endhighlight %}

### dataSource.filters `array`
{:#members:datasource-filters}

Lists out the items which supports filtering of values without displaying the members in UI of the PivotGrid.

#### Default Value: []

**Example:**

{% highlight javascript %}
 
    $("#PivotGrid1").ejPivotGrid({ dataSource: { filters: itemsArray } });
{% endhighlight %}


### dataSource.filters.fieldName `string`
{:#members:datasource-filters-fieldname}

Allows you to bind the item by using its unique name as field name.

#### Default Value: ""

**Example:**

{% highlight javascript %}
 
    $("#PivotGrid1").ejPivotGrid({ dataSource: { filters: [{ fieldName : "MyFieldName" }] } });
{% endhighlight %}

### dataSource.filters.fieldCaption `string`
{:#members:datasource-filters-fieldcaption}

Allows you to set the display name for the item.

#### Default Value: ""

**Example:**

{% highlight javascript %}
 
    $("#PivotGrid1").ejPivotGrid({ dataSource: { filters: [{ fieldCaption : "MyFieldCaption" }] } });
{% endhighlight %}

### dataSource.filters.filterItems `object`
{:#members:datasource-filters-filteritems}

Applies the filter to field members.

#### Default Value: null

**Example:**

{% highlight javascript %}
 
    $("#PivotGrid1").ejPivotGrid({ dataSource: { filters: [{ fieldName: "Country", filterItems : { filterType: ej.PivotAnalysis.FilterType.Exclude, values: ["Canada", "France"] } }] } });
{% endhighlight %}

### dataSource.filters.filterItems.filterType `enum`
{:#members:datasource-filters-filteritems-filtertype}

<ts ref = "ej.PivotAnalysis.FilterType"/>

Sets the type of filter to include/exclude the mentioned values.

>**Note**: This is applicable only for the relational datasource.

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
 
    $("#PivotGrid1").ejPivotGrid({ dataSource: { filters: [{ fieldName: "Country", filterItems : { filterType: ej.PivotAnalysis.FilterType.Include, values: valueArray } }] } });
{% endhighlight %}

### dataSource.filters.filterItems.values `array`
{:#members:datasource-filters-filteritems-values}

Contains the collection of items to be included/excluded among the field members.

#### Default Value: []

**Example:**

{% highlight javascript %}
 
    $("#PivotGrid1").ejPivotGrid({ dataSource: { filters: [{ fieldName: "Country", filterItems : { filterType: ej.PivotAnalysis.FilterType.Exclude, values: ["Canada", "France"] } }] } });
{% endhighlight %}

### dataSource.cube `string`
{:#members:datasource-cube}

Contains the respective cube name as string type in the OLAP database.

#### Default Value: “”

**Example:**

{% highlight javascript %}
 
    $("#PivotGrid1").ejPivotGrid({ dataSource: { cube: "Adventure Works" } });
{% endhighlight %}

### dataSource.sourceInfo `string`
{:#members:datasource-sourceinfo}

To set the data source name to fetch the data.

>**Note**: This is applicable only for the Mondrian connection.

#### Default Value: “”

**Example:**

{% highlight javascript %}
 
    $("#PivotGrid1").ejPivotGrid({ dataSource: { sourceInfo: "Provider Mondrian" } });
{% endhighlight %}

### dataSource.providerName `string`
{:#members:datasource-providername}

Sets the provider name for PivotGrid to identify whether the provider is SSAS or Mondrian. 

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
            <td class="description">To bind an OLAP data source to PivotGrid through SSAS provider.</td>
        </tr>
        <tr>
            <td class="name">mondrian</td>
            <td class="description">To bind a relational data source to PivotGrid through Mondrian provider.</td>
        </tr>
    </tbody>
</table>

**Example:**

{% highlight javascript %}
 
    $("#PivotGrid1").ejPivotGrid({ dataSource: { providerName: "mondrian" } });
{% endhighlight %}

### dataSource.data `object`
{:#members:datasource-data}

Provides the raw data source for the PivotGrid.

#### Default Value: null

**Example:**

{% highlight javascript %}
 
    $("#PivotGrid1").ejPivotGrid({ dataSource: { data: value } });
{% endhighlight %}

### dataSource.catalog `string`
{:#members:datasource-catalog}

In connection with an OLAP database, this property contains the database name as string to fetch the data from the given connection string.

#### Default Value: “”

**Example:**

{% highlight javascript %}
 
    $("#PivotGrid1").ejPivotGrid( { dataSource: { catalog: "databaseName" } } );
{% endhighlight %}

### dataSource.enableAdvancedFilter `boolean`
{:#members:datasource-enableadvancedfilter}

Allows you to filter the members (by its name and values) through advanced filtering (e.g., Microsoft Excel) option at OLAP data source in client-mode.

#### Default Value: false

**Example:**

{% highlight javascript %}
 
    $("#PivotGrid1").ejPivotGrid({ dataSource: { enableAdvancedFilter: true } });
{% endhighlight %}

### dataSource.reportName `string`
{:#members:datasource-reportName}

Sets a name to the report that is bound to the control.

#### Default Value: ""

**Example:**

{% highlight javascript %}
 
    $("#PivotGrid1").ejPivotGrid({ dataSource: { reportName: "Default Report" } });
{% endhighlight %}

### dataSource.pagerOptions `object`
{:#members:datasource-pageroptions}

Allows to set the page size and current page number for each axis on applying the paging.

> **Note**: This is applicable only for binding the OLAP data from client-side.

#### Default Value: {}

**Example:**

{% highlight javascript %}
 
    $("#PivotGrid1").ejPivotGrid({ dataSource: { pagerOptions: pagerSettings } }); 
{% endhighlight %}

### dataSource.pagerOptions.categoricalPageSize `number`
{:#members:datasource-pageroptions-categoricalpagesize}

Allows to set the number of categorical columns to be displayed in each page on applying the paging.

#### Default Value: 0

**Example:**

{% highlight javascript %}
 
    $("#PivotGrid1").ejPivotGrid({ dataSource: { pagerOptions: { categoricalPageSize: 10 } } }); 
{% endhighlight %}

### dataSource.pagerOptions.seriesPageSize `number`
{:#members:datasource-pageroptions-seriespagesize}

Allows to set the number of series rows to be displayed in each page on applying the paging.

#### Default Value: 0

**Example:**

{% highlight javascript %}
 
    $("#PivotGrid1").ejPivotGrid({ dataSource: { pagerOptions: { seriesPageSize: 5 } } }); 
{% endhighlight %}

### dataSource.pagerOptions.categoricalCurrentPage `number`
{:#members:datasource-pageroptions-categoricalcurrentpage}

Allows to set the page number to be loaded in the categorical axis by default.

> **Note**: This is applicable only for binding the OLAP data from client-side.

#### Default Value: 1

**Example:**

{% highlight javascript %}
 
    $("#PivotGrid1").ejPivotGrid({ dataSource: { pagerOptions: { categoricalCurrentPage: 3 } } }); 
{% endhighlight %}

### dataSource.pagerOptions.seriesCurrentPage `number`
{:#members:datasource-pageroptions-seriescurrentpage}

Allows to set the page number to be loaded in the series axis by default.

#### Default Value: 1

**Example:**

{% highlight javascript %}
 
    $("#PivotGrid1").ejPivotGrid({ dataSource: { pagerOptions: { seriesCurrentPage: 7 } } }); 
{% endhighlight %}

### valueSortSettings `object`
{:#members:valueSortSettings}

Holds the necessary properties for value sorting.

>**Note**: This is applicable only for the relational datasource.

#### Default Value: {}

{% highlight javascript %}
 
    $("#PivotGrid1").ejPivotGrid({ valueSortSettings: { } }); 
{% endhighlight %}

### valueSortSettings.headerText `string`
{:#members:valueSortSettings-headerText}

Contains the header of the specific column to which value sorting is applied.

>**Note**: This is applicable only for the relational datasource.

#### Default Value: ""

{% highlight javascript %}
 
    $("#PivotGrid1").ejPivotGrid({ valueSortSettings: { headerText: "Bike##FY 2005##Amount" } });
{% endhighlight %}

### valueSortSettings.headerDelimiters `string`
{:#members:valueSortSettings-headerDelimiters}

Allows you to set the string for separating column headers provided in the **headerText** property.

>**Note**: This is applicable only for the relational datasource.

#### Default Value: ""

{% highlight javascript %}
 
    $("#PivotGrid1").ejPivotGrid({ valueSortSettings: { headerDelimiters: "##" } });
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
            <td class="description">Displays the members without sorting in any order.</td>
        </tr>
    </tbody>
</table>

{% highlight javascript %}
 
    $("#PivotGrid1").ejPivotGrid({ valueSortSettings: { sortOrder: ej.PivotAnalysis.SortOrder.Descending } });
{% endhighlight %}

### frozenHeaderSettings `object`
{:#members:frozenheadersettings}

Object that holds the settings of frozen headers.

#### Default Value: {}

{% highlight javascript %}
 
    $("#PivotGrid1").ejPivotGrid({ frozenHeaderSettings: { enableFrozenHeaders: true } }); 
{% endhighlight %}

### frozenHeaderSettings.enableFrozenRowHeaders `boolean`
{:#members:frozenheadersettings-enablefrozenrowheaders}

Allows you to freeze the row headers alone when scrolling the horizontal scroll bar.

#### Default Value: false

{% highlight javascript %}
 
    $("#PivotGrid1").ejPivotGrid({ frozenHeaderSettings: { enableFrozenRowHeaders: true } });
{% endhighlight %}

### frozenHeaderSettings.enableFrozenColumnHeaders `boolean`
{:#members:frozenheadersettings-enablefrozencolumnheaders}

Allows you to freeze the column headers alone when scrolling the vertical scroll bar.

#### Default Value: false

{% highlight javascript %}
 
    $("#PivotGrid1").ejPivotGrid({ frozenHeaderSettings: { enableFrozenColumnHeaders: true } });
{% endhighlight %}

### frozenHeaderSettings.enableFrozenHeaders `boolean`
{:#members:frozenheadersettings-enablefrozenheaders}

Allows you to freeze both row headers and column headers while scrolling.

#### Default Value: false

{% highlight javascript %}
 
    $("#PivotGrid1").ejPivotGrid({ frozenHeaderSettings: { enableFrozenHeaders: true } });
{% endhighlight %}

### frozenHeaderSettings.scrollerSize `number`
{:#members:frozenheadersettings-scrollersize}

Allows you to set the size of the scrollbar (horizontal and vertical) that is visible in the PivotGrid.

#### Default Value: 18

{% highlight javascript %}
 
    $("#PivotGrid1").ejPivotGrid({ frozenHeaderSettings: { scrollerSize: 18 } });
{% endhighlight %}

### headerSettings `object`
{:#members:headersettings}

Allows you to display the header name in the PivotGrid control.

#### Default Value: {}

**Example:**

{% highlight javascript %}
 
    $("#PivotGrid1").ejPivotGrid({ headerSettings: { showRowItems: true, showColumnItems: true } });
{% endhighlight %}

### headerSettings.showRowItems `boolean`
{:#members:headersettings-showrowitems}

Allows you to enable/disable the row header names in the PivotGrid control.

#### Default Value: false

**Example:**

{% highlight javascript %}
 
    $("#PivotGrid1").ejPivotGrid({ headerSettings: { showRowItems: true } });
{% endhighlight %}

### headerSettings.showColumnItems `boolean`
{:#members:headersettings-showcolumnitems}

Allows you to enable/disable the column header names in the PivotGrid control.

#### Default Value: false

**Example:**

{% highlight javascript %}
 
    $("#PivotGrid1").ejPivotGrid({ headerSettings: { showColumnItems: true } });
{% endhighlight %}


### showUniqueNameOnPivotButton `boolean`
{:#members:showUniqueNameOnPivotButton}

Allows you to show the appropriate unique name in the pivot button.

> **Note**: This is applicable only for the OLAP datasource.

#### Default Value: false

**Example:**

{% highlight javascript %}
 
    $("#PivotGrid1").ejPivotGrid({ showUniqueNameOnPivotButton: true });
{% endhighlight %}

### customObject `object`
{:#members:customobject}

Object is utilized to pass additional information between the client-end and the service-end while operating the control in server mode.

#### Default Value: null

**Example:**

{% highlight javascript %}
 
    $("#PivotGrid1").ejPivotGrid({ customObject: { Language: "en-US" } });
{% endhighlight %}

### collapsedMembers `object`
{:#members:collapsedmembers}

Allows you to collapse specified members in each field by default.

#### Default Value: null

**Example:**

{% highlight javascript %}
 
    $("#PivotGrid1").ejPivotGrid({ collapsedMembers: { Country: ["Canada", "France"] } });
{% endhighlight %}

### enableCellContext `boolean`
{:#members:enablecellcontext}

Allows you to access each cell by right-clicking the mouse.

#### Default Value: false

**Example:**

{% highlight javascript %}
 
    $("#PivotGrid1").ejPivotGrid({ enableCellContext: true });
{% endhighlight %}

### enableCellSelection `boolean`
{:#members:enablecellselection}

Enables the cell selection for a specific range of value cells.

#### Default Value: false

**Example:**

{% highlight javascript %}
 
    $("#PivotGrid1").ejPivotGrid({ enableCellSelection: true });
{% endhighlight %}

### enableDrillThrough `boolean`
{:#members:enabledrillthrough}

Enables the Drill-Through feature which retrieves raw items that are used to create a specific cell in the PivotGrid.

#### Default Value: false

**Example:**

{% highlight javascript %}
 
    $("#PivotGrid1").ejPivotGrid({ enableDrillThrough: true });
{% endhighlight %}

### enableCellClick `boolean`
{:#members:enablecellclick}

Allows you to get cell details in JSON format by clicking the value cell.

#### Default Value: false

**Example:**

{% highlight javascript %}
 
    $("#PivotGrid1").ejPivotGrid({ enableCellClick: true });
{% endhighlight %}

### enableCellDoubleClick `boolean`
{:#members:enablecelldoubleclick}

Allows you to get cell details in JSON format by double-clicking the value cell.

#### Default Value: false

**Example:**

{% highlight javascript %}
 
    $("#PivotGrid1").ejPivotGrid({ enableCellDoubleClick: true });
{% endhighlight %}

### enableCellEditing `boolean`
{:#members:enablecellediting}

Allows you to edit value cells for write-back support in the PivotGrid. This is applicable only for the server-mode.

#### Default Value: false

**Example:**

{% highlight javascript %}
 
    $("#PivotGrid1").ejPivotGrid({ enableCellEditing:true });
{% endhighlight %}


### enableCollapseByDefault `boolean`
{:#members:enablecollapsebydefault}

Collapses the pivot items along rows and columns by default. It works only for the relational data source.

#### Default Value: false

**Example:**

{% highlight javascript %}

    $("#PivotGrid1").ejPivotGrid({ enableCollapseByDefault: true });
{% endhighlight %}

### enableColumnGrandTotal `boolean`
{:#members:enablecolumngrandtotal}

Enables/disables the display of grand total for all columns.

#### Default Value: true

**Example:**

{% highlight javascript %}

    $("#PivotGrid1").ejPivotGrid({ enableColumnGrandTotal: true });
{% endhighlight %}

### enableConditionalFormatting `boolean`
{:#members:enableconditionalformatting}

Allows you to format a specific set of cells based on the condition. 

#### Default Value: false

**Example:**

{% highlight javascript %}

    $("#PivotGrid1").ejPivotGrid({ enableConditionalFormatting:true });
{% endhighlight %}


### enableAdvancedFilter `boolean`
{:#members:enableadvancedfilter}

Enables the advanced filtering options such as value filtering, label filtering, and sorting for each field in the server mode.

#### Default Value: false

**Example:**

{% highlight javascript %}
 
    $("#PivotGrid1").ejPivotGrid({ enableAdvancedFilter: true });
{% endhighlight %}

### enableDeferUpdate `boolean`
{:#members:enabledeferupdate}

Allows you to refresh the control on-demand and not during every UI operation.

#### Default Value: false

**Example:**

{% highlight javascript %}
 
    $("#PivotGrid1").ejPivotGrid({ enableDeferUpdate: true });
{% endhighlight %}


### enableGroupingBar `boolean`
{:#members:enablegroupingbar}

Enables the display of GroupingBar allowing you to filter, sort, and remove fields obtained from the datasource.

#### Default Value: false

**Example:**

{% highlight javascript %}
 
    $("#PivotGrid1").ejPivotGrid({ enableGroupingBar: true });
{% endhighlight %}

### maxNodeLimitInMemberEditor `number`
{:#members:maxNodeLimitInMemberEditor}

Allows you to set the maximum number of nodes as well as child nodes to be displayed in the member editor.

#### Default Value: 1000

**Example:**

{% highlight javascript %}
 
    $("#PivotGrid1").ejPivotGrid({ maxNodeLimitInMemberEditor: 1500 });
{% endhighlight %}

### enableMemberEditorPaging `boolean`
{:#members:enablemembereditorpaging}

Enables/disables paging in the member editor for viewing the large count of members in pages. 

#### Default Value: false

**Example:**

{% highlight javascript %}
 
    $("#PivotGrid1").ejPivotGrid({ enableMemberEditorPaging: true });
{% endhighlight %}

### memberEditorPageSize `number`
{:#members:membereditorpagesize}

Allows you to set the number of members to be displayed in each page of member editor on applying paging in it. 

#### Default Value: 100

**Example:**

{% highlight javascript %}
 
    $("#PivotGrid1").ejPivotGrid({ memberEditorPageSize: 50 });
{% endhighlight %}

### enableMemberEditorSorting `boolean`
{:#members:enablemembereditorsorting}

Enables/Disables sorting option in member editor dialog for the members of the respective field.

#### Default Value: false

**Example:**

{% highlight javascript %}

    $("#PivotGrid1").ejPivotGrid({ enableMemberEditorSorting: true });
{% endhighlight %}

### enableGrandTotal `boolean`
{:#members:enablegrandtotal}

Enables/disables the display of grand total for rows and columns.

#### Default Value: true

**Example:**

{% highlight javascript %}
 
    $("#PivotGrid1").ejPivotGrid({ enableGrandTotal: true });
{% endhighlight %}

### enableJSONRendering `boolean`
{:#members:enablejsonrendering}

Allows you to load the PivotGrid using the JSON data.

#### Default Value: false

**Example:**

{% highlight javascript %}
 
    $("#PivotGrid1").ejPivotGrid({ enableJSONRendering: true });
{% endhighlight %}

### enablePivotFieldList `boolean`
{:#members:enablepivotfieldlist}

Enables rendering of the PivotGrid widget along with the PivotTable field list which allows UI operations.

#### Default Value: true

**Example:**

{% highlight javascript %}
 
    $("#PivotGrid1").ejPivotGrid({ enablePivotFieldList: true });
{% endhighlight %}

### enableRowGrandTotal `boolean`
{:#members:enablerowgrandtotal}

Enables the display of grand total for all rows.

#### Default Value: true

**Example:**

{% highlight javascript %}
 
    $("#PivotGrid1").ejPivotGrid({ enableRowGrandTotal: true });
{% endhighlight %}

### enableRTL `boolean`
{:#members:enablertl}

Allows you to view the layout of PivotGrid from right to left.

#### Default Value: false

**Example:**

{% highlight javascript %}
 
    $("#PivotGrid1").ejPivotGrid({ enableRTL: true });
{% endhighlight %}

### enableToolTip `boolean`
{:#members:enabletooltip}

Allows you to enable the ToolTip.

#### Default Value: false

**Example:**

{% highlight javascript %}
 
    $("#PivotGrid1").ejPivotGrid({ enableToolTip: true });
{% endhighlight %}

### enableToolTipAnimation `boolean`
{:#members:enabletooltipanimation}

Allows you to enable the animation effects in the tooltip.

#### Default Value: false

**Example:**

{% highlight javascript %}
 
    $("#PivotGrid1").ejPivotGrid({ enableToolTipAnimation: true });
{% endhighlight %}

### enableColumnResizing `boolean`
{:#members:enablecolumnresizing}

Allows you to adjust the width of columns dynamically within given widget size.

#### Default Value: false

**Example:**

{% highlight javascript %}
 
    $("#PivotGrid1").ejPivotGrid({ enableColumnResizing: true });
{% endhighlight %}

### resizeColumnsToFit `boolean`
{:#members:resizecolumnstofit}

Allows you to fit the width of the column based on its maximum text width.

#### Default Value: true

**Example:**

{% highlight javascript %}
 
    $("#PivotGrid1").ejPivotGrid({ resizeColumnsToFit: true });
{% endhighlight %}

### enableContextMenu `boolean`
{:#members:enablecontextmenu}

Allows you to enable/disable the context menu of pivot buttons in the PivotGrid.

#### Default Value: false

**Example:**

{% highlight javascript %}
 
    $("#PivotGrid1").ejPivotGrid({ enableContextMenu: true });
{% endhighlight %}

### enableVirtualScrolling `boolean`
{:#members:enablevirtualscrolling}

Allows you to view the large amount of data through virtual scrolling.

#### Default Value: false

**Example:**

{% highlight javascript %}
 
    $("#PivotGrid1").ejPivotGrid({ enableVirtualScrolling: true });
{% endhighlight %}

### enablePaging `boolean`
{:#members:enablepaging}

Allows you to view the large amount of data by applying paging.

#### Default Value: false

**Example:**

{% highlight javascript %}
 
    $("#PivotGrid1").ejPivotGrid({ enablePaging: true });
{% endhighlight %}

### hyperlinkSettings `object`
{:#members:hyperlinksettings}

Allows you to configure the hyperlink settings of the PivotGrid control.

#### Default Value: {}

**Example:**

{% highlight javascript %}
 
    $("#PivotGrid1").ejPivotGrid({ hyperlinkSettings: { enableValueCellHyperlink: true, enableRowHeaderHyperlink: true } });
{% endhighlight %}

### hyperlinkSettings.enableColumnHeaderHyperlink `boolean`
{:#members:hyperlinksettings-enablecolumnheaderhyperlink}

Allows you to enable/disable the hyperlink for the column header.

#### Default Value: false

**Example:**

{% highlight javascript %}
 
    $("#PivotGrid1").ejPivotGrid({ hyperlinkSettings: { enableColumnHeaderHyperlink: true } });
{% endhighlight %}

### hyperlinkSettings.enableRowHeaderHyperlink `boolean`
{:#members:hyperlinksettings-enablerowheaderhyperlink}

Allows you to enable/disable the hyperlink for the row header.

#### Default Value: false

**Example:**

{% highlight javascript %}
 
    $("#PivotGrid1").ejPivotGrid({ hyperlinkSettings: { enableRowHeaderHyperlink: true } });
{% endhighlight %}

### hyperlinkSettings.enableSummaryCellHyperlink `boolean`
{:#members:hyperlinksettings-enablesummarycellhyperlink}

Allows you to enable/disable the hyperlink for summary cells.

#### Default Value: false

**Example:**

{% highlight javascript %}
 
    $("#PivotGrid1").ejPivotGrid({ hyperlinkSettings: { enableSummaryCellHyperlink: true } });
{% endhighlight %}

### hyperlinkSettings.enableValueCellHyperlink `boolean`
{:#members:hyperlinksettings-enablevaluecellhyperlink}

Allows you to enable/disable the hyperlink for value cells.

#### Default Value: false

**Example:**

{% highlight javascript %}
 
    $("#PivotGrid1").ejPivotGrid({ hyperlinkSettings: { enableValueCellHyperlink: true } });
{% endhighlight %}

### isResponsive `boolean`
{:#members:isresponsive}

Allows you to enable PivotGrid’s responsiveness in the browser layout.

#### Default Value: false

**Example:**

{% highlight javascript %}
 
    $("#PivotGrid1").ejPivotGrid({ isResponsive: true });
{% endhighlight %}

### jsonRecords `string`
{:#members:jsonrecords}

Contains the serialized JSON string which renders the PivotGrid.

#### Default Value: ""

**Example:**

{% highlight javascript %}
 
    $("#PivotGrid1").ejPivotGrid({ jsonRecords: serializedJSON });
{% endhighlight %}

### layout `enum`
{:#members:layout}

<ts name = "ej.PivotGrid.Layout"/>

Sets the summary layout for PivotGrid.
Following are the ways in which summary can be positioned: normal summary (bottom), top summary, no summary, and excel-like summary.

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
 
    $("#PivotGrid1").ejPivotGrid({ layout: ej.PivotGrid.Layout.NoSummaries });
{% endhighlight %}

### locale `string`
{:#members:locale}

Allows the user to set the localized language for the widget.

#### Default Value: "en-US"

**Example:**

{% highlight javascript %}
 
    $("#PivotGrid1").ejPivotGrid({ locale: "en-US" });
{% endhighlight %}


### operationalMode `enum`
{:#members:operationalmode}

<ts name = "ej.Pivot.OperationalMode"/>

Sets the mode for PivotGrid widget for binding the data source either in the server-side or client-side.

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
 
    $("#PivotGrid1").ejPivotGrid({ operationalMode: ej.Pivot.OperationalMode.ServerMode });
{% endhighlight %}

### serviceMethodSettings `object`
{:#members:servicemethodsettings}

Allows you to set the custom name for the methods at service-end, communicated during AJAX post.

#### Default Value: {}

**Example:**

{% highlight javascript %}
 
    $("#PivotGrid1").ejPivotGrid({ serviceMethodSettings: { initialize: "InitializeGrid"} });
{% endhighlight %}

### serviceMethodSettings.drillDown `string`
{:#members:servicemethodsettings-drilldown}

Allows you to set the custom name for service method which is responsible for drill up/down operation in the PivotGrid.

#### Default Value: "DrillGrid"

**Example:**

{% highlight javascript %}
 
    $("#PivotGrid1").ejPivotGrid({ serviceMethodSettings: { drillDown: "DrillGridMyMethod" } });
{% endhighlight %}

### serviceMethodSettings.exportPivotGrid `string`
{:#members:servicemethodsettings-exportpivotgrid}

Allows you to set the custom name for the service method that is responsible for exporting.

#### Default Value: "Export"

**Example:**

{% highlight javascript %}
 
    $("#PivotGrid1").ejPivotGrid({ serviceMethodSettings: { exportPivotGrid: "ExportMyMethod" } });
{% endhighlight %}

### serviceMethodSettings.deferUpdate `string`
{:#members:servicemethodsettings-deferupdate}

Allows you to set the custom name for the service method responsible for performing server-side actions based on defer update.

#### Default Value: "DeferUpdate"

**Example:**

{% highlight javascript %}
 
    $("#PivotGrid1").ejPivotGrid({ serviceMethodSettings: { deferUpdate: "DeferUpdateMethod" } });
{% endhighlight %}

### serviceMethodSettings.fetchMembers `string`
{:#members:servicemethodsettings-fetchmembers}

Allows you to set the custom name for the service method that is responsible for getting values of the tree-view inside filter dialog.

#### Default Value: "FetchMembers"

**Example:**

{% highlight javascript %}
 
    $("#PivotGrid1").ejPivotGrid({ serviceMethodSettings:  { fetchMembers: "FetchMembersMethod" } });
{% endhighlight %}
 
### serviceMethodSettings.filtering `string`
{:#members:servicemethodsettings-filtering}

Allows you to set the custom name for the service method that is responsible for filtering operation in the PivotGrid.

#### Default Value: "Filtering"

**Example:**

{% highlight javascript %}
 
    $("#PivotGrid1").ejPivotGrid({ serviceMethodSettings:  { filtering : "FilteringMethod" } });
{% endhighlight %}
 
### serviceMethodSettings.initialize `string`
{:#members:servicemethodsettings-initialize}

Allows you to set the custom name for the service method that is responsible for initializing the PivotGrid.

#### Default Value: "InitializeGrid"

**Example:**

{% highlight javascript %}
 
    $("#PivotGrid1").ejPivotGrid({ serviceMethodSettings: { initialize: "InitializeGrid" } });
{% endhighlight %}

### serviceMethodSettings.nodeDropped `string`
{:#members:servicemethodsettings-nodedropped}

Allows you to set the custom name for the service method that is responsible for the server-side action when dropping a node from the field list.

#### Default Value: "NodeDropped"

**Example:**

{% highlight javascript %}
 
    $("#PivotGrid1").ejPivotGrid({ serviceMethodSettings: { nodeDropped: "nodedroppedMethod" } });
{% endhighlight %}

### serviceMethodSettings.nodeStateModified `string`
{:#members:servicemethodsettings-nodestatemodified}

Allows you to set the custom name for the service method that is responsible for server-side action when changing the checked state of a node in the field list.

#### Default Value: "NodeStateModified"

**Example:**

{% highlight javascript %}
 
    $("#PivotGrid1").ejPivotGrid({ serviceMethodSettings: { nodeStateModified: "NodeStateModifiedMethod" } });
{% endhighlight %}

### serviceMethodSettings.paging `string`
{:#members:servicemethodsettings-paging}

Allows you to set the custom name for the service method that is responsible for performing paging operation in the PivotGrid.

#### Default Value: "Paging"

**Example:**

{% highlight javascript %}
 
    $("#PivotGrid1").ejPivotGrid({ serviceMethodSettings: { paging: "PagingMyMethod" } });
{% endhighlight %}

### serviceMethodSettings.sorting `string`
{:#members:servicemethodsettings-sorting}

Allows you to set the custom name for the service method that is responsible for sorting operation in the PivotGrid.

#### Default Value: "Sorting"

**Example:**

{% highlight javascript %}
 
    $("#PivotGrid1").ejPivotGrid({ serviceMethodSettings: { sorting: "SortingMethod" } });
{% endhighlight %}

### serviceMethodSettings.memberExpand `string`
{:#members:servicemethodsettings-memberexpand}

Allows you to set the custom name for the service method that is responsible for expanding members in the member editor.

#### Default Value: "MemberExpanded"

**Example:**

{% highlight javascript %}
 
    $("#PivotGrid1").ejPivotGrid({ serviceMethodSettings: { memberExpand: "MemberExpandedMethod" } });
{% endhighlight %}

### serviceMethodSettings.cellEditing `string`
{:#members:servicemethodsettings-cellediting}

Allows you to set the custom name for the service method that is responsible for editing the cells.

#### Default Value: "CellEditing"

**Example:**

{% highlight javascript %}
 
    $("#PivotGrid1").ejPivotGrid({ serviceMethodSettings: { cellEditing: "MyCellEditingMethod" } });
{% endhighlight %}

### serviceMethodSettings.saveReport `string`
{:#members:servicemethodsettings-savereport}

Allows you to set the custom name for the service method that is responsible for saving the current report to the database.

#### Default Value: "SaveReport"

**Example:**

{% highlight javascript %}
 
    $("#PivotGrid1").ejPivotGrid({ serviceMethodSettings: { saveReport: "MySaveReportMethod" } });
{% endhighlight %}

### serviceMethodSettings.loadReport `string`
{:#members:servicemethodsettings-loadreport}

Allows you to set the custom name for the service method that is responsible for loading a report from the database.

#### Default Value: "LoadReportFromDB"

**Example:**

{% highlight javascript %}
 
    $("#PivotGrid1").ejPivotGrid({ serviceMethodSettings: { loadReport: "MyLoadReportMethod" } });
{% endhighlight %}

### serviceMethodSettings.calculatedField `string`
{:#members:servicemethodsettings-calculatedfield}

Allows you to set the custom name for the service method that is responsible for adding a calculated field to the report.

#### Default Value: "CalculatedField"

**Example:**

{% highlight javascript %}
 
    $("#PivotGrid1").ejPivotGrid({ serviceMethodSettings: { calculatedField: "MyCalculatedFieldMethod" } });
{% endhighlight %}

### serviceMethodSettings.drillThroughHierarchies `string`
{:#members:servicemethodsettings-drillthroughhierarchies}

Allows you to set the custom name for the service method that is responsible for performing the drill through operation.

#### Default Value: "DrillThroughHierarchies"

**Example:**

{% highlight javascript %}
 
    $("#PivotGrid1").ejPivotGrid({ serviceMethodSettings: { drillThroughHierarchies: "MyDrillThroughHierarchiesMethod" } });
{% endhighlight %}

### serviceMethodSettings.drillThroughDataTable `string`
{:#members:servicemethodsettings-drillthroughdatatable}

Allows you to set the custom name for the service method that is responsible for performing drill through operation in the data table.

#### Default Value: "DrillThroughDataTable"

**Example:**

{% highlight javascript %}
 
    $("#PivotGrid1").ejPivotGrid({ serviceMethodSettings: { drillThroughDataTable: "MyDrillThroughDataTableMethod" } });
{% endhighlight %}

### serviceMethodSettings.valueSorting `string`
{:#members:servicemethodsettings-valuesorting}

Allows you to set the custom name for the service method that is responsible for performing value sorting operation in the PivotGrid.

#### Default Value: "ValueSorting"

**Example:**

{% highlight javascript %}
 
    $("#PivotGrid1").ejPivotGrid({ serviceMethodSettings: { valueSorting: "MyValueSorting" } });
{% endhighlight %}

### serviceMethodSettings.removeButton `string`
{:#members:servicemethodsettings-removebutton}

Allows you to set the custom name for the service method that is responsible for removing the pivot button from the GroupingBar/field list.

#### Default Value: "RemoveButton"

**Example:**

{% highlight javascript %}
 
    $("#PivotGrid1").ejPivotGrid({ serviceMethodSettings: { removeButton: "MyRemoveButton" } });
{% endhighlight %}

### serviceMethodSettings.writeBack `string`
{:#members:servicemethodsettings-writeback}

Allows you to set the custom name for the service method that is responsible for write-back operation in the OLAP Cube. This is applicable only in the server-side component.

#### Default Value: "WriteBack"

**Example:**

{% highlight javascript %}
 
    $("#PivotGrid1").ejPivotGrid({ serviceMethodSettings: { writeBack: "WriteBackMethod" } });
{% endhighlight %}

### url `string`
{:#members:url}

Connects the service using the specified URL for any server updates.

#### Default Value: “”

**Example:**

{% highlight javascript %}
 
    $("#PivotGrid1").ejPivotGrid({ url: "/PivotService" });
{% endhighlight %}

### enableCompleteDataExport `boolean`
{:#members:enableCompleteDataExport}

Allows you to export entire data instead of current page data, while paging option is enabled.

#### Default Value: false

**Example:**

{% highlight javascript %}
 
    $("#PivotGrid1").ejPivotGrid({ enableCompleteDataExport: true });
{% endhighlight %}

### enableXHRCredentials `boolean`
{:#members:enableXHRCredentials}

Allows you to enable "withCredentials" property inside XMLHttpRequest object for CORS(Cross-Origin Resource Sharing) request.

#### Default Value: false

**Example:**

{% highlight javascript %}
 
    $("#PivotGrid").ejPivotGrid({ enableXHRCredentials: true });
{% endhighlight %}

## Methods

### doAjaxPost()
{:#methods:doajaxpost}

Performs an asynchronous HTTP (AJAX) request.

**Example:**

{% highlight javascript %}
 
    var gridObj = $("#PivotGrid1").data("ejPivotGrid");
    gridObj.doAjaxPost("POST", "/PivotService/Initialize", { "key", "Hello World" }, successEvent, null);
{% endhighlight %}

### doPostBack()
{:#methods:dopostback}

Performs an asynchronous HTTP (FullPost) submit.

**Example:**

{% highlight javascript %}
 
    var gridObj = $("#PivotGrid1").data("ejPivotGrid");
    gridObj.doPostBack("/PivotService/Initialize", { "key", "Hello World" });
{% endhighlight %}

### exportPivotGrid()
{:#methods:exportpivotgrid}

Exports the PivotGrid to the specified format.

**Example:**

{% highlight javascript %}
 
    var gridObj = $("# PivotGrid1").data("ejPivotGrid");
    gridObj.exportPivotGrid(ej.PivotGrid.ExportOptions.Excel);
{% endhighlight %}

### refreshPagedPivotGrid()
{:#methods:refreshpagedpivotgrid}

This function re-renders the PivotGrid when clicking the navigation buttons on the PivotPager.

**Example:**

{% highlight javascript %}
 
    var gridObj = $("#PivotGrid1").data("ejPivotGrid");
    gridObj.refreshPagedPivotGrid("series", 2);
{% endhighlight %}

### refreshPivotGrid()
{:#methods:refreshpivotgrid}

This function refreshes the PivotGrid with the modified data input in client-mode.

**Example:**

{% highlight javascript %}

    var gridObj = $("#PivotGrid1").data("ejPivotGrid");
    gridObj.refreshPivotGrid();
{% endhighlight %}

### refreshControl()
{:#methods:refreshcontrol}

This function re-renders the control with the report available at that instant.

**Example:**

{% highlight javascript %}

    var gridObj = $("#PivotGrid1").data("ejPivotGrid");
    gridObj.model.dataSource = newDataSource;
    gridObj.refreshControl();
{% endhighlight %}

### destroy()
{:#methods:destroy}

This function destroys the PivotGrid widget associated events that are bound using "this._on" and brings the control to pre-init state.

**Example:**

{% highlight javascript %}

    var gridObj = $("#PivotGrid1").data("ejPivotGrid");
    gridObj.destroy();
{% endhighlight %}

### calculateCellWidths()
{:#methods:calculatecellwidths}

This function returns the height of all rows and the width of all columns.

#### Returns:

object

**Example:**

{% highlight javascript %}

    var gridObj = $("#PivotGrid1").data("ejPivotGrid");
    var gridDimensions = gridObj.calculateCellWidths();
{% endhighlight %}

### openConditionalFormattingDialog()
{:#methods:openconditionalformattingdialog}

This function creates the conditional formatting dialog to apply conditional formatting for the PivotGrid control.

**Example:**

{% highlight javascript %}

    var gridObj = $("#PivotGrid1").data("ejPivotGrid");
    gridObj.openConditionalFormattingDialog();
{% endhighlight %}

### saveReport()
{:#methods:savereport}

This function saves the current report to the database/local storage.

**Example:**

{% highlight javascript %}

    var gridObj = $("#PivotGrid1").data("ejPivotGrid");
    var storageOption = "local"; //it takes the string value "local" for local storage and "database" for storing to database.
    var url = "";//it takes the service url for storing to database. For local it is not required.
    gridObj.saveReport("reportName", storageOption, url);
{% endhighlight %}

### loadReport()
{:#methods:loadreport}

This function loads the specified report from the database/local storage.

**Example:**

{% highlight javascript %}

    var gridObj = $("#PivotGrid1").data("ejPivotGrid");
    var storageOption = "local"; //it takes the string value "local" for loading a report from local storage and "database" for loading from database.
    var url = "";//it takes the service method url for loading report from database. For local it is not required.
    gridObj.loadReport("reportName", storageOption, url);
{% endhighlight %}

### excelLikeLayout()
{:#methods:excellikelayout}

This function reconstructs the JSON data that is formed for rendering the PivotGrid in the excel-like layout format.

**Example:**

{% highlight javascript %}

    var gridObj = $("#PivotGrid1").data("ejPivotGrid");
    gridObj.excelLikeLayout(JSONObjectArray);
{% endhighlight %}

### getOlapReport()
{:#methods:getolapreport}

Returns the OlapReport string that is maintained along with the axis elements information.

#### Returns:

string

**Example:**

{% highlight javascript %}
 
    var gridObj = $("#PivotGrid1").data("ejPivotGrid");
    var report = gridObj.getOlapReport();
{% endhighlight %}

### setOlapReport()
{:#methods:setolapreport}

Sets the OlapReport string along with the axis information.

**Example:**

{% highlight javascript %}
 
    var gridObj = $("#PivotGrid1").data("ejPivotGrid");
    gridObj.setOlapReport(olapReportObj);
{% endhighlight %}

### getJSONRecords()
{:#methods:getjsonrecords}

Returns the JSON records that are formed to render the control.

#### Returns:

array

**Example:**

{% highlight javascript %}
 
    var gridObj = $("#PivotGrid1").data("ejPivotGrid");
    var jsonRecords = gridObj.getJSONRecords();
{% endhighlight %}

### setJSONRecords()
{:#methods:setjsonrecords}

Sets the JSON records that are formed to render the control.

**Example:**

{% highlight javascript %}
 
    var gridObj = $("#PivotGrid1").data("ejPivotGrid");
    gridObj.setJSONRecords(jsonRecords);
{% endhighlight %}

### refreshFieldCaption()
{:#methods:refreshfieldcaption}

This function allows you to change the caption of the pivot item (name displayed in UI) on-demand for the relational datasource in client-mode.

**Example:**

{% highlight javascript %}

    var gridObj = $("#PivotGrid1").data("ejPivotGrid");
    gridObj.refreshFieldCaption( "name", "caption", "axisClassName");
{% endhighlight %}

### renderControlFromJSON()
{:#methods:rendercontrolfromjson}

This function receives the JSON formatted datasource to render the PivotGrid control.

**Example:**

{% highlight javascript %}
 
    var gridObj = $("#PivotGrid1").data("ejPivotGrid");
    gridObj.renderControlFromJSON({ this.getJSONRecords() });
{% endhighlight %}

## Events

### afterServiceInvoke
{:#events:afterserviceinvoke}

Triggers when it reaches client-side after the AJAX request.

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
<td class="description last">returns the current action of PivotGrid control.</td>
</tr>
<tr>
<td class="name">customObject</td>
<td class="type">object</td>
<td class="description last">returns the custom object bound with PivotGrid control.</td>
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
 
    $("#PivotGrid1").ejPivotGrid({
        afterServiceInvoke: function (args) {}
    });
{% endhighlight %}


### beforeServiceInvoke
{:#events:beforeserviceinvoke}

Triggers before any AJAX request is passed from the PivotGrid to service methods.

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
<td class="description last">returns the current action of PivotGrid control.</td>
</tr>
<tr>
<td class="name">customObject</td>
<td class="type">object</td>
<td class="description last">returns the custom object bound with PivotGrid control.</td>
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
    
    $("#PivotGrid1").ejPivotGrid({
        beforeServiceInvoke: function (args) {}
    });
{% endhighlight %}

### beforePivotEnginePopulate
{:#events:beforepivotenginepopulate}

Triggers before the pivot engine starts to populate.

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
<td class="name">pivotGridObject</td>
<td class="type">object</td>
<td class="description last">returns the PivotGrid object</td>
</tr>
</tbody>
</table>

**Example:**

{% highlight javascript %}
 
    $("#PivotGrid1").ejPivotGrid({
        beforePivotEnginePopulate: function (args) {}
    });
{% endhighlight %}

### cellClick
{:#events:cellclick}

Triggers when click action is performed over a value cell.

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
<td class="description last">returns the custom object bound with PivotGrid control.</td>
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
 
    $("#PivotGrid1").ejPivotGrid({
        cellClick: function (args) {}
    });
{% endhighlight %}


### cellDoubleClick
{:#events:celldoubleclick}

Triggers when double-click action is performed over a value cell.

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
<td class="description last">returns the JSON details of the double respective on cell.</td>
</tr>
<tr>
<td class="name">customObject</td>
<td class="type">object</td>
<td class="description last">returns the custom object bound with PivotGrid control.</td>
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
 
    $("#PivotGrid1").ejPivotGrid({
        cellDoubleClick: function (args) {}
    });
{% endhighlight %}

### cellContext
{:#events:cellcontext}

Triggers when right-click action is performed on a cell.

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
<td class="name">cellPosition</td>
<td class="type">string</td>
<td class="description last">returns the cell position (row index and column index) in table.</td>
</tr>
<tr>
<td class="name">cellType</td>
<td class="type">string</td>
<td class="description last">returns the type of the cell.</td>
</tr>
<tr>
<td class="name">cellValue</td>
<td class="type">string</td>
<td class="description last">returns the content of the cell.</td>
</tr>
<tr>
<td class="name">uniqueName</td>
<td class="type">string</td>
<td class="description last">returns the unique name of levels/members.</td>
</tr>
<tr>
<td class="name">role</td>
<td class="type">string</td>
<td class="description last">returns the role of the cell in PivotGrid.</td>
</tr>
<tr>
<td class="name">rawdata</td>
<td class="type">object</td>
<td class="description last">returns JSON record corresponding to the selected cell.</td>
</tr>
<tr>
<td class="name">args</td>
<td class="type">object</td>
<td class="description last">returns the original event object.</td>
</tr>
</tbody>
</table>

**Example:**

{% highlight javascript %}
 
    $("#PivotGrid1").ejPivotGrid({
        cellContext: function (args) {}
    });
{% endhighlight %}


### cellSelection
{:#events:cellselection}

Triggers when a specific range of value cells is selected.

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
<td class="name">JSONRecords</td>
<td class="type">object</td>
<td class="description last">returns the JSON records of the selected range of cells.</td>
</tr>
<tr>
<td class="name">rowheader</td>
<td class="type">object</td>
<td class="description last">Returns the row headers corresponding to the selected value cells.</td>
</tr>
<tr>
<td class="name">columnheader</td>
<td class="type">object</td>
<td class="description last">Returns the column headers corresponding to the selected value cells.</td>
</tr>
<tr>
<td class="name">measureCount</td>
<td class="type">string</td>
<td class="description last">Returns the information about the measure associated with the selected cell.</td>
</tr>
</tbody>
</table>

**Example:**

{% highlight javascript %}
 
    $("#PivotGrid1").ejPivotGrid({
        cellSelection: function (args) {}
    });
{% endhighlight %}

### columnHeaderHyperlinkClick
{:#events:columnheaderhyperlinkclick}

Triggers when the hyperlink of column header is clicked.

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
<td class="description last">returns the information about the clicked cell</td>
</tr>
<tr>
<td class="name">element</td>
<td class="type">object</td>
<td class="description last">returns the HTML element of the control.</td>
</tr>
<tr>
<td class="name">customObject</td>
<td class="type">object</td>
<td class="description last">returns the custom object bound to the control.</td>
</tr>
</tbody>
</table>

**Example:**

{% highlight javascript %}
 
    $("#PivotGrid1").ejPivotGrid({
        columnHeaderHyperlinkClick: function (args) {}
    });
{% endhighlight %}


### drillSuccess
{:#events:drillsuccess}

Triggers after performing drill operation in the PivotGrid.

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
<td class="description last">returns the HTML element of the control.</td>
</tr>
</tbody>
</table>

**Example:**

{% highlight javascript %}
 
    $("#PivotGrid1").ejPivotGrid({
        drillSuccess: function (args) {}
    });
{% endhighlight %}


### drillThrough
{:#events:drillthrough}

Triggers while clicking "OK" in the drill-through dialog.

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
<td class="description last">returns the HTML element of PivotGrid control.</td>
</tr>
</tbody>
</table>

**Example:**

{% highlight javascript %}
 
    $("#PivotGrid1").ejPivotGrid({
        drillThrough: function (args) {}
    });
{% endhighlight %}


### load
{:#events:load}

Triggers when the PivotGrid loading is initiated.

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
<td class="description last">returns the HTML element of PivotGrid control.</td>
</tr>
</tbody>
</table>

**Example:**

{% highlight javascript %}
 
    $("#PivotGrid1").ejPivotGrid({
        load: function (args) {}
    });
{% endhighlight %}

### renderComplete
{:#events:rendercomplete}

Triggers when PivotGrid widget completes all operations at client-side after any AJAX request.

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
<td class="description last">returns the current action of PivotGrid control.</td>
</tr>
<tr>
<td class="name">customObject</td>
<td class="type">object</td>
<td class="description last">returns the custom object bound with the control.</td>
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
 
    $("#PivotGrid1").ejPivotGrid({
        renderComplete: function (args) {}
    });
{% endhighlight %}

### renderFailure
{:#events:renderfailure}

Triggers when any error occurred during the AJAX request.

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
<td class="description last">returns the current action of PivotGrid control.</td>
</tr>
<tr>
<td class="name">customObject</td>
<td class="type">Object</td>
<td class="description last">returns the custom object bound with the control.</td>
</tr>
<tr>
<td class="name">element</td>
<td class="type">object</td>
<td class="description last">returns the HTML element of PivotGrid control.</td>
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
 
    $("#PivotGrid1").ejPivotGrid({
        renderFailure: function (args) {}
    });
{% endhighlight %}


### renderSuccess
{:#events:rendersuccess}

Triggers when the PivotGrid successfully reaches the client-side after any AJAX request. 

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
<td class="description last">returns the current action of PivotGrid control.</td>
</tr>
<tr>
<td class="name">customObject</td>
<td class="type">object</td>
<td class="description last">returns the custom object bound with the control.</td>
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
 
    $("#PivotGrid1").ejPivotGrid({
        renderSuccess: function (args) {}
    });
{% endhighlight %}


### rowHeaderHyperlinkClick
{:#events:rowheaderhyperlinkclick}

Triggers when the hyperlink of row header is clicked.

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
<td class="description last">returns the information about the clicked cell</td>
</tr>
<tr>
<td class="name">element</td>
<td class="type">object</td>
<td class="description last">returns the HTML element of the control.</td>
</tr>
<tr>
<td class="name">customObject</td>
<td class="type">object</td>
<td class="description last">returns the custom object bound to the control.</td>
</tr>
</tbody>
</table>

**Example:**

{% highlight javascript %}
 
    $("#PivotGrid1").ejPivotGrid({
        rowHeaderHyperlinkClick: function (args) {}
    });
{% endhighlight %}

### summaryCellHyperlinkClick
{:#events:summarycellhyperlinkclick}

Triggers when the hyperlink of summary cell is clicked.

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
<td class="description last">returns the information about the clicked cell</td>
</tr>
<tr>
<td class="name">element</td>
<td class="type">object</td>
<td class="description last">returns the HTML element of the control.</td>
</tr>
<tr>
<td class="name">customObject</td>
<td class="type">object</td>
<td class="description last">returns the custom object bound to the control.</td>
</tr>
</tbody>
</table>

**Example:**

{% highlight javascript %}
 
    $("#PivotGrid1").ejPivotGrid({
        summaryCellHyperlinkClick: function (args) {}
    });
{% endhighlight %}

### valueCellHyperlinkClick
{:#events:valuecellhyperlinkclick}

Triggers when the hyperlink of value cell is clicked.

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
<td class="description last">returns the information about the clicked cell</td>
</tr>
<tr>
<td class="name">element</td>
<td class="type">object</td>
<td class="description last">returns the HTML element of the control.</td>
</tr>
<tr>
<td class="name">customObject</td>
<td class="type">object</td>
<td class="description last">returns the custom object bound to the control.</td>
</tr>
</tbody>
</table>

**Example:**

{% highlight javascript %}
 
    $("#PivotGrid1").ejPivotGrid({
        valueCellHyperlinkClick: function (args) {}
    });
{% endhighlight %}

### saveReport
{:#events:saveReport}

Triggers before saving the current report to the database.

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
<td class="name">report</td>
<td class="type">object</td>
<td class="description last">returns the report to be stored in database.</td>
</tr>
</tbody>
</table>

**Example:**

{% highlight javascript %}
 
    $("#PivotGrid1").ejPivotGrid({
        saveReport: function (args) {}
    });
{% endhighlight %}

### loadReport
{:#events:loadReport}

Triggers before loading a report from the database.

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
<td class="description last">returns the PivotGrid object.</td>
</tr>
<tr>
<td class="name">dataModel</td>
<td class="type">string</td>
<td class="description last">returns whether the control is bound with OLAP or Relational data source.</td>
</tr>
</tbody>
</table>

**Example:**

{% highlight javascript %}
 
    $("#PivotGrid1").ejPivotGrid({
        loadReport: function (args) {}
    });
{% endhighlight %}

### beforeExport
{:#events:beforeExport}

Triggers before performing exporting in the pivot grid.

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
<td class="description last">contains the url of the service responsible for exporting.</td>
</tr>
<tr>
<td class="name">fileName</td>
<td class="type">string</td>
<td class="description last">contains the name of the exporting file.</td>
</tr>
</tbody>
</table>

**Example:**

{% highlight javascript %}
 
    $("#PivotGrid1").ejPivotGrid({
        beforeExport: function (args) {}
    });
{% endhighlight %}

### cellEdit
{:#events:celledit}

Triggers before editing the cells.

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
<td class="name">editCellsInfo</td>
<td class="type">array</td>
<td class="description last">contains the array of cells selected for editing.</td>
</tr>
</tbody>
</table>

**Example:**

{% highlight javascript %}
 
    $("#PivotGrid1").ejPivotGrid({
        cellEdit: function (args) {}
    });
{% endhighlight %}

