---
layout: post
title: Properties, Methods and Events of ejTreeGrid Widget
description: Methods, members, events available in ejTreeGrid
documentation: API
platform: js-api
keywords: ejTreeGrid, API, Essential JS TreeGrid
---

# ejTreeGrid

 Custom Design for HTML TreeGrid control.


#### Syntax

{% highlight javascript %}

$(element).ejTreeGrid()

{% endhighlight %}

#### Example


{% highlight html %}
 
<treegrid id="treegrid">treegrid</treegrid> 
 
<script>
// Create TreeGrid
$('#treegrid').ejTreeGrid();    
</script>

{% endhighlight %}


#### Requires

* module:jQuery
* module:jquery.globalize.js
* module:jquery.easing.1.3.js
* module:jsrender.js
* module:ej.web.all.js


## Members


### allowColumnResize `boolean`
{:#members:allowcolumnresize}

Enables or disables the ability to resize the column width interactively.


#### Default Value

 * false


#### Example


{% highlight html %}   
              
        $("#treegrid").ejTreeGrid({ allowColumnResize:  true });
                                 
{% endhighlight %}

### allowColumnReordering `boolean`
{:#members:allowcolumnreordering}

Enables or disables the option for column reordering

#### Default Value

 * false


#### Example


{% highlight html %}   
              
        $("#treegrid").ejTreeGrid({ allowColumnReordering :  true });
                                 
{% endhighlight %}



### allowDragAndDrop `boolean`
{:#members:allowdraganddrop}

Enables or disables the ability to drag and drop the row interactively to reorder the rows.


#### Default Value

* false


#### Example


{% highlight html %}
 
        $("#treegrid").ejTreeGrid({  allowDragAndDrop : true });
        
{% endhighlight %}


### allowFiltering `boolean`
{:#members:allowfiltering}

Enables or disables the ability to filter the data on all the columns. Enabling this property will display a row with editor controls corresponding to each column. You can restrict filtering on particular column by disabling this property directly on that column instance itself.


#### Default Value

* false


#### Example


{% highlight html %}

        $("#treegrid").ejTreeGrid({  allowFiltering : true });
{% endhighlight %}


### allowKeyboardNavigation `boolean`
{:#members:allowkeyboardnavigation}

Enables or disables keyboard navigation.


#### Default Value

* true


#### Example


{% highlight html %}
                  
        $("#treegrid").ejTreeGrid({ allowKeyboardNavigation : true});                   
{% endhighlight %}


### allowMultiSorting `boolean`
{:#members:allowmultisorting}

Enables or disables the ability to sort the rows based on multiple columns/fields by clicking on each column header. Rows will be sorted recursively on clicking the column headers.


#### Default Value

* false


#### Example


{% highlight html %}
                   
        $("#treegrid").ejTreeGrid({ allowMultiSorting : true});                 

{% endhighlight %}


### allowSelection `boolean`
{:#members:allowselection}

Enables or disables the ability to select a row interactively.


#### Default Value

* true


#### Example


{% highlight html %}
   
        $("#treegrid").ejTreeGrid({ allowSelection:  true });                    

{% endhighlight %}


### allowSorting `boolean`
{:#members:allowsorting}

Enables or disables the ability to sort the rows based on a single field/column by clicking on that column header. When enabled, rows can be sorted only by single field/column.


#### Default Value

* false


#### Example


{% highlight html %}

        $("#treegrid").ejTreeGrid({ allowSorting : true });
        
{% endhighlight %}

### allowSearching `boolean`
{:#members:allowsearching}

Enables or disables the toolbar searching in TreeGrid.


#### Default Value

* false


#### Example


{% highlight html %}

        $("#treegrid").ejTreeGrid({ allowSearching : true });
        
{% endhighlight %}

### allowPaging `boolean`
{:#members:allowpaging}

Enables/disables pagination of rows in TreeGrid

#### Default Value

* false


#### Example


{% highlight html %}

        $("#treegrid").ejTreeGrid({ allowPaging : true });
        
{% endhighlight %}

### allowTextWrap `boolean`
{:#members:allowtextwrap}
 
Gets or sets a value that indicates whether the Content will wrap to the next line if the content exceeds the boundary of the Column Cells.

#### Default Value

* false

#### Example

{% highlight html %}   
              
        $("#treegrid").ejTreeGrid({ allowTextWrap : true });
                                 
{% endhighlight %}


### altRowTemplateID `string`
{:#members:altrowtemplateid}

Specifies the id of the template that has to be applied for alternate rows.


#### Default Value

* ""


#### Example


{% highlight html %}
                   
        $("#treegrid").ejTreeGrid(
 {
    altRowTemplateID: "altRowCustomTemplate"
 });            

{% endhighlight %}


### expandStateMapping `string`
{:#members:expandstatemapping}

Specifies the mapping property path for the expand status of a record in data source.


#### Default Value
{:.param}

* ""

#### Example
{:.example}


{% highlight html %}
 
<div id="treegrid"></div> 
<script>                  
       $("#treegrid").ejTreeGrid({ expandStateMapping : "isExpanded" });
</script>

{% endhighlight %}

### childMapping `string`
{:#members:childmapping}

Specifies the mapping property path for sub tasks in datasource


#### Default Value
{:.param}

* ""


#### Example
{:.example}


{% highlight html %}
 
<script>                          
        $("#treegrid").ejTreeGrid({  childMapping : "Children" });
</script>

{% endhighlight %}


### columns `array`
{:#members:columns}

Option for adding columns; each column has the option to bind to a field in the dataSource.


#### Example


{% highlight html %}
                          
        $("#treegrid").ejTreeGrid(
 {
    columns: [{ field: "Name", headerText: "Name", isTemplateColumn: true, templateID: "customColumnTemplate" },
                          { field: "Type", headerText: "Type" },
                          { field: "DateCreated", headerText: "Date Created" },
                          { field: "DateModified", headerText: "Date Modified" }]       
 });            

{% endhighlight %}


### columns.allowFiltering `boolean`
{:#members:columns-allowfiltering}

Enables or disables the ability to filter the rows based on this column.


#### Default Value

* false


#### Example


{% highlight html %}
 
        $("#treegrid").ejTreeGrid({ columns: [{ allowFiltering: true },{allowFiltering: false }] });
{% endhighlight %}

### columns.allowFilteringBlankContent `boolean`
{:#members:columns-allowfilteringblankcontent}

Enables the blanks option in ejDropDownList mapped in TreeGrid column

#### Default Value

* true


#### Example


{% highlight html %}
 
        $("#treegrid").ejTreeGrid({ columns: [{ allowFilteringBlankContent: false }});
		
{% endhighlight %}

### columns.allowSorting `boolean`
{:#members:columns-allowsorting}

Enables or disables the ability to sort the rows based on this column/field.

#### Default Value

* false


#### Example


{% highlight html %}
 
        $("#treegrid").ejTreeGrid({ columns: [{ allowSorting: true },{allowSorting: false }]  });

{% endhighlight %}

### columns.allowCellSelection `boolean`
{:#members:columns-allowcellselection}

Enables/disables cell selection.

#### Default Value

* false


#### Example


{% highlight html %}
 
        $("#treegrid").ejTreeGrid({ columns: [{ allowCellSelection: true },{allowCellSelection: false }]  });

{% endhighlight %}

### columns.editParams `Object`
{:#members:columns-editparams}

To customize the ej controls defined in TreeGrid column with their native property.


#### Default Value

* -


#### Example


{% highlight html %}
      
        $("#treegrid").ejTreeGrid({columns: [                    
{ field: "priority", headerText: "Priority", editType: "dropdownedit", dropdownData: stageData, editParams: { fields: { text: "text", value: "value" } } }]
});

{% endhighlight %}

### columns.editTemplate `Object`
{:#members:columns-edittemplate}

Gets or sets a template that displays a custom editor for editing the column values.

#### Default Value:

* null

#### Example

{:.example}
{% highlight html %}

$("#Treegrid ").ejTreeGrid ({
      //...
      columns: [
                 { field: "taskName", headerText: "Task Name", editType: "stringedit",
                 editTemplate: {
                        create: function () {
                                return "<input>";
                        },
                        write: function (args) {
                                obj = $('#TreeGridContainer').ejTreeGrid('instance');
                                var data = ej.DataManager(obj.model.flatRecords).executeLocal(new ej.Query().select("taskName"));
                                args.element.ejAutocomplete({ width: "100%", height:"28px", dataSource: data, enableDistinct: true, value: args.rowdata !== undefined ? args.rowdata["taskName"] : "" });
                        },
                        read: function (args) {
                                args.ejAutocomplete('suggestionList').css('display', 'none');
                                return args.ejAutocomplete("getValue");
                        },
                 },
            ],
     //...
});

{% endhighlight %}

### columns.editType `enum`
{:#members:columns-edittype}

<ts name = "ej.TreeGrid.EditingType"/>

Specifies the edit type of the column.

<table class="params">
<thead>
<tr>
<th>Name</th>
<th>Description</th>
</tr>
</thead>
<tbody>
<tr>
<td class="name">String</td>
<td class="description">It Specifies String edit type.</td>
</tr>
<tr>
<td class="name">Boolean</td>
<td class="description">It Specifies Boolean edit type.</td>
</tr>
<tr>
<td class="name">Numeric</td>
<td class="description">It Specifies Numeric edit type.</td>
</tr>
<tr>
<td class="name">Dropdown</td>
<td class="description">It Specifies Dropdown edit type.</td>
</tr>
<tr>
<td class="name">DatePicker</td>
<td class="description">It Specifies DatePicker edit type.</td>
</tr>
<tr>
<td class="name">DateTimePicker</td>
<td class="description">It Specifies DateTimePicker edit type.</td>
</tr>
<tr>
<td class="name">Maskedit</td>
<td class="description">It Specifies Maskedit edit type.</td>
</tr>
</tbody>
</table>

#### Default Value

* ej.TreeGrid.EditingType.String


#### Example


{% highlight html %}
 
 $("#treegrid").ejTreeGrid({columns: [{ editType: ej.TreeGrid.EditingType.String},{editType: ej.TreeGrid.EditingType.Boolean}]});

{% endhighlight %}

### columns.dropdownData `string`
{:#members:columns-dropdowndata}

To bind the dropdown data for TreeGrid column mapped with ejDropDownList


#### Default Value

* -


#### Example


{% highlight html %}
       var dataSource = [
                    //
          { id: 4, text: "Critical", value: "Critical" }
        ];
        $("#treegrid").ejTreeGrid(columns: [                    
{ field: "priority", headerText: "Priority", editType: "dropdownedit", dropdownData: dataSource}]);
	
{% endhighlight %}

### columns.field `string`
{:#members:columns-field}

Specifies the name of the field from the dataSource to bind with this column.


#### Default Value

* ""


#### Example


{% highlight html %}
      
        $("#treegrid").ejTreeGrid({columns: [{ field: "Name"},{field: "Type"}]});

{% endhighlight %}


### columns.template `string`
{:#members:columns-template}

Specifies the template string of the script element to enable column template for a column.

#### Default Value
* ""

#### Example

{% highlight html %}      

$("#treegrid").ejTreeGrid({
    columns: [{
         isTemplateColumn: true,
         template: "<script type="text/x-jsrender" id="columnTemplate">
                   <div style="display:inline-block;">
                   <img src="../images/gantt/.png" height="40" /></div></script>"
           }]
});

{% endhighlight %}


### columns.templateID `string`
{:#members:columns-templateid}

Specifies the template ID of the script element to enable column template for a column.

#### Default Value
* ""

#### Example

{% highlight js %}      

<script type="text/x-jsrender" id="columnTemplate">      
  <div style="display:inline-block;">
   <img src="../images/gantt/.png" height="40" />
  </div>        
</script>

{% endhighlight %}

{% highlight html %}      

$("#treegrid").ejTreeGrid({
    columns: [{
        isTemplateColumn: true,
        templateID: "columnTemplate"
    }]
});

{% endhighlight %}

### columns.angularTemplate `string`
{:#members:columns-angulartemplate}

Specifies the template ID or the template string of the AngularJS script element to enable column template for a column.

#### Default Value
* ""

#### Example

{% highlight js %}   

<script type="text/ng-template" id="ngColumnTemplate">
    <div style="padding:5px;">
        <img src="content/images/treegrid/{{data.FullName}}.png" />
    </div>
</script>

{% endhighlight %}

{% highlight html %}    

$("#treegrid").ejTreeGrid({
   columns: [{
     isTemplateColumn: true,
     angularTemplate: "#ngColumnTemplate"  
   }]
});

{% endhighlight %}

### columns.filterEditType `enum`
{:#members:columns-filteredittype}

<ts name = "ej.TreeGrid.EditingType"/>

Specifies the type of the editor control to be used to filter the rows.

<table class="params">
<thead>
<tr>
<th>Name</th>
<th>Description</th>
</tr>
</thead>
<tbody>
<tr>
<td class="name">String</td>
<td class="description">It Specifies String edit type.</td>
</tr>
<tr>
<td class="name">Boolean</td>
<td class="description">It Specifies Boolean edit type.</td>
</tr>
<tr>
<td class="name">Numeric</td>
<td class="description">It Specifies Numeric edit type.</td>
</tr>
<tr>
<td class="name">Dropdown</td>
<td class="description">It Specifies Dropdown edit type.</td>
</tr>
<tr>
<td class="name">DatePicker</td>
<td class="description">It Specifies DatePicker edit type.</td>
</tr>
<tr>
<td class="name">DateTimePicker</td>
<td class="description">It Specifies DateTimePicker edit type.</td>
</tr>
</tbody>
</table>

#### Default Value

* ej.TreeGrid.EditingType.String


#### Example


{% highlight html %}
       
        $("#treegrid").ejTreeGrid({columns: [{ filterEditType: ej.TreeGrid.EditingType.String},{filterEditType: ej.TreeGrid.EditingType.Boolean}]});

{% endhighlight %}

### columns.filterType `enum`
{:#members:columns-filtertype}

<ts name="ej.TreeGrid.FilterType"/>

Gets or sets a value to render either excel or menu filtering in TreeGrid column filtering.

<table class="params">
<thead>
<tr>
<th>Name</th>
<th>Description</th>
</tr>
</thead>
<tbody>
<tr>
<td class="name">Menu</td>
<td class="description">Specifies the filter type as menu.</td>
</tr>
<tr>
<td class="name">Excel</td>
<td class="description">Specifies the filter type as excel.</td>
</tr>
</tbody>
</table>

#### Default Value

* null

#### Example


{% highlight html %}
         
        $("#treegrid").ejTreeGrid({columns: [{ headerText: "TaskName",filterType:"excel"}]});

{% endhighlight %}

### columns.headerText `string`
{:#members:columns-headertext}

Header text of the column.


#### Default Value

* null


#### Example


{% highlight html %}
         
        $("#treegrid").ejTreeGrid({columns: [{ headerText: "Name"},{headerText: "Type"}]});

{% endhighlight %}

### columns.displayAsCheckbox `boolean`
{:#members:columns-displayascheckbox}

Gets or sets a value that indicates to display a column value as checkbox or string

#### Default Value

* false

#### Example

{% highlight html %}
         
        $("#treegrid").ejTreeGrid({columns: [{ field: "Approved", displayAsCheckbox: true, editType: ej.TreeGrid.EditingType.Boolean}]});

{% endhighlight %}


### columns.showCheckbox `boolean`
{:#members:columns-showcheckbox}

Enables or disables the checkbox visibility in a column for checkbox selection.

#### Default Value

* false

#### Example

{% highlight html %}
         
        $("#treegrid").ejTreeGrid({columns: [{ field: "name",showCheckbox: true}]});

{% endhighlight %}


### columns.visible `boolean`
{:#members:columns-visible}

Controls the visibility of the column.


#### Default Value

* true


#### Example


{% highlight html %}
         
        $("#treegrid").ejTreeGrid({columns: [{ field: "name",visible: true},{field: "Type",visible: false}]});

{% endhighlight %}

### columns.width `number`
{:#members:columns-width}

Gets or sets a value for treegrid column width

#### Default Value

* -

#### Example
{% highlight html %}
         
        $("#treegrid").ejTreeGrid({columns: [{  width: 40 }]});
{% endhighlight %}


### columns.headerTemplateID `string`
{:#members:columns-headertemplateid}

Specifies the header template value for the column header

#### Default Value

* ""

#### Example

{% highlight html %}
         
        $("#treegrid").ejTreeGrid({columns: [{  headerTemplateID: "#dataTemplate1"},{ headerTemplateID: "#dataTemplate2"}]});

{% endhighlight %}


### columns.format `object`
{:#members:columns-format}

Specifies the display format of a column

#### Default Value

* null


#### Example

{% highlight html %}
         
        $("#treegrid").ejTreeGrid({columns: [{ field: "Currency",  format: "{0:C2}" }, //... ]});

{% endhighlight %}


### columns.isTemplateColumn `boolean`
{:#members:columns-istemplatecolumn}

Specifies whether the column is a template column

#### Default Value

* false

#### Example

{% highlight html %}
         
     $("#treegrid").ejTreeGrid({columns: [{ field:"CustomColumn", isTemplateColumn: true, templateID: "customColumnTemplate"}]});

{% endhighlight %}

### columns.headerTextAlign `enum`
{:#members:columns-headertextalign}

<ts name = "ej.TextAlign"/>

Specifies the alignment of the column header text

<table class="params">
<thead>
<tr>
<th>Name</th>
<th>Description</th>
</tr>
</thead>
<tbody>
<tr>
<td class="name">Left</td>
<td class="description">align the header text to the left</td>
</tr>
<tr>
<td class="name">Right</td>
<td class="description">align the header text to the right</td>
</tr>
<tr>
<td class="name">Justify</td>
<td class="description">To justify the header alignment</td>
</tr>
<tr>
<td class="name">Center</td>
<td class="description">align the header text to the center</td>
</tr>
</tbody>
</table>

#### Default Value

* ej.TextAlign.Left

#### Example

{% highlight html %}
         
        $("#treegrid").ejTreeGrid({columns: [{  headerTextAlign: ej.TextAlign.Center},{headerTextAlign: ej.TextAlign.Right}]});

{% endhighlight %}

### columns.isFrozen `boolean`
{:#members:columns-isfrozen}

Specifies whether the column is frozen

#### Default Value

* false

#### Example

{% highlight html %}
         
        $("#treegrid").ejTreeGrid({columns: [{  isFrozen: true}]});

{% endhighlight %}

### columns.textAlign `enum`
{:#members:columns-textalign}

<ts name = "ej.TextAlign"/>

Specifies the text alignment for the column

<table class="params">
<thead>
<tr>
<th>Name</th>
<th>Description</th>
</tr>
</thead>
<tbody>
<tr>
<td class="name">Left</td>
<td class="description">align the content text to the left</td>
</tr>
<tr>
<td class="name">Right</td>
<td class="description">align the content text to the right</td>
</tr>
<tr>
<td class="name">Justify</td>
<td class="description">To justify the content alignment</td>
</tr>
<tr>
<td class="name">Center</td>
<td class="description">align the content text to the center</td>
</tr>
</tbody>
</table>

#### Default Value

* ej.TextAlign.Left

#### Example

{% highlight html %}
         
        $("#treegrid").ejTreeGrid({columns: [{  textAlign: ej.TextAlign.Center},{ textAlign: ej.TextAlign.Right}]});

{% endhighlight %}

### columns.allowEditing `boolean`
{:#members:columns-allowediting}

Enables or disables the ability to edit a row or cell.

#### Default Value

* false

#### Example

{% highlight html %}
         
        $("#treegrid").ejTreeGrid({columns: [{  allowEditing: false }]});

{% endhighlight %}

### columns.commands `array`
{:#members:columns-commands}

Gets or sets an object to define a command column in TreeGrid.

#### Default Value:
{:.param}
* []

#### Example
{:.example}
{% highlight html %}
$("#treegrid").ejTreeGrid({ columns:[{
              headerText: "Manage Records",
              commands: [
                  { type: ej.TreeGrid.UnboundType.Edit, buttonOptions: { text: "Edit" } },
                  { type: ej.TreeGrid.UnboundType.Delete, buttonOptions: { text: "Delete" } },
                  { type: ej.TreeGrid.UnboundType.Save, buttonOptions: { text: "Save" } },
                  { type: ej.TreeGrid.UnboundType.Cancel, buttonOptions: { text: "Cancel" } }
               ],
             }
    ] });
{% endhighlight %}

### columns.commands.buttonOptions `object`
{:#members:columns-commands-buttonoptions}

Gets or sets an object to customize command button with available ejButton properties.

#### Default Value:
{:.param}
* -

#### Example
{:.example}
{% highlight html %}
$("#treegrid").ejTreeGrid({ columns:[{commands: [buttonOptions: { text: "Edit" } }]}]});
{% endhighlight %}

### columns.commands.type `enum`
{:#members:columns-commands-type}

<ts name="ej.TreeGrid.UnboundType"/>

Gets or sets a value that define the command column buttons to be displayed.

#### Default Value:
{:.param}
* -

<table>
<tr>
<th>Name</th>
<th>Description</th>
</tr>
<tr>
<td class="name">Edit</td>
<td class="description">Unbound type to perform edit action</td>
</tr>
<tr>
<td class="name">Save</td>
<td class="description">Unbound type to perform save action</td>
</tr> 
<tr>
<td class="name">Delete</td>
<td class="description">Unbound type to perform delete action</td>
</tr> 
<tr>
<td class="name">Cancel</td>
<td class="description">Unbound type to perform cancel action</td>
</tr> 
</table>

#### Example
{% highlight html %}
<div id="TreeGrid"></div> 
<script>
$("#TreeGrid").ejTreeGrid({    
    columns:[          
           {
              headerText: "Manage Records",
              commands: [
                  { type: ej.TreeGrid.UnboundType.Edit, buttonOptions: { text: "Edit" } },
                  { type: ej.TreeGrid.UnboundType.Delete, buttonOptions: { text: "Delete" } },
                  { type: ej.TreeGrid.UnboundType.Save, buttonOptions: { text: "Save" } },
                  { type: ej.TreeGrid.UnboundType.Cancel, buttonOptions: { text: "Cancel" } }
               ]             
           }
	] 
});
</script> 
{% endhighlight %}

### columns.showInColumnChooser `boolean`
{:#members:columns-showincolumnchooser}

We can include or exclude particular column from column visibility list in column menu.

#### Default Value

* true

#### Example

{% highlight html %}
         
        $("#treegrid").ejTreeGrid({columns: [{  showInColumnChooser: false }]});

{% endhighlight %}

### columns.clipMode `enum`
{:#members:columns-clipmode}

<ts name = "ej.TreeGrid.ClipMode"/>

Sets the clip mode for TreeGrid cell as ellipsis or clipped content(both header and content)

<table class="params">
<thead>
<tr>
<th>Name</th>
<th>Description</th>
</tr>
</thead>
<tbody>
<tr>
<td class="name">Ellipsis</td>
<td class="description">Shows ellipsis for the overflown cell.</td>
</tr>
<tr>
<td class="name">Clip</td>
<td class="description">Truncate the text in the cell.</td>
</tr>
</tbody>
</table>

#### Default Value

* ej.TreeGrid.ClipMode.Clip


#### Example


{% highlight html %}
       
        $("#treegrid").ejTreeGrid({columns: [{ clipMode: ej.TreeGrid.ClipMode.Clip},{clipMode: ej.TreeGrid.ClipMode.Ellipsis}]});

{% endhighlight %}

### columns.tooltip  `string`
{:#members:columns-tooltip}

Sets the tooltip template for the specific column.

#### Default Value

* null

#### Example

{% highlight html %}
         
        $("#treegrid").ejTreeGrid({columns: [{  tooltip: "" }]});

{% endhighlight %}

### columns.headerTooltip   `string`
{:#members:columns-headertooltip}

Sets the tooltip template for the column header

#### Default Value

* null

#### Example

{% highlight html %}
         
        $("#treegrid").ejTreeGrid({columns: [{  headerTooltip: "" }]});

{% endhighlight %}

### columns.validationRules `Object`
{:#members:columns-validationrules}

specifies the conditions for saving data to the database while adding or editing the fields.

#### Example
{:.example}
{% highlight html %}
<div id="treegrid"></div>          
<script>
$("#treegrid").ejTreeGrid({
  editSettings: {allowEditing: true, allowAdding: true},
  columns:[{field:"TaskID", validationRules: { required: true, number: true }},{field:"TaskName"},{field:"StartDate"}] 
});
</script> 
{% endhighlight %}

### columns.priority `number`
{:#members:columns-priority}

Gets or sets the priority value of the column. It is used to show/hide TreeGrid columns in responsive mode.

#### Default Value

* -1

#### Example

{:.example}
{% highlight html %}
<div id="treegrid"></div>          
<script>
$("#treegrid").ejTreeGrid({
      //...
      columns: [
                { field: "taskID", headerText: "Task Id", width: "45", editType: "numericedit" },
                { field: "taskName", headerText: "Task Name", width: "90", editType: "stringedit" },
                { field: "startDate", headerText: "Start Date", editType: "datepicker", format: dateFormat },
                { field: "endDate", headerText: "End Date", format: dateFormat, editType: "datepicker", priority:5 },
                { field: "duration", headerText: "Duration", editType: "numericedit", priority: 6 },
                { field: "progress", headerText: "Progress", editType: "numericedit",priority:6 }
            ],
      //... 
});
</script> 
{% endhighlight %}

### columnDialogFields `array`
{:#members:columndialogfields}

To Specify the column fields to be displayed in the dialog while inserting a column using column menu.

#### Default Value
{:.param}

* []


#### Example
{:.example}


{% highlight html %}
 
<div id="treegrid"></div> 
<script>  
        $("#treegrid").ejTreeGrid({ columnDialogFields: ["field", "headerText", "editType", "width", "visible", "allowSorting", "textAlign", "headerTextAlign"] });                   
</script>

{% endhighlight %}

### columns.allowFreezing `boolean`
{:#members:columns-allowfreezing}

Enables or disables the ability to freeze/unfreeze the columns

#### Default Value

* false

#### Example

{% highlight html %}
         
        $("#treegrid").ejTreeGrid({columns: [{  allowFreezing: false }]});

{% endhighlight %}

### contextMenuSettings `object`
{:#members:contextmenusettings}

Options for displaying and customizing context menu items.


### contextMenuSettings.contextMenuItems `array`
{:#members:contextmenusettings-contextmenuitems}

Option for adding items to context menu.


#### Default Value

* []


#### Example


{% highlight html %}
   
        $("#treegrid").ejTreeGrid({ contextMenuItems: [ej.TreeGrid.ContextMenuItems.Add,ej.TreeGrid.ContextMenuItems.Edit] });                   

{% endhighlight %}


### contextMenuSettings.showContextMenu `boolean`
{:#members:contextmenusettings-showcontextmenu}

Shows/hides the context menu.


#### Default Value

* false


#### Example


{% highlight html %}
  
        $("#treegrid").ejTreeGrid(contextMenuSettings :{ showContextMenu:  true });                      

{% endhighlight %}

### cssClass `string`
{:#members:cssclass}

Specify the CSS class for TreeGrid to achieve custom theme.


#### Default Value
{:.param}

* ""

#### Example
{:.example}


{% highlight html %}
 
<div id="treeGrid"></div> 
<script>          
        $("#treeGrid").ejTreeGrid({  cssClass : "gradient-lime" });
</script>

{% endhighlight %}

### dataSource `array`
{:#members:datasource}

Specifies hierarchical or self-referential data to populate the TreeGrid.


#### Default Value

* null


#### Example


{% highlight html %}
          
        $("#treegrid").ejTreeGrid(
 {
    dataSource:[{Id:2,TaskName:"Testing",startDate:"12/1/2000",Duration:5 }]    
 });            

{% endhighlight %}


### headerTextOverflow `enum`
{:#members:headertextoverflow}

<ts name = "ej.TreeGrid.HeaderTextOverflow"/>

Specifies whether to wrap the header text when it is overflown i.e., when it exceeds the header width.

<table class="params">
<thead>
<tr>
<th>Name</th>
<th>Description</th>
</tr>
</thead>
<tbody>
<tr>
<td class="name">None</td>
<td class="description">You can disable the word wrap</td>
</tr>
<tr>
<td class="name">Wrap</td>
<td class="description">You can wrap the header content</td>
</tr>
</tbody>
</table>

#### Default Value
{:.param}

* ej.TreeGrid.HeaderTextOverflow.None

#### Example


{% highlight html %}
         
        $("#treegrid").ejTreeGrid({ headerTextOverflow: ej.TreeGrid.HeaderTextOverflow.Wrap});

{% endhighlight %}


### dragTooltip `object`
{:#members:dragtooltip}

Options for displaying and customizing the tooltip. This tooltip will show the preview of the row that is being dragged.


### dragTooltip.showTooltip `boolean`
{:#members:dragtooltip-showtooltip}

Specifies whether to show tooltip while dragging a row.


#### Default Value

* true


#### Example


{% highlight html %}
                 
        $("#treegrid").ejTreeGrid(dragTooltip :{ showTooltip:  true });

{% endhighlight %}


### dragTooltip.tooltipItems `array`
{:#members:dragtooltip-tooltipitems}

Option to add field names whose corresponding values in the dragged row needs to be shown in the preview tooltip.


#### Default Value

* []


#### Example


{% highlight html %}

        $("#treegrid").ejTreeGrid(dragTooltip :{ tooltipItems: ["TaskName","TaskID","StartDate"] });                       

{% endhighlight %}


### dragTooltip.tooltipTemplate `string`
{:#members:dragtooltip-tooltiptemplate}

Custom template for that tooltip that is shown while dragging a row.


#### Default Value

* null


#### Example


{% highlight html %}
                  
        $("#treegrid").ejTreeGrid(dragTooltip :{ tooltipTemplate: "" });        

{% endhighlight %}


### editSettings `object`
{:#members:editsettings}

Options for enabling and configuring the editing related operations. 


### editSettings.allowAdding `boolean`
{:#members:editsettings-allowadding}

Enables or disables the button to add new row in context menu as well as in toolbar.


#### Default Value

* true


#### Example


{% highlight html %}
                  
        $("#treegrid").ejTreeGrid({  editSettings:{allowAdding : true} });

{% endhighlight %}


### editSettings.allowDeleting `boolean`
{:#members:editsettings-allowdeleting}

Enables or disables the button to delete the selected row in context menu as well as in toolbar.


#### Default Value

* true


#### Example


{% highlight html %}
                  
        $("#treegrid").ejTreeGrid({  editSettings:{allowDeleting : true} });    

{% endhighlight %}


### editSettings.allowEditing `boolean`
{:#members:editsettings-allowediting}

Enables or disables the ability to edit a row or cell.


#### Default Value

* false


#### Example


{% highlight html %}
                  
        $("#treegrid").ejTreeGrid({  editSettings:{allowEditing : true} });     

{% endhighlight %}

### editSettings.beginEditAction `enum`
{:#members:editsettings-begineditaction}

<ts name = "ej.TreeGrid.BeginEditAction"/>

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

* ej.TreeGrid.BeginEditAction.DblClick

#### Example


{% highlight html %}
                 
        $("#treegrid").ejTreeGrid({  editSettings:{beginEditAction : ej.TreeGrid.BeginEditAction.Click} });

{% endhighlight %}

### editSettings.editMode `enum`
{:#members:editsettings-editmode}

<ts name = "ej.TreeGrid.EditMode"/>

specifies the edit mode in TreeGrid , "cellEditing" is for cell type editing and "rowEditing" is for entire row.

<table class="params">
<thead>
<tr>
<th>Name</th>
<th>Description</th>
</tr>
</thead>
<tbody>
<tr>
<td class="name">CellEditing</td>
<td class="description">you can edit a cell.</td>
</tr>
<tr>
<td class="name">RowEditing</td>
<td class="description">you can edit a row.</td>
</tr>
<tr>
<td class="name">DialogEditing</td>
<td class="description">you can edit a row in dialog form.</td>
</tr>
</tbody>
</table>


#### Default Value

* ej.TreeGrid.EditMode.CellEditing


#### Example


{% highlight html %}
                 
        $("#treegrid").ejTreeGrid({  editSettings:{editMode : ej.TreeGrid.EditMode.CellEditing} });

{% endhighlight %}


### editSettings.rowPosition `enum`
{:#members:editsettings-rowposition}

<ts name = "ej.TreeGrid.RowPosition"/>

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
<td class="name">Above</td>
<td class="description">you can add a new row to above selected row.</td>
</tr>
<tr>
<td class="name">Below</td>
<td class="description">you can add a new row to below selected row.</td>
</tr>
<tr>
<td class="name">Child</td>
<td class="description">you can add a new row as a child for selected row.</td>
</tr>
</tbody>
</table>


#### Default Value

* "top"


#### Example


{% highlight html %}
   
 $("#treegrid").ejTreeGrid({  editSettings:{rowPosition : ej.TreeGrid.RowPosition.Bottom} });

{% endhighlight %}

### editSettings.dialogEditorTemplateID  `string`
{:#members:editsettings-dialogeditortemplateid}

Specifies the template ID for the custom dialog.


#### Default Value

* null


#### Example


{% highlight html %}
                  
        $("#treegrid").ejTreeGrid({  editSettings:{dialogEditorTemplateID  : ""} });     

{% endhighlight %}

### editSettings.showDeleteConfirmDialog `boolean`

{:#members:editsettings-showdeleteconfirmdialog }

Enable or disable the confirmation dialog while deleting the record.

#### Default Value

* false

#### Example
{% highlight html %}
        $("#treegrid").ejTreeGrid({  editSettings:{showDeleteConfirmDialog  : true} });     
{% endhighlight %}

### enableAltRow `boolean`
{:#members:enablealtrow}

Specifies whether to render alternate rows in different background colors.


#### Default Value

* true


#### Example


{% highlight html %}
                  
        $("#treegrid").ejTreeGrid({ enableAltRow : false});                     

{% endhighlight %}


### enableCollapseAll `boolean`
{:#members:enablecollapseall}

Specifies whether to load all the rows in collapsed state when the TreeGrid is rendered for the first time.


#### Default Value

* false


#### Example


{% highlight html %}
                 
        $("#treegrid").ejTreeGrid(
 {
    enableCollapseAll: false
 });            

{% endhighlight %}


### enableResize `boolean`
{:#members:enableresize}

Specifies whether to resize TreeGrid whenever window size changes.


#### Default Value

* false


#### Example


{% highlight html %}
        
        $("#treegrid").ejTreeGrid({enableResize:true});

{% endhighlight %}


### enableVirtualization `boolean`
{:#members:enablevirtualization}

Specifies whether to render only the visual elements that are visible in the UI. When you enable this property, it will reduce the loading time for loading large number of records. 


#### Default Value

* false


#### Example


{% highlight html %}
                 
        $("#treegrid").ejTreeGrid({ enableVirtualization : true});                      

{% endhighlight %}

### enableLoadOnDemand `boolean`
{:#members:enableloadondemand}

Gets or sets a value that indicates whether to enable load on demand approach, for rendering child records and page records.

#### Default Value

* false


#### Example


{% highlight html %}
                 
        $("#treegrid").ejTreeGrid({ enableLoadOnDemand : true});                      

{% endhighlight %}


### columnResizeSettings `object`
{:#members:columnresizesettings}

Specifies the settings for column resize

### columnResizeSettings.columnResizeMode `enum`
{:#members:columnresizesettings-columnresizemode}

<ts name = "ej.TreeGrid.ColumnResizeMode"/>

Specifies the mode for column resizing 

<table class="params">
<thead>
<tr>
<th>Name</th>
<th>Description</th>
</tr>
</thead>
<tbody>
<tr>
<td class="name">FixedColumns</td>
<td class="description">At load time column are rendered with given width value, while resizing the column only current column width is changed</td>
</tr>
<tr>
<td class="name">Normal</td>
<td class="description">At load time columns are stretched with control width,while resizing the column, current column width updated based on next column</td>
</tr>
<tr>
<td class="name">NextColumn</td>
<td class="description">In this mode columns are stretched with control width in load time and on resizing action.</td>
</tr>
</tbody>
</table>

#### Default Value
{:.param}

* ej.TreeGrid.ColumnResizeMode.Normal

#### Example


{% highlight html %}
 
        $("#treegrid").ejTreeGrid({  columnResizeSettings: { columnResizeMode : ej.TreeGrid.ColumnResizeMode.FixedColumns} });

{% endhighlight %}

### commonWidth `number`
{:#members:commonwidth}

Defines the common width for all the columns in TreeGrid

#### Default Value

* 150


#### Example


{% highlight html %}
 
        $("#treegrid").ejTreeGrid({  commonWidth:180 });

{% endhighlight %}

### filterSettings `object`
{:#members:filtersettings}

Options for filtering and customizing filter actions.

### filterSettings.filterBarMode `string`
{:#members:filtersettings-filterbarmode}

Specifies the mode on which column filtering should start

#### Default Value

* "immediate"


#### Example


{% highlight html %}
 
        $("#treegrid").ejTreeGrid({  filterSettings: { filterBarMode : "onEnter"} });

{% endhighlight %}

### filterSettings.filterType `enum`
{:#members:filtersettings-filtertype}

<ts name = "ej.TreeGrid.FilterType"/>

Specifies the type of column filtering.

<table class="params">
<thead>
<tr>
<th>Name</th>
<th>Description</th>
</tr>
</thead>
<tbody>
<tr>
<td class="name">FilterBar</td>
<td class="description">Enables the filterbar filtering</td>
</tr>
<tr>
<td class="name">Menu</td>
<td class="description">Enables the menu filtering</td>
</tr>
</tbody>
</table>

#### Default Value
{:.param}

* ej.TreeGrid.FilterType.FilterBar


#### Example


{% highlight html %}
 
        $("#treegrid").ejTreeGrid({  filterSettings: { filterType : ej.TreeGrid.FilterType.Menu} });

{% endhighlight %}


### filterSettings.filteredColumns `array`
{:#members:filtersettings-filteredcolumns}

Specifies the column collection for filtering the TreeGrid content on initial load

#### Default Value

* []

### filterSettings.filteredColumns.value `string`
{:#members:filtersettings-filteredcolumns-value}

Specifies the value to be filtered in TreeGrid.

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
   
$("#treegrid").ejTreeGrid({
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

### filterSettings.maxFilterChoice `number`
{:#members:filtersettings-maxfilterchoice}

Gets or sets a value that indicates the maximum number of filter choices that can be showed in the excel styled filter menu.

#### Default Value

* 1000

#### Example

{% highlight html %}
   
$("#treegrid").ejTreeGrid({
    filterSettings: {
        maxFilterChoice:500,
    },
});                   

{% endhighlight %}

### filterSettings.enableCaseSensitivity `boolean`
{:#members:filtersettings-enablecasesensitivity}

Gets or sets a value that indicates to perform the filter operation with case sensitive in excel styled filter menu mode.

#### Default Value

* false

#### Example

{% highlight html %}
   
$("#treegrid").ejTreeGrid({
    filterSettings: {
        enableCaseSensitivity:true,
    },
});                   

{% endhighlight %}

### filterSettings.enableComplexBlankFilter `boolean`
{:#members:filtersettings-enablecomplexblankfilter}

Enables or disables the ability to filter the columns with empty, null and undefined values.

#### Default Value

* true

#### Example

{% highlight html %}
   
$("#treegrid").ejTreeGrid({
    filterSettings: {
        enableComplexBlankFilter:false,
    },
});                   

{% endhighlight %}

### filterSettings.filterHierarchyMode `enum`
{:#members:filtersettings-filterhierarchymode}

<ts name = "ej.TreeGrid.FilterHierarchyMode"/>

Specifies the mode of filtering to filter the record with or without hierarchy.

<table class="params">
<thead>
<tr>
<th>Name</th>
<th>Description</th>
</tr>
</thead>
<tbody>
<tr>
<td class="name">Parent</td>
<td class="description">Shows the filtered record with parent record</td>
</tr>
<tr>
<td class="name">Child</td>
<td class="description">Shows the filtered record with child record</td>
</tr>
<tr>
<td class="name">Both</td>
<td class="description">shows the filtered record with both parent and child record</td>
</tr>
<tr>
<td class="name">None</td>
<td class="description">Shows only filtered record.</td>
</tr>
</tbody>
</table>

#### Default Value
{:.param}

* ej.TreeGrid.FilterHierarchyMode.Parent


#### Example

{% highlight html %}
 
        $("#treegrid").ejTreeGrid({  filterSettings: { filterHierarchyMode : ej.TreeGrid.FilterHierarchyMode.Child} });

{% endhighlight %}

### locale `string`
{:#members:locale}

Specifies the localization information to customize the User Interface (UI) to support regional language and culture


#### Default Value

* "en-US"


#### Example


{% highlight html %}
                  
        $("#treegrid").ejTreeGrid({  locale : "fr-FR" });                   

{% endhighlight %}

### parseRowTemplate  `boolean`
{:#members:parserowtemplate}

Enables or disables internal parsing of a row. When disabled this property, row will be displayed using the defined template without any internal event bindings.


#### Default Value

* true


#### Example


{% highlight html %}
                  
        $("#treegrid").ejTreeGrid({  parseRowTemplate : false });                   

{% endhighlight %}

### idMapping `string`
{:#members:idmapping}

Specifies the name of the field in the dataSource, which contains the id of that row.


#### Default Value

* ""


#### Example


{% highlight html %}
                  
        $("#treegrid").ejTreeGrid({  IdMapping : "ID" });                   

{% endhighlight %}

### isResponsive `boolean`
{:#members:isresponsive}

Enables or disables the responsiveness of TreeGrid


#### Default Value

* "false"


#### Example


{% highlight html %}
                  
        $("#treegrid").ejTreeGrid({  isResponsive : true });                   

{% endhighlight %}

### parentIdMapping `string`
{:#members:parentidmapping}

Specifies the name of the field in the dataSource, which contains the parent's id. This is necessary to form a parent-child hierarchy, if the dataSource contains self-referential data.


#### Default Value

* ""


#### Example


{% highlight html %}
                
        $("#treegrid").ejTreeGrid({  parentIdMapping : "ID" });             

{% endhighlight %}


### pageSettings `object`
{:#members:pagesettings}

Specifies the options for customizing the pager.


### pageSettings.pageCount `number`
{:#members:pagesettings-pagecount}

Using this property we can specify the number of pages should pager contains, according to this count TreeGrid height will be updated.


#### Default Value
{:.param}

* 8


#### Example
{:.example}


{% highlight html %}
 
<div id="treegrid"></div> 
<script>                          
        $("#treegrid").ejGantt({  
                        pageSettings:{pageCount: 10, }
                });
</script>              

{% endhighlight %}


### pageSettings.pageSize `number`
{:#members:pagesettings-pagesize}

This specifies the number of rows to display in each page.


#### Default Value
{:.param}

* 12


#### Example
{:.example}


{% highlight html %}
 
<div id="treegrid"></div> 
<script>                  
        $("#treegrid").ejTreeGrid({  
                pageSettings:{pageSize : 10}
        });
</script>               

{% endhighlight %}

### pageSettings.totalRecordsCount `number`
{:#members:pagesettings-totalrecordscount}

Get the value of records which is bound to TreeGrid. The totalRecordsCount value is calculated based on the datasource bound to TreeGrid.


#### Default Value
{:.param}

* null


#### Example
{:.example}


{% highlight html %}
 
<div id="treegrid"></div> 
<script>                  
        $("#treegrid").ejTreeGrid({  
                        pageSettings:{totalRecordsCount : null}
                });
</script>               

{% endhighlight %}

### pageSettings.currentPage `number`
{:#members:pagesettings-currentpage}

Specifies the current page to display at load time.

#### Default Value
{:.param}

* 1


#### Example
{:.example}


{% highlight html %}
 
<div id="treegrid"></div> 
<script>                  
        $("#treegrid").ejTreeGrid({  
                        pageSettings:{currentPage : 2}
                });
</script>               

{% endhighlight %}

### pageSettings.pageSizeMode `enum`
{:#members:pagesettings-pagesizemode}

<ts name = "ej.TreeGrid.PageSizeMode"/>

Specifies the mode of record count in a page, whether it should count all the records or the root to count zero level parent records.  

<table class="params">
<thead>
<tr>
<th>Name</th>
<th>Description</th>
</tr>
</thead>
<tbody>
<tr>
<td class="name">All</td>
<td class="description">To count all the parent and child records.</td>
</tr>
<tr>
<td class="name">Root</td>
<td class="description">To count the Zeroth level parent records.</td>
</tr>
</tbody>
</table>

#### Default Value

* ej.TreeGrid.PageSizeMode.All


#### Example


{% highlight html %}
          
        $("#treegrid").ejTreeGrid({ pageSettings :{ pageSizeMode:ej.TreeGrid.PageSizeMode.Root } });                   

{% endhighlight %}


### pageSettings.printMode `enum`
{:#members:pagesettings-printmode}

<ts name = "ej.TreeGrid.PrintMode"/>

Specifies the mode of printing the control, whether it should print the all the records or the current page content.  

<table class="params">
<thead>
<tr>
<th>Name</th>
<th>Description</th>
</tr>
</thead>
<tbody>
<tr>
<td class="name">AllPages</td>
<td class="description">To print all the pages</td>
</tr>
<tr>
<td class="name">CurrentPage</td>
<td class="description">To print only the current page content.</td>
</tr>
</tbody>
</table>

#### Default Value

* ej.TreeGrid.PrintMode.AllPages


#### Example


{% highlight html %}
          
        $("#treegrid").ejTreeGrid({ pageSettings :{ printMode:ej.TreeGrid.PrintMode.CurrentPage} });                   

{% endhighlight %}

### pageSettings.template `string`
{:#members:pagesettings-template}

Specifies the Custom template for Pager control.


#### Default Value

* null


#### Example


{% highlight html %}
                  
        $("#treegrid").ejTreeGrid({ pageSettings :{ template:"PageTemplate" }});        

{% endhighlight %}

### cellTooltipTemplate `string`
{:#members:celltooltiptemplate}

Specifies the template for cell tooltip


#### Default Value

* null


#### Example


{% highlight html %}
                  
        $("#treegrid").ejTreeGrid({ cellTooltipTemplate : "CellTooltipTemplate"});        

{% endhighlight %}


### query `object`
{:#members:query}

Specifies ej.Query to select data from the dataSource. This property is applicable only when the dataSource is ej.DataManager.


#### Default Value

* null


#### Example


{% highlight html %}
                          
        $("#treegrid").ejTreeGrid(
 {
    query:ej.Query().from("Categories").select("CategoryID,CategoryName").take(3);      
 });            

{% endhighlight %}


### rowHeight `number`
{:#members:rowheight}

Specifies the height of a single row in tree grid. Also, we need to set same height in the CSS style with class name e-rowcell.


#### Default Value

* 30


#### Example


{% highlight html %}
                          
        $("#treegrid").ejTreeGrid({  
                        rowHeight : 30,
                        });
{% endhighlight %}



### rowTemplateID `string`
{:#members:rowtemplateid}

Specifies the id of the template to be applied for all the rows.


#### Default Value

* ""


#### Example


{% highlight html %}
                
        $("#treegrid").ejTreeGrid(
 {
    rowTemplateID: "customTemplate"
 });            

{% endhighlight %}


### selectedRowIndex `number`
{:#members:selectedrowindex}

Specifies the index of the selected row.


#### Default Value

* -1


#### Example


{% highlight html %}
                 
        $("#treegrid").ejTreeGrid(
 {
    selectedRowIndex:2
 });            

{% endhighlight %}

### selectedCellIndexes `array`
{:#members:selectedcellindexes}

Specifies the selected cell information on rendering TreeGrid.

### selectedCellIndexes.rowIndex `number`
{:#members:selectedcellindexes-rowIndex}


Specifies the row index of the cell to be selected in TreeGrid control


#### Default Value
{:.param}

* ""

### selectedCellIndexes.cellIndex `number`
{:#members:selectedcellindexes-cellIndex}

Specifies the cell index to be selected in the row.


#### Default Value
{:.param}

* " "

#### Example
{:.example}


{% highlight html %} 
                 
        $("#treegrid").ejTreeGrid({selectedCellIndexes:[{rowIndex: 2, cellIndex: 3}]});            

{% endhighlight %}

### selectionSettings `object`
{:#members:selectionsettings}

Specifies the settings for row and cell selection.

### selectionSettings.selectionMode `enum`
{:#members:selectionsettings-selectionmode}

<ts name = "ej.TreeGrid.SelectionMode"/>

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
{:.param}

* ej.TreeGrid.SelectionMode.Row

#### Example


{% highlight html %}
          
<div id="treegrid"></div> 
<script>   
         $("#treegrid").ejTreeGrid({ 
         selectionSettings:{selectionMode : ej.TreeGrid.SelectionMode.Row  }
         });   
</script>           

{% endhighlight %}


### selectionSettings.selectionType `enum`
{:#members:selectionsettings-selectiontype}

<ts name = "ej.TreeGrid.SelectionType"/>

Specifies the type of selection whether single, multiple or checkbox.

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
<tr>
<td class="name">Checkbox</td>
<td class="description">you can select rows using checkbox.</td>
</tr>
</tbody>
</table>

#### Default Value

* ej.TreeGrid.SelectionType.Single

#### Example

{% highlight html %}
          
        $("#treegrid").ejTreeGrid({ 
        selectionSettings:{selectionType : ej.TreeGrid.SelectionType.Multiple }
        });                   

{% endhighlight %}


### selectionSettings.enableHierarchySelection `boolean`
{:#members:selectionsettings-enablehierarchyselection}

Enables or disables the selection by hierarchy in check box selection

#### Default Value
{:.param}

* true

#### Example


{% highlight html %}
          
<div id="treegrid"></div> 
<script>   
        $("#treegrid").ejTreeGrid({ 
         selectionSettings:{enableHierarchySelection : false }
         });                      
</script>           

{% endhighlight %}


### selectionSettings.enableSelectAll `boolean`
{:#members:selectionsettings-enableselectall}

Toggles the visibility of the checkbox in column header, using which all the check boxes can be selected or unselected.

#### Default Value

* true

#### Example

{% highlight html %}
          
        $("#treegrid").ejTreeGrid({ 
        selectionSettings:{enableSelectAll : false }
        });                   

{% endhighlight %}

### showColumnOptions `boolean`
{:#members:showcolumnoptions}

Enables/disables the options for inserting , deleting and renaming  columns.

#### Default Value
{:.param}

* false

#### Example
{:.example}


{% highlight html %}
 
<div id="treegrid"></div> 
<script>   
        $("#treegrid").ejTreeGrid({ showColumnOptions:  true });                      * 
</script>

{% endhighlight %}


### showColumnChooser `boolean`
{:#members:showcolumnchooser}

Controls the visibility of the menu button, which is displayed on the column header. Clicking on this button will show a popup menu. When you choose `Columns` item from this popup, a list box with column names will be shown, from which you can select/deselect a column name to control the visibility of the respective columns.


#### Default Value
{:.param}
* false


#### Example


{% highlight html %}
 
  
        $("#treegrid").ejTreeGrid({ showColumnChooser:  true });      
        
{% endhighlight %}

### showDetailsRow `boolean`
{:#members:showdetailsrow}

Specifies the visibility of details view


#### Default Value
{:.param}
* false


#### Example


{% highlight html %}
                 
$("#treegrid").ejTreeGrid({
    showDetailsRow: true
});

{% endhighlight %}

### showDetailsRowInfoColumn `boolean`
{:#members:showdetailsrowinfocolumn}

Specifies the visibility of the expander column which is used to expand or collapse the details view


#### Default Value
{:.param}
* false


#### Example


{% highlight html %}
                 
$("#treegrid").ejTreeGrid({
    showDetailsRowInfoColumn: true
});

{% endhighlight %}

### detailsTemplate `string`
{:#members:detailstemplate}

Specifies the template for details view


#### Default Value
{:.param}
* ""


#### Example


{% highlight html %}
                 
$("#treegrid").ejTreeGrid({
    detailsTemplate: "#detailsTemplate"
});

{% endhighlight %}

### detailsRowHeight `number`
{:#members:detailsrowheight}

Specifies the row height of the details view


#### Default Value
{:.param}
* 100

#### Example

{% highlight html %}
                 
$("#treegrid").ejTreeGrid({
    detailsRowHeight: "150",
});

{% endhighlight %}

### showStackedHeader `boolean`
{:#members:showstackedheader}

Gets or sets a value that indicates stacked header should be shown on TreeGrid layout when the property &ldquo;stackedHeaderRows&rdquo; is set.

#### Default Value:
{:.param}
* false

#### Example
{:.example}
{% highlight html %}  

<div id="treeGrid"></div> 
<script>
$("#treeGrid").ejTreeGrid({
   showStackedHeader:true,
   stackedHeaderRows:
   [{
          stackedHeaderColumns: [
                  { column: "ID,Name,category,units", headerText: "Shipment details", cssClass: "temp" },
                  { column: "unitPrice,price", headerText: "Price details" }
           ]    
   ]},          
   columns: [
       { field: "ID", headerText: "S.No", width: columnWidth },
                    { field: "Name", headerText: "Shipment Name", isFrozen:true },
                    { field: "category", headerText: "Category" },
                    { field: "units", headerText: "Units" },
                    { field: "unitPrice", headerText: "Unit Price($)" },
                    { field: "price", headerText: "Price($)" }
      ]
});
</script> 

{% endhighlight %}

### stackedHeaderRows `array`
{:#members:stackedheaderrows}

Gets or sets an object that indicates to managing the collection of stacked header rows for the treegrid.

#### Default Value:
{:.param}
* []

#### Example
{:.example}
{% highlight html %}  
<div id="treeGrid"></div> 
<script>
$("#treeGrid").ejTreeGrid({
   showStackedHeader:true,
   stackedHeaderRows:
   [{
          stackedHeaderColumns: [
                  { column: "ID,Name,category,units", headerText: "Shipment details", cssClass: "temp" },
                  { column: "unitPrice,price", headerText: "Price details" }
           ]    
   ]},          
   columns: [
       { field: "ID", headerText: "S.No", width: columnWidth },
                    { field: "Name", headerText: "Shipment Name", isFrozen:true },
                    { field: "category", headerText: "Category" },
                    { field: "units", headerText: "Units" },
                    { field: "unitPrice", headerText: "Unit Price($)" },
                    { field: "price", headerText: "Price($)" }
      ]
});
</script> 
{% endhighlight %}

### stackedHeaderRows.stackedHeaderColumns `array`
{:#members:stackedheaderrows-stackedheadercolumns}

Gets or sets a value that indicates whether to add stacked header columns into the stacked header rows

#### Default Value:
{:.param}
* []

#### Example
{:.example}
{% highlight html %}  
<div id="treeGrid"></div> 
<script>
$("#treeGrid").ejTreeGrid({
   showStackedHeader:true,
   stackedHeaderRows:
   [{
          stackedHeaderColumns: [
                  { column: "ID,Name,category,units", headerText: "Shipment details", cssClass: "temp" },
                  { column: "unitPrice,price", headerText: "Price details" }
           ]    
   ]},       
});
</script> 
{% endhighlight %}

### stackedHeaderRows.stackedHeaderColumns.column `object`
{:#members:stackedheaderrows-stackedheadercolumns-column}

Gets or sets a value that indicates the header text for the particular stacked header column.

#### Default Value:
{:.param}
* null

#### Example
{:.example}
{% highlight html %}  
<div id="treeGrid"></div> 
<script>
$("#treeGrid").ejTreeGrid({
   showStackedHeader:true,
   stackedHeaderRows:
   [{
          stackedHeaderColumns: [
                  { column: "ID,Name,category,units", headerText: "Shipment details", cssClass: "temp" },
                  { column: "unitPrice,price", headerText: "Price details" }
           ] 
   ]},       
});
</script> 
{% endhighlight %}

### stackedHeaderRows.stackedHeaderColumns.cssClass `string`
{:#members:stackedheaderrows-stackedheadercolumns-cssclass}

Gets or sets a value that indicates class to the corresponding stackedHeaderColumn.

#### Default Value:
{:.param}
* null

#### Example
{:.example}
{% highlight html %}  
<div id="treeGrid"></div> 
<script>
$("#treeGrid").ejTreeGrid({
   showStackedHeader:true,
   stackedHeaderRows:
   [{
          stackedHeaderColumns: [
                  { column: "ID,Name,category,units", headerText: "Shipment details", cssClass: "temp" },
                  { column: "unitPrice,price", headerText: "Price details" }
           ]   
   ]},       
});
</script> 

{% endhighlight %}

### stackedHeaderRows.stackedHeaderColumns.headerText `string`
{:#members:stackedheaderrows-stackedheadercolumns-headertext}

Gets or sets a value that indicates the header text for the particular stacked header column.

#### Default Value:
{:.param}
* null

#### Example
{:.example}
{% highlight html %}  
<div id="treeGrid"></div> 
<script>
$("#treeGrid").ejTreeGrid({
   showStackedHeader:true,
   stackedHeaderRows:
   [{
           stackedHeaderColumns: [
                  { column: "ID,Name,category,units", headerText: "Shipment details" },
                  { column: "unitPrice,price", headerText: "Price details" }
           ]  
   ]},       
});
</script> 
{% endhighlight %}

### stackedHeaderRows.stackedHeaderColumns.textAlign `string`
{:#members:stackedheaderrows-stackedheadercolumns-textalign}

Gets or sets a value that indicates the text alignment of the corresponding headerText.

#### Default Value:
{:.param}
* ej.TextAlign.Left

#### Example
{:.example}
{% highlight html %}  

<div id="treeGrid"></div> 
<script>
$("#treeGrid").ejTreeGrid({
   showStackedHeader:true,
   stackedHeaderRows:
   [{
           stackedHeaderColumns: [
                  { column: "ID,Name,category,units", headerText: "Shipment details", textAlign: ej.TextAlign.Right },
                  { column: "unitPrice,price", headerText: "Price details" }
           ]  
   ]},       
});
</script> 

{% endhighlight %}

### stackedHeaderRows.stackedHeaderColumns.tooltip `string`
{:#members:stackedheaderrows-stackedheadercolumns-tooltip}

Sets the template for tooltip for the Grid stackedHeaderColumns.

#### Default Value:
{:.param}
* null

#### Example
{:.example}
{% highlight html %}  

<script type="text/template" id="colTip">
  {{:value }}
</script>

<div id="treeGrid"></div> 
<script>
$("#treeGrid").ejTreeGrid({
   showStackedHeader:true,
   stackedHeaderRows:
   [{
           stackedHeaderColumns: [
                  { column: "ID,Name,category,units", headerText: "Shipment details", tooltip:"#colTip" },
                  { column: "unitPrice,price", headerText: "Price details" }
           ] 
   ]},       
});
</script> 

{% endhighlight %}

### searchSettings `object`
{:#members:searchsettings}

Specifies the toolbar searching customizations.

### searchSettings.fields `array`
{:#members:searchsettings-fields}
Gets or Sets a specific column for searching the tree grid content.

#### Default Value

* []

#### Example

{% highlight html %}
                 
$("#treegrid").ejTreeGrid({
    searchSettings: {
            fields:["TaskId","TaskName"],
    }
});
{% endhighlight %}

### searchSettings.key `string`
{:#members:searchsettings-key}
Gets or Sets a key word for searching the tree grid content.

#### Default Value

* ""

#### Example

{% highlight html %}
                 
$("#treegrid").ejTreeGrid({
    searchSettings: {
            key:"task 1",
    }
});
{% endhighlight %}

### searchSettings.operator `string`
{:#members:searchsettings-operator}

Specifies the operator for the search key words in toolbar searching.

**List of enum type operators**

1. ej.FilterOperators.contain
2. ej.FilterOperators.equal
3. ej.FilterOperators.notEqual
4. ej.FilterOperators.startsWith
5. ej.FilterOperators.endsWith

#### Default Value

* "contains"

#### Example

{% highlight html %}
                 
$("#treegrid").ejTreeGrid({
    searchSettings: {
            operator:"startsWith",
    }
});
{% endhighlight %}

### searchSettings.ignoreCase `boolean`
{:#members:searchsettings-ignorecase}
Enables or disables the case sensitivity while searching.

#### Default Value

* true

#### Example

{% highlight html %}
                 
$("#treegrid").ejTreeGrid({
    searchSettings: {
            ignoreCase:false,
    }
});
{% endhighlight %}

### showSummaryRow `boolean`
{:#members:showsummaryrow}

Specifies the visibility of summary row

#### Default Value
{:.param}
* false

#### Example

{% highlight html %}
                 
$("#treegrid").ejTreeGrid({
    showSummaryRow: true
});
{% endhighlight %}

### showTotalSummary `boolean`
{:#members:showtotalsummary}

Specifies the visibility of total summary row for the corresponding summary column

#### Default Value
{:.param}
* false

#### Example

{% highlight html %}
                 
$("#treegrid").ejTreeGrid({
    showTotalSummary: true
});
{% endhighlight %}

### summaryRows `array`
{:#members:summaryrows}

Specifies the summary row collection object to be displayed

#### Default Value
{:.param}
* []

### summaryRows.title `string`
{:#members:summaryrows-title}

Specifies the title for summary row collection in TreeGrid

#### Default Value
{:.param}
* -

### summaryRows.summaryColumns `array`
{:#members:summaryrows-summarycolumns}

Specifies the summary columns in the summary rows.

#### Default Value
{:.param}
* -

### summaryRows.summaryColumns.summaryType `enum`
{:#members:summaryrows-summarycolumns-summarytype}

<ts name = "ej.TreeGrid.SummaryType"/>

Specifies the summary type to perform calculations in a corresponding summary column. See <a href="global.html#enum:summarytype">summaryType</a>.

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
<td class="description">Displays the sum of summary column</td>
</tr>
<tr>
<td class="name">Average</td>
<td class="description">Displays the average of summary column</td>
</tr>
<tr>
<td class="name">Maximum</td>
<td class="description">Displays the maximum value of summary column</td>
</tr>
<tr>
<td class="name">Minimum</td>
<td class="description">Displays the minimum value of summary column</td>
</tr>
<tr>
<td class="name">Count</td>
<td class="description">Displays the total count of summary column</td>
</tr>
<tr>
<td class="name">MinimumDate</td>
<td class="description">Displays the minimum date value in summary column</td>
</tr>
<tr>
<td class="name">MaximumDate</td>
<td class="description">Displays the maximum date value in summary column</td>
</tr>
<tr>
<td class="name">TrueCount</td>
<td class="description">Displays the true count value for boolean summary columns</td>
</tr>
<tr>
<td class="name">FalseCount</td>
<td class="description">Displays the false count value for boolean summary columns</td>
</tr>
</tbody>
</table>

#### Default Value
{:.param}
* -

### summaryRows.summaryColumns.dataMember `string`
{:#members:summaryrows-summarycolumns-datamember}

Specifies summary column used to perform the summary calculation.

#### Default Value
{:.param}
* -

### summaryRows.summaryColumns.displayColumn `string`
{:#members:summaryrows-summarycolumns-displaycolumn}

Specifies the required column to display the summary.

#### Default Value
{:.param}
* -

### summaryRows.summaryColumns.prefix `string`
{:#members:summaryrows-summarycolumns-prefix}

Specifies the text to be displayed before the summary column value.

#### Default Value
{:.param}
* -

### summaryRows.summaryColumns.suffix `string`
{:#members:summaryrows-summarycolumns-suffix}

Specifies the text to be displayed after the summary column value.

#### Default Value
{:.param}
* -

### summaryRows.summaryColumns.format `string`
{:#members:summaryrows-summarycolumns-format}

Specifies the format to be applied on the summary column value.

#### Default Value
{:.param}
* -

#### Example

{% highlight html %}
                 
$("#treegrid").ejTreeGrid({
    summaryRows: [{
        title: "Maximum",
        summaryColumns: [{
            summaryType: ej.TreeGrid.SummaryType.Maximum,
            dataMember: "TotalUnits",
            displayColumn: "TotalUnits",
            prefix: "Individual maximum unit = ",
        }, {
            summaryType: ej.TreeGrid.SummaryType.Maximum,
            dataMember: "TotalCosts",
            displayColumn: "TotalCosts",
            prefix: "Individual maximum Cost = ",
			suffix:"/-",
            format: "{0:C}"
        }]
    }, ],
});
{% endhighlight %}

### showGridCellTooltip `boolean`
{:#members:showgridcelltooltip}

Specifies whether to show tooltip when mouse is hovered on the cell.


#### Default Value
{:.param}
* true


#### Example


{% highlight html %}
                 
$("#treegrid").ejTreeGrid({
    showGridCellTooltip: true
});
{% endhighlight %}


### showGridExpandCellTooltip `boolean`
{:#members:showgridexpandcelltooltip}

Specifies whether to show tooltip for the cells, which has expander button.


#### Default Value
{:.param}
* true


#### Example


{% highlight html %}
                  
$("#treegrid").ejTreeGrid({
    showGridExpandCellTooltip: true
});
{% endhighlight %}


### sizeSettings `object`
{:#members:sizesettings}

Options for setting width and height for TreeGrid.


### sizeSettings.height `string`
{:#members:sizesettings-height}

Height of the TreeGrid.


#### Default Value
{:.param}
* null


#### Example


{% highlight html %}
          
        $("#treegrid").ejTreeGrid({sizeSettings{height:'450px'}});

{% endhighlight %}


### sizeSettings.width `string`
{:#members:sizesettings-width}

Width of the TreeGrid.


#### Default Value
{:.param}

* null


#### Example


{% highlight html %}
          
        $("#treegrid").ejTreeGrid({sizeSettings{width:'500px'}});

{% endhighlight %}


### sortSettings `object`
{:#members:sortsettings}

Options for sorting the rows.


### sortSettings.sortedColumns `array`
{:#members:sortsettings-sortedcolumns}

Option to add columns based on which the rows have to be sorted recursively.


#### Default Value
{:.param}
* []


#### Example


{% highlight html %}
          
        $("#treegrid").ejTreeGrid({ sortSettings:{sortedColumns : [{ field:"startDate",direction:"ascending" }]}});      

{% endhighlight %}

### sortSettings.sortedColumns.field `string`
{:#members:sortsettings-sortedcolumns-field}

Specifies the field to be sorted in TreeGrid


#### Default Value
{:.param}

* ""


#### Example
{:.example}


{% highlight html %}
        
        $("#treegrid").ejTreeGrid({ sortSettings:{sortedColumns : [{ field:"startDate" }]}});                

{% endhighlight %}

### sortSettings.sortedColumns.direction `string`
{:#members:sortsettings-sortedcolumns-direction}

Specifies the sort direction in TreeGrid


#### Default Value
{:.param}

* ""


#### Example
{:.example}


{% highlight html %}
 
    $("#treegrid").ejTreeGrid({ sortSettings:{sortedColumns : [{ direction:"ascending" }]}});                  

{% endhighlight %}


### toolbarSettings `object`
{:#members:toolbarsettings}

Options for displaying and customizing the toolbar items.


### toolbarSettings.showToolbar `boolean`
{:#members:toolbarsettings-showtoolbar}

Shows/hides the toolbar.


#### Default Value
{:.param}
* false


#### Example


{% highlight html %}
   
        $("#treegrid").ejTreeGrid({ showToolbar:  true });                       

{% endhighlight %}


### toolbarSettings.toolbarItems `array`
{:#members:toolbarsettings-toolbaritems}

Specifies the list of toolbar items to be rendered in TreeGrid toolbar

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
<td class="name">ExpandAll</td>
<td class="description">Enables the expand all icon in toolbar</td>
</tr>
<tr>
<td class="name">Collapse All</td>
<td class="description">Enables the collapse all icon in toolbar</td>
</tr>
<tr>
<td class="name">PdfExport</td>
<td class="description">Enables the PDF export icon in toolbar</td>
</tr>
<tr>
<td class="name">ExcelExport</td>
<td class="description">Enables the excel export icon in toolbar</td>
</tr>
<tr>
<td class="name">Print</td>
<td class="description">Enables the printing icon in toolbar</td>
</tr>
</tbody>
</table>

#### Default Value
{:.param}
* []


#### Example


{% highlight html %}
 
        $("#treegrid").ejTreeGrid({ toolbarItems: [ej.TreeGrid.ToolbarItems.Add,ej.TreeGrid.ToolbarItems.Edit] });                       

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
                 
        $("#treegrid").ejTreeGrid({toolbarSettings: {customToolbarItems: [{ text: "Reset",tooltipText:"Column Visibility" }]}});

{% endhighlight %}


### toolbarSettings.customToolbarItems.templateID `string`
{:#members:toolbarsettings-customtoolbaritems-templateid}

Allows the user to insert the custom icons in toolbar using script templates. Using this property we can bind HTML elements and other EJ controls to TreeGrid toolbar.


#### Default Value

* ""


#### Example


{% highlight html %}

         $("#treegrid").ejTreeGrid({toolbarSettings: {customToolbarItems: [{ templateID: "#ColumnVisibility",tooltipText:"Column Visibility" }]}});                     

{% endhighlight %}


### toolbarSettings.customToolbarItems.tooltipText `string`
{:#members:toolbarsettings-customtoolbaritems-tooltiptext}

Allows the user to display custom tooltip text for TreeGrid custom toolbar items.


#### Default Value

* ""


#### Example


{% highlight html %}
                  
        $("#treegrid").ejTreeGrid({toolbarSettings: {customToolbarItems: [{ templateID: "#ColumnVisibility",tooltipText:"Column Visibility" },{ text: "Reset",tooltipText:"Column Visibility" }]}});     

{% endhighlight %}


### treeColumnIndex `number`
{:#members:treecolumnindex}

Specifies the index of the column that needs to have the expander button. By default, cells in the first column contain the expander button.


#### Default Value
{:.param}
* 0


#### Example


{% highlight html %}
         
        $("#treegrid").ejTreeGrid(
 {
    treeColumnIndex: 1
 });            

{% endhighlight %}



## Methods

### addRow(data, rowPosition)
{:#methods:addrow}

Add a new row in TreeGrid, while allowAdding is set to true

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
<td class="description">Item to add in TreeGrid row.</td>
</tr>
<tr>
<td class="name">rowPosition</td>
<td class="type">string</td>
<td class="description">Defines in which position the row wants to be added</td>
</tr>
</tbody>
</table>


#### Example


{% highlight html %}
 
<div id="treegrid"></div> 
 
<script>
// Create TreeGrid object
var treeGridObj = $("#treegrid").data("ejTreeGrid");
var data = {taskId:"40",taskName:"New Task 40",startDate:"2/20/2014",startDate:"2/25/2014"};
treeGridObj.addRow(data, ej.TreeGrid.RowPosition.Child); // To add a task
</script>
{% endhighlight %}


### clearSelection(index)
{:#methods:clearselection}

To clear all the selection in TreeGrid

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
<td class="description">you can pass a row index to clear the row selection.</td>
</tr>
</tbody>
</table>

#### Example


{% highlight html %}
 
<div id="treegrid"></div> 
<script>
// Create Tree Grid object
var treegridObj = $("#treegrid").data("ejTreeGrid");
treegridObj.clearSelection(2);
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
<td class="description">Defines that we need to preserve the previously selected cells or not</td>
</tr>
</tbody>
</table>


#### Example


{% highlight html %}
 
<div id="treegrid"></div> 
 
<script>
// Create treegrid
var treegridObj = $("#treegrid").data("ejTreeGrid");
var indexes = [{rowIndex:4, cellIndex: 4}, {rowIndex: 3, cellIndex: 3}];
treegridObj.selectCells(indexes, true); // To add a task
</script>
{% endhighlight %}

### renameColumn(columnIndex,name)
{:#methods:renamecolumn}

To rename a column with the specified name

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
<td class="name">columnIndex</td>
<td class="type">number</td>
<td class="description">Index of the column to be renamed</td>
</tr>
<tr>
<td class="name">name</td>
<td class="type">string</td>
<td class="description">Header text of the column </td>
</tr>
</tbody>
</table>


#### Example


{% highlight html %}
 
<div id="treegrid"></div> 
 
<script>
// Create treegrid
var treegridObj = $("#treegrid").data("ejTreeGrid");
treegridObj.renameColumn(1, "New Text"); // To re name the column
</script>
{% endhighlight %}

### deleteColumn(columnIndex)
{:#methods:deletecolumn}

To delete the specified column

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
<td class="name">columnIndex</td>
<td class="type">number</td>
<td class="description">Index of the column to be deleted</td>
</tr>
</tbody>
</table>


#### Example


{% highlight html %}
 
<div id="treegrid"></div> 
 
<script>
// Create treegrid
var treegridObj = $("#treegrid").data("ejTreeGrid");
treegridObj.deleteColumn(1); // To delete the specified column
</script>
{% endhighlight %}

### collapseAll()
{:#methods:collapseall}

To collapse all the parent items in tree grid

#### Example

{% highlight html %}
 
<div id="treegrid"></div> 
 
<script>
// Create Tree Grid object
var treegridObj = $("#treegrid").data("ejTreeGrid");
treegridObj.collapseAll(); // To collapse all parent items in tree grid
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
<td class="description">you can pass a header text of a column to hide.</td>
</tr>
</tbody>
</table>


#### Example



{% highlight html %}
 
<div id="treegrid"></div> 
 
<script>
// Create Tree Grid object
var treegridObj = $("#treegrid").data("ejTreeGrid");
treegridObj.hideColumn("Task Name");
</script> 

{% endhighlight %}

### expandAtLevel(index)
{:#methods:expandatlevel}

Expands the records at specific hierarchical level

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
<td class="description">you can pass the level as index number to expand</td>
</tr>
</tbody>
</table>

#### Example

{% highlight html %}
 
<div id="treegrid"></div> 
 
<script>
// Create Tree Grid object
var treegridObj = $("#treegrid").data("ejTreeGrid");
treegridObj.expandAtLevel(2);
</script> 

{% endhighlight %}

### collapseAtLevel(index)
{:#methods:collapseatlevel}

Collapses the records at specific hierarchical level

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
<td class="description">you can pass the particular level as index.</td>
</tr>
</tbody>
</table>

#### Example

{% highlight html %}
 
<div id="treegrid"></div> 
 
<script>
// Create Tree Grid object
var treegridObj = $("#treegrid").data("ejTreeGrid");
treegridObj.collapseAtLevel(2);
</script> 

{% endhighlight %}

### refresh(dataSource, query)
{:#methods:refresh}

To refresh the changes in tree grid

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
<td class="name">dataSource</td>
<td class="type">array</td>
<td class="description">Pass which data source you want to show in tree grid</td>
</tr>
<tr>
<td class="name">query</td>
<td class="type">object</td>
<td class="description">Pass which data you want to show in tree grid</td>
</tr>
</tbody>
</table>


#### Example



{% highlight html %}
 
<div id="treegrid"></div> 
 
<script>
// Create treegrid object
var treegridObj = $("#treegrid").data("ejTreeGrid");
var dataManager = ej.DataManager(projectData);
var query = ej.Query().select(["taskID", "taskName", "startDate", "endDate", "subtasks", "progress", "duration"]);
treegridObj.refresh(dataManager, query) // To refresh the tree grid content
</script>
{% endhighlight %}



### freezePrecedingColumns (field)
{:#methods:freezeprecedingcolumns}

Freeze all the columns preceding to the column specified by the field name.

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
<td class="name">field</td>
<td class="type">string</td>
<td class="description">Freeze all Columns before this field column.</td>
</tr>
</tbody>
</table>

#### Example

{% highlight html %}
 
<div id="treegrid"></div> 
 
<script>
// Create Tree Grid object
var treegridObj = $("#treegrid").data("ejTreeGrid");
treegridObj.freezePrecedingColumns(field); 
</script>
{% endhighlight %}


### freezeColumn (field, isFrozen)
{:#methods:freezecolumn}

Freeze/unfreeze the specified column.

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
<td class="name">field</td>
<td class="type">string</td>
<td class="description">Freeze/Unfreeze this field column.</td>
</tr>
<tr>
<td class="name">isFrozen</td>
<td class="type">boolean</td>
<td class="description">Decides to Freeze/Unfreeze this field column.</td>
</tr>
</tbody>
</table>

#### Example

{% highlight html %}
 
<div id="treegrid"></div> 
 
<script>
// Create Tree Grid object
var treegridObj = $("#treegrid").data("ejTreeGrid");
treegridObj.freezeColumn(field, isFrozen); 
</script>
{% endhighlight %}


### saveCell()
{:#methods:savecell}

To save the edited cell in TreeGrid


#### Example


{% highlight html %}
 
<div id="treegrid"></div> 
 
<script>
// Create Tree Grid object
var treegridObj = $("#treegrid").data("ejTreeGrid");
treegridObj.saveCell(); 
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
<td class="description">you can pass a header text of a column to show.</td>
</tr>
</tbody>
</table>


#### Example



{% highlight html %}
 
<div id="treegrid"></div> 
 
<script>
// Create Tree Grid object
var treegridObj = $("#treegrid").data("ejTreeGrid");
treegridObj.showColumn("Task Name");
</script> 

{% endhighlight %}


### sortColumn(fieldName, columnSortDirection)
{:#methods:sortcolumn}

To sorting the data based on the particular fields

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
<td class="description">you can pass a name of column to sort.</td>
</tr>
<tr>
<td class="name">columnSortDirection</td>
<td class="type">string</td>
<td class="description">you can pass a sort direction to sort the column.</td>
</tr>
</tbody>
</table>


#### Example



{% highlight html %}
 
<div id="treegrid"></div> 
 
<script>
// Create Tree Grid object
var treegridObj = $("#treegrid").data("ejTreeGrid");
treegridObj.sortColumn("Start Date", ej.sortOrder.Descending); // To sort the data
</script>
{% endhighlight %}

### reorderColumn(fieldName, targetIndex)
{:#methods:reordercolumn}

To reorder the column with field name and target index values

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
<td class="description">you can pass a name of column to reorder.</td>
</tr>
<tr>
<td class="name">targetIndex</td>
<td class="type">string</td>
<td class="description">you can pass a target column index to be inserted.</td>
</tr>
</tbody>
</table>


#### Example



{% highlight html %}
 
<div id="treegrid"></div> 
 
<script>
// Create Tree Grid object
var treegridObj = $("#treegrid").data("ejTreeGrid");
treegridObj.reorderColumn("startDate", 4); // To sort the data
</script>
{% endhighlight %}

### getUpdatedRecords()
{:#methods:getupdatedrecords}

To get the updated data source of TreeGrid.

#### Returns:
{:#methods:returns:}

array

Usage: We can able to get the updated record collection by using this method.

#### Example

{% highlight html %}
  
<div id="TreeGridContainer"></div> 
 
<script>
// Create TreeGrid object.
var treeObject = $("#TreeGridContainer").data("ejTreeGrid");
// Gets the updated data source collection of TreeGrid
treeObject.getUpdatedRecords();
</script>
{% endhighlight %}

Demo [Link](http://jsplayground.syncfusion.com/cxcfhp5i)

### gotoPage(pageIndex)
{:#methods:gotopage}

Sends request to navigate to a specific page in TreeGrid.

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
<td class="name">PageIndex</td>
<td class="type">number</td>
<td class="description">Pass the page index to perform paging at specified page index.</td>
</tr>
</tbody>
</table>

Usage: we can able to change the active page at run time.

#### Example


{% highlight html %}
  
<div id="TreeGridContainer"></div> 
 
<script>
// Create TreeGrid object.
var treeObject = $("#TreeGridContainer").data("ejTreeGrid");
// Sends a paging request to the TreeGrid with specified page index
treeObject.gotoPage(3);
</script>

{% endhighlight %}

Demo [Link](http://jsplayground.syncfusion.com/we1l1qkr)

### updateCheckboxColumn(fieldName)
{:#methods:updatecheckboxcolumn}

To change the checkbox selection to any column. 

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
<td class="description">Pass the column field name to check box selection to that column.</td>
</tr>
</tbody>
</table>

Usage: we can able to change the selection checkbox column dynamically.

#### Example


{% highlight html %}
  
<div id="TreeGridContainer"></div> 
 
<script>
// Create TreeGrid object.
var treeObject = $("#TreeGridContainer").data("ejTreeGrid");
// Sends a column fieldname to change the checkbox selection to that column.
treeObject.updateCheckboxColumn('taskName');
</script>

{% endhighlight %}

Demo [Link](http://jsplayground.syncfusion.com/2b0p5ytm)

### getSelectedCells()
{:#methods:getselectedcells}

Gets the selected cell(s) element details in TreeGrid. 

#### Returns:
{:#methods:returns:}

array

Usage: we can able to get cell elements of selected cells for further processing.

#### Example


{% highlight html %}
  
<div id="TreeGridContainer"></div> 
 
<script>
// Create TreeGrid object.
var treeObject = $("#TreeGridContainer").data("ejTreeGrid");
// Gets the selected cell element list
treeObject.getSelectedCells();
</script>
{% endhighlight %}

Demo [Link](http://jsplayground.syncfusion.com/aovokclp)

### updateResponsiveMinWidth(width)
{:#methods:updateresponsiveminwidth}

Sets the minimum responsive width for TreeGrid.

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
<td class="type">String</td>
<td class="description">Pass the minimum responsive width, above which the TreeGrid needs to work in responsive mode.</td>
</tr>
</tbody>
</table>


Usage: we can able to change the minimum responsive width of TreeGrid dynamically.

#### Returns

{:#methods:returns:}

void

#### Example


{% highlight html %}
  
<div id="TreeGridContainer"></div> 
 
<script>
// Create TreeGrid object.
var treeObject = $("#TreeGridContainer").data("ejTreeGrid");
// Sends the minimum width in pixel to make the TreeGrid to behave as responsive above this width.
treeObject.updateResponsiveMinWidth("200px");
</script>

{% endhighlight %}

Demo [Link](http://jsplayground.syncfusion.com/edphz55n)

### showAddDialog()
{:#methods:showadddialog}

To open the dialog to add new record/row in TreeGrid.

Usage: we can able to open add dialog dynamically.

#### Example


{% highlight html %}
  
<div id="TreeGridContainer"></div> 
 
<script>
// Create TreeGrid object.
var treeObject = $("#TreeGridContainer").data("ejTreeGrid");
// Show Add dialog box to add new record.
treeObject.showAddDialog();
</script>

{% endhighlight %}

Demo [Link](http://jsplayground.syncfusion.com/4nwaeooa)

### showEditDialog(index)
{:#methods:showeditdialog}

To open the dialog to edit a row/record in TreeGrid.

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
<td class="name">Index</td>
<td class="type">number</td>
<td class="description">Pass the index of row to be edit.</td>
</tr>
</tbody>
</table>

Usage: we can able to edit any row dynamically through edit dialog. If the index value is not passed as parameter then the selected row gets edited. It’s necessary to select a row before opening edit dialog when you are not passing any index as parameter.

#### Example


{% highlight html %}
  
<div id="TreeGridContainer"></div> 
 
<script>
// Create TreeGrid object.
var treeObject = $("#TreeGridContainer").data("ejTreeGrid");
// Show edit dialog box to edit the row at index ‘3’.
treeObject.showEditDialog(3);
</script>

{% endhighlight %}

Demo [Link](http://jsplayground.syncfusion.com/i0ilxy1m)

### scrollOffset(left, top)
{:#methods:scrolloffset}

Sets the scroll left and scroll top offsets of TreeGrid.

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
<td class="name">Left</td>
<td class="type">String</td>
<td class="description">Pass a value to set left position of horizontal scroll bar.</td>
</tr>
<tr>
<td class="name">Top</td>
<td class="type">String</td>
<td class="description">Pass a value to set top position of vertical scroll bar.</td>
</tr>
</tbody>
</table>

Usage: we can able to change the left and top position of horizontal and vertical scroll bar dynamically.

#### Example


{% highlight html %}
  
<div id="TreeGridContainer"></div> 
 
<script>
// Create TreeGrid object.
var treeObject = $("#TreeGridContainer").data("ejTreeGrid");
// Set horizontal scroll bar left value and vertical scroll bar top value.
treeObject.scrollOffset(50,50);
</script>

{% endhighlight %}

Demo [Link](http://jsplayground.syncfusion.com/ukm0behc)

### getScrollTopOffset()
{:#methods:getscrolltopoffset}

Gets the scroll top offset of TreeGrid. 


#### Returns:
{:#methods:returns:}

number

Usage: we can able to get scroll top offset of TreeGrid dynamically.

#### Example

{% highlight html %}
  
<div id="TreeGridContainer"></div> 
 
<script>
// Create TreeGrid object.
var treeObject = $("#TreeGridContainer").data("ejTreeGrid");
//Get vertical scroll bar top value.
treeObject.getScrollTopOffset();
</script>
{% endhighlight %}

Demo [Link](http://jsplayground.syncfusion.com/t44osvai)

### getScrollLeftOffset()
{:#methods:getscrollleftoffset}

Gets the scroll left offset of TreeGrid. 

#### Returns:
{:#methods:returns:}

number

Usage: we can able to get scroll left offset of TreeGrid dynamically.

#### Example


{% highlight html %}
  
<div id="TreeGridContainer"></div> 
 
<script>
// Create TreeGrid object.
var treeObject = $("#TreeGridContainer").data("ejTreeGrid");
//Get horizontal scroll bar left value.
treeObject. getScrollLeftOffset()
</script>
{% endhighlight %}

Demo [Link](http://jsplayground.syncfusion.com/at3xgdb3)

### scrollToTop()
{:#methods:scrolltotop}

Sets the scroll top offset of TreeGrid to `0`.

Usage: we can able to scroll the TreeGrid's content to `0` offset vertically.

#### Example


{% highlight html %}
  
<div id="TreeGridContainer"></div> 
 
<script>
// Create TreeGrid object.
var treeObject = $("#TreeGridContainer").data("ejTreeGrid");
//Set Vertical scroll bar to zeroth position.
treeObject.scrollToTop();
</script>
{% endhighlight %}

Demo [Link](http://jsplayground.syncfusion.com/j4cxwi1h)

### scrollToBottom()
{:#methods:scrolltobottom}

Sets the scroll top offset of TreeGrid to maximum value. 

Usage:we can able to scroll the TreeGrid's content to the maximum offset vertically.

#### Example


{% highlight html %}
  
<div id="TreeGridContainer"></div> 
 
<script>
// Create TreeGrid object.
var treeObject = $("#TreeGridContainer").data("ejTreeGrid");
//Set Vertical scroll bar to end position.
treeObject. scrollToBottom()
</script>
{% endhighlight %}

Demo [Link](http://jsplayground.syncfusion.com/wmqgjqt0)

### expandCollapseRow(index)
{:#methods:expandcollapserow}

To expand and collapse an item in TreeGrid using item’s index.

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
<td class="name">Index</td>
<td class="type">number</td>
<td class="description">Pass the row index of row to expand/collapse.</td>
</tr>
</tbody>
</table>

Usage: we can able to expand/collapse any specific parent record dynamically by passing its row index.

#### Example


{% highlight html %}
  
<div id="TreeGridContainer"></div> 
 
<script>
// Create TreeGrid object.
var treeObject = $("#TreeGridContainer").data("ejTreeGrid");
// Show expand/collapse the parent record at index ‘5’.
treeObject.expandCollapseRow(5);
</script>

{% endhighlight %}

Demo [Link](http://jsplayground.syncfusion.com/upojiocv)

### expandAll()
{:#methods:expandall}

To expand all the root level nodes in TreeGrid.

Usage: we can able to expand all the parents records in TreeGrid control dynamically.

#### Example


{% highlight html %}
  
<div id="TreeGridContainer"></div> 
 
<script>
// Create TreeGrid object.
var treeObject = $("#TreeGridContainer").data("ejTreeGrid");
// To expand all the parent records.
treeObject.expandAll();
</script>
{% endhighlight %}

Demo [Link](http://jsplayground.syncfusion.com/uhhuxbm3)

### showHideDetailsRow(rowIndex)
{:#methods:showhidedetailsrow}

Show/Hide the detail row of a specific record.

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
<td class="name">rowIndex</td>
<td class="type">number</td>
<td class="description">Pass the row index of record to show/hide the detail row.</td>
</tr>
</tbody>
</table>

Usage: we can able to dynamically show/hide the detail row of any record by passing its index as parameter.

#### Example


{% highlight html %}
  
<div id="TreeGridContainer"></div> 
 
<script>
// Create TreeGrid object.
var treeObject = $("#TreeGridContainer").data("ejTreeGrid");
// Show the detail row of record at index ‘3’.
treeObject.showHideDetailsRow(3);
</script>

{% endhighlight %}

Demo [Link](http://jsplayground.syncfusion.com/jdi5qebc)

### filterColumn(fieldName, filterOperator, filterValue, predicate, match case, actualFilterValue)
{:#methods:filtercolumn}

Sends filtering request to filter a column in TreeGrid.

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
<td class="description">string/integer/dateTime operator.</td>
</tr>
<tr>
<td class="name">filterValue</td>
<td class="type">string</td>
<td class="description">Pass the value to be filtered in a column.</td>
</tr>
<tr>
<td class="name">predicate</td>
<td class="type">string</td>
<td class="description">Pass the predicate as and/or.</td>
</tr>
<tr>
<td class="name">match case</td>
<td class="type">boolean</td>
<td class="description">Optional pass the match case value as true/false.</td>
</tr>
<tr>
<td class="name">actualFilterValue</td>
<td class="type">object</td>
<td class="description">Optional actualFilterValue denote the filter object of current filtered columns. </td>
</tr>
</tbody>
</table>

Usage: we can able to perform filter operation dynamically.

#### Example


{% highlight html %}
  
<div id="TreeGridContainer"></div> 
 
<script>
// Create TreeGrid object.
var treeObject = $("#TreeGridContainer").data("ejTreeGrid");
// To filter taskName column with text starts with "plan".
treeObject.filterColumn("taskName", "startswith", "plan", "and");
</script>

{% endhighlight %}

Demo [Link](http://jsplayground.syncfusion.com/1u5o3ncv)

### columnIndex(index)
{:#methods:columnindex}

To change the index of the tree column in TreeGrid.

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
<td class="name">Index</td>
<td class="type">number</td>
<td class="description">Pass the column index to make the column as treeColumnIndex.</td>
</tr>
</tbody>
</table>

Usage: we can able to change any column as tree column dynamically. 

#### Example

{% highlight html %}
  
<div id="TreeGridContainer"></div> 
 
<script>
// Create TreeGrid object.
var treeObject = $("#TreeGridContainer").data("ejTreeGrid");
//Change second column as treeColumn.
treeObject.columnIndex(2);
</script>

{% endhighlight %}

Demo [Link](http://jsplayground.syncfusion.com/vvxsymxn)

### clearSorting()
{:#methods:clearsorting}

To clear the sorting from sorted columns in TreeGrid.

#### Example


{% highlight html %}
  
<div id="TreeGridContainer"></div> 
 
<script>
// Create TreeGrid object.
var treeObject = $("#TreeGridContainer").data("ejTreeGrid");
//Clear sorting from sorted column.
treeObject.clearSorting();
</script>

{% endhighlight %}

Demo [Link](http://jsplayground.syncfusion.com/nwig1elj)

### getColumnIndexByField(fieldName)
{:#methods:getcolumnindexbyfield}

Gets the column index of specific column with data source field.

#### Returns:
{:#methods:returns:}

number

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
<td class="description">Pass the column field name to get its index.</td>
</tr>
</tbody>
</table>

Usage: we can able to get the index of any column by passing its field name as parameter.

#### Example


{% highlight html %}
  
<div id="TreeGridContainer"></div> 
 
<script>
// Create TreeGrid object.
var treeObject = $("#TreeGridContainer").data("ejTreeGrid");
//get index of “taskName” column.
treeObject.getColumnIndexByField("taskName");
</script>

{% endhighlight %}

Demo [Link](http://jsplayground.syncfusion.com/1spkbqua)

### getFieldNameByHeaderText(headerText)
{:#methods:getfieldnamebyheadertext}

Gets the column field name using column header text.

#### Returns:
{:#methods:returns:}

string

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
<td class="description">Pass the column header text to get its field name.</td>
</tr>
</tbody>
</table>

Usage: we can able to get the field name of any column by passing its header text as parameter.

#### Example


{% highlight html %}
  
<div id="TreeGridContainer"></div> 
 
<script>
// Create TreeGrid object.
var treeObject = $("#TreeGridContainer").data("ejTreeGrid");
//get the field name of column having header text as “Task Name”.
treeObject.getFieldNameByHeaderText("Task Name");
</script>

{% endhighlight %}

Demo [Link](http://jsplayground.syncfusion.com/1spkbqua)

### getColumnByHeaderText(headerText)
{:#methods:getcolumnbyheadertext}

Gets the column object of specific column.

#### Returns:
{:#methods:returns:}

object

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
<td class="description">Pass the column header text to get details of that column.</td>
</tr>
</tbody>
</table>

Usage: we can able to get the object of any column by passing its header text as parameter.

#### Example


{% highlight html %}
  
<div id="TreeGridContainer"></div> 
 
<script>
// Create TreeGrid object.
var treeObject = $("#TreeGridContainer").data("ejTreeGrid");
 //get the details of column having header text as “Task Name”.
treeObject.getColumnByHeaderText("Task Name");
</script>

{% endhighlight %}

Demo [Link](http://jsplayground.syncfusion.com/jsc43oni)

### clearFilter(fieldName)
{:#methods:clearfilter}

Clears the filter applied to a specific column.

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
<td class="description">Pass the column field name to clear filtering done in that column.</td>
</tr>
</tbody>
</table>

Usage: we can able to clear the filtering done in any specific column dynamically by passing its field name as parameter.

#### Example


{% highlight html %}
  
<div id="TreeGridContainer"></div> 
 
<script>
// Create TreeGrid object.
var treeObject = $("#TreeGridContainer").data("ejTreeGrid");
//clear the filtering done in the “taskName” column
treeObject.clearFilter("taskName");
</script>

{% endhighlight %}

Demo [Link](http://jsplayground.syncfusion.com/1j2h0ylb)

### getColumnByField(fieldName)
{:#methods:getcolumnbyfield}

Gets the column object of specific column.

#### Returns:
{:#methods:returns:}

object

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
<td class="description">Pass the column field name to get details of that column.</td>
</tr>
</tbody>
</table>

Usage: we can able to get the detail collection of any column by passing its field name as parameter.

#### Example


{% highlight html %}
  
<div id="TreeGridContainer"></div> 
 
<script>
// Create TreeGrid object.
var treeObject = $("#TreeGridContainer").data("ejTreeGrid");
//get the details of column having fieldName as “taskName”.
treeObject. getColumnByField("taskName");
</script>

{% endhighlight %}

Demo [Link](http://jsplayground.syncfusion.com/g3lrtszu)

## Events

### actionBegin
{:#events:actionbegin}

Triggered before every success event of TreeGrid action.

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
<td class="description">Event parameters before completing the sorting operation in TreeGrid:
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
<td class="description">Returns the TreeGrid model.</td>
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
<td class="description">Returns the direction of sorting ascending or descending.</td>
</tr>
</tbody>
</table>
</td>
</tr>
<tr>
<td class="name">argument</td>
<td class="type">Object</td>
<td class="description">Event parameters while performing expand operation:
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
<td class="description">Returns the value of expanding parent element.</td>
</tr>
<tr>
<td class="name">model</td>
<td class="type">object</td>
<td class="description">Returns the TreeGrid model.</td>
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
<td class="description">Event parameters while performing collapse operation:
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
<td class="description">Returns the value of collapsing parent element.</td>
</tr>
<tr>
<td class="name">model</td>
<td class="type">object</td>
<td class="description">Returns the TreeGrid model.</td>
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
<td class="description">Event parameters before completing the delete operation:
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
<td class="description">Returns the data or deleting element.</td>
</tr>
<tr>
<td class="name">model</td>
<td class="type">object</td>
<td class="description">Returns the TreeGrid model.</td>
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
 
<div id="treegrid"></div> 
<script>
$("#treegrid").ejTreeGrid({
   actionBegin: function (args) {}
});
</script>
{% endhighlight %}


### actionComplete
{:#events:actioncomplete}


Triggered for every TreeGrid action success event.

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
<td class="description">Event parameters when TreeGrid is initialized:
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
<td class="description">Event parameters after perform the sorting in grid tree is completed:
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
<td class="description">Returns the TreeGrid model.</td>
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
<td class="description">Returns the TreeGrid model.</td>
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
<td class="description">Returns the TreeGrid model.</td>
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
 
<div id="treegrid"></div> 
<script>
$("#treegrid").ejTreeGrid({
   actionComplete: function (args) {}
});
</script>
{% endhighlight %}

### beforePrint
{:#events:beforeprint}

Triggered before the printing initiated in TreeGrid.

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
<td class="description">Arguments when beforePrint event is triggered.
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
<td class="name">element</td>
<td class="type">object</td>
<td class="description">Returns the treegrid element which is going to be print</td>
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
 
<div id="treegrid"></div> 
<script>
$("#treegrid").ejTreeGrid({
   beforePrint: function (args) {}
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
 
<div id="treegrid"></div> 
<script>
$("#treegrid").ejTreeGrid({
   beginEdit: function (args) {}
});
</script>
{% endhighlight %}


### collapsed
{:#events:collapsed}


Triggered after collapsed the TreeGrid record

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
<td class="type">number</td>
<td class="description">Returns the row index of collapsed record.</td>
</tr>
<tr>
<td class="name">data</td>
<td class="type">object</td>
<td class="description">Returns the data of collapsed record..</td>
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
<tr>
<td class="name">type</td>
<td class="type">string</td>
<td class="description">Returns the event type.</td>
</tr>
</tbody>
</table>
</td>
</tr>
</tbody>
</table>




#### Example



{% highlight html %}
 
<div id="treegrid"></div> 
<script>
$("#treegrid").ejTreeGrid({
   collapsed: function (args) {}
});
</script>
{% endhighlight %}



### collapsing
{:#events:collapsing}


Triggered while collapsing the TreeGrid record

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
<td class="type">number</td>
<td class="description">Returns the row index of collapsing record.</td>
</tr>
<tr>
<td class="name">data</td>
<td class="type">object</td>
<td class="description">Returns the data of collapsing record..</td>
</tr>
<tr>
<td class="name">type</td>
<td class="type">string</td>
<td class="description">Returns the event Type.</td>
</tr>
<tr>
<td class="name">expanded</td>
<td class="type">boolean</td>
<td class="description">Returns state of a record whether it is in expanded or collapsing state.</td>
</tr>
</tbody>
</table>
</td>
</tr>
</tbody>
</table>




#### Example



{% highlight html %}
 
<div id="treegrid"></div> 
<script>
$("#TreeGrid").ejTreeGrid({
   collapsing: function (args) {}
});
</script>
{% endhighlight %}

### columnDragStart
{:#events:columndragstart}

Triggered  when you start to drag a column

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
<td class="description">Arguments when columnDragStart event is triggered.
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
<td class="description">Returns the control model values.</td>
</tr>
<tr>
<td class="name">type</td>
<td class="type">string</td>
<td class="description">Returns the event Type.</td>
</tr>
<tr>
<td class="name">draggedColumn</td>
<td class="type">object</td>
<td class="description">Returns the column data which is dragged</td>
</tr>
<tr>
<td class="name">draggedColumnIndex</td>
<td class="type">number</td>
<td class="description">Returns the index of the column being dragged</td>
</tr>
</tbody>
</table>
</td>
</tr>
</tbody>
</table>

#### Example

{% highlight html %}
 
<div id="treegrid"></div> 
<script>
$("#TreeGrid").ejTreeGrid({
   columnDragStart: function (args) {}
});
</script>
{% endhighlight %}

### columnDrag
{:#events:columndrag}

Triggered while dragging a column 

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
<td class="description">Arguments when columnDrag event is triggered.
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
<td class="description">Returns the control model values.</td>
</tr>
<tr>
<td class="name">type</td>
<td class="type">string</td>
<td class="description">Returns the event Type.</td>
</tr>
<tr>
<td class="name">draggedColumn</td>
<td class="type">object</td>
<td class="description">Returns the column data which is dragged</td>
</tr>
<tr>
<td class="name">draggedColumnIndex</td>
<td class="type">number</td>
<td class="description">Returns the index of the column being dragged</td>
</tr>
<tr>
<td class="name">targetColumn</td>
<td class="type">object</td>
<td class="description">Returns the target column data</td>
</tr>
<tr>
<td class="name">targetColumnIndex</td>
<td class="type">number</td>
<td class="description">Returns the index of the target column</td>
</tr>
<tr>
<td class="name">canDrop</td>
<td class="type">boolean</td>
<td class="description">Returns that we can drop over the column or not.</td>
</tr>
</tbody>
</table>
</td>
</tr>
</tbody>
</table>

#### Example

{% highlight html %}
 
<div id="treegrid"></div> 
<script>
$("#TreeGrid").ejTreeGrid({
   columnDrag: function (args) {}
});
</script>
{% endhighlight %}

### columnDrop
{:#events:columndrop}

Triggered when a column is dropped

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
<td class="description">Arguments when columnDrop event is triggered.
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
<td class="description">Returns the control model values.</td>
</tr>
<tr>
<td class="name">type</td>
<td class="type">string</td>
<td class="description">Returns the event Type.</td>
</tr>
<tr>
<td class="name">draggedColumn</td>
<td class="type">object</td>
<td class="description">Returns the column data which is dragged</td>
</tr>
<tr>
<td class="name">draggedColumnIndex</td>
<td class="type">number</td>
<td class="description">Returns the index of the column being dragged</td>
</tr>
<tr>
<td class="name">targetColumn</td>
<td class="type">object</td>
<td class="description">Returns the target column data</td>
</tr>
<tr>
<td class="name">targetColumnIndex</td>
<td class="type">number</td>
<td class="description">Returns the index of the target column</td>
</tr>
</tbody>
</table>
</td>
</tr>
</tbody>
</table>

#### Example

{% highlight html %}
 
<div id="treegrid"></div> 
<script>
$("#TreeGrid").ejTreeGrid({
   columnDrop: function (args) {}
});
</script>
{% endhighlight %}

### columnResized
{:#events:columnresized}


Triggered after a column resized

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
<td class="description">Arguments when columnResized event is triggered.
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
<td class="description">Returns the control model values.</td>
</tr>
<tr>
<td class="name">type</td>
<td class="type">string</td>
<td class="description">Returns the event Type.</td>
</tr>
<tr>
<td class="name">column</td>
<td class="type">object</td>
<td class="description">Returns the column data which is resized</td>
</tr>
<tr>
<td class="name">columnIndex</td>
<td class="type">number</td>
<td class="description">Returns the index of the column being resized.</td>
</tr>
<tr>
<td class="name">newWidth</td>
<td class="type">number</td>
<td class="description">Returns resized column width after resized.</td>
</tr>
<tr>
<td class="name">oldWidth</td>
<td class="type">number</td>
<td class="description">Returns resized column width before resizing</td>
</tr>
</tbody>
</table>
</td>
</tr>
</tbody>
</table>

#### Example

{% highlight html %}
 
<div id="treegrid"></div> 
<script>
$("#TreeGrid").ejTreeGrid({
   columnResized: function (args) {}
});
</script>
{% endhighlight %}

### columnResizeStart
{:#events:columnresizestart}

Triggered while start to resize a column

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
<td class="description">Arguments when columnResizeStart event is triggered.
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
<td class="description">Returns the control model values.</td>
</tr>
<tr>
<td class="name">type</td>
<td class="type">string</td>
<td class="description">Returns the event Type.</td>
</tr>
<tr>
<td class="name">column</td>
<td class="type">object</td>
<td class="description">Returns the column data in which the resizing started</td>
</tr>
<tr>
<td class="name">columnIndex</td>
<td class="type">number</td>
<td class="description">Returns the column index in which the resizing started</td>
</tr>
<tr>
<td class="name">oldWidth</td>
<td class="type">number</td>
<td class="description">Returns column width before dragging</td>
</tr>
<tr>
<td class="name">target</td>
<td class="type">object </td>
<td class="description">Returns initial column element object.</td>
</tr>
</tbody>
</table>
</td>
</tr>
</tbody>
</table>

#### Example

{% highlight html %}
 
<div id="treegrid"></div> 
<script>
$("#TreeGrid").ejTreeGrid({
   columnResizeStart: function (args) {}
});
</script>
{% endhighlight %}

### columnResizeEnd
{:#events:columnresizeend}

Triggered when a column has been resized

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
<td class="description">Arguments when columnResizeEnd event is triggered.
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
<td class="description">Returns the control model values.</td>
</tr>
<tr>
<td class="name">type</td>
<td class="type">string</td>
<td class="description">Returns the event Type.</td>
</tr>
<tr>
<td class="name">column</td>
<td class="type">object</td>
<td class="description">Returns the column data in which the resizing started</td>
</tr>
<tr>
<td class="name">columnIndex</td>
<td class="type">number</td>
<td class="description">Returns the column index in which the resizing started</td>
</tr>
<tr>
<td class="name">extra</td>
<td class="type">number</td>
<td class="description">Returns the column width difference, before and after the resizing</td>
</tr>
<tr>
<td class="name">newWidth</td>
<td class="type">number</td>
<td class="description">Returns the new column width after resized</td>
</tr>
<tr>
<td class="name">oldWidth</td>
<td class="type">number</td>
<td class="description">Returns column width before dragging</td>
</tr>
<tr>
<td class="name">target</td>
<td class="type">object </td>
<td class="description">Returns initial column element object.</td>
</tr>
</tbody>
</table>
</td>
</tr>
</tbody>
</table>

#### Example

{% highlight html %}
 
<div id="treegrid"></div> 
<script>
$("#TreeGrid").ejTreeGrid({
   columnResizeEnd: function (args) {}
});
</script>
{% endhighlight %}

### contextMenuOpen
{:#events:contextmenuopen}


Triggered while Context Menu is rendered in TreeGrid control

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
<td class="description">Returns the TreeGrid model.</td>
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
 
<div id="treegrid"></div> 
<script>
$("#treegrid").ejTreeGrid({
   contextMenuOpen: function (args) {}
});
</script>
{% endhighlight %}

### create
{:#events:create}

Triggered when TreeGrid is rendered completely 

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
<td class="description">Returns the TreeGrid model</td>
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
 
<div id="treegrid"></div> 
<script>
$("#treegrid").ejTreeGrid({
   create: function (args) {}
});
</script>
{% endhighlight %}

### detailsDataBound 
{:#events:detailsdatabound }

Triggered while rendering details template in TreeGrid

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
<td class="description">Arguments when detailsDataBound event is triggered.
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
<td class="description">Returns the data collection of selected row.</td>
</tr>
<tr>
<td class="name">detailsElement</td>
<td class="type">object</td>
<td class="description">Returns the details element of selected row.</td>
</tr>
<tr>
<td class="name">rowIndex</td>
<td class="type">number</td>
<td class="description">Returns the rowIndex of selected row.</td>
</tr>
<tr>
<td class="name">model</td>
<td class="type">object</td>
<td class="description">Returns the TreeGrid model</td>
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
 
<div id="treegrid"></div> 
<script>
$("#treegrid").ejTreeGrid({
   detailsDataBound: function (args) {}
});
</script>
{% endhighlight %}

### detailsShown 
{:#events:detailsshown }

Triggered when details template pop-up is shown.

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
<td class="description">Arguments when detailsShown event is triggered.
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
<td class="description">Returns the data collection of selected row.</td>
</tr>
<tr>
<td class="name">detailsElement</td>
<td class="type">object</td>
<td class="description">Returns the details element of selected row.</td>
</tr>
<tr>
<td class="name">rowIndex</td>
<td class="type">number</td>
<td class="description">Returns the rowIndex of selected row.</td>
</tr>
<tr>
<td class="name">model</td>
<td class="type">object</td>
<td class="description">Returns the TreeGrid model</td>
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
 
<div id="treegrid"></div> 
<script>
$("#treegrid").ejTreeGrid({
   detailsShown: function (args) {}
});
</script>
{% endhighlight %}

### detailsHidden 
{:#events:detailshidden }

Triggered when details template pop-up is hidden.

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
<td class="description">Arguments when detailsHidden event is triggered.
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
<td class="description">Returns the TreeGrid model</td>
</tr>
<tr>
<td class="name">rowData</td>
<td class="type">object</td>
<td class="description">Returns the data collection of hidden details Template</td>
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
 
<div id="treegrid"></div> 
<script>
$("#treegrid").ejTreeGrid({
   detailsHidden: function (args) {}
});
</script>
{% endhighlight %}

### endEdit
{:#events:endedit}


Triggered after saved the modified cellValue in TreeGrid

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
 
<div id="treegrid"></div> 
<script>
$("#treegrid").ejTreeGrid({
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
<td class="description">Returns the row index of expanded record.</td>
</tr>
<tr>
<td class="name">data</td>
<td class="type">object</td>
<td class="description">Returns the data of expanded record..</td>
</tr>
<tr>
<td class="name">requestType</td>
<td class="type">string</td>
<td class="description">Returns Request Type.</td>
</tr>
<tr>
<td class="name">expanded</td>
<td class="type">boolean</td>
<td class="description">Returns state of a record whether it is in expanded or expanded state.</td>
</tr>
<tr>
<td class="name">type</td>
<td class="type">string</td>
<td class="description">Returns the event type.</td>
</tr>
</tbody>
</table>
</td>
</tr>
</tbody>
</table>




#### Example



{% highlight html %}
 
<div id="treegrid"></div> 
<script>
$("#treegrid").ejTreeGrid({
   expanded: function (args) {}
});
</script>
{% endhighlight %}



### expanding
{:#events:expanding}


Triggered while expanding the TreeGrid record

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
<td class="type">number</td>
<td class="description">Returns the row index of expanding record.</td>
</tr>
<tr>
<td class="name">data</td>
<td class="type">object</td>
<td class="description">Returns the data of expanding record..</td>
</tr>
<tr>
<td class="name">type</td>
<td class="type">string</td>
<td class="description">Returns the event Type.</td>
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
 
<div id="treegrid"></div> 
<script>
$("#treegrid").ejTreeGrid({
   expanding: function (args) {}
});
</script>
{% endhighlight %}


### load
{:#events:load}


Triggered while Treegrid is loaded

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
<td class="description">Returns the TreeGrid model</td>
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
 
<div id="treegrid"></div> 
<script>
$("#treegrid").ejTreeGrid({
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
 
<div id="treegrid"></div> 
<script>
$("#treegrid").ejTreeGrid({
   queryCellInfo: function (args) {}
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
<td class="description">Returns the data of rendering row record.</td>
</tr>
</tbody>
</table>
</td>
</tr>
</tbody>
</table>




#### Example


{% highlight html %}
 
<div id="treegrid"></div> 
<script>
$("#treegrid").ejTreeGrid({
   rowDataBound: function (args) {}
});
</script>
{% endhighlight %}


### rowDrag
{:#events:rowdrag}


Triggered while dragging a row in TreeGrid control

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
<td class="name">dropPosition</td>
<td class="type">string</td>
<td class="description">Returns the drop position details such as insertAbove,insertBelow,insertAsChild and invalidPosition</td>
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
<td class="name">model</td>
<td class="type">object</td>
<td class="description">Returns the TreeGrid model.</td>
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
 
<div id="treegrid"></div> 
<script>
$("#treegrid").ejTreeGrid({
   rowDrag: function (args) {}
});
</script>
{% endhighlight %}


### rowDragStart
{:#events:rowdragstart}


Triggered while start to drag row in TreeGrid control

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
<td class="description">Returns the TreeGrid model.</td>
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
 
<div id="treegrid"></div> 
<script>
$("#treegrid").ejTreeGrid({
   rowDragStart: function (args) {}
});
</script>
{% endhighlight %}


### rowDragStop
{:#events:rowdragstop}


Triggered while drop a row in TreeGrid control

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
<td class="description">Returns the TreeGrid model.</td>
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
 
<div id="treegrid"></div> 
<script>
$("#treegrid").ejTreeGrid({
   rowDragStop: function (args) {}
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
 
<div id="treegrid"></div> 
<script>
$("#treegrid").ejTreeGrid({
   cellSelecting: function (args) {}
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
 
<div id="treegrid"></div> 
<script>
$("#treegrid").ejTreeGrid({
   cellSelected: function (args) {}
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
<tr>
<td class="name">type</td>
<td class="type">string</td>
<td class="description">Returns the event type.</td>
</tr>
</tbody>
</table>
</td>
</tr>
</tbody>
</table>




#### Example


{% highlight html %}
 
<div id="treegrid"></div> 
<script>
$("#treegrid").ejTreeGrid({
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
<td class="name">targetRow</td>
<td class="type">object</td>
<td class="description">Returns the selecting row element.</td>
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
<td class="name">previousTreeGridRow</td>
<td class="type">object</td>
<td class="description">Returns the previous selected row element.</td>
</tr>
</tbody>
</table>
</td>
</tr>
</tbody>
</table>




#### Example


{% highlight html %}
 
<div id="treegrid"></div> 
<script>
$("#treegrid").ejTreeGrid({
   rowSelecting: function (args) {}
});
</script>
{% endhighlight %}

### recordClick
{:#events:recordclick}

Triggered while clicking a row, even when allowSelection property is disabled.

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
<td class="description">Arguments when recordClick event is triggered.
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
<td class="name">cell</td>
<td class="type">object</td>
<td class="description">Returns the element of clicked cell.</td>
</tr>
<tr>
<td class="name">cellIndex</td>
<td class="type">number</td>
<td class="description">Returns the index of the clicked cell.</td>
</tr>
<tr>
<td class="name">cellValue</td>
<td class="type">object</td>
<td class="description">Returns the data of clicked cell.</td>
</tr>
<tr>
<td class="name">row</td>
<td class="type">object</td>
<td class="description">Returns the element of the clicked row.</td>
</tr>
<tr>
<td class="name">rowIndex</td>
<td class="type">number</td>
<td class="description">Returns the index of the clicked row.</td>
</tr>
<tr>
<td class="name">columnName</td>
<td class="type">string</td>
<td class="description">Returns the column name of the clicked cell.</td>
</tr>
</tbody>
</table>
</td>
</tr>
</tbody>
</table>




#### Example



{% highlight html %}
 
<div id="treegrid"></div> 
<script>
$("#treegrid").ejTreeGrid({
   recordClick: function (args) {}
});
</script>
{% endhighlight %}

### recordDoubleClick
{:#events:recorddoubleclick}

Triggered during record double click action, even when allowSelection property is disabled.

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
<td class="description">Arguments when recordDoubleClick event is triggered.
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
<td class="name">cell</td>
<td class="type">object</td>
<td class="description">Returns the element of clicked cell.</td>
</tr>
<tr>
<td class="name">cellIndex</td>
<td class="type">number</td>
<td class="description">Returns the index of the clicked cell.</td>
</tr>
<tr>
<td class="name">cellValue</td>
<td class="type">object</td>
<td class="description">Returns the data of clicked cell.</td>
</tr>
<tr>
<td class="name">row</td>
<td class="type">object</td>
<td class="description">Returns the element of the clicked row.</td>
</tr>
<tr>
<td class="name">rowIndex</td>
<td class="type">number</td>
<td class="description">Returns the index of the clicked row.</td>
</tr>
<tr>
<td class="name">columnName</td>
<td class="type">string</td>
<td class="description">Returns the column name of the clicked cell.</td>
</tr>
</tbody>
</table>
</td>
</tr>
</tbody>
</table>




#### Example



{% highlight html %}
 
<div id="treegrid"></div> 
<script>
$("#treegrid").ejTreeGrid({
   recordDoubleClick: function (args) {}
});
</script>
{% endhighlight %}

### toolbarClick
{:#events:toolbarclick}

Triggered when toolbar item is clicked in TreeGrid.

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
<td class="description">Arguments when toolbarClick event is triggered.
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
<td class="description">Returns the TreeGrid model.</td>
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
 
<div id="treegrid"></div> 
<script>
$("#treegrid").ejTreeGrid({
   toolbarClick: function (args) {}
});
</script>
{% endhighlight %}


