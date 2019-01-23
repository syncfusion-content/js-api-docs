---
layout: post
title: Properties, Methods and Events of Syncfusion ejGantt Widget
description: Methods, members, events available in ejGantt
documentation: UG
platform: js-api
keywords: ejGantt, API, Essential JS Gantt
---

# ejGantt

The Essential JavaScript Gantt control is designed to visualize and edit the project schedule, and track the project progress. 


#### Syntax

$(element).ejGantt(options);

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
<td class="name">options</td>
<td class="type"><span class="param-type">object</span></td>
<td class="description last">settings for ejGantt</td>
</tr>
</tbody>
</table>

#### Example
{:.example}


{% highlight html %}
 
<div id="gantt">Gantt</div> 
 
<script>
// Create Gantt
$('#gantt').ejGantt({
    dataSource: projectData,
}); 
</script>

{% endhighlight %}


#### Requires
{:.require}

* module:jQuery
* module:jquery.globalize.js
* module:jquery.easing.1.3.js
* module:jsrender.js
* module:ej.web.all.js


## Members

### addDialogFields `array`
{:#members:adddialogfields}

Specifies the fields to be included in the add dialog in Gantt


#### Default Value

* []


#### Example
{:.example}


{% highlight html %}
 
<div id="gantt"></div> 
<script>                  
        $("#gantt").ejGantt(
 {
    addDialogFields: [{ field: "taskId", editType: "stringedit" }]
 });            
</script>

{% endhighlight %}

### addDialogFields.field `string`
{:#members:adddialogfields-field}

Specifies mapping name to include required fields in Gantt


#### Default Value

* ""


#### Example


{% highlight html %}

<div id="gantt"></div> 
<script>                  
        $("#gantt").ejGantt(
 {
    addDialogFields: [{ field: "taskId" }]
 });            
</script>
{% endhighlight %}


### addDialogFields.editType `string`
{:#members:adddialogfields-edittype}

Specifies editType of fields to be included in the add dialog in Gantt


#### Default Value

* ""


#### Example


{% highlight html %}

<div id="gantt"></div> 
<script>                  
        $("#gantt").ejGantt(
 {
    addDialogFields: [{ editType: "stringedit" }]
 });            
</script>
{% endhighlight %}

### addDialogFields.displayInGeneralTab `boolean`
{:#members:adddialogfields-displayingeneraltab}

Specifies the custom column field was displayed in General tab of add dialog or not.

#### Default Value

* false

#### Example
{:.example}

{% highlight html %}

<div id="gantt"></div> 
<script>                  
$("#gantt").ejGantt(
{
     addDialogFields: [{ field:"customColumn", displayInGeneralTab: true }]
});
</script>

{% endhighlight %}

### allowColumnResize `boolean`
{:#members:allowcolumnresize}

Enables or disables the ability to resize column.


#### Default Value

* false


#### Example
{:.example}


{% highlight html %}
 
<div id="gantt"></div> 
<script>                   
        $("#gantt").ejGantt({ allowColumnResize:  true });                      * 
</script>

{% endhighlight %}

### allowDragAndDrop `boolean`
{:#members:allowdraganddrop}

Enables or disables the ability to drag and drop the row interactively to reorder the rows


#### Default Value

* false


#### Example
{:.example}


{% highlight html %}
 
<div id="gantt"></div> 
<script>        
        $("#gantt").ejGantt({ allowDragAndDrop:  true });
</script>

{% endhighlight %}

### allowGanttChartEditing `boolean`
{:#members:allowganttchartediting}

Enables or Disables Gantt chart editing in Gantt


#### Default Value

* true


#### Example
{:.example}


{% highlight html %}
 
<div id="gantt"></div> 
<script>          
        $("#gantt").ejGantt(
 {
    allowGanttChartEditing:true
 });            
</script>

{% endhighlight %}


### allowKeyboardNavigation `boolean`
{:#members:allowkeyboardnavigation}

Enables or Disables Keyboard navigation in Gantt


#### Default Value

* true


#### Example
{:.example}


{% highlight html %}
 
<div id="gantt"></div> 
<script>                  
        $("#gantt").ejGantt({ allowKeyboardNavigation : true});                 
</script>

{% endhighlight %}


### allowMultiSorting `boolean`
{:#members:allowmultisorting}

Specifies enabling or disabling multiple sorting for Gantt columns


#### Default Value

* false


#### Example
{:.example}


{% highlight html %}
 
<div id="gantt"></div> 
<script>                  
        $("#gantt").ejGantt({ allowMultiSorting : true});                       
</script>

{% endhighlight %}

### allowMultipleExporting `boolean`
{:#members:allowmultipleexporting}

Enables or disables the option for multiple exporting 


#### Default Value

* false


#### Example
{:.example}


{% highlight html %}
 
<div id="gantt"></div> 
<script>                  
        $("#gantt").ejGantt({ allowMultipleExporting : true});                       
</script>

{% endhighlight %}


### allowSelection `boolean`
{:#members:allowselection}

Enables or disables the interactive selection of a row.


#### Default Value

* true


#### Example
{:.example}


{% highlight html %}
 
<div id="gantt"></div> 
<script>   
        $("#gantt").ejGantt({ allowSelection:  true });                 * 
</script>

{% endhighlight %}


### allowSorting `boolean`
{:#members:allowsorting}

Enables or disables sorting. When enabled, we can sort the column by clicking on the column.


#### Default Value

* false


#### Example
{:.example}


{% highlight html %}
 
<div id="gantt"></div> 
<script>        
        $("#gantt").ejGantt({ allowSorting:  true });            
</script>

{% endhighlight %}

### allowUnscheduledTask `boolean`
{:#members:allowunscheduledtask}

Enables or disables the rendering of unscheduled tasks.


#### Default Value

* false


#### Example
{:.example}


{% highlight html %}
 
<div id="gantt"></div> 
<script>        
        $("#gantt").ejGantt({ allowUnscheduledTask:  true });            
</script>

{% endhighlight %}

### baselineColor `string`
{:#members:baselinecolor}

Specifies the baseline background color in Gantt


#### Default Value

* "#fba41c"


#### Example
{:.example}


{% highlight html %}
 
<div id="gantt"></div> 
<script>  
        $("#gantt").ejGantt(
 {
    baselineColor: "blue"
 });            
</script>

{% endhighlight %}

### baselineEndDateMapping `string`
{:#members:baselineenddatemapping}

Specifies the mapping property path for baseline end date in datasource


#### Default Value

* ""


#### Example
{:.example}


{% highlight html %}
 
<div id="gantt"></div> 
<script>                  
        $("#gantt").ejGantt({  baselineEndDateMapping : "BaselineEndDate" });
</script>

{% endhighlight %}

### baselineStartDateMapping `string`
{:#members:baselinestartdatemapping}

Specifies the mapping property path for baseline start date of a task in datasource


#### Default Value

* ""


#### Example
{:.example}


{% highlight html %}
 
<div id="gantt"></div> 
<script>                  
        $("#gantt").ejGantt({  baselineStartDateMapping : "BaselineStartDate" });               
</script>

{% endhighlight %}

### cellTooltipTemplate `string`
{:#members:celltooltiptemplate}

Specifies the template for cell tooltip

#### Default Value

* null


#### Example


{% highlight html %}
                  
        $("#gantt").ejGantt({ cellTooltipTemplate : "CellTooltipTemplate"});        

{% endhighlight %}

### childMapping `string`
{:#members:childmapping}

Specifies the mapping property path for sub tasks in datasource


#### Default Value

* ""


#### Example
{:.example}


{% highlight html %}
 
<div id="gantt"></div> 
<script>                          
        $("#gantt").ejGantt({  childMapping : "Children" });
</script>

{% endhighlight %}

### columnDialogFields `array`
{:#members:columndialogfields}

To Specify the column fields to be displayed in the dialog while inserting a column using column menu.


#### Default Value

* []


#### Example
{:.example}


{% highlight html %}
 
<div id="gantt"></div> 
<script>  
        $("#gantt").ejGantt({ columnDialogFields: ["field", "headerText", "editType", "width", "visible", "allowSorting", "textAlign", "headerTextAlign"] });                   
</script>

{% endhighlight %}

### connectorLineBackground `string`
{:#members:connectorlinebackground}

Specifies the background of connector lines in Gantt


#### Default Value

* ""


#### Example
{:.example}


{% highlight html %}
 
<div id="gantt"></div> 
<script>                          
        $("#gantt").ejGantt({  
                        connectorLineBackground : "#F2F2F2"});
</script>

{% endhighlight %}


### connectorlineWidth `number`
{:#members:connectorlinewidth}

Specifies the width of the connector lines in Gantt


#### Default Value

* 1


#### Example
{:.example}


{% highlight html %}
 
<div id="gantt"></div> 
<script>                  
        $("#gantt").ejGantt({  
                        connectorlineWidth : 1 });
</script>

{% endhighlight %}


### cssClass `string`
{:#members:cssclass}

Specify the CSS class for Gantt to achieve custom theme.


#### Default Value

* ""


#### Example
{:.example}


{% highlight html %}
 
<div id="gantt"></div> 
<script>          
        $("#gantt").ejGantt({  cssClass : "gradient-lime" });
</script>

{% endhighlight %}

### dataSource `array`
{:#members:datasource}

Collection of data or hierarchical data to represent in Gantt


#### Default Value

* null


#### Example
{:.example}


{% highlight html %}
 
<div id="gantt"></div> 
<script>          
        $("#gantt").ejGantt(
 {
    dataSource:[{Id:2,TaskName:"Testing",startDate:"12/1/2000",Duration:5 }]    
 });            
</script>

{% endhighlight %}

### dateFormat `string`
{:#members:dateformat}

Specifies the dateFormat for Gantt , given format is displayed in tooltip , Grid .


#### Default Value

* "MM/dd/yyyy"


#### Example
{:.example}


{% highlight html %}
 
<div id="gantt"></div> 
<script>          
        $("#gantt").ejGantt(
 {
    dateFormat: "dd/MM/yyyy"
 });            
</script>

{% endhighlight %}

### dayWorkingTime `array`
{:#members:dayworkingtime}

Specifies the customized working time for tasks in Gantt 


#### Default Value

* [{ "from": "08:00 AM", "to": "12:00 PM" , background: ""  }, { "from": "01:00 PM", "to": "05:00 PM" , background: "" }]


#### Example
{:.example}


{% highlight html %}
 
<div id="gantt"></div> 
<script>          
        $("#gantt").ejGantt(
 {
    dayWorkingTime: [{ "from": "08:00 AM", "to": "12:00 PM" , background: "#FF0000" }, { "from": "01:00 PM", "to": "05:00 PM" , background: "#0000FF" }]
 });            
</script>

{% endhighlight %}

### dragTooltip `object`
{:#members:dragtooltip}

Option for customizing the drag tooltip while reordering the rows.


### dragTooltip.showTooltip `boolean`
{:#members:dragtooltip-showtooltip}

Specifies option to enable/disable tooltip while drag and drop a row.


#### Default Value

* true


#### Example


{% highlight html %}

<div id="gantt"></div> 
<script>          
        $("#gantt").ejGantt({  dragTooltip : { showTooltip:  true } });
</script>
{% endhighlight %}


### dragTooltip.tooltipItems `array`
{:#members:dragtooltip-tooltipitems}

Specifies the data source fields to be displayed in the drag tooltip.


#### Default Value

* []


#### Example


{% highlight html %}
                    
<div id="gantt"></div> 
<script>          
        $("#gantt").ejGantt({  dragTooltip : { tooltipItems: ["TaskName","TaskID","StartDate"] } });
</script>

{% endhighlight %}


### dragTooltip.tooltipTemplate `string`
{:#members:dragtooltip-tooltiptemplate}

Specifies the custom template for drag tooltip.


#### Default Value

* null


#### Example

{% highlight html %}               
                    
<div id="gantt"></div> 
<script>          
        $("#gantt").ejGantt({  dragTooltip : { tooltipTemplate: "" } });
</script>
{% endhighlight %}


### durationMapping `string`
{:#members:durationmapping}

Specifies the mapping property path for duration of a task in datasource


#### Default Value

* ""


#### Example
{:.example}


{% highlight html %}
 
<div id="gantt"></div> 
<script>          
        $("#gantt").ejGantt({  durationMapping : "Duration" });
</script>

{% endhighlight %}


### durationUnit `enum`
{:#members:durationunit}

<ts name = "ej.Gantt.DurationUnit"/>

Specifies the duration unit for each tasks whether days or hours or minutes

<table class="params">
<thead>
<tr>
<th>Name</th>
<th>Description</th>
</tr>
</thead>
<tbody>
<tr>
<td class="name">Day</td>
<td class="description">Sets the Duration Unit as day.</td>
</tr>
<tr>
<td class="name">Hour</td>
<td class="description">Sets the Duration Unit as hour.</td>
</tr>
<tr>
<td class="name">Minute</td>
<td class="description">Sets the Duration Unit as minute.</td>
</tr>
</tbody>
</table>

#### Default Value

* ej.Gantt.DurationUnit.Day


#### Example
{:.example}


{% highlight html %}
 
<div id="gantt"></div> 
<script>                          
        $("#gantt").ejGantt({  
                        durationUnit : ej.Gantt.DurationUnit.Hour });
</script>

{% endhighlight %}

### durationUnitMapping `string`
{:#members:durationunitmapping }

Specifies the mapping property path for task duration unit in datasource

#### Default Value

* ""


#### Example
{:.example}


{% highlight html %}
 
<div id="gantt"></div> 
<script>                  
        $("#gantt").ejGantt({  
                        durationUnitMapping : "durationUnit"});
</script>

{% endhighlight %}

### editDialogFields `array`
{:#members:editdialogfields}

Specifies the fields to be included in the edit dialog in Gantt


#### Default Value

* []


#### Example
{:.example}


{% highlight html %}
 
<div id="gantt"></div> 
<script>                  
        $("#gantt").ejGantt(
 {
    editDialogFields: [{ field: "taskId", editType: "stringedit" }]
 });            
</script>

{% endhighlight %}

### editDialogFields.field `string`
{:#members:editdialogfields-field}

Specifies mapping name to include required fields in Gantt


#### Default Value

* ""


#### Example


{% highlight html %}

<div id="gantt"></div> 
<script>                  
        $("#gantt").ejGantt(
 {
    editDialogFields: [{ field: "taskId" }]
 });            
</script>
{% endhighlight %}


### editDialogFields.editType `string`
{:#members:editdialogfields-edittype}

Specifies editType of fields to be included in the edit dialog in Gantt


#### Default Value

* ""


#### Example


{% highlight html %}

<div id="gantt"></div> 
<script>                  
        $("#gantt").ejGantt(
 {
    editDialogFields: [{ editType: "stringedit" }]
 });            
</script>
{% endhighlight %}

### editDialogFields.displayInGeneralTab `boolean`
{:#members:editdialogfields-displayingeneraltab}

Specifies the custom column field was displayed in General tab of edit dialog or not.

#### Default Value

* false

#### Example
{:.example}

{% highlight html %}

<div id="gantt"></div> 
<script>                  
$("#gantt").ejGantt(
{
     editDialogFields: [{ field:"customColumn", displayInGeneralTab: true }]
});
</script>

{% endhighlight %}

### editSettings `object`
{:#members:editsettings}

Specifies the editSettings options in Gantt.


### editSettings.allowAdding `boolean`
{:#members:editsettings-allowadding}

Enables or disables add record icon in Gantt toolbar


#### Default Value

* false


#### Example
{:.example}


{% highlight html %}
 
<div id="gantt"></div> 
<script>                  
        $("#gantt").ejGantt({  editSettings:{allowAdding : true} });
</script>

{% endhighlight %}


### editSettings.allowDeleting `boolean`
{:#members:editsettings-allowdeleting}

Enables or disables delete icon in Gantt toolbar


#### Default Value

* false


#### Example
{:.example}


{% highlight html %}
 
<div id="gantt"></div> 
<script>                  
        $("#gantt").ejGantt({  editSettings:{allowDeleting : true} });  
</script>

{% endhighlight %}


### editSettings.allowEditing `boolean`
{:#members:editsettings-allowediting}

Specifies the option for enabling or disabling editing in Gantt grid part


#### Default Value

* false


#### Example
{:.example}


{% highlight html %}
 
<div id="gantt"></div> 
<script>                  
        $("#gantt").ejGantt({  editSettings:{allowEditing : true} });   
</script>

{% endhighlight %}

### editSettings.allowIndent `boolean`
{:#members:editsettings-allowindent}

Specifies the option for enabling or disabling indent action in Gantt.


#### Default Value

* false


#### Example
{:.example}


{% highlight html %}
 
<div id="gantt"></div> 
<script>                  
        $("#gantt").ejGantt({  editSettings:{allowIndent : true} });   
</script>

{% endhighlight %}

### editSettings.beginEditAction `enum`
{:#members:editsettings-begineditaction}

<ts name = "ej.Gantt.BeginEditAction"/>

Specifies the mouse action whether single click or double click to begin the editing

<table class="params">
<thead>
<tr>
<th>Name</th>
<th>Description</th>
</tr>
</thead>
<tbody>
<tr>
<td class="name">DblClick</td>
<td class="description">you can begin the editing at double click</td>
</tr>
<tr>
<td class="name">Click</td>
<td class="description">you can begin the editing at single click</td>
</tr>
</tbody>
</table>


#### Default Value

* ej.Gantt.BeginEditAction.DblClick

#### Example


{% highlight html %}
                 
        $("#Gantt").ejGantt({  editSettings:{beginEditAction : ej.Gantt.BeginEditAction.Click} });

{% endhighlight %}

### editSettings.editMode `string`
{:#members:editsettings-editmode}

Specifies the edit mode in Gantt, "normal" is for dialog editing ,"cellEditing" is for cell type editing


#### Default Value

* normal


#### Example
{:.example}


{% highlight html %}
 
<div id="gantt"></div> 
<script>                  
        $("#gantt").ejGantt({  editSettings:{editMode : "normal"} });
</script>

{% endhighlight %}


### editSettings.rowPosition `enum`
{:#members:editsettings-rowposition}

<ts name = "ej.Gantt.RowPosition"/>

Specifies the position where the new row has to be added.

<table class="params">
<thead>
<tr>
<th>Name</th>
<th>Description</th>
</tr>
</thead>
<tbody>
<tr>
<td class="name">Top</td>
<td class="description">you can add a new row at top.</td>
</tr>
<tr>
<td class="name">Bottom</td>
<td class="description">you can add a new row at bottom.</td>
</tr>
<tr>
<td class="name">AboveSelectedRow</td>
<td class="description">you can add a new row to above selected row.</td>
</tr>
<tr>
<td class="name">BelowSelectedRow</td>
<td class="description">you can add a new row to below selected row.</td>
</tr>
<tr>
<td class="name">Child</td>
<td class="description">you can add a new row as a child for selected row.</td>
</tr>
</tbody>
</table>


#### Default Value

* ej.Gantt.RowPosition.BelowSelectedRow


#### Example


{% highlight html %}
   
 $("#gantt").ejGantt({  editSettings:{rowPosition : ej.Gantt.RowPosition.AboveSelectedRow} });

{% endhighlight %}

### editSettings.showDeleteConfirmDialog `boolean`

{:#members:editsettings-showdeleteconfirmdialog }

Enable or disable the confirmation dialog while deleting the record.

#### Default Value
* false

#### Example
{% highlight html %}
        $("#gantt").ejGantt ({  editSettings:{showDeleteConfirmDialog  : true} });     
{% endhighlight %}

### enableAltRow `boolean`
{:#members:enablealtrow}

Enables or Disables enableAltRow row effect in Gantt


#### Default Value

* true

#### Example
{:.example}


{% highlight html %}
 
<div id="gantt"></div> 
<script>                  
        $("#gantt").ejGantt({ enableAltRow : true});                    
</script>

{% endhighlight %}

### enableCollapseAll `boolean`
{:#members:enablecollapseall}

Enables or disables the collapse all records when loading the Gantt.


#### Default Value

* false


#### Example
{:.example}


{% highlight html %}
 
<div id="gantt"></div> 
<script>                  
        $("#gantt").ejGantt(
 {
    enableCollapseAll: false
 });            
</script>

{% endhighlight %}

### enableContextMenu `boolean`
{:#members:enablecontextmenu}

Enables or disables the contextmenu for Gantt , when enabled contextmenu appears on right clicking Gantt


#### Default Value

* false


#### Example
{:.example}


{% highlight html %}
 
<div id="gantt"></div> 
<script>                  
        $("#gantt").ejGantt(
 {
    enableContextMenu: false
 });            
</script>

{% endhighlight %}

### enablePredecessorValidation `boolean`
{:#members:enablepredecessorvalidation}

Enable or disable predecessor validation. When it is true, all the task's start and end dates are aligned based on its predecessors start and end dates.

#### Default Value

* true

#### Example
{:.example}


{% highlight html %}
 
<div id="gantt"></div> 
<script>        
        $("#gantt").ejGantt({ enablePredecessorValidation:  false });            
</script>

{% endhighlight %}

### enableProgressBarResizing `boolean`
{:#members:enableprogressbarresizing}

Indicates whether we can edit the progress of a task interactively in Gantt.


#### Default Value

* true


#### Example
{:.example}


{% highlight html %}
 
<div id="gantt"></div> 
<script>  
        $("#gantt").ejGantt({ enableProgressBarResizing:  true });                      
</script>

{% endhighlight %}


### enableResize `boolean`
{:#members:enableresize}

Enables or disables the option for dynamically updating the Gantt size on window resizing


#### Default Value

* false


#### Example
{:.example}


{% highlight html %}
 
<div id="gantt"></div> 
<script>                  
        $("#gantt").ejGantt(
 {
    enableResize: false
 });            
</script>

{% endhighlight %}

### enableSerialNumber `boolean`
{:#members:enableSerialNumber}

Enables or disables serial number column for Gantt. When enabled, the records will be number sequenced.

#### Default Value

* false

#### Example
{:.example}


{% highlight html %}
 
<div id="gantt"></div> 
<script>        
        $("#gantt").ejGantt({ enableSerialNumber:  true });            
</script>

{% endhighlight %}

### enableTaskbarDragTooltip `boolean`
{:#members:enabletaskbardragtooltip}

Enables or disables tooltip while editing (dragging/resizing) the taskbar.


#### Default Value

* true


#### Example
{:.example}


{% highlight html %}
 
<div id="gantt"></div> 
<script>                  
        $("#gantt").ejGantt({  
                        enableTaskbarDragTooltip : true});
</script>

{% endhighlight %}


### enableTaskbarTooltip `boolean`
{:#members:enabletaskbartooltip}

Enables or disables tooltip for taskbar.


#### Default Value

* true


#### Example
{:.example}


{% highlight html %}
 
<div id="gantt"></div> 
<script>                  
        $("#gantt").ejGantt({  enableTaskbarTooltip : true });  
</script>

{% endhighlight %}


### enableVirtualization `boolean`
{:#members:enablevirtualization}

Enables/Disables virtualization for rendering Gantt items.


#### Default Value

* false


#### Example
{:.example}


{% highlight html %}
 
<div id="gantt"></div> 
<script>                  
        $("#gantt").ejGantt({ enableVirtualization : true});                    
</script>

{% endhighlight %}

### enableWBS `boolean`
{:#members:enablewbs}

Enables/disables work breakdown structure column. 


#### Default Value

* false

#### Example
{:.example}


{% highlight html %}
 
<div id="gantt"></div> 
<script>                  
        $("#gantt").ejGantt({ enableWBS : true});                    
</script>

{% endhighlight %}

### enableWBSPredecessor `boolean`
{:#members:enablewbspredecessor}

Enables/disables WBS predecessor column. 


#### Default Value

* false

#### Example
{:.example}


{% highlight html %}
 
<div id="gantt"></div> 
<script>                  
        $("#gantt").ejGantt({ enableWBSPredecessor : true});                    
</script>

{% endhighlight %}

### endDateMapping `string`
{:#members:enddatemapping}

Specifies the mapping property path for end Date of a task in datasource


#### Default Value

* ""


#### Example
{:.example}


{% highlight html %}
 
<div id="gantt"></div> 
<script>                          
        $("#gantt").ejGantt({  endDateMapping : "EndDate" });   
</script>

{% endhighlight %}

### expandStateMapping `string`
{:#members:expandstatemapping}

Specifies the mapping property path for the expand status of a record in data source.


#### Default Value

* ""

#### Example
{:.example}


{% highlight html %}
 
<div id="gantt"></div> 
<script>                  
        $("#gantt").ejGantt({  expandStateMapping : "isExpanded" });
</script>

{% endhighlight %}

### filterSettings `object`
{:#members:filtersettings}

Options for filtering and customizing filter actions.

### filterSettings.filteredColumns `array`
{:#members:filtersettings-filteredcolumns}

Specifies the column collection for filtering the Gantt content on initial load

#### Default Value
* []

### filterSettings.filteredColumns.value `string`
{:#members:filtersettings-filteredcolumns-value}

Specifies the value to be filtered in Gantt.

#### Default Value
* -

### filterSettings.filteredColumns.field `string`
{:#members:filtersettings-filteredcolumns-field}

Specifies the field where filtering has to be performed.

#### Default Value
* -

### filterSettings.filteredColumns.predicate `string`
{:#members:filtersettings-filteredcolumns-predicate}

Specifies the predicate(and/or) value to perform filtering.

#### Default Value
* -

### filterSettings.filteredColumns.operator `string`
{:#members:filtersettings-filteredcolumns-operator}

Specifies the filter condition to filtered column. See <a href="global.html#enum:filteroperator">operator</a>

#### Default Value

* -

#### Example

{% highlight html %}

$("#gantt").ejGantt({
    filterSettings: {
        filteredColumns: [{
            value: "plan",
            field: "taskName",
            predicate: "and",
            operator: "startswith"
        }]
    },
});                   

{% endhighlight %}

### groupCollection `array`
{:#members:groupcollection}

Specifies the data collection for grouping the resources in resource allocation view in Gantt.

#### Default Value

* []

#### Example
{:.example}

{% highlight html %}
 
<div id="gantt"></div> 
<script>                  
        $("#gantt").ejGantt(
 {
   groupCollection:[{id:1; name:"Team A" }]     
 });            
</script>

{% endhighlight %}

### groupIdMapping `string`
{:#members:groupidmapping}
Specifies the mapping property path for group ID in datasource in resource allocation view type.

#### Default Value

* ""

#### Example
{:.example}

{% highlight html %}
 
<div id="gantt"></div> 
<script>                          
        $("#gantt").ejGantt({  groupIdMapping : "groupId" });    
</script>

{% endhighlight %}


### groupNameMapping `string`
{:#members:groupnamemapping}
Specifies the mapping property path for group name in datasource in resource allocation view type.

#### Default Value

* ""

#### Example
{:.example}

{% highlight html %}
 
<div id="gantt"></div> 
<script>                          
        $("#gantt").ejGantt({  groupNameMapping : "groupName" });    
</script>

{% endhighlight %}

### highlightNonWorkingTime `boolean`
{:#members:highlightnonworkingtime}

Specifies whether to highlight the non working time in Gantt.

#### Default Value
* false

#### Example

{% highlight html %}
 
<div id="gantt"></div> 
<script>  
        $("#gantt").ejGantt({ highlightNonWorkingTime:  true });
</script>

{% endhighlight %}

### highlightWeekends `boolean`
{:#members:highlightweekends}

Specifies whether to highlight the weekends in Gantt .


#### Default Value

* true


#### Example
{:.example}


{% highlight html %}
 
<div id="gantt"></div> 
<script>  
        $("#gantt").ejGantt({ highlightWeekends:  true });
</script>

{% endhighlight %}


### holidays `array`
{:#members:holidays}

Collection of holidays with date, background and label information to be displayed in Gantt.


#### Default Value

* []


#### Example
{:.example}


{% highlight html %}
 
<div id="gantt"></div> 
<script>                          
        $("#gantt").ejGantt(
 {
   holidays:[{day:"12/2/2000",background:"cyan",label:"local holiday" }]        
 });            
</script>

{% endhighlight %}

### holidays.day `string`
{:#members:holidays-day}

Specifies holiday date to be displayed in Gantt


#### Default Value

* ""


#### Example


{% highlight html %}

<div id="gantt"></div> 
<script>                  
        $("#gantt").ejGantt(
 {
    holidays:[{day:"12/2/2000" }]
 });            
</script>
{% endhighlight %}

### holidays.background `string`
{:#members:holidays-background}

Specifies the background color for holiday date in Gantt Schedule


#### Default Value

* ""


#### Example


{% highlight html %}

<div id="gantt"></div> 
<script>                  
        $("#gantt").ejGantt(
 {
    holidays:[{background:"cyan" }]   
 });            
</script>
{% endhighlight %}


### holidays.label `string`
{:#members:holidays-label}

Specifies the label to be displayed for rendered holiday in Gantt


#### Default Value

* ""


#### Example


{% highlight html %}

<div id="gantt"></div> 
<script>                  
        $("#gantt").ejGantt(
 {
    holidays:[{label:"local holiday" }]
 });            
</script>
{% endhighlight %}

### includeWeekend `boolean`
{:#members:includeweekend}

Specifies whether to include weekends while calculating the duration of a task.


#### Default Value

* true


#### Example
{:.example}


{% highlight html %}
 
<div id="gantt"></div> 
<script>  
        $("#gantt").ejGantt({ includeWeekend:  true });                 
</script>

{% endhighlight %}

### isResponsive `boolean`
{:#members:isresponsive}

Enables or disables the responsiveness of Gantt

#### Default Value

* false


#### Example


{% highlight html %}
                  
        $("#gantt").ejGantt({  isResponsive : true });                   

{% endhighlight %}

### leftTaskLabelMapping `string`
{:#members:lefttasklabelmapping}

Specifies the data source field name to be displayed as left task label

#### Default Value

* ""


#### Example
{:.example}


{% highlight html %}
 
<div id="gantt"></div> 
<script>                  
        $("#gantt").ejGantt(
 {
    leftTaskLabelMapping: "taskId",
 });            
</script>

{% endhighlight %}

### leftTaskLabelTemplate `string`
{:#members:lefttasklabeltemplate}

Specifies the template for left task label


#### Default Value

* ""


#### Example
{:.example}


{% highlight html %}
 
<div id="gantt"></div> 
<script>                  
        $("#gantt").ejGantt(
 {
    leftTaskLabelTemplate: "#customTaskLeftLabel",
 });            
</script>

{% endhighlight %}

### locale `string`
{:#members:locale}

Specify the locale for Gantt


#### Default Value

* "en-US"


#### Example
{:.example}


{% highlight html %}
 
<div id="gantt"></div> 
<script>          
        $("#gantt").ejGantt({  locale : "it-IT" });
</script>

{% endhighlight %}

### milestoneMapping `string`
{:#members:milestonemapping}

Specifies the mapping property path for milestone in datasource


#### Default Value

* ""


#### Example
{:.example}


{% highlight html %}
 
<div id="gantt"></div> 
<script>                          
        $("#gantt").ejGantt({  milestoneMapping : "milestone" });       
</script>

{% endhighlight %}

### milestoneTemplate `string`
{:#members:milestonetemplate}

To Specify the JsRender script Id to customize the mile stone with our preference


#### Default Value

* ""


#### Example
{:.example}


{% highlight html %}
 
<div id="gantt"></div> 
<script>          
        $("#gantt").ejGantt(
 {
    milestoneTemplate: "MilestoneTemplate"
 });            
</script>

{% endhighlight %}

### nonWorkingBackground `string`
{:#members:nonworkingbackground}

Specifies the background color for non working time in Gantt.

#### Default Value

* ""

#### Example

{% highlight html %}
 
<div id="gantt"></div> 
<script>
        $("#gantt").ejGantt({nonWorkingBackground: "#0000FF"});
</script>

{% endhighlight %}

### notesMapping `string`
{:#members:notesmapping }

Specifies the mapping property path for the task description in datasource

#### Default Value

* ""


#### Example
{:.example}


{% highlight html %}
 
<div id="gantt"></div> 
<script>                  
        $("#gantt").ejGantt({  
                        notesMapping : "notes"});
</script>

{% endhighlight %}

### parentProgressbarBackground `string`
{:#members:parentprogressbarbackground}

Specifies the background of parent progressbar in Gantt


#### Default Value

* ""


#### Example
{:.example}


{% highlight html %}
 
<div id="gantt"></div> 
<script>                  
        $("#gantt").ejGantt({  
        parentProgressbarBackground : "#F2F2F2"});
</script>

{% endhighlight %}

### parentTaskIdMapping `string`
{:#members:parenttaskidmapping}

Specifies the mapping property path for parent task Id in self reference datasource


#### Default Value

* ""


#### Example
{:.example}


{% highlight html %}
 
<div id="gantt"></div> 
<script>                  
        $("#gantt").ejGantt({  parentTaskIdMapping : "ID" });               
</script>

{% endhighlight %}

### parentTaskbarBackground `string`
{:#members:parenttaskbarbackground}

Specifies the background of parent taskbar in Gantt


#### Default Value

* ""


#### Example
{:.example}


{% highlight html %}
 
<div id="gantt"></div> 
<script>                  
        $("#gantt").ejGantt({  
                        parentTaskbarBackground : "#F2F2F2"});
</script>

{% endhighlight %}

### parentTaskbarTemplate `string`
{:#members:parenttaskbartemplate}

Specifies the template for parent taskbar


#### Default Value

* ""


#### Example
{:.example}


{% highlight html %}
 
<div id="gantt"></div> 
<script>          
        $("#gantt").ejGantt(
 {
    parentTaskbarTemplate: "ParentTaskbarTemplate"
 });            
</script>

{% endhighlight %}

### predecessorMapping `string`
{:#members:predecessormapping}

Specifies the mapping property path for predecessors of a task in datasource


#### Default Value

* ""


#### Example
{:.example}


{% highlight html %}
 
<div id="gantt"></div> 
<script>                          
        $("#gantt").ejGantt({  predecessorMapping : "predecessor" });           
</script>

{% endhighlight %}

### predecessorTooltipTemplate `string`
{:#members:predecessortooltiptemplate}

Specifies the JsRender template id or template script for predecessor tooltip on mouse action.


#### Default Value

* ""


#### Example
{:.example}


{% highlight html %}
 
<div id="gantt"></div> 
<script>                  
        $("#gantt").ejGantt(
 {
    predecessorTooltipTemplate: "PredecessorTooltipTemplate"
 });            
</script>

{% endhighlight %}

### progressMapping `string`
{:#members:progressmapping}

Specifies the mapping property path for progress percentage of a task in datasource


#### Default Value

* ""


#### Example
{:.example}


{% highlight html %}
 
<div id="gantt"></div> 
<script>                  
        $("#gantt").ejGantt({  progressMapping : "progress" });                 
</script>

{% endhighlight %}

### progressbarBackground `string`
{:#members:progressbarbackground}

Specifies the background of progressbar in Gantt


#### Default Value

* ""


#### Example
{:.example}


{% highlight html %}
 
<div id="gantt"></div> 
<script>  
        $("#gantt").ejGantt({  
                        progressbarBackground : "#F2F2F2"});
</script>

{% endhighlight %}


### progressbarHeight `number`
{:#members:progressbarheight}


Specified the height of the progressbar in taskbar


#### Default Value

* 100


#### Example
{:.example}


{% highlight html %}
 
<div id="gantt"></div> 
<script>          
        $("#gantt").ejGantt({  
                        progressbarHeight : 100 });
</script>

{% endhighlight %}


### progressbarTooltipTemplate `string`
{:#members:progressbartooltiptemplate}

Specifies the template for tooltip on resizing progressbar


#### Default Value

* null


#### Example
{:.example}


{% highlight html %}
 
<div id="gantt"></div> 
<script>          
        $("#gantt").ejGantt(
 {
    progressbarTooltipTemplate: ""
 });            
</script>

{% endhighlight %}


### progressbarTooltipTemplateId `string`
{:#members:progressbartooltiptemplateid}

Specifies the template ID for customized tooltip for progressbar editing in Gantt


#### Default Value

* null


#### Example
{:.example}


{% highlight html %}
 
<div id="gantt"></div> 
<script>  
        $("#gantt").ejGantt(
 {
    progressbarTooltipTemplateId: "tooltipTemplateID"
 });            
</script>

{% endhighlight %}

### query `object`
{:#members:query}

It receives query to retrieve data from the table (query is same as SQL).


#### Default Value

* null


#### Example
{:.example}


{% highlight html %}
<div id="gantt"></div> 
<script>                          
        $("#gantt").ejGantt(
 {
    query:ej.Query().from("Categories").select("CategoryID,CategoryName").take(3);      
 });            
</script>

{% endhighlight %}

### readOnly `boolean`
{:#members:readonly}

Enables or disables Gantt to read-only mode

#### Default Value

* false

#### Example
{:.example}

{% highlight html %}
 
<div id="gantt"></div> 
<script>          
        $("#gantt").ejGantt(
 {
    readOnly: true
 });            
</script>

{% endhighlight %}

### renderBaseline `boolean`
{:#members:renderbaseline}

Enables or Disables rendering baselines in Gantt , when enabled baseline is rendered in Gantt


#### Default Value

* false


#### Example
{:.example}


{% highlight html %}
 
<div id="gantt"></div> 
<script>          
        $("#gantt").ejGantt(
 {
    renderBaseline: false
 });            
</script>

{% endhighlight %}

### resourceCollectionMapping `string`
{:#members:resourcecollectionmapping}
Specifies the mapping property path for resource collection in datasource in resource allocation view type.

#### Default Value

* ""

#### Example
{:.example}

{% highlight html %}
 
<div id="gantt"></div> 
<script>                          
        $("#gantt").ejGantt({  resourceCollectionMapping : "resources" });    
</script>

{% endhighlight %}

### resourceIdMapping `string`
{:#members:resourceidmapping}

Specifies the mapping property name for resource ID in resource Collection in Gantt


#### Default Value

* ""


#### Example
{:.example}


{% highlight html %}
 
<div id="gantt"></div> 
<script>  
        $("#gantt").ejGantt(
 {
    resourceIdMapping: "peopleID"
 });            
</script>

{% endhighlight %}


### resourceInfoMapping `string`
{:#members:resourceinfomapping}

Specifies the mapping property path for resources of a task in datasource


#### Default Value

* ""


#### Example
{:.example}


{% highlight html %}
 
<div id="gantt"></div> 
<script>                          
        $("#gantt").ejGantt({  resourceInfoMapping : "resources" });    
</script>

{% endhighlight %}


### resourceNameMapping `string`
{:#members:resourcenamemapping}


Specifies the mapping property path for resource name of a task in Gantt


#### Default Value

* ""


#### Example
{:.example}


{% highlight html %}
 
<div id="gantt"></div> 
<script>          
        $("#gantt").ejGantt(
 {
    resourceNameMapping: "EmployeeName"
 });            
</script>

{% endhighlight %}

### resourceUnitMapping `string`
{:#members:resourceunitmapping}

Specifies the mapping property path for resource's percent effort involved in a task in datasource

#### Default Value

* ""


#### Example
{:.example}


{% highlight html %}
 
<div id="gantt"></div> 
<script>                  
        $("#gantt").ejGantt({  
                        resourceUnitMapping : "Unit"});
</script>

{% endhighlight %}

### resources `array`
{:#members:resources}

Collection of data regarding resources involved in entire project


#### Default Value

* []


#### Example
{:.example}


{% highlight html %}
 
<div id="gantt"></div> 
<script>                  
        $("#gantt").ejGantt(
 {
   resources:[{id:1; name:"jack" }]     
 });            
</script>

{% endhighlight %}


### rightTaskLabelMapping `string`
{:#members:righttasklabelmapping}

Specifies the data source field name to be displayed as right task label


#### Default Value

* ""


#### Example
{:.example}


{% highlight html %}
 
<div id="gantt"></div> 
<script>                  
        $("#gantt").ejGantt(
 {
    rightTaskLabelMapping: "taskName",
 });            
</script>

{% endhighlight %}

### rightTaskLabelTemplate `string`
{:#members:righttasklabeltemplate}

Specifies the template for right task label


#### Default Value

* ""


#### Example
{:.example}


{% highlight html %}
 
<div id="gantt"></div> 
<script>                  
        $("#gantt").ejGantt(
 {
    rightTaskLabelTemplate: "#customTaskRightLabel",
 });            
</script>

{% endhighlight %}

### roundOffDayworkingTime `boolean`
{:#members:roundoffdayworkingtime}


Specifies whether rounding off the day working time edits


#### Default Value

* true


#### Example
{:.example}


{% highlight html %}
 
<div id="gantt"></div> 
<script>                          
        $("#gantt").ejGantt({  
                        roundOffDayworkingTime : true });
</script>

{% endhighlight %}


### rowHeight `number`
{:#members:rowheight}

Specifies the height of a single row in Gantt. Also, we need to set same height in the CSS style with class name e-rowcell.


#### Default Value

* 30


#### Example
{:.example}


{% highlight html %}
 
<div id="gantt"></div> 
<script>                          
        $("#gantt").ejGantt({  
                        rowHeight : 30,
                        });
</script>

{% endhighlight %}

### scheduleEndDate `string`
{:#members:scheduleenddate}


Specifies end date of the Gantt schedule. By default, end date will be rounded to its next Saturday.


#### Default Value

* null


#### Example
{:.example}


{% highlight html %}
 
<div id="gantt"></div> 
<script>                          
        $("#gantt").ejGantt(
 {
    scheduleEndDate:"12/2/2000"
 });            
</script>

{% endhighlight %}


### scheduleHeaderSettings `object`
{:#members:scheduleheadersettings}

Specifies the options for customizing schedule header.


### scheduleHeaderSettings.dayHeaderFormat `string`
{:#members:scheduleheadersettings-dayheaderformat}

Specified the format for day view in schedule header


#### Default Value

* ""


#### Example
{:.example}


{% highlight html %}
 
<div id="gantt"></div> 
<script>                          
        $("#gantt").ejGantt({  
                        scheduleHeaderSettings:{dayHeaderFormat : "ddd" }
                });
</script>              

{% endhighlight %}


### scheduleHeaderSettings.hourHeaderFormat `string`
{:#members:scheduleheadersettings-hourheaderformat}

Specified the format for Hour view in schedule header


#### Default Value

* "HH"


#### Example
{:.example}


{% highlight html %}
 
<div id="gantt"></div> 
<script>                  
        $("#gantt").ejGantt({  
                        scheduleHeaderSettings:{hourHeaderFormat : 'HH'}
                });
</script>               

{% endhighlight %}


### scheduleHeaderSettings.minutesPerInterval `enum`
{:#members:scheduleheadersettings-minutesperinterval}

<ts name = "ej.Gantt.minutesPerInterval"/>

Specifies the number of minutes per interval

<table class="params">
<thead>
<tr>
<th>Name</th>
<th>Description</th>
</tr>
</thead>
<tbody>
<tr>
<td class="name">Auto</td>
<td class="description">Sets the interval automatically according with schedule start and end date.</td>
</tr>
<tr>
<td class="name">OneMinute</td>
<td class="description">Sets one minute intervals per hour.</td>
</tr>
<tr>
<td class="name">FiveMinutes</td>
<td class="description">Sets Five minute intervals per hour.</td>
</tr>
<tr>
<td class="name">FifteenMinutes</td>
<td class="description">Sets fifteen minute intervals per hour.</td>
</tr>
<tr>
<td class="name">ThirtyMinutes</td>
<td class="description">Sets thirty minute intervals per hour.</td>
</tr>
</tbody>
</table>

#### Default Value

* ej.Gantt.minutesPerInterval.Auto


#### Example
{:.example}


{% highlight html %}
 
<div id="gantt"></div> 
<script>                          
        $("#gantt").ejGantt({  
                        scheduleHeaderSettings:{minutesPerInterval : ej.Gantt.minutesPerInterval.OneMinute}});              
</script>              

{% endhighlight %}


### scheduleHeaderSettings.monthHeaderFormat `string`
{:#members:scheduleheadersettings-monthheaderformat}

Specified the format for month view in schedule header


#### Default Value

* "MMM"


#### Example
{:.example}


{% highlight html %}
 
<div id="gantt"></div> 
<script>                          
        $("#gantt").ejGantt({  
                        scheduleHeaderSettings:{monthHeaderFormat : "MMM" }
               });
</script>              

{% endhighlight %}


### scheduleHeaderSettings.scheduleHeaderType `enum`
{:#members:scheduleheadersettings-scheduleheadertype}

<ts name = "ej.Gantt.ScheduleHeaderType"/>

Specifies the schedule mode

<table class="params">
<thead>
<tr>
<th>Name</th>
<th>Description</th>
</tr>
</thead>
<tbody>
<tr>
<td class="name">Year</td>
<td class="description">Sets year Schedule Mode.</td>
</tr>
<tr>
<td class="name">Month</td>
<td class="description">Sets month Schedule Mode.</td>
</tr>
<tr>
<td class="name">Week</td>
<td class="description">Sets week Schedule Mode.</td>
</tr>
<tr>
<td class="name">Day</td>
<td class="description">Sets day Schedule Mode.</td>
</tr>
<tr>
<td class="name">Hour</td>
<td class="description">Sets hour Schedule Mode.</td>
</tr>
</tbody>
</table>

#### Default Value

* ej.Gantt.ScheduleHeaderType.Week


#### Example
{:.example}


{% highlight html %}
 
<div id="gantt"></div> 
<script>                          
    $("#gantt").ejGantt({  
               scheduleHeaderSettings:{scheduleHeaderType : ej.Gantt.ScheduleHeaderType.Month}
    });
</script>              

{% endhighlight %}

### scheduleHeaderSettings.timescaleStartDateMode `enum`
{:#members:scheduleheadersettings-timescalestartdatemode}

<ts name = "ej.Gantt.TimescaleRoundMode"/>

Specifies the round-off mode for the start date in schedule header.

<table class="params">
<thead>
<tr>
<th>Name</th>
<th>Description</th>
</tr>
</thead>
<tbody>
<tr>
<td class="name">Auto</td>
<td class="description">The round-off value will be automatically calculated based on the data source values.</td>
</tr>
<tr>
<td class="name">Week</td>
<td class="description">Schedule header start date will round-off to the immediate week.</td>
</tr>
<tr>
<td class="name">Month</td>
<td class="description">Schedule headers start date will round off to the immediate month</td>
</tr>
<tr>
<td class="name">Year</td>
<td class="description">Schedule headers start date will round off to the immediate year</td>
</tr>
</tbody>
</table>

#### Default Value

* ej.Gantt.TimescaleRoundMode.Auto


#### Example
{:.example}


{% highlight html %}
 
<div id="gantt"></div> 
<script>                          
        $("#gantt").ejGantt({  
                        scheduleHeaderSettings:{timescaleStartDateMode : ej.Gantt.TimescaleRoundMode.Week}
                });              
</script>              

{% endhighlight %}

### scheduleHeaderSettings.weekendBackground `string`
{:#members:scheduleheadersettings-weekendbackground}

Specified the background for weekends in Gantt


#### Default Value

* "#F2F2F2"


#### Example
{:.example}


{% highlight html %}
 
<div id="gantt"></div> 
<script>                  
        $("#gantt").ejGantt({  
                        scheduleHeaderSettings:{weekendBackground : "#F2F2F2"}});
</script>

{% endhighlight %}


### scheduleHeaderSettings.weekHeaderFormat `string`
{:#members:scheduleheadersettings-weekheaderformat}

Specified the format for week view in schedule header


#### Default Value

* "MMM dd , yyyy"


#### Example
{:.example}


{% highlight html %}
 
<div id="gantt"></div> 
<script>                          
        $("#gantt").ejGantt({  
                        scheduleHeaderSettings:{weekHeaderFormat : "MMM dd , yyyy" }
               });
</script>

{% endhighlight %}


### scheduleHeaderSettings.yearHeaderFormat `string`
{:#members:scheduleheadersettings-yearheaderformat}

Specified the format for year view in schedule header


#### Default Value

* "yyyy"


#### Example
{:.example}


{% highlight html %}
 
<div id="gantt"></div> 
<script>                          
        $("#gantt").ejGantt({  
                        scheduleHeaderSettings:{yearHeaderFormat : "yyyy" }
               });
</script>               

{% endhighlight %}


### scheduleHeaderSettings.timescaleUnitSize `string`
{:#members:scheduleheadersettings-timescaleunitsize}

Specifies the size of the lowest time unit along the timescale, with minimum value as "50%" and maximum value as "500%". It is also possible to set the value in pixels.


#### Default Value

* "100%"


#### Example
{:.example}


{% highlight html %}
 
<div id="gantt"></div> 
<script>                          
        $("#gantt").ejGantt({  
                        scheduleHeaderSettings:{timescaleUnitSize : "250%" }
               });
</script>               

{% endhighlight %}


### scheduleHeaderSettings.weekStartDay `number`
{:#members:scheduleheadersettings-weekstartday}

Specifies the start day of the week in week timescale mode


#### Default Value

* 0


#### Example
{:.example}


{% highlight html %}
 
<div id="gantt"></div> 
<script>                          
        $("#gantt").ejGantt({  
                        scheduleHeaderSettings:{weekStartDay : 3 }
               });
</script>               

{% endhighlight %}

### scheduleHeaderSettings.updateTimescaleView `boolean`
{:#members:scheduleheadersettings-updatetimescaleview}

Enable or disable the automatic timescale update on cell editing, dialog editing and taskbar editing.

#### Default Value

* true

#### Example
{:.example}

{% highlight html %}
 
<div id="gantt"></div> 
<script>                          
    $("#gantt").ejGantt({  
       scheduleHeaderSettings:{updateTimescaleView : false }
    });
</script>               

{% endhighlight %}

### scheduleStartDate `string`
{:#members:schedulestartdate}

Specifies start date of the Gantt schedule. By default, start date will be rounded to its previous Sunday.


#### Default Value


* null


#### Example
{:.example}


{% highlight html %}
 
<div id="gantt"></div> 
<script>                          
        $("#gantt").ejGantt(
 {
    scheduleStartDate:"12/2/2000"
 });            
</script>

{% endhighlight %}

### selectedCellIndexes `array`
{:#members:selectedcellindexes}

Specifies the selected cell information on rendering Gantt.

### selectedCellIndexes.rowIndex `number`
{:#members:selectedcellindexes-rowindex}


Specifies the row index of the cell to be selected Gantt control


#### Default Value

* -1

### selectedCellIndexes.cellIndex `number`
{:#members:selectedcellindexes-cellindex}

Specifies the cell index to be selected in the row.


#### Default Value

* -1

#### Example
{:.example}


{% highlight html %}
 
<div id="gantt"></div> 
<script>                  
        $("#gantt").ejGantt(
 {
    selectedCellIndexes:[{rowIndex: 2, cellIndex: 3}];
 });            
</script>

{% endhighlight %}

### selectedRowIndex `number`
{:#members:selectedrowindex}

Specifies the selected row Index in Gantt , the row with given index will highlighted


#### Default Value

* -1


#### Example
{:.example}


{% highlight html %}
 
<div id="gantt"></div> 
<script>                  
        $("#gantt").ejGantt(
 {
    selectedRowIndex:2
 });            
</script>

{% endhighlight %}

### selectionType `enum`
{:#members:selectiontype}

<ts name = "ej.Gantt.SelectionType"/>

Specifies the row selection type.

<table class="params">
<thead>
<tr>
<th>Name</th>
<th>Description</th>
</tr>
</thead>
<tbody>
<tr>
<td class="name">Single</td>
<td class="description">you can select a single row.</td>
</tr>
<tr>
<td class="name">Multiple</td>
<td class="description">you can select a multiple row.</td>
</tr>
</tbody>
</table>

#### Default Value

* ej.Gantt.SelectionType.Single


#### Example


{% highlight html %}
          
<div id="gantt"></div> 
<script>   
        $("#gantt").ejGantt({ selectionType:ej.Gantt.SelectionType.Multiple });                      * 
</script>           

{% endhighlight %}

### selectionMode `enum`
{:#members:selectionmode}

<ts name = "ej.Gantt.SelectionMode"/>

Specifies the type of selection whether to select row or cell.

<table class="params">
<thead>
<tr>
<th>Name</th>
<th>Description</th>
</tr>
</thead>
<tbody>
<tr>
<td class="name">Row</td>
<td class="description">you can select a row.</td>
</tr>
<tr>
<td class="name">Cell</td>
<td class="description">you can select a cell.</td>
</tr>
</tbody>
</table>

#### Default Value

* ej.Gantt.SelectionMode.Row


#### Example


{% highlight html %}
          
<div id="gantt"></div> 
<script>   
        $("#gantt").ejGantt({ selectionMode:ej.Gantt.SelectionMode.Row });                      * 
</script>           

{% endhighlight %}

### showColumnChooser `boolean`
{:#members:showcolumnchooser}

Enables or disables the column chooser.


#### Default Value

* false


#### Example
{:.example}


{% highlight html %}
 
<div id="gantt"></div> 
<script>   
        $("#gantt").ejGantt({ showColumnChooser:  true });                      * 
</script>

{% endhighlight %}

### showColumnOptions `boolean`
{:#members:showcolumnoptions}

Enables/disables the options for inserting , deleting and renaming  columns.       

#### Default Value

* false

#### Example
{:.example}


{% highlight html %}
 
<div id="gantt"></div> 
<script>   
        $("#gantt").ejGantt({ showColumnOptions:  true });                      * 
</script>

{% endhighlight %}

### showGridCellTooltip `boolean`
{:#members:showgridcelltooltip}

Specifies the template for cell tooltip

#### Default Value

* true


#### Example
{:.example}


{% highlight html %}
 
<div id="gantt"></div> 
<script>                  
        $("#gantt").ejGantt({  
                        showGridCellTooltip : true});
</script>

{% endhighlight %}


### showGridExpandCellTooltip `boolean`
{:#members:showgridexpandcelltooltip}

Specifies whether to show grid cell tooltip over expander cell alone.


#### Default Value

* true


#### Example
{:.example}


{% highlight html %}
 
<div id="gantt"></div> 
<script>                  
        $("#gantt").ejGantt({  
                        showGridExpandCellTooltip : true});
</script>

{% endhighlight %}


### showProgressStatus `boolean`
{:#members:showprogressstatus}

Specifies whether display task progress inside taskbar.


#### Default Value

* true


#### Example
{:.example}


{% highlight html %}
 
<div id="gantt"></div> 
<script>                  
        $("#gantt").ejGantt({  
                        showProgressStatus : true});
</script>

{% endhighlight %}


### showResourceNames `boolean`
{:#members:showresourcenames}

Specifies whether to display resource names for a task beside taskbar.


#### Default Value

* true


#### Example
{:.example}


{% highlight html %}
 
<div id="gantt"></div> 
<script>                  
        $("#gantt").ejGantt({  
                        showResourceNames : true});
</script>

{% endhighlight %}


### showTaskNames `boolean`
{:#members:showtasknames}

Specifies whether to display task name beside task bar.


#### Default Value


* true


#### Example
{:.example}


{% highlight html %}
 
<div id="gantt"></div> 
<script>                  
        $("#gantt").ejGantt({  
                        showTaskNames : true});
</script>

{% endhighlight %}


### sizeSettings `object`
{:#members:sizesettings}

Specifies the size option of Gantt control.


### sizeSettings.height `string`
{:#members:sizesettings-height}


Specifies the height of Gantt control


#### Default Value

* ""


#### Example
{:.example}


{% highlight html %}
 
<div id="gantt"></div> 
<script>                  
        $("#gantt").ejGantt(
 {
    sizeSettings:{height: "700px"}
 });            
</script>

{% endhighlight %}


### sizeSettings.width `string`
{:#members:sizesettings-width}

Specifies the width of Gantt control


#### Default Value

* ""


#### Example
{:.example}


{% highlight html %}
 
<div id="gantt"></div> 
<script>          
        $("#gantt").ejGantt(
 {
    sizeSettings:{width: "700px"}
 });            
</script>

{% endhighlight %}



### sortSettings `object`
{:#members:sortsettings}

Specifies the sorting options for Gantt.


### sortSettings.sortedColumns `array`
{:#members:sortsettings-sortedcolumns}

Specifies the sorted columns for Gantt


#### Default Value

* []


#### Example
{:.example}


{% highlight html %}
 
<div id="gantt"></div> 
<script>          
        $("#gantt").ejGantt({ sortSettings:{sortedColumns : [{ field:"startDate",direction:"ascending" }]}});                  
</script>

{% endhighlight %}

### sortSettings.sortedColumns.field `string`
{:#members:sortsettings-sortedcolumns-field}

Specifies the field to be sorted in Gantt


#### Default Value

* ""


#### Example
{:.example}


{% highlight html %}
 
<div id="gantt"></div> 
<script>          
        $("#gantt").ejGantt({ sortSettings:{sortedColumns : [{ field:"startDate" }]}});                  
</script>

{% endhighlight %}

### sortSettings.sortedColumns.direction `string`
{:#members:sortsettings-sortedcolumns-direction}

Specifies the sort direction in Gantt


#### Default Value

* ""


#### Example
{:.example}


{% highlight html %}
 
<div id="gantt"></div> 
<script>          
        $("#gantt").ejGantt({ sortSettings:{sortedColumns : [{ direction:"ascending" }]}});                  
</script>

{% endhighlight %}

### splitterPosition `string`
{:#members:splitterposition}

Specifies splitter position in Gantt.


#### Default Value

* null


#### Example
{:.example}


{% highlight html %}
 
<div id="gantt"></div> 
<script>                                  
        $("#gantt").ejGantt({  splitterPosition : "50%" });     
</script>

{% endhighlight %}

### splitterSettings `object`
{:#members:splittersettings}

Option to configure the splitter position.


### splitterSettings.position `string`
{:#members:splittersettings-position}

Specifies position of the splitter in Gantt , splitter can be placed either based on percentage values or pixel values.

#### Default Value

* ""

#### Example
{:.example}


{% highlight html %}
 
<div id="gantt"></div> 
<script>                  
        $("#gantt").ejGantt({  splitterSettings:{position : "300px"} });
</script>

{% endhighlight %}


### splitterSettings.index `string`
{:#members:splittersettings-index}

Specifies the position of splitter in Gantt, based on column index in Gantt.

#### Default Value

* ""

#### Example
{:.example}


{% highlight html %}
 
<div id="gantt"></div> 
<script>                  
        $("#gantt").ejGantt({  splitterSettings:{index : "3"} });
</script>

{% endhighlight %}

### startDateMapping `string`
{:#members:startdatemapping}


Specifies the mapping property path for start date of a task in datasource


#### Default Value

* ""


#### Example
{:.example}


{% highlight html %}
 
<div id="gantt"></div> 
<script>                                  
        $("#gantt").ejGantt({  startDateMapping : "startDate" });                
</script>

{% endhighlight %}


### stripLines `array`
{:#members:striplines}

Specifies the options for striplines


#### Default Value

* []


#### Example
{:.example}


{% highlight html %}
 
<div id="gantt"></div> 
<script>                  
        $("#gantt").ejGantt(stripLines: [
   {
    day: "12/2/2000,
    label: "Project Release",
    lineStyle: "dotted",
    lineColor: "DarkBlue",
    lineWidth: 2
  }
]); 
</script>

{% endhighlight %}

### stripLines.day `string`
{:#members:striplines-day}

Specifies date to render striplines in Gantt


#### Default Value

* ""


#### Example


{% highlight html %}

<div id="gantt"></div> 
<script>                  
        $("#gantt").ejGantt(
 {
     $("#gantt").ejGantt(stripLines: [{ day: "12/2/2000"}]); 
 });            
</script>
{% endhighlight %}

### stripLines.label `string`
{:#members:striplines-label}

Specifies label to be displayed for striplines in Gantt


#### Default Value

* ""


#### Example


{% highlight html %}

<div id="gantt"></div> 
<script>                  
        $("#gantt").ejGantt(
 {
     $("#gantt").ejGantt(stripLines: [{ label: "Project Release" }]); 
 });            
</script>
{% endhighlight %}

### stripLines.lineStyle `string`
{:#members:striplines-linestyle}

Specifies line style for rendered striplines in Gantt


#### Default Value

* ""


#### Example


{% highlight html %}

<div id="gantt"></div> 
<script>                  
        $("#gantt").ejGantt(
 {
     $("#gantt").ejGantt(stripLines: [{ lineStyle: "dotted"}]); 
 });            
</script>
{% endhighlight %}

### stripLines.lineColor `string`
{:#members:striplines-linecolor}

Specifies the line color for rendered striplines in Gantt


#### Default Value

* ""


#### Example


{% highlight html %}

<div id="gantt"></div> 
<script>                  
        $("#gantt").ejGantt(
 {
     $("#gantt").ejGantt(stripLines: [{ lineColor: "Darkblue"}]); 
 });            
</script>
{% endhighlight %}

### stripLines.lineWidth `string`
{:#members:striplines-linewidth}

Specifies the width of the stripline in Gantt


#### Default Value

* ""


#### Example


{% highlight html %}

<div id="gantt"></div> 
<script>                  
        $("#gantt").ejGantt(
 {
     $("#gantt").ejGantt(stripLines: [{ lineWidth : "2"}]); 
 });            
</script>
{% endhighlight %}

### taskCollectionMapping `string`
{:#members:taskcollectionmapping}
Specifies the mapping property path for assigned task collection for resources in datasource in resource allocation view type.

#### Default Value

* ""

#### Example
{:.example}

{% highlight html %}
 
<div id="gantt"></div> 
<script>                          
        $("#gantt").ejGantt({  taskCollectionMapping : "tasks" });    
</script>

{% endhighlight %}

### taskIdMapping `string`
{:#members:taskidmapping}

Specifies the mapping property path for task Id in datasource


#### Default Value

* ""


#### Example
{:.example}


{% highlight html %}
 
<div id="gantt"></div> 
<script>                                  
        $("#gantt").ejGantt({  taskIdMapping : "ID" }); 
</script>

{% endhighlight %}


### taskNameMapping `string`
{:#members:tasknamemapping}

Specifies the mapping property path for task name in datasource


#### Default Value

* ""


#### Example
{:.example}


{% highlight html %}
 
<div id="gantt"></div> 
<script>          
        $("#gantt").ejGantt({  taskNameMapping : "Name" });     
</script>

{% endhighlight %}

### taskSchedulingMode `enum`
{:#members:taskschedulingmode}

<ts name = "ej.Gantt.TaskSchedulingMode"/>

Specifies the task scheduling mode for a project and this will be set to all the tasks available in the project

<table class="params">
<thead>
<tr>
<th>Name</th>
<th>Description</th>
</tr>
</thead>
<tbody>
<tr>
<td class="name">Auto</td>
<td class="description">All the tasks in the project will be displayed in auto scheduled mode,
 where the tasks are scheduled automatically over non-working days and holidays.</td>
</tr>
<tr>
<td class="name">Manual</td>
<td class="description">All the tasks in the project will be displayed in manually scheduled mode.</td>
</tr>
<tr>
<td class="name">Custom</td>
<td class="description">Project consists of tasks with both auto and manually scheduled modes, based on the datasource values</td>
</tr>
</tbody>
</table>

#### Default Value

*  ej.Gantt.TaskSchedulingMode.Auto


#### Example
{:.example}


{% highlight html %}
 
<div id="gantt"></div> 
<script>                          
        $("#gantt").ejGantt({  
                        taskSchedulingMode : ej.Gantt.TaskSchedulingMode.Auto });
</script>

{% endhighlight %}

### taskSchedulingModeMapping `string`
{:#members:taskschedulingmodemapping }

Specifies the mapping property path for the task scheduling mode for a task in datasource

#### Default Value

* "auto"


#### Example
{:.example}


{% highlight html %}
 
<div id="gantt"></div> 
<script>                  
        $("#gantt").ejGantt({  
                        taskSchedulingModeMapping : "taskMode"});
</script>

{% endhighlight %}

### taskType `enum`
{:#members:tasktype}

<ts name = "ej.Gantt.TaskType"/>

Specifies the nature of a task for calculating the work,  and it can fixed duration, fixed work and fixed resource unit

<table class="params">
<thead>
<tr>
<th>Name</th>
<th>Description</th>
</tr>
</thead>
<tbody>
<tr>
<td class="name">FixedUnit</td>
<td class="description">Resource unit remains constant while editing the work and duration values.</td>
</tr>
<tr>
<td class="name">FixedWork</td>
<td class="description">Work value of a task remains constant while editing duration and resource unit values.</td>
</tr>
<tr>
<td class="name">FixedDuration</td>
<td class="description">Duration value remains constant while editing work and resource unit values.</td>
</tr>
</tbody>
</table>

#### Default Value

*  ej.Gantt.TaskType.FixedUnit


#### Example
{:.example}


{% highlight html %}
 
<div id="gantt"></div> 
<script>                          
        $("#gantt").ejGantt({  
                        taskType : ej.Gantt.TaskType.FixedWork });
</script>

{% endhighlight %}

### taskbarBackground `string`
{:#members:taskbarbackground}

Specifies the background of the taskbar in Gantt


#### Default Value

* ""


#### Example
{:.example}


{% highlight html %}
 
<div id="gantt"></div> 
<script>  
        $("#gantt").ejGantt({  
                        taskbarBackground : "#F2F2F2"});
</script>

{% endhighlight %}


### taskbarEditingTooltipTemplate `string`
{:#members:taskbareditingtooltiptemplate}

Specifies the template script for customized tooltip for taskbar editing in Gantt


#### Default Value

* ""


#### Example
{:.example}


{% highlight html %}
 
<div id="gantt"></div> 
<script>                  
        $("#gantt").ejGantt(
 {
    taskbarEditingTooltipTemplate: "tooltipTemplate"
 });            
</script>

{% endhighlight %}

### taskbarEditingTooltipTemplateId `string`
{:#members:taskbareditingtooltiptemplateid}


Specifies the template Id for customized tooltip for taskbar editing in Gantt


#### Default Value

* ""


#### Example
{:.example}


{% highlight html %}
 
<div id="gantt"></div> 
<script>          
        $("#gantt").ejGantt(
 {
    taskbarEditingTooltipTemplateId: "TooltipTemplateId"
 });            
</script>

{% endhighlight %}

### taskbarHeight `number`
{:#members:taskbarheight}


Specifies the height of taskBar in Gantt.


#### Default Value

* 20


#### Example
{:.example}


{% highlight html %}
 
<div id="gantt"></div> 
<script>          
        $("#gantt").ejGantt(
 {
    taskbarHeight: 25
 });            
</script>

{% endhighlight %}

### taskbarTemplate `string`
{:#members:taskbartemplate}

To Specify the JsRender script Id to customize the task bar with our preference


#### Default Value

* ""


#### Example
{:.example}


{% highlight html %}
 
<div id="gantt"></div> 
<script>          
        $("#gantt").ejGantt(
 {
    taskbarTemplate: "TaskbarTemplate"
 });            
</script>

{% endhighlight %}

### taskbarTooltipTemplate `string`
{:#members:taskbartooltiptemplate}

Specifies the template for tooltip on mouse action on taskbars


#### Default Value

* ""


#### Example
{:.example}


{% highlight html %}
 
<div id="gantt"></div> 
<script>                  
        $("#gantt").ejGantt(
 {
    taskbarTooltipTemplate: "TooltipTemplate"
 });            
</script>

{% endhighlight %}

### taskbarTooltipTemplateId `string`
{:#members:taskbartooltiptemplateid}

Specifies the template id for tooltip on mouse action on taskbars


#### Default Value

* ""


#### Example
{:.example}


{% highlight html %}
 
<div id="gantt"></div> 
<script>          
        $("#gantt").ejGantt(
 {
    taskbarTooltipTemplateId: "TooltipTemplateId"
 });            
</script>

{% endhighlight %}

### toolbarSettings `object`
{:#members:toolbarsettings}

Specifies the toolbarSettings options.


### toolbarSettings.showToolbar `boolean`
{:#members:toolbarsettings-showtoolbar}

Specifies the state of enabling or disabling toolbar


#### Default Value

* true


#### Example
{:.example}


{% highlight html %}
 
<div id="gantt"></div> 
<script>  
        $("#gantt").ejGantt({ showToolbar:  true });                     
</script>

{% endhighlight %}


### toolbarSettings.toolbarItems `array`
{:#members:toolbarsettings-toolbaritems}

<ts name="ej.Gantt.ToolbarItems" />

Specifies the list of toolbar items to be rendered in Gantt toolbar

<table class="params">
<thead>
<tr>
<th>Name</th>
<th>Description</th>
</tr>
</thead>
<tbody>
<tr>
<td class="name">Add</td>
<td class="description">Enables the add icon in toolbar</td>
</tr>
<tr>
<td class="name">Edit</td>
<td class="description">Enables the edit icon in toolbar</td>
</tr>
<tr>
<td class="name">Delete</td>
<td class="description">Enables the edit icon in toolbar</td>
</tr>
<tr>
<td class="name">Update</td>
<td class="description">Enables the update icon in toolbar</td>
</tr>
<tr>
<td class="name">Cancel</td>
<td class="description">Enables the cancel icon in toolbar</td>
</tr>
<tr>
<td class="name">Search</td>
<td class="description">Enables the search icon in toolbar</td>
</tr>
<tr>
<td class="name">Indent</td>
<td class="description">Enables the indent icon in toolbar</td>
</tr>
<tr>
<td class="name">Outdent</td>
<td class="description">Enables the outdent icon in toolbar</td>
</tr>
<tr>
<td class="name">ExpandAll</td>
<td class="description">Enables the expand all icon in toolbar</td>
</tr>
<tr>
<td class="name">Collapse All</td>
<td class="description">Enables the collapse all icon in toolbar</td>
</tr>
<tr>
<td class="name">PrevTimeSpan</td>
<td class="description">Enables the previous time span icon in toolbar</td>
</tr>
<tr>
<td class="name">NextTimeSpan</td>
<td class="description">Enables the next time span icon in toolbar</td>
</tr>
<tr>
<td class="name">CriticalPath</td>
<td class="description">Enables the critical path icon in toolbar</td>
</tr>
<tr>
<td class="name">ExcelExport</td>
<td class="description">Enables the excel export toolbar icon</td>
</tr>
<tr>
<td class="name">PdfExport</td>
<td class="description">Enables the pdf export toolbar icon</td>
</tr>
</tbody>
</table>

#### Default Value
* []

#### Example
{:.example}


{% highlight html %}
 
<div id="gantt"></div> 
<script>  
        $("#gantt").ejGantt({ toolbarSettings: { toolbarItems: [ej.Gantt.ToolbarItems.Add,ej.Gantt.ToolbarItems.Edit] } });                   
</script>

{% endhighlight %}

### toolbarSettings.customToolbarItems `array`
{:#members:toolbarsettings-customtoolbaritems}

Allows the user to insert custom toolbar items.

### toolbarSettings.customToolbarItems.text `string`
{:#members:toolbarsettings-customtoolbaritems-text}

Allows the user to insert the custom icons in toolbar using CSS class name selector.


#### Default Value

* ""


#### Example


{% highlight html %}
            <div id="gantt"></div> 
<script>      
        $("#gantt").ejGantt({toolbarSettings: {customToolbarItems: [{ text: "Reset",tooltipText:"Reset" }]}});
</script>
{% endhighlight %}


### toolbarSettings.customToolbarItems.templateID `string`
{:#members:toolbarsettings-customtoolbaritems-templateid}

Allows the user to insert the custom icons in toolbar using script templates. Using this property we can bind HTML elements and other EJ controls to Gantt toolbar.


#### Default Value

* ""


#### Example


{% highlight html %}
 <div id="gantt"></div> 
<script>      
         $("#gantt").ejGantt({toolbarSettings: {customToolbarItems: [{ templateID: "#ColumnVisibility",tooltipText:"Column Visibility" }]}});  
</script>				

{% endhighlight %}


### toolbarSettings.customToolbarItems.tooltipText `string`
{:#members:toolbarsettings-customtoolbaritems-tooltiptext}

Allows the user to display custom tooltip text for Gantt custom toolbar items.


#### Default Value

* ""


#### Example


{% highlight html %}
        <div id="gantt"></div> 
<script>            
        $("#gantt").ejGantt({toolbarSettings: {customToolbarItems: [{ templateID: "#ColumnVisibility",tooltipText:"Column Visibility" },{ text: "Reset",tooltipText:"Column Visibility" }]}});  
</script>				

{% endhighlight %}

### treeColumnIndex `number`
{:#members:treecolumnindex}

Specifies the tree expander column in Gantt


#### Default Value

* 0


#### Example
{:.example}


{% highlight html %}
 
<div id="gantt"></div> 
<script>          
        $("#gantt").ejGantt(
 {
    treeColumnIndex: 1
 });            
</script>

{% endhighlight %}

### validateManualTasksOnLinking `boolean`
{:#members:validatemanualtasksonlinking}

Enables or disables the schedule date validation while connecting a manually scheduled task with predecessor

#### Default Value

* false


#### Example
{:.example}


{% highlight html %}
 
<div id="gantt"></div> 
<script>          
        $("#gantt").ejGantt(
 {
    validateManualTasksOnLinking: true
 });            
</script>

{% endhighlight %}

### viewType `enum`
{:#members:viewtype}

<ts name = "ej.Gantt.ViewType"/>

Specifies the view type for a project in the Gantt.

<table class="params">
<thead>
<tr>
<th>Name</th>
<th>Description</th>
</tr>
</thead>
<tbody>
<tr>
<td class="name">ProjectView</td>
<td class="description">Displays the project in task view in Gantt.</td>
</tr>
<tr>
<td class="name">ResourceView</td>
<td class="description">Displays the project in resource allocation view in Gantt.</td>
</tr>
<tr>
<td class="name">HistogramView</td>
<td class="description">Displays the project in histogram view in Gantt</td>
</tr>
</tbody>
</table>

#### Default Value

* ej.Gantt.ViewType.ProjectView


#### Example
{:.example}


{% highlight html %}
 
<div id="gantt"></div> 
<script>                          
        $("#gantt").ejGantt({  
                        viewType : ej.Gantt.ViewType.ResourceView });
</script>

{% endhighlight %}

### weekendBackground `string`
{:#members:weekendbackground}

Specifies the weekendBackground color in Gantt


#### Default Value

* "#F2F2F2"


#### Example
{:.example}


{% highlight html %}
 
<div id="gantt"></div> 
<script>          
        $("#gantt").ejGantt(
 {
    weekendBackground: "blue"
 });            
</script>

{% endhighlight %}

### workMapping `string`
{:#members:workmapping}

Specifies the mapping property path for the work field of a task in the data source. When it is mapped the end date and duration for a task will be calculated automatically.


#### Default Value

* ""


#### Example
{:.example}


{% highlight html %}
 
<div id="gantt"></div> 
<script>                  
        $("#gantt").ejGantt({  workMapping : "estimatedHours" });
</script>

{% endhighlight %}

### workUnit `enum`
{:#members:workunit}

<ts name = "ej.Gantt.WorkUnit"/>

Specifies the unit for the work involved in a task and it can be day, hour or minute

<table class="params">
<thead>
<tr>
<th>Name</th>
<th>Description</th>
</tr>
</thead>
<tbody>
<tr>
<td class="name">Day</td>
<td class="description">Displays the work involved in a task in days.</td>
</tr>
<tr>
<td class="name">Hour</td>
<td class="description">Displays the work involved in a task in hours.</td>
</tr>
<tr>
<td class="name">Minute</td>
<td class="description">Displays the work involved in a task in minutes</td>
</tr>
</tbody>
</table>

#### Default Value

*  ej.Gantt.WorkUnit.Hour


#### Example
{:.example}


{% highlight html %}
 
<div id="gantt"></div> 
<script>                          
        $("#gantt").ejGantt({  
                        workUnit : ej.Gantt.WorkUnit.Day });
</script>

{% endhighlight %}

### workWeek `array`
{:#members:workweek}

Gets or sets the working days of a week in a project.

#### Default Value

* ["Monday","Tuesday","Wednesday","Thursday","Friday"]

#### Example

{:.example}
{% highlight html %}
 
<div id="gantt"></div> 
<script>          
$("#gantt").ejGantt(
{      
        workweek:["Sunday","Monday","Tuesday","Wednesday","Thursday"],
});            
</script>

{% endhighlight %}

### workingTimeScale `enum`
{:#members:workingtimescale}

<ts name = "ej.Gantt.workingTimeScale"/>

Specifies the working time schedule of day

<table class="params">
<thead>
<tr>
<th>Name</th>
<th>Description</th>
</tr>
</thead>
<tbody>
<tr>
<td class="name">TimeScale8Hours</td>
<td class="description">Sets eight hour timescale.</td>
</tr>
<tr>
<td class="name">TimeScale24Hours</td>
<td class="description">Sets twenty four hour timescale.</td>
</tr>
</tbody>
</table>

#### Default Value

* ej.Gantt.workingTimeScale.TimeScale8Hours


#### Example
{:.example}


{% highlight html %}
 
<div id="gantt"></div> 
<script>                          
        $("#gantt").ejGantt({  
                        workingTimeScale : ej.Gantt.workingTimeScale.TimeScale24Hours
            });
</script>

{% endhighlight %}

## Methods

### addRecord(data, rowPosition)
{:#methods:addrecord}

To add a new item in Gantt

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
<td class="name">data</td>
<td class="type">object</td>
<td class="description">Item to add in Gantt row.</td>
</tr>
<tr>
<td class="name">rowPosition</td>
<td class="type">string</td>
<td class="description">Defines in which position the row wants to add</td>
</tr>
</tbody>
</table>


#### Example


{% highlight html %}
 
<div id="gantt"></div> 
 
<script>
// Create Gantt
var ganttObj = $("#gantt").data("ejGantt");
var data = {taskId:"40",taskName:"New Task 40",startDate:"2/20/2014",startDate:"2/25/2014"};
ganttObj.addRecord(data, ej.Gantt.AddRowPosition.Child); // To add a task
</script>
{% endhighlight %}

### cancelEdit()
{:#methods:canceledit}

To cancel the edited state of an item in Gantt

#### Example

{% highlight html %}
 
<div id="gantt"></div> 
 
<script>
// Create Gantt object
var ganttObj = $("#gantt").data("ejGantt");
ganttObj.cancelEdit(); // To cancel edited
</script>
{% endhighlight %}

### clearFilter()
{:#methods:clearfilter}

To clear all the filtered columns in Gantt.

#### Example

{% highlight html %}

<div id="gantt"></div>  
<script>
        var ganttObj = $("#gantt").data("ejGantt");
        ganttObj.clearFilter();
</script>

{% endhighlight %}

### clearSorting()
{:#methods:clearsorting}

To clear the sorted columns in Gantt.

#### Example

{% highlight html %}
  
<div id="gantt"></div> 
 
<script>
var ganttObject = $("#gantt").data("ejGantt");
ganttObject.clearSorting();
</script>

{% endhighlight %}

### collapseAllItems()
{:#methods:collapseallitems}

To collapse all the parent items in Gantt


#### Example


{% highlight html %}
 
<div id="gantt"></div> 
 
<script>
// Create Gantt
var ganttObj = $("#gantt").data("ejGantt");
ganttObj.collapseAllItems(); // To collapse all parent items in Gantt
</script>
{% endhighlight %}

### deleteDependency(fromTaskId,toTaskId)
{:#methods:deletedependency}

To delete the dependency between the two tasks.

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
<td class="name">fromTaskId</td>
<td class="type">number</td>
<td class="description">taskID of predecessor task</td>
</tr>
<tr>
<td class="name">toTaskId</td>
<td class="type">number</td>
<td class="description">taskID of successor task</td>
</tr>
</tbody>
</table>


#### Example


{% highlight html %}
 
<div id="gantt"></div> 
 
<script>
// Create Gantt
var ganttObj = $("#gantt").data("ejGantt");
ganttObj.deleteDependency(3, 6); // To delete dependency between two tasks.
</script>
{% endhighlight %}

### deleteItem()
{:#methods:deleteitem}

To delete a selected item in Gantt


#### Example


{% highlight html %}
 
<div id="gantt"></div> 
 
<script>
// Create Gantt
var ganttObj = $("#gantt").data("ejGantt");
ganttObj.deleteItem(); // To delete a task
</script>
{% endhighlight %}


### destroy()
{:#methods:destroy}

destroy the Gantt widget all events bound using this._on will be unbind automatically and bring the control to pre-init state.


#### Example


{% highlight html %}
 
<div id="gantt"></div> 
 
<script>
// Create Gantt Object
var ganttObj = $("#gantt").data("ejGantt");
ganttObj.destroy(); // destroy the Gantt
</script>
{% endhighlight %}

### expandAllItems()
{:#methods:expandallitems}

To Expand all the parent items in Gantt


#### Example


{% highlight html %}
 
<div id="gantt"></div> 
 
<script>
// Create Gantt Object
var ganttObj = $("#gantt").data("ejGantt");
ganttObj.expandAllItems(); // To expand all parent items in Gantt
</script>
{% endhighlight %}


### expandCollapseRecord(taskId)
{:#methods:expandcollapserecord}

To expand and collapse an item in Gantt using item's ID

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
<td class="name">taskId</td>
<td class="type">Number</td>
<td class="description">Expand or Collapse a record based on task id.</td>
</tr>
</tbody>
</table>

#### Example


{% highlight html %}
 
<div id="gantt"></div> 
 
<script>
// Create Gantt object.
var ganttObj = $("#gantt").data("ejGantt");
ganttObj.expandCollapseRecord(23); // To expand collapse an item
</script>
{% endhighlight %}

### export(action, \[serverEvent\], \[multipleExport\])
{:#methods:export}

Export the Gantt content to excel or PDF document.

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
<td class="name">action</td>
<td class="type"><span class="param-type">string</span></td>
<td class="description last">Pass the controller action name corresponding to exporting</td>
</tr>
<tr>
<td class="name">serverEvent</td>
<td class="type"><span class="param-type">string</span></td>
<td class="description last"><span class="optional">optional</span>ASP server event name corresponding to exporting</td>
</tr>
<tr>
<td class="name">multipleExport</td>
<td class="type"><span class="param-type">boolean</span></td>
<td class="description last"><span class="optional">optional</span>Pass the multiple exporting value as true/false</td>
</tr>
</tbody>
</table>

#### Returns:
{:#methods:returns:}

Void

#### Example
{:.example}


{% highlight html %}
 
<script>
// Create Gantt object.
var ganttObj = $("#Gantt").data("ejGantt");
// Sends an exporting request
gridObj.export("/api/GanttExport/ExcelExport"); 
</script>
{% endhighlight %}


{% highlight html %}
 
<script>
// Sends an exporting request
$("#Gantt").ejGantt("export","/api/GanttExport/ExcelExport");        
</script>
{% endhighlight %}

### filterColumn(fieldName, filterOperator, filterValue, [predicate], [matchCase])
{:#methods:filtercolumn}

Sends filtering request to filter a column in Gantt dynamically.

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
<td class="name">fieldName</td>
<td class="type">string</td>
<td class="description">Pass the field name of the column.</td>
</tr>
<tr>
<td class="name">filterOperator</td>
<td class="type">string</td>
<td class="description">string/integer/date operator.</td>
</tr>
<tr>
<td class="name">filterValue</td>
<td class="type">string</td>
<td class="description">Pass the value to be filtered in a column.</td>
</tr>
<tr>
<td class="name">predicate</td>
<td class="type">string</td>
<td class="description">Optional - Pass the predicate as and/or.</td>
</tr>
<tr>
<td class="name">matchCase</td>
<td class="type">boolean</td>
<td class="description">Optional - pass the match case value as true/false.</td>
</tr>
</tbody>
</table>

#### Example

{% highlight html %}
 
<div id="gantt"></div>  
<script>
        var obj = $("#gantt").ejGantt("instance");
        obj.filterColumn("taskName", "startswith", "plan");
</script>

{% endhighlight %}

### filterContent(ejPredicate)
{:#methods:filtercontent}

To filter multiple columns with multiple conditions dynamically in Gantt.

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
<td class="name">ejPredicate</td>
<td class="type">object</td>
<td class="description">Pass the filtering column details and conditions as ejPredicate instance. The ejPredicate object is defined as fieldName,filterOperator, filterValue and ignoreCase properties.
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
<td class="name">fieldName</td>
<td class="type">string</td>
<td class="description">Pass the field name of the column.</td>
</tr>
<tr>
<td class="name">filterOperator</td>
<td class="type">string</td>
<td class="description">string/integer/date operator.</td>
</tr>
<tr>
<td class="name">filterValue</td>
<td class="type">string</td>
<td class="description">Pass the value to be filtered in a column.</td>
</tr>
<tr>
<td class="name">ignoreCase</td>
<td class="type">boolean</td>
<td class="description">Optional - pass the ignore case value as true/false.</td>
</tr>
</tbody>
</table>
</td>
</tr>
</tbody>
</table>

#### Example

{% highlight html %}
 
<div id="gantt"></div>  
<script>
        var obj = $("#gantt").ejGantt("instance");
        var predicate = ej.Predicate("taskName", ej.FilterOperators.equal, "planning", false)
                          .or("taskName", ej.FilterOperators.equal, "plan budget", false)
                          .and("progress", ej.FilterOperators.equal, 100, true);
        obj.filterContent(predicate);
</script>

{% endhighlight %}

### getColumns()
{:#methods:getcolumns}

To get available column collection in Gantt.

#### Example

{% highlight html %}
 
<div id="gantt">Gantt</div> 
 
<script>
var ganttObject = $("#gantt").data("ejGantt"),
    columns = ganttObject.getColumns();
</script>
{% endhighlight %}

### getResourceViewEditColumns()
{:#methods:getresourcevieweditcolumns}

To get the column collection which are used to edit the task by using task add/edit dialog in resource view.

#### Example

{% highlight html %}
 
<div id="gantt">Gantt</div> 
 
<script>
var ganttObject = $("#gantt").data("ejGantt"),
    columns = ganttObject.getResourceViewEditColumns();
</script>
{% endhighlight %}

### hideColumn(headerText)
{:#methods:hidecolumn}

To hide the column by using header text

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
<td class="name">headerText</td>
<td class="type">string</td>
<td class="description">you can pass a header text of a column to hide</td>
</tr>
</tbody>
</table>


#### Example


{% highlight html %}
 
<div id="gantt">Gantt</div> 
 
<script>
// Create Gantt
var ganttObj = $("#gantt").data("ejGantt");
ganttObj.hideColumn("Task Name");
</script>
{% endhighlight %}


### indentItem()
{:#methods:indentitem}

To indent a selected item in Gantt


#### Example


{% highlight html %}
 
<div id="gantt"></div> 
 
<script>
// Create Gantt
var ganttObj = $("#gantt").data("ejGantt");
ganttObj.indentItem(); // To indent a selected item in Gantt
</script>
{% endhighlight %}


### openAddDialog()
{:#methods:openadddialog}

To Open the dialog to add new task to the Gantt


#### Example


{% highlight html %}
 
<div id="gantt"></div> 
 
<script>
// Create Gantt Object.
var ganttObj = $("#gantt").data("ejGantt");
ganttObj.openAddDialog(); // To open the add dialog
</script>
{% endhighlight %}


### openEditDialog()
{:#methods:openeditdialog}

To Open the dialog to edit existing task to the Gantt


#### Example


{% highlight html %}
 
<div id="gantt"></div> 
 
<script>
// Create Gantt object
var ganttObj = $("#gantt").data("ejGantt");
ganttObj.openEditDialog(); // To open the add dialog
</script>
{% endhighlight %}


### outdentItem()
{:#methods:outdentitem}

To outdent a selected item in Gantt


#### Example


{% highlight html %}
 
<div id="gantt"></div> 
 
<script>
// Create Gantt
var ganttObj = $("#gantt").data("ejGantt");
ganttObj.outdentItem(); // To outdent a selected item in Gantt
</script>
{% endhighlight %}

### saveEdit()
{:#methods:saveedit}

To save the edited state of an item in Gantt


#### Example


{% highlight html %}
 
<div id="gantt"></div> 
 
<script>
// Create Gantt
var ganttObj = $("#gantt").data("ejGantt");
ganttObj.saveEdit(); // To save edited state of an item
</script>
{% endhighlight %}

### searchItem(searchString)
{:#methods:searchitem}

To search an item with search string provided at the run time

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
<td class="name">searchString</td>
<td class="type">string</td>
<td class="description">you can pass a text to search in Gantt Control.</td>
</tr>
</tbody>
</table>


#### Example


{% highlight html %}
 
<div id="gantt"></div> 
 
<script>
// Create Gantt Object
var ganttObj = $("#gantt").data("ejGantt");
ganttObj.searchItem($("#text").val()); // To search a task
</script>
{% endhighlight %}

### selectCells(Indexes,preservePreviousSelectedCell)
{:#methods:selectcells}

To select cell based on the cell and row index dynamically.

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
<td class="name">Indexes</td>
<td class="type">array</td>
<td class="description">array of cell indexes to be select</td>
</tr>
<tr>
<td class="name">preservePreviousSelectedCell</td>
<td class="type">boolean</td>
<td class="description">Defines that we need to preserve the previously selected cells of not</td>
</tr>
</tbody>
</table>


#### Example


{% highlight html %}
 
<div id="gantt"></div> 
 
<script>
// Create Gantt
var ganttObj = $("#gantt").data("ejGantt");
var indexes = [{rowIndex:4, cellIndex: 4}, {rowIndex: 3, cellIndex: 3}];
ganttObj.selectCells(indexes, true); // To add a task
</script>
{% endhighlight %}

### selectMultipleRows(rowIndexes)
{:#methods:selectmultiplerows}

To select multiple rows dynamically.

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
<td class="name">rowIndexes</td>
<td class="type">array</td>
<td class="description">array of row indexes to select</td>
</tr>
</tbody>
</table>


#### Example


{% highlight html %}
 
<div id="gantt"></div> 
 
<script>
// Create Gantt
 var ganttObj = $("#gantt").data("ejGantt"),
     rowIndexes = [12,0,4,7];
 ganttObj.selectMultipleRows(rowIndexes);
</script>
{% endhighlight %}

### setScrollTop(top)
{:#methods:setscrolltop}

Method to set scroll top value for Gantt control.

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
<td class="name">Top</td>
<td class="type">number</td>
<td class="description">Pass a value to set top position of vertical scroll bar.</td>
</tr>
</tbody>
</table>

Usage: we can able to change the top position of vertical scroll bar dynamically.

#### Example

{% highlight html %}
  
<div id="gantt"></div> 
<script>
var ganttObject = $("#gantt").data("ejGantt");
ganttObject.setScrollTop(200);
</script>

{% endhighlight %}

### setSplitterIndex(index)
{:#methods:setsplitterindex}

Positions the splitter by the specified column index.

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
<td class="name">index</td>
<td class="type">Number</td>
<td class="description">Set the splitter position based on column index.</td>
</tr>
</tbody>
</table>

#### Example

{% highlight html %}
 
<div id="gantt"></div> 
 
<script>
// Create Gantt object
var ganttObj = $("#gantt").data("ejGantt");
ganttObj.setSplitterIndex(3); // Set splitter position after column index 3
</script>
{% endhighlight %}

### setSplitterPosition(width)
{:#methods:setsplitterposition}

To set the grid width in Gantt

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
<td class="name">width</td>
<td class="type">string</td>
<td class="description">you can give either percentage or pixels value</td>
</tr>
</tbody>
</table>


#### Example


{% highlight html %}
 
<div id="gantt"></div> 
 
<script>
// Create Gantt
var ganttObj = $("#gantt").data("ejGantt");
ganttObj.ejGantt("setSplitterPosition","40%");
</script>
{% endhighlight %}

### showColumn(headerText)
{:#methods:showcolumn}

To show the column by using header text

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
<td class="name">headerText</td>
<td class="type">string</td>
<td class="description">you can pass a header text of a column to show</td>
</tr>
</tbody>
</table>


#### Example


{% highlight html %}
 
<div id="gantt">Gantt</div> 
 
<script>
// Create Gantt
var ganttObj = $("#gantt").data("ejGantt");
ganttObj.showColumn("Task Name");
</script>
{% endhighlight %}

### showCriticalPath(isShown)
{:#methods:showcriticalpath}

To show/hide the critical tasks in current project.

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
<td class="name">isShown</td>
<td class="type">boolean</td>
<td class="description">To show/hide the critical tasks</td>
</tr>
</tbody>
</table>

#### Example

{% highlight html %}
 
<div id="gantt"></div>  
<script>
        var ganttObj = $("#gantt").data("ejGantt");
        ganttObj.showCriticalPath(true);
</script>

{% endhighlight %}

### sortColumn(mappingName, columnSortDirection)
{:#methods:sortcolumn}

To sort the column in required direction

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
<td class="name">mappingName</td>
<td class="type">string</td>
<td class="description">Defines the column's mapping name in which sorting have to be performed</td>
</tr>
<tr>
<td class="name">columnSortDirection</td>
<td class="type">string</td>
<td class="description">Defines the sort direction whether the column has to sorted in ascending/descending order. By default it is sorting in an ascending order</td>
</tr>
</tbody>
</table>


#### Example


{% highlight html %}
 
<div id="gantt"></div> 
 
<script>
// Create Gantt
var ganttObj = $("#gantt").data("ejGantt");
ganttObj.sortColumn("startDate","ascending"); // To sort a column
</script>
{% endhighlight %}

### updateDependency(fromTaskId,toTaskId, predecessorType, offset)
{:#methods:updatedependency}

To update the predecessor type and offset value for existing task dependency.

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
<td class="name">fromTaskId</td>
<td class="type">number</td>
<td class="description">taskID of predecessor task</td>
</tr>
<tr>
<td class="name">toTaskId</td>
<td class="type">number</td>
<td class="description">taskID of successor task</td>
</tr>
<tr>
<td class="name">predecessorType</td>
<td class="type">string</td>
<td class="description">Type of dependency task.</td>
</tr>
<tr>
<td class="name">offset</td>
<td class="type">number</td>
<td class="description">Offset value of dependency task.</td>
</tr>
</tbody>
</table>

#### Example

{% highlight html %}
 
<div id="gantt"></div> 
 
<script>
// Create Gantt
var ganttObj = $("#gantt").data("ejGantt");
ganttObj.updateDependency(3, 6, "SS", 3); // To update predecessor type and offset value.
</script>
{% endhighlight %}

### updateRecordByTaskId(data)
{:#methods:updaterecordbytaskid}

To update the value of Gantt record by using it's task id value.

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
<td class="name">data</td>
<td class="type">object</td>
<td class="description">object with modified field values and current task id value</td>
</tr>
</tbody>
</table>

#### Example

{% highlight html %}
 
<div id="gantt"></div>  
<script>
        var ganttObj = $("#gantt").data("ejGantt");
        var data = { taskID: 4, taskName: "updated value"};
        ganttObj.updateRecordByTaskId(data);
</script>

{% endhighlight %}

### updateRecordByIndex(index, data)
{:#methods:updaterecordbyindex}

To update the value of Gantt record by using row index.

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
<td class="name">index</td>
<td class="type">number</td>
<td class="description">index of Gantt record to be updated</td>
</tr>
<tr>
<td class="name">data</td>
<td class="type">object</td>
<td class="description">object with modified field value</td>
</tr>
</tbody>
</table>

#### Example

{% highlight html %}
 
<div id="gantt"></div>  
<script>
        var ganttObj = $("#gantt").data("ejGantt");
        var data = { taskName: "updated value"};
        ganttObj.updateRecordByIndex(4, data);
</script>

{% endhighlight %}

### updateScheduleDates(startDate, endDate)
{:#methods:updatescheduledates}

To update the schedule start date and schedule end date of project.

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
<td class="name">startDate</td>
<td class="type">string</td>
<td class="description">New schedule start date of project</td>
</tr>
<tr>
<td class="name">endDate</td>
<td class="type">string</td>
<td class="description">New schedule end date of project</td>
</tr>
</tbody>
</table>

#### Example

{% highlight html %}
 
<div id="gantt"></div> 
<script>
var ganttObject = $("#gantt").data("ejGantt");
ganttObject.updateScheduleDates("5/25/2017", "9/27/2017");
</script>

{% endhighlight %}

### updateTaskId(currentId, newId)
{:#methods:updatetaskid}

To change an existing Gantt ID by new ID value dynamically

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
<td class="name">currentId</td>
<td class="type">number</td>
<td class="description">you can pass an existing ID value to be change</td>
</tr>
<tr>
<td class="name">newId</td>
<td class="type">number</td>
<td class="description">you can pass a new ID value to be change</td>
</tr>
</tbody>
</table>


#### Example


{% highlight html %}
 
<div id="gantt"></div> 
 
<script>
// Create Gantt
var ganttObj = $("#gantt").data("ejGantt");
ganttObj.updateTaskId(5, 15);
</script>
{% endhighlight %}

## Events


### actionBegin
{:#events:actionbegin}

Triggered for every Gantt action before its starts.

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
<td class="name">argument</td>
<td class="type">Object</td>
<td class="description">Event parameters when Gantt is initialized:
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
<td class="type">boolean</td>
<td class="description">Returns the cancel option value.</td>
</tr>
<tr>
<td class="name">model</td>
<td class="type">object</td>
<td class="description">Returns the grid model.</td>
</tr>
<tr>
<td class="name">type</td>
<td class="type">string</td>
<td class="description">Returns the name of the event.</td>
</tr>
</tbody>
</table>
</td>
</tr>
<tr>
<td class="name">argument</td>
<td class="type">Object</td>
<td class="description">Event parameters while perform sorting in grid tree action starts:
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
<td class="type">boolean</td>
<td class="description">Returns the cancel option value.</td>
</tr>
<tr>
<td class="name">columnName</td>
<td class="type">string</td>
<td class="description">Returns the current grouped column field name.</td>
</tr>
<tr>
<td class="name">model</td>
<td class="type">object</td>
<td class="description">Returns the Gantt model.</td>
</tr>
<tr>
<td class="name">requestType</td>
<td class="type">string</td>
<td class="description">Returns request type.</td>
</tr>
<tr>
<td class="name">type</td>
<td class="type">string</td>
<td class="description">Returns the name of the event.</td>
</tr>
<tr>
<td class="name">columnSortDirection</td>
<td class="type">string</td>
<td class="description">Returns the direction of sorting ascending or descending</td>
</tr>
</tbody>
</table>
</td>
</tr>
<tr>
<td class="name">argument</td>
<td class="type">Object</td>
<td class="description">Event parameters while searching action starts:
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
<td class="type">boolean</td>
<td class="description">Returns the cancel option value.</td>
</tr>
<tr>
<td class="name">keyValue</td>
<td class="type">string</td>
<td class="description">Returns the value of searching element.</td>
</tr>
<tr>
<td class="name">model</td>
<td class="type">object</td>
<td class="description">Returns the Gantt model.</td>
</tr>
<tr>
<td class="name">requestType</td>
<td class="type">string</td>
<td class="description">Returns request type.</td>
</tr>
<tr>
<td class="name">type</td>
<td class="type">string</td>
<td class="description">Returns the name of the event.</td>
</tr>
</tbody>
</table>
</td>
</tr>
<tr>
<td class="name">argument</td>
<td class="type">Object</td>
<td class="description">Event parameters while performing the delete operation starts:
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
<td class="type">boolean</td>
<td class="description">Returns the cancel option value.</td>
</tr>
<tr>
<td class="name">data</td>
<td class="type">string</td>
<td class="description">Returns the data of deleting element.</td>
</tr>
<tr>
<td class="name">model</td>
<td class="type">object</td>
<td class="description">Returns the Gantt model.</td>
</tr>
<tr>
<td class="name">requestType</td>
<td class="type">string</td>
<td class="description">Returns request type.</td>
</tr>
<tr>
<td class="name">type</td>
<td class="type">string</td>
<td class="description">Returns the name of the event.</td>
</tr>
</tbody>
</table>
</td>
</tr>
<tr>
<td class="name">argument</td>
<td class="type">Object</td>
<td class="description">Event parameters while performing the add operation starts:
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
<td class="type">boolean</td>
<td class="description">Returns the cancel option value.</td>
</tr>
<tr>
<td class="name">data</td>
<td class="type">string</td>
<td class="description">Returns the data adding element.</td>
</tr>
<tr>
<td class="name">recordIndex</td>
<td class="type">number</td>
<td class="description">Returns selected record index</td>
</tr>
<tr>
<td class="name">requestType</td>
<td class="type">string</td>
<td class="description">Returns request type.</td>
</tr>
</tbody>
</table>
</td>
</tr>
<tr>
<td class="name">argument</td>
<td class="type">Object</td>
<td class="description">Event parameters while performing the edit operation starts:
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
<td class="type">boolean</td>
<td class="description">Returns the cancel option value.</td>
</tr>
<tr>
<td class="name">data</td>
<td class="type">string</td>
<td class="description">Returns the data editing element</td>
</tr>
<tr>
<td class="name">recordIndex</td>
<td class="type">number</td>
<td class="description">Returns selected record index</td>
</tr>
<tr>
<td class="name">requestType</td>
<td class="type">string</td>
<td class="description">Returns request type.</td>
</tr>
</tbody>
</table>
</td>
</tr>
<tr>
<td class="name">argument</td>
<td class="type">Object</td>
<td class="description">Event parameters before opening of task dependency edit dialog:
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
<td class="type">boolean</td>
<td class="description">Returns the cancel option value.</td>
</tr>
<tr>
<td class="name">data</td>
<td class="type">object</td>
<td class="description">Returns the task dependency data.</td>
</tr>
<tr>
<td class="name">requestType</td>
<td class="type">string</td>
<td class="description">Returns request type as "beforeDependencyEditDialogOpen".</td>
</tr>
</tbody>
</table>
</td>
</tr>
<tr>
<td class="name">argument</td>
<td class="type">Object</td>
<td class="description">Event parameters after opening of edit task dependency dialog:
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
<td class="type">boolean</td>
<td class="description">Returns the cancel option value.</td>
</tr>
<tr>
<td class="name">data</td>
<td class="type">object</td>
<td class="description">Returns the task dependency data.</td>
</tr>
<tr>
<td class="name">element</td>
<td class="type">string</td>
<td class="description">Returns the edit dialog element.</td>
</tr>
<tr>
<td class="name">requestType</td>
<td class="type">string</td>
<td class="description">Returns request type as "afterDependencyEditDialogOpen".</td>
</tr>
</tbody>
</table>
</td>
</tr>
</tbody>
</table>


#### Example


{% highlight html %}
 
<div id="gantt"></div> 
<script>
$("#gantt").ejGantt({
   actionBegin: function (args) {}
});
</script>
{% endhighlight %}


### actionComplete
{:#events:actioncomplete}

Triggered for every Gantt action success event.

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
<td class="name">argument</td>
<td class="type">Object</td>
<td class="description">Event parameters when Gantt is initialized:
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
<td class="type">boolean</td>
<td class="description">Returns the cancel option value.</td>
</tr>
<tr>
<td class="name">model</td>
<td class="type">object</td>
<td class="description">Returns the grid model.</td>
</tr>
<tr>
<td class="name">type</td>
<td class="type">string</td>
<td class="description">Returns the name of the event.</td>
</tr>
</tbody>
</table>
</td>
</tr>
<tr>
<td class="name">argument</td>
<td class="type">Object</td>
<td class="description">Event parameters after perform the sorting in TreeGrid part is completed:
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
<td class="type">boolean</td>
<td class="description">Returns the cancel option value.</td>
</tr>
<tr>
<td class="name">columnName</td>
<td class="type">string</td>
<td class="description">Returns the current grouped column field name.</td>
</tr>
<tr>
<td class="name">model</td>
<td class="type">object</td>
<td class="description">Returns the Gantt model.</td>
</tr>
<tr>
<td class="name">requestType</td>
<td class="type">string</td>
<td class="description">Returns request type.</td>
</tr>
<tr>
<td class="name">type</td>
<td class="type">string</td>
<td class="description">Returns the name of the event.</td>
</tr>
<tr>
<td class="name">columnSortDirection</td>
<td class="type">string</td>
<td class="description">Returns the direction of sorting ascending or descending</td>
</tr>
</tbody>
</table>
</td>
</tr>
<tr>
<td class="name">argument</td>
<td class="type">Object</td>
<td class="description">Event parameters after searching completed:
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
<td class="type">boolean</td>
<td class="description">Returns the cancel option value.</td>
</tr>
<tr>
<td class="name">keyValue</td>
<td class="type">string</td>
<td class="description">Returns the value of searched element.</td>
</tr>
<tr>
<td class="name">model</td>
<td class="type">object</td>
<td class="description">Returns the Gantt model.</td>
</tr>
<tr>
<td class="name">requestType</td>
<td class="type">string</td>
<td class="description">Returns request type.</td>
</tr>
<tr>
<td class="name">type</td>
<td class="type">string</td>
<td class="description">Returns the name of the event.</td>
</tr>
</tbody>
</table>
</td>
</tr>
<tr>
<td class="name">argument</td>
<td class="type">Object</td>
<td class="description">Event parameters while performing after completing the delete operation is completed:
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
<td class="type">boolean</td>
<td class="description">Returns the cancel option value.</td>
</tr>
<tr>
<td class="name">data</td>
<td class="type">string</td>
<td class="description">Returns the data of deleted element.</td>
</tr>
<tr>
<td class="name">model</td>
<td class="type">object</td>
<td class="description">Returns the Gantt model.</td>
</tr>
<tr>
<td class="name">requestType</td>
<td class="type">string</td>
<td class="description">Returns request type.</td>
</tr>
<tr>
<td class="name">type</td>
<td class="type">string</td>
<td class="description">Returns the name of the event.</td>
</tr>
</tbody>
</table>
</td>
</tr>
<tr>
<td class="name">argument</td>
<td class="type">Object</td>
<td class="description">Event parameters after the add operation completed:
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
<td class="type">boolean</td>
<td class="description">Returns the cancel option value.</td>
</tr>
<tr>
<td class="name">data</td>
<td class="type">string</td>
<td class="description">Returns the data added element.</td>
</tr>
<tr>
<td class="name">recordIndex</td>
<td class="type">number</td>
<td class="description">Returns selected record index</td>
</tr>
<tr>
<td class="name">requestType</td>
<td class="type">string</td>
<td class="description">Returns request type.</td>
</tr>
</tbody>
</table>
</td>
</tr>
<tr>
<td class="name">argument</td>
<td class="type">Object</td>
<td class="description">Event parameters after the edit operation completed:
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
<td class="type">boolean</td>
<td class="description">Returns the cancel option value.</td>
</tr>
<tr>
<td class="name">data</td>
<td class="type">string</td>
<td class="description">Returns the data added element.</td>
</tr>
<tr>
<td class="name">recordIndex</td>
<td class="type">number</td>
<td class="description">Returns selected record index</td>
</tr>
<tr>
<td class="name">requestType</td>
<td class="type">string</td>
<td class="description">Returns request type.</td>
</tr>
</tbody>
</table>
</td>
</tr>
</tbody>
</table>


#### Example


{% highlight html %}
 
<div id="gantt"></div> 
<script>
$("#gantt").ejGantt({
   actionComplete: function (args) {}
});
</script>
{% endhighlight %}


### beginEdit
{:#events:beginedit}

Triggered while enter the edit mode in the TreeGrid cell

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
<td class="name">argument</td>
<td class="type">Object</td>
<td class="description">Arguments when beginEdit event is triggered.
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
<td class="type">boolean</td>
<td class="description">Returns the cancel option value.</td>
</tr>
<tr>
<td class="name">rowElement</td>
<td class="type">object</td>
<td class="description">Returns the row element of editing cell.</td>
</tr>
<tr>
<td class="name">cellElement</td>
<td class="type">object</td>
<td class="description">Returns the Element of editing cell.</td>
</tr>
<tr>
<td class="name">data</td>
<td class="type">object</td>
<td class="description">Returns the data of current cell record.</td>
</tr>
<tr>
<td class="name">columnIndex</td>
<td class="type">number</td>
<td class="description">Returns the column Index of cell belongs.</td>
</tr>
</tbody>
</table>
</td>
</tr>
</tbody>
</table>


#### Example


{% highlight html %}
 
<div id="gantt"></div> 
<script>
$("#gantt").ejGantt({
   beginEdit: function (args) {}
});
</script>
{% endhighlight %}

### cellSelected
{:#events:cellselected}

Triggered after selected a cell

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
<td class="name">argument</td>
<td class="type">Object</td>
<td class="description">Arguments when cellSelected event is triggered.
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
<td class="type">boolean</td>
<td class="description">Returns the cancel option value.</td>
</tr>
<tr>
<td class="name">cellIndex</td>
<td class="type">number</td>
<td class="description">Returns the cell index on the selection.</td>
</tr>
<tr>
<td class="name">rowIndex</td>
<td class="type">number</td>
<td class="description">Returns the row index on the selection</td>
</tr>
<tr>
<td class="name">targetCell</td>
<td class="type">object</td>
<td class="description">Returns the selecting cell element</td>
</tr>
<tr>
<td class="name">targetRow</td>
<td class="type">object</td>
<td class="description">Returns the selecting row element</td>
</tr>
<tr>
<td class="name">data</td>
<td class="type">object</td>
<td class="description">Returns the selecting record object</td>
</tr>
<tr>
<td class="name">model</td>
<td class="type">object</td>
<td class="description">Returns the Gantt object Model</td>
</tr>
<tr>
<td class="name">previousData</td>
<td class="type">object</td>
<td class="description">Returns the previously selected row data</td>
</tr>
<tr>
<td class="name">previousCellIndex</td>
<td class="type">object</td>
<td class="description">Returns the previously selected cell index</td>
</tr>
<tr>
<td class="name">previousRowIndex</td>
<td class="type">object</td>
<td class="description">Returns the previously selected row index</td>
</tr>
<tr>
<td class="name">previousTargetCell</td>
<td class="type">object</td>
<td class="description">Returns the previously selected cell element</td>
</tr>
<tr>
<td class="name">previousTargetRow</td>
<td class="type">object</td>
<td class="description">Returns the previously selected row element</td>
</tr>
</tbody>
</table>
</td>
</tr>
</tbody>
</table>


#### Example


{% highlight html %}
 
<div id="gantt"></div> 
<script>
$("#gantt").ejGantt({
   cellSelected: function (args) {}
});
</script>
{% endhighlight %}

### cellSelecting
{:#events:cellselecting}

Triggered before selecting a cell

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
<td class="name">argument</td>
<td class="type">Object</td>
<td class="description">Arguments when cellSelecting event is triggered.
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
<td class="type">boolean</td>
<td class="description">Returns the cancel option value.</td>
</tr>
<tr>
<td class="name">cellIndex</td>
<td class="type">number</td>
<td class="description">Returns the cell index on the selection.</td>
</tr>
<tr>
<td class="name">rowIndex</td>
<td class="type">number</td>
<td class="description">Returns the row index on the selection</td>
</tr>
<tr>
<td class="name">targetCell</td>
<td class="type">object</td>
<td class="description">Returns the selecting cell element</td>
</tr>
<tr>
<td class="name">targetRow</td>
<td class="type">object</td>
<td class="description">Returns the selecting row element</td>
</tr>
<tr>
<td class="name">data</td>
<td class="type">object</td>
<td class="description">Returns the selecting record object</td>
</tr>
<tr>
<td class="name">model</td>
<td class="type">object</td>
<td class="description">Returns the Gantt object Model</td>
</tr>
</tbody>
</table>
</td>
</tr>
</tbody>
</table>


#### Example


{% highlight html %}
 
<div id="gantt"></div> 
<script>
$("#gantt").ejGantt({
   cellSelecting: function (args) {}
});
</script>
{% endhighlight %}

### collapsed
{:#events:collapsed}


Triggered after collapsed the Gantt record

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
<td class="name">argument</td>
<td class="type">Object</td>
<td class="description">Arguments when collapsed event is triggered.
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
<td class="type">boolean</td>
<td class="description">Returns the cancel option value.</td>
</tr>
<tr>
<td class="name">recordIndex</td>
<td class="type">Number</td>
<td class="description">Returns the row index of collapsed record.</td>
</tr>
<tr>
<td class="name">data</td>
<td class="type">object</td>
<td class="description">Returns the data of collapsed record.</td>
</tr>
<tr>
<td class="name">requestType</td>
<td class="type">string</td>
<td class="description">Returns Request Type.</td>
</tr>
<tr>
<td class="name">expanded</td>
<td class="type">boolean</td>
<td class="description">Returns state of a record whether it is in expanded or collapsed state.</td>
</tr>
</tbody>
</table>
</td>
</tr>
</tbody>
</table>


#### Example


{% highlight html %}
 
<div id="gantt"></div> 
<script>
$("#gantt").ejGantt({
   collapsed: function (args) {}
});
</script>
{% endhighlight %}


### collapsing
{:#events:collapsing}

Triggered while collapsing the Gantt record

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
<td class="name">argument</td>
<td class="type">Object</td>
<td class="description">Arguments when collapsing event is triggered.
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
<td class="type">boolean</td>
<td class="description">Returns the cancel option value.</td>
</tr>
<tr>
<td class="name">recordIndex</td>
<td class="type">Number</td>
<td class="description">Returns the row index of collapsing record.</td>
</tr>
<tr>
<td class="name">data</td>
<td class="type">object</td>
<td class="description">Returns the data of edited cell record..</td>
</tr>
<tr>
<td class="name">expanded</td>
<td class="type">boolean</td>
<td class="description">Returns state of a record whether it is in expanded or collapsed state.</td>
</tr>
</tbody>
</table>
</td>
</tr>
</tbody>
</table>


#### Example


{% highlight html %}
 
<div id="gantt"></div> 
<script>
$("#gantt").ejGantt({
   collapsing: function (args) {}
});
</script>
{% endhighlight %}


### contextMenuOpen
{:#events:contextmenuopen}

Triggered while Context Menu is rendered in Gantt control

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
<td class="name">argument</td>
<td class="type">Object</td>
<td class="description">Arguments when context menu is rendered.
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
<td class="type">boolean</td>
<td class="description">Returns the cancel option value.</td>
</tr>
<tr>
<td class="name">contextMenuItems</td>
<td class="type">array</td>
<td class="description">Returns the default context menu items to which we add custom items.</td>
</tr>
<tr>
<td class="name">model</td>
<td class="type">object</td>
<td class="description">Returns the Gantt model.</td>
</tr>
<tr>
<td class="name">requestType</td>
<td class="type">string</td>
<td class="description">Returns request type.</td>
</tr>
<tr>
<td class="name">type</td>
<td class="type">string</td>
<td class="description">Returns the name of the event.</td>
</tr>
</tbody>
</table>
</td>
</tr>
</tbody>
</table>


#### Example


{% highlight html %}
 
<div id="gantt"></div> 
<script>
$("#gantt").ejGantt({
   contextMenuOpen: function (args) {}
});
</script>
{% endhighlight %}

### create
{:#events:create}

Triggered when Gantt is rendered completely.

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
<td class="name">argument</td>
<td class="type">Object</td>
<td class="description">Arguments when create event is triggered.
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
<td class="type">boolean</td>
<td class="description">Returns the cancel option value.</td>
</tr>
<tr>
<td class="name">model</td>
<td class="type">object</td>
<td class="description">Returns the Gantt model</td>
</tr>
<tr>
<td class="name">type</td>
<td class="type">string</td>
<td class="description">Returns the name of the event.</td>
</tr>
</tbody>
</table>
</td>
</tr>
</tbody>
</table>

#### Example


{% highlight html %}
 
<div id="Gantt"></div> 
<script>
$("#Gantt").ejGantt({
   create: function (args) {}
});
</script>
{% endhighlight %}

### endEdit
{:#events:endedit}

Triggered after save the modified cellValue in Gantt.

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
<td class="name">argument</td>
<td class="type">Object</td>
<td class="description">Arguments when endEdit event is triggered.
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
<td class="type">boolean</td>
<td class="description">Returns the cancel option value.</td>
</tr>
<tr>
<td class="name">rowElement</td>
<td class="type">object</td>
<td class="description">Returns the row element of editing cell.</td>
</tr>
<tr>
<td class="name">cellElement</td>
<td class="type">object</td>
<td class="description">Returns the Element of editing cell.</td>
</tr>
<tr>
<td class="name">data</td>
<td class="type">object</td>
<td class="description">Returns the data of edited cell record.</td>
</tr>
<tr>
<td class="name">columnName</td>
<td class="type">string</td>
<td class="description">Returns the column name of edited cell belongs.</td>
</tr>
<tr>
<td class="name">columnObject</td>
<td class="type">object</td>
<td class="description">Returns the column object of edited cell belongs.</td>
</tr>
</tbody>
</table>
</td>
</tr>
</tbody>
</table>


#### Example


{% highlight html %}
 
<div id="gantt"></div> 
<script>
$("#gantt").ejGantt({
   endEdit: function (args) {}
});
</script>
{% endhighlight %}


### expanded
{:#events:expanded}

Triggered after expand the record

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
<td class="name">argument</td>
<td class="type">Object</td>
<td class="description">Arguments when expanded event is triggered.
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
<td class="type">boolean</td>
<td class="description">Returns the cancel option value.</td>
</tr>
<tr>
<td class="name">recordIndex</td>
<td class="type">number</td>
<td class="description">Returns the row index of record.</td>
</tr>
<tr>
<td class="name">data</td>
<td class="type">object</td>
<td class="description">Returns the data of expanded record.</td>
</tr>
<tr>
<td class="name">requestType</td>
<td class="type">string</td>
<td class="description">Returns Request Type.</td>
</tr>
<tr>
<td class="name">expanded</td>
<td class="type">boolean</td>
<td class="description">Returns state of a record whether it is in expanded or collapsed state.</td>
</tr>
</tbody>
</table>
</td>
</tr>
</tbody>
</table>


#### Example


{% highlight html %}
 
<div id="gantt"></div> 
<script>
$("#gantt").ejGantt({
   expanded: function (args) {}
});
</script>
{% endhighlight %}


### expanding
{:#events:expanding}

Triggered while expanding the Gantt record

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
<td class="name">argument</td>
<td class="type">Object</td>
<td class="description">Arguments when expanding event is triggered.
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
<td class="type">boolean</td>
<td class="description">Returns the cancel option value.</td>
</tr>
<tr>
<td class="name">recordIndex</td>
<td class="type">object</td>
<td class="description">Returns the row index of record.</td>
</tr>
<tr>
<td class="name">data</td>
<td class="type">object</td>
<td class="description">Returns the data of edited cell record..</td>
</tr>
<tr>
<td class="name">expanded</td>
<td class="type">boolean</td>
<td class="description">Returns state of a record whether it is in expanded or collapsed state.</td>
</tr>
</tbody>
</table>
</td>
</tr>
</tbody>
</table>


#### Example


{% highlight html %}
 
<div id="gantt"></div> 
<script>
$("#gantt").ejGantt({
   expanding: function (args) {}
});
</script>
{% endhighlight %}


### load
{:#events:load}

Triggered while Gantt is loaded

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
<td class="name">argument</td>
<td class="type">Object</td>
<td class="description">Arguments when load event is triggered.
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
<td class="type">boolean</td>
<td class="description">Returns the cancel option value.</td>
</tr>
<tr>
<td class="name">model</td>
<td class="type">object</td>
<td class="description">Returns the Gantt model</td>
</tr>
<tr>
<td class="name">type</td>
<td class="type">string</td>
<td class="description">Returns the name of the event.</td>
</tr>
</tbody>
</table>
</td>
</tr>
</tbody>
</table>


#### Example


{% highlight html %}
 
<div id="gantt"></div> 
<script>
$("#gantt").ejGantt({
   load: function (args) {}
});
</script>
{% endhighlight %}


### queryCellInfo
{:#events:querycellinfo}

Triggered while rendering each cell in the TreeGrid

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
<td class="name">argument</td>
<td class="type">Object</td>
<td class="description">Arguments when queryCellInfo event is triggered.
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
<td class="type">boolean</td>
<td class="description">Returns the cancel option value.</td>
</tr>
<tr>
<td class="name">cellElement</td>
<td class="type">object</td>
<td class="description">Returns the selecting cell element.</td>
</tr>
<tr>
<td class="name">cellValue</td>
<td class="type">string</td>
<td class="description">Returns the value of cell.</td>
</tr>
<tr>
<td class="name">data</td>
<td class="type">object</td>
<td class="description">Returns the data of current cell record.</td>
</tr>
<tr>
<td class="name">column</td>
<td class="type">object</td>
<td class="description">Returns the column of cell belongs.</td>
</tr>
</tbody>
</table>
</td>
</tr>
</tbody>
</table>


#### Example


{% highlight html %}
 
<div id="gantt"></div> 
<script>
$("#gantt").ejGantt({
   queryCellInfo: function (args) {}
});
</script>
{% endhighlight %}


### queryTaskbarInfo
{:#events:querytaskbarinfo}

Triggered while rendering each taskbar in the Gantt 

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
<td class="name">argument</td>
<td class="type">Object</td>
<td class="description">Arguments when queryTaskbarInfo event is triggered.
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
<td class="type">boolean</td>
<td class="description">Returns the cancel option value.</td>
</tr>
<tr>
<td class="name">taskbarBackground</td>
<td class="type">string</td>
<td class="description">Returns the taskbar background of current item.</td>
</tr>
<tr>
<td class="name">progressbarBackground</td>
<td class="type">string</td>
<td class="description">Returns the progressbar background of current item.</td>
</tr>
<tr>
<td class="name">parentTaskbarBackground</td>
<td class="type">string</td>
<td class="description">Returns the parent taskbar background of current item.</td>
</tr>
<tr>
<td class="name">parentProgressbarBackground</td>
<td class="type">string</td>
<td class="description">Returns the parent progressbar background of current item.</td>
</tr>
<tr>
<td class="name">taskbarTextColor</td>
<td class="type">string</td>
<td class="description">Returns the taskbar text color of current item.</td>
</tr>
<tr>
<td class="name">taskbarBorder</td>
<td class="type">string</td>
<td class="description">Returns the taskbar border color of current item.</td>
</tr>
<tr>
<td class="name">parentTaskbarBorder</td>
<td class="type">string</td>
<td class="description">Returns the parent taskbar border color of current item.</td>
</tr>
<tr>
<td class="name">progressbarBorder</td>
<td class="type">string</td>
<td class="description">Returns the progressbar border color of current item.</td>
</tr>
<tr>
<td class="name">parentProgressbarBorder</td>
<td class="type">string</td>
<td class="description">Returns the parent progressbar border color of current item. </td>
</tr>
<tr>
<td class="name">milestoneBackground</td>
<td class="type">string</td>
<td class="description">Returns the milestone background of current item.  </td>
</tr>
<tr>
<td class="name">baselineBackground</td>
<td class="type">string</td>
<td class="description">Returns the baseline background of current item.  </td>
</tr>
<tr>
<td class="name">data</td>
<td class="type">object</td>
<td class="description">Returns the data of the record.</td>
</tr>
</tbody>
</table>
</td>
</tr>
</tbody>
</table>


#### Example


{% highlight html %}
 
<div id="gantt"></div> 
<script>
$("#gantt").ejGantt({
   queryTaskbarInfo: function (args) {}
});
</script>
{% endhighlight %}


### rowDataBound
{:#events:rowdatabound}

Triggered while rendering each row

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
<td class="name">argument</td>
<td class="type">Object</td>
<td class="description">Arguments when rowDataBound event is triggered.
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
<td class="type">boolean</td>
<td class="description">Returns the cancel option value.</td>
</tr>
<tr>
<td class="name">rowElement</td>
<td class="type">object</td>
<td class="description">Returns the row element of rendering row.</td>
</tr>
<tr>
<td class="name">data</td>
<td class="type">object</td>
<td class="description">Returns the data of rendering row record..</td>
</tr>
</tbody>
</table>
</td>
</tr>
</tbody>
</table>


#### Example


{% highlight html %}
 
<div id="gantt"></div> 
<script>
$("#gantt").ejGantt({
   rowDataBound: function (args) {}
});
</script>
{% endhighlight %}

### rowDrag
{:#events:rowdrag}


Triggered while dragging a row in Gantt control

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
<td class="name">argument</td>
<td class="type">Object</td>
<td class="description">Arguments when dragging a row.
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
<td class="type">boolean</td>
<td class="description">Returns the cancel option value.</td>
</tr>
<tr>
<td class="name">draggedRow</td>
<td class="type">object</td>
<td class="description">Returns the row which we start to drag.</td>
</tr>
<tr>
<td class="name">draggedRowIndex</td>
<td class="type">number</td>
<td class="description">Returns the row index which we start to drag.</td>
</tr>
<tr>
<td class="name">targetRow</td>
<td class="type">object</td>
<td class="description">Returns the row on which we are dragging.</td>
</tr>
<tr>
<td class="name">targetRowIndex</td>
<td class="type">number</td>
<td class="description">Returns the row index on which we are dragging.</td>
</tr>
<tr>
<td class="name">canDrop</td>
<td class="type">boolean</td>
<td class="description">Returns that we can drop over that record or not.</td>
</tr>
<tr>
<td class="name">dropPosition </td>
<td class="type">string</td>
<td class="description">Returns the drop position value on current target row.</td>
</tr>
<tr>
<td class="name">model</td>
<td class="type">object</td>
<td class="description">Returns the Gantt model.</td>
</tr>
<tr>
<td class="name">requestType</td>
<td class="type">string</td>
<td class="description">Returns request type.</td>
</tr>
<tr>
<td class="name">type</td>
<td class="type">string</td>
<td class="description">Returns the name of the event.</td>
</tr>
<tr>
<td class="name">roundOffDuration</td>
<td class="type">boolean</td>
<td class="description">Duration is rounded off when it is set true.</td>
</tr>
</tbody>
</table>
</td>
</tr>
</tbody>
</table>




#### Example


{% highlight html %}
 
<div id="gantt"></div> 
<script>
$("#gantt").ejGantt({
   rowDrag: function (args) {}
});
</script>
{% endhighlight %}


### rowDragStart
{:#events:rowdragstart}


Triggered while start to drag row in Gantt control

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
<td class="name">argument</td>
<td class="type">Object</td>
<td class="description">Arguments when drag starts.
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
<td class="type">boolean</td>
<td class="description">Returns the cancel option value.</td>
</tr>
<tr>
<td class="name">draggedRow</td>
<td class="type">object</td>
<td class="description">Returns the row which we start to drag.</td>
</tr>
<tr>
<td class="name">draggedRowIndex</td>
<td class="type">boolean</td>
<td class="description">Returns the row index which we start to drag.</td>
</tr>
<tr>
<td class="name">model</td>
<td class="type">object</td>
<td class="description">Returns the Gantt model.</td>
</tr>
<tr>
<td class="name">requestType</td>
<td class="type">string</td>
<td class="description">Returns request type.</td>
</tr>
<tr>
<td class="name">type</td>
<td class="type">string</td>
<td class="description">Returns the name of the event.</td>
</tr>
</tbody>
</table>
</td>
</tr>
</tbody>
</table>




#### Example


{% highlight html %}
 
<div id="gantt"></div> 
<script>
$("#gantt").ejGantt({
   rowDragStart: function (args) {}
});
</script>
{% endhighlight %}


### rowDragStop
{:#events:rowdragstop}


Triggered while drop a row in Gantt control

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
<td class="name">argument</td>
<td class="type">Object</td>
<td class="description">Arguments when dragging a row.
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
<td class="type">boolean</td>
<td class="description">Returns the cancel option value.</td>
</tr>
<tr>
<td class="name">draggedRow</td>
<td class="type">object</td>
<td class="description">Returns the row which we start to drag.</td>
</tr>
<tr>
<td class="name">draggedRowIndex</td>
<td class="type">number</td>
<td class="description">Returns the row index which we start to drag.</td>
</tr>
<tr>
<td class="name">targetRow</td>
<td class="type">object</td>
<td class="description">Returns the row which we are dropped to row.</td>
</tr>
<tr>
<td class="name">targetRowIndex</td>
<td class="type">number</td>
<td class="description">Returns the row index which we are dropped to row.</td>
</tr>
<tr>
<td class="name">model</td>
<td class="type">object</td>
<td class="description">Returns the Gantt model.</td>
</tr>
<tr>
<td class="name">requestType</td>
<td class="type">string</td>
<td class="description">Returns request type.</td>
</tr>
<tr>
<td class="name">type</td>
<td class="type">string</td>
<td class="description">Returns the name of the event.</td>
</tr>
</tbody>
</table>
</td>
</tr>
</tbody>
</table>

#### Example

{% highlight html %}
 
<div id="gantt"></div> 
<script>
$("#gantt").ejGantt({
   rowDragStop: function (args) {}
});
</script>
{% endhighlight %}

### rowSelected
{:#events:rowselected}

Triggered after the row is selected.

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
<td class="name">argument</td>
<td class="type">Object</td>
<td class="description">Arguments when rowSelected event is triggered.
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
<td class="type">boolean</td>
<td class="description">Returns the cancel option value.</td>
</tr>
<tr>
<td class="name">targetRow</td>
<td class="type">object</td>
<td class="description">Returns the selecting row element.</td>
</tr>
<tr>
<td class="name">recordIndex</td>
<td class="type">number</td>
<td class="description">Returns the index of selecting row record.</td>
</tr>
<tr>
<td class="name">data</td>
<td class="type">object</td>
<td class="description">Returns the data of selected record.</td>
</tr>
</tbody>
</table>
</td>
</tr>
</tbody>
</table>


#### Example


{% highlight html %}
 
<div id="gantt"></div> 
<script>
$("#gantt").ejGantt({
   rowSelected: function (args) {}
});
</script>
{% endhighlight %}


### rowSelecting
{:#events:rowselecting}

Triggered before the row is going to be selected.

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
<td class="name">argument</td>
<td class="type">Object</td>
<td class="description">Arguments when rowSelecting event is triggered.
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
<td class="type">boolean</td>
<td class="description">Returns the cancel option value.</td>
</tr>
<tr>
<td class="name">data</td>
<td class="type">object</td>
<td class="description">Returns the data selecting record.</td>
</tr>
<tr>
<td class="name">recordIndex</td>
<td class="type">string</td>
<td class="description">Returns the index of selecting row record.</td>
</tr>
<tr>
<td class="name">targetChartRow</td>
<td class="type">object</td>
<td class="description">Returns the selecting row chart element.</td>
</tr>
<tr>
<td class="name">targetGridRow</td>
<td class="type">object</td>
<td class="description">Returns the selecting row grid element.</td>
</tr>
<tr>
<td class="name">previousData</td>
<td class="type">object</td>
<td class="description">Returns the previous selected data.</td>
</tr>
<tr>
<td class="name">previousIndex</td>
<td class="type">string</td>
<td class="description">Returns the previous selected row index.</td>
</tr>
<tr>
<td class="name">previousChartRow</td>
<td class="type">object</td>
<td class="description">Returns the previous selected row chart element.</td>
</tr>
<tr>
<td class="name">previousGridRow</td>
<td class="type">object</td>
<td class="description">Returns the previous selected row grid element.</td>
</tr>
</tbody>
</table>
</td>
</tr>
</tbody>
</table>


#### Example


{% highlight html %}
 
<div id="gantt"></div> 
<script>
$("#gantt").ejGantt({
   rowSelecting: function (args) {}
});
</script>
{% endhighlight %}

### splitterResized
{:#events:splitterresized}

Triggered after splitter resizing action in Gantt

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
<td class="name">argument</td>
<td class="type">Object</td>
<td class="description">Arguments when splitterResized event is triggered.
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
<td class="type">boolean</td>
<td class="description">Returns the cancel option value.</td>
</tr>
<tr>
<td class="name">currentSplitterPosition</td>
<td class="type">string</td>
<td class="description">Returns the value based on current splitter position.</td>
</tr>
<tr>
<td class="name">customSplitterPosition</td>
<td class="type">string</td>
<td class="description">To set custom position for splitter after resize action.</td>
</tr>
<tr>
<td class="name">isOnResize</td>
<td class="type">boolean</td>
<td class="description">Returns the value to differentiate whether splitter resizing is performed either by manual resizing or by method</td>
</tr>
<tr>
<td class="name">isSplitterIndex</td>
<td class="type">boolean</td>
<td class="description">To differentiate `customSplitterPosition` value was index or position.</td>
</tr>
<tr>
<td class="name">prevSplitterPosition</td>
<td class="type">string</td>
<td class="description">Returns the previous splitter position</td>
</tr>
</tbody>
</table>
</td>
</tr>
</tbody>
</table>

#### Example

{% highlight html %}
 
<div id="gantt"></div> 
<script>
$("#gantt").ejGantt({
   splitterResized: function (args) {}
});
</script>
{% endhighlight %}


### taskbarClick
{:#events:taskbarclick}

Triggered when taskbar item is clicked in Gantt.

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
<td class="name">argument</td>
<td class="type"><span class="param-type">Object</span></td>
<td class="description last">Arguments when taskbarClick event is triggered.
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
<td class="name">data</td>
<td class="type"><span class="param-type">object</span></td>
<td class="description">Returns currently clicked row data</td>
</tr>
<tr>
<td class="name">index</td>
<td class="type"><span class="param-type">number</span></td>
<td class="description">Returns the current item index.</td>
</tr>
<tr>
<td class="name">model</td>
<td class="type"><span class="param-type">object</span></td>
<td class="description">Returns the Gantt model.</td>
</tr>
<tr>
<td class="name">taskbarElement</td>
<td class="type"><span class="param-type">object</span></td>
<td class="description">Returns the clicked row element</td>
</tr>
<tr>
<td class="name">target</td>
<td class="type"><span class="param-type">object</span></td>
<td class="description">Returns the target element.</td>
</tr>
<tr>        
<td class="name">type</td>
<td class="type"><span class="param-type">string</span></td>
<td class="description">Returns the name of the event.</td>
</tr>
</tbody>
</table>
</td>
</tr>
</tbody>
</table>

#### Example
{:.example}

{% highlight html %}
 
<div id="gantt"></div> 
<script>
$("#gantt").ejGantt({
   taskbarClick: function (args) {}
});
</script>
{% endhighlight %}

### taskbarEdited
{:#events:taskbaredited}

Triggered after completing the editing operation in taskbar

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
<td class="name">argument</td>
<td class="type">Object</td>
<td class="description">Arguments when taskbarEdited event is triggered.
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
<td class="type">boolean</td>
<td class="description">Returns the cancel option value.</td>
</tr>
<tr>
<td class="name">data</td>
<td class="type">object</td>
<td class="description">Returns the data of edited record.</td>
</tr>
<tr>
<td class="name">previousData</td>
<td class="type">object</td>
<td class="description">Returns the previous data value of edited record.</td>
</tr>
<tr>
<td class="name">dragging</td>
<td class="type">boolean</td>
<td class="description">Returns 'true' if taskbar is dragged.</td>
</tr>
<tr>
<td class="name">leftResizing</td>
<td class="type">boolean</td>
<td class="description">Returns 'true' if taskbar is left resized.</td>
</tr>
<tr>
<td class="name">rightResizing</td>
<td class="type">boolean</td>
<td class="description">Returns 'true' if taskbar is right resized.</td>
</tr>
<tr>
<td class="name">progressResizing</td>
<td class="type">boolean</td>
<td class="description">Returns 'true' if taskbar is progress resized.</td>
</tr>
<tr>
<td class="name">editingFields</td>
<td class="type">object</td>
<td class="description">Returns the field values of record being edited.</td>
</tr>
<tr>
<td class="name">model</td>
<td class="type">object</td>
<td class="description">Returns the Gantt model.</td>
</tr>
</tbody>
</table>
</td>
</tr>
</tbody>
</table>


#### Example


{% highlight html %}
 
<div id="gantt"></div> 
<script>
$("#gantt").ejGantt({
   taskbarEdited: function (args) {}
});
</script>
{% endhighlight %}


### taskbarEditing
{:#events:taskbarediting}

Triggered while editing the Gantt chart (dragging, resizing the taskbar )

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
<td class="name">argument</td>
<td class="type">Object</td>
<td class="description">Arguments when taskbarEditing event is triggered.
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
<td class="type">boolean</td>
<td class="description">Returns the cancel option value.</td>
</tr>
<tr>
<td class="name">model</td>
<td class="type">object</td>
<td class="description">Returns the Gantt model.</td>
</tr>
<tr>
<td class="name">rowData</td>
<td class="type">object</td>
<td class="description">Returns the row object being edited.</td>
</tr>
<tr>
<td class="name">editingFields</td>
<td class="type">object</td>
<td class="description">Returns the field values of record being edited.</td>
</tr>
<tr>
<td class="name">type</td>
<td class="type">string</td>
<td class="description">Returns the name of the event.</td>
</tr>
<tr>
<td class="name">roundOffDuration</td>
<td class="type">boolean</td>
<td class="description">Returns duration value will be round-off or not.</td>
</tr>
</tbody>
</table>
</td>
</tr>
</tbody>
</table>


#### Example


{% highlight html %}
 
<div id="gantt"></div> 
<script>
$("#gantt").ejGantt({
   taskbarEditing: function (args) {}
});
</script>
{% endhighlight %}

### toolbarClick
{:#events:toolbarclick}

Triggered when toolbar item is clicked in Gantt.

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
<td class="name">argument</td>
<td class="type"><span class="param-type">Object</span></td>
<td class="description last">Arguments when toolbarClick event is triggered.
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
<td class="description">Returns the cancel option value.</td>
</tr>
<tr>
<td class="name">currentTarget</td>
<td class="type"><span class="param-type">object</span></td>
<td class="description">Returns the current item.</td>
</tr>
<tr>
<td class="name">model</td>
<td class="type"><span class="param-type">object</span></td>
<td class="description">Returns the Gantt model.</td>
</tr>
<tr>
<td class="name">itemName</td>
<td class="type"><span class="param-type">string</span></td>
<td class="description">Returns the name of the toolbar item on which mouse click has been performed</td>
</tr>
<tr>
<td class="name">type</td>
<td class="type"><span class="param-type">string</span></td>
<td class="description">Returns the name of the event.</td>
</tr>
</tbody>
</table>
</td>
</tr>
</tbody>
</table>

#### Example
{:.example}

{% highlight html %}
 
<div id="gantt"></div> 
<script>
$("#gantt").ejGantt({
   toolbarClick: function (args) {}
});
</script>
{% endhighlight %}

