---
layout: post
title: Properties, Methods and Events of ejReportDesigner Widget , Syncfusion
description: Public API, Events documentation for ejReportDesigner
platform: js-api
metaname: 
metacontent: 
---

# ejReportDesigner

Report Designer allows to design the report that can be published in the server or downloaded in the local physical path.

#### Syntax

{% highlight js %}

        $(element).ejReportDesigner();

{% endhighlight %}

#### Example 

{% highlight js %}

<div id="container"></div> 
<script> 
    // Create Report Designer
    $('#container').ejReportDesigner(); 
</script>

{% endhighlight %}

#### Requires

* module:jquery-1.10.2.js

* module:jquery.easing.1.3.js 

* module:jsrender.js

* module:codemirror.js

* module:show-hint.js

* module:sql.js

* module:sql-hint.js

* module:ej.core.js

* module:ej.data.js

* module:ej.touch.js

* module:ej.draggable.js

* module:ej.scroller.js

* module:ej.globalize.js

* module:ej.waitingpopup.js

* module:ej.button.js

* module:ej.checkbox.js

* module:ej.radiobutton.js

* module:ej.autocomplete.js

* module:ej.datepicker.js

* module:ej.timepicker.js

* module:ej.datetimepicker.js

* module:ej.daterangepicker.js

* module:ej.dialog.js

* module:ej.dropdownlist.js

* module:ej.tooltip.js

* module:ej.listbox.js

* module:ej.map.js

* module:ej.editor.js

* module:ej.maskedit.js

* module:ej.menu.js

* module:ej.pager.js

* module:ej.slider.js

* module:ej.splitbutton.js

* module:ej.toolbar.js

* module:ej.tab.js

* module:ej.treeview.js

* module:ej.uploadbox.js

* module:ej.colorpicker

* module:ej.grid.js

* module:ej.reportviewer.js

* module:ej.chart.js

* module:ej.circulargauge.js

* module:ej.lineargauge.js

* module:ej.bulletgraph.js

## Members

### configurePaneSettings `object`
{:#members:configurepanesettings}

Shows or hides the items of configuration pane in ReportDesigner control.

### configurePaneSettings.items `enum`
{:#members:configurepanesettings-items}

<ts name="ej.ReportDesigner.ConfigureItems"/>

Shows or hides the grouped items in the configuration pane with the help of enum ej.ReportDesigner.ConfigureItems

<table class="params">
  <thead>
    <tr>
      <th>Name</th>
      <th>Description</th>
    </tr>
  </thead>
  <tbody>
    <tr>
      <td class="name">Property</td>
      <td class="description">Shows or hides the properties panel in configuration pane.</td>
    </tr>
    <tr>
      <td class="name">Data</td>
      <td class="description">Shows or hides the data panel in configuration pane.</td>
    </tr>
    <tr>
      <td class="name">Parameter</td>
      <td class="description">Shows or hides the parameter panel in configuration pane.</td>
    </tr>
    <tr>
      <td class="name">ImageManager</td>
      <td class="description">Shows or hides the image manager panel in configuration pane.</td>
    </tr>
     <tr>
      <td class="name">All</td>
      <td class="description">Shows all the configuration pane items.</td>
    </tr>
  </tbody>
</table>

#### Default value 

<li>ej.ReportDesigner.ConfigureItems.All</li>

#### Example

* Show all configure pane items.

{% highlight html %}
 
<div id="container"></div>
<script>
    $("#container").ejReportDesigner({
        configurePaneSettings: { items: ej.ReportDesigner.ConfigureItems.All }
    });
</script>

{% endhighlight %}

* Hide all configure pane items.

{% highlight html %}
 
<div id="container"></div>
<script>
    $("#container").ejReportDesigner({
        configurePaneSettings: { items: ~ej.ReportDesigner.ConfigureItems.All }
    });
</script>

{% endhighlight %}

* Hide **Properties** panel from configure pane items.

{% highlight html %}
 
<div id="container"></div>
<script>
    $("#container").ejReportDesigner({
        configurePaneSettings: { items: ej.ReportDesigner.ConfigureItems.All & ~ej.ReportDesigner.ConfigureItems.Property}
    });
</script>

{% endhighlight %}

* Hide all items except **Data** panel from configure pane items.

{% highlight html %}
 
<div id="container"></div>
<script>
    $("#container").ejReportDesigner({
        configurePaneSettings: { items: ej.ReportDesigner.ConfigureItems.All & ~ej.ReportDesigner.ConfigureItems.Property  & ~ej.ReportDesigner.ConfigureItems.Parameter  & ~ej.ReportDesigner.ConfigureItems.ImageManager}
    });
</script>

{% endhighlight %}

### configurePaneSettings.showConfigurePane `boolean`
{:#members:configurepanesettings-showconfigurepane}

Shows or hides the configuration pane in ReportDesigner control.

#### Default value 

<li>true</li>

#### Example

* Show configure pane.

{% highlight html %}
 
<div id="container"></div>
<script>
    $("#container").ejReportDesigner({
        configurePaneSettings: { showConfigurePane: true }
    });
</script>

{% endhighlight %}

* Hide configure pane.

{% highlight html %}
 
<div id="container"></div>
<script>
    $("#container").ejReportDesigner({
        configurePaneSettings: { showConfigurePane: false }
    });
</script>

{% endhighlight %}

### locale `string`
{:#members:locale}

Specifies the locale for report designer.

#### Default Value

* "en-US"

#### Example

{% highlight html %}
 
<div id="container"></div> 
<script>          
    $("#container").ejReportDesigner({
            locale: "fr-FR"
    });             
</script>

{% endhighlight %}

### permissionSettings `object`
{:#members:permissionsettings}

Shows or hides the create, edit, and delete options in data source and dataset panels.

## permissionSettings.dataSet `enum`
{:#members:permissionsettings-dataset}

<ts name="ej.ReportDesigner.Permission"/>

Shows or hides the create, edit and delete options in dataset pane with the help of ej.ReportDesigner.Permission enum.

<table class="params">
  <thead>
    <tr>
      <th>Name</th>
      <th>Description</th>
    </tr>
  </thead>
  <tbody>
    <tr>
      <td class="name">Create</td>
      <td class="description">Shows or hides create option in dataset pane.</td>
    </tr>
    <tr>
      <td class="name">Edit</td>
      <td class="description">Shows or hides the edit option in dataset pane.</td>
    </tr>
    <tr>
      <td class="name">Delete</td>
      <td class="description">Shows or hides the delete option in dataset pane.</td>
    </tr>
     <tr>
      <td class="name">All</td>
      <td class="description">Shows all the options in dataset pane.</td>
    </tr>
  </tbody>
</table>

#### Default value 

<li>ej.ReportDesigner.Permission.All</li>

#### Example

* Show all options in dataset pane.

{% highlight html %}
 
<div id="container"></div>
<script>
    $("#container").ejReportDesigner({
        permissionSettings: { dataSet: ej.ReportDesigner.Permission.All }
    });
</script>

{% endhighlight %}

* Hide all options in dataset pane.

{% highlight html %}
 
<div id="container"></div>
<script>
    $("#container").ejReportDesigner({
        permissionSettings: { dataSet: ~ej.ReportDesigner.Permission.All }
    });
</script>

{% endhighlight %}

* Hide **Create** option from dataset pane.

{% highlight html %}
 
<div id="container"></div>
<script>
    $("#container").ejReportDesigner({
        permissionSettings: { dataSet: ej.ReportDesigner.Permission.All & ~ej.ReportDesigner.Permission.Create}
    });
</script>

{% endhighlight %}

* Hide all items except  **Create** option from dataset pane.

{% highlight html %}
 
<div id="container"></div>
<script>
    $("#container").ejReportDesigner({
        permissionSettings: { dataSet: ej.ReportDesigner.Permission.All & ~ej.ReportDesigner.Permission.Edit  & ~ej.ReportDesigner.Permission.Delete}
    });
</script>

{% endhighlight %}

### permissionSettings.dataSource `enum`
{:#members:permissionsettings-datasource}

<ts name="ej.ReportDesigner.Permission"/>

Shows or hides the create, edit and delete options in data source pane with the help of ej.ReportDesigner.Permission enum.

<table class="params">
  <thead>
    <tr>
      <th>Name</th>
      <th>Description</th>
    </tr>
  </thead>
  <tbody>
    <tr>
      <td class="name">Create</td>
      <td class="description">Shows or hides create option in data source pane.</td>
    </tr>
    <tr>
      <td class="name">Edit</td>
      <td class="description">Shows or hides the edit option in data source pane.</td>
    </tr>
    <tr>
      <td class="name">Delete</td>
      <td class="description">Shows or hides the delete option in data source pane.</td>
    </tr>
     <tr>
      <td class="name">All</td>
      <td class="description">Shows all the options in data source pane.</td>
    </tr>
  </tbody>
</table>

#### Default value 

<li>ej.ReportDesigner.Permission.All</li>

#### Example

* Show all options in data source pane.

{% highlight html %}
 
<div id="container"></div>
<script>
    $("#container").ejReportDesigner({
        permissionSettings: { dataSource: ej.ReportDesigner.Permission.All }
    });
</script>

{% endhighlight %}

* Hide all options in data source pane.

{% highlight html %}
 
<div id="container"></div>
<script>
    $("#container").ejReportDesigner({
        permissionSettings: { dataSource: ~ej.ReportDesigner.Permission.All }
    });
</script>

{% endhighlight %}

* Hide **Create** option from data source pane.

{% highlight html %}
 
<div id="container"></div>
<script>
    $("#container").ejReportDesigner({
        permissionSettings: { dataSource: ej.ReportDesigner.Permission.All & ~ej.ReportDesigner.Permission.Create}
    });
</script>

{% endhighlight %}

* Hide all items except  **Create** option from data source pane.

{% highlight html %}
 
<div id="container"></div>
<script>
    $("#container").ejReportDesigner({
        permissionSettings: { dataSource: ej.ReportDesigner.Permission.All & ~ej.ReportDesigner.Permission.Edit  & ~ej.ReportDesigner.Permission.Delete}
    });
</script>

{% endhighlight %}

### reportDataExtensions `array`
{:#members:reportdataextensions}

Gets or sets the list of custom data extension items.

#### Default Value

* []

### reportDataExtensions.name `string`
{:#members:reportdataextensions-name}

Gets or sets the name of the datasource type.

#### Default Value

* empty

### reportDataExtensions.className `string`
{:#members:reportdataextensions-classname}

Gets or sets the class name of the data extension.

#### Default Value

* empty

### reportDataExtensions.imageClass `string`
{:#members:reportdataextensions-imageclass}

Gets or sets the image class name to load image in data pane tile.

#### Default Value

* empty

### reportDataExtensions.displayName `string`
{:#members:reportdataextensions-displayname}

Gets or sets the name for data extension item to display in the data pane tile.

#### Default Value

* empty

#### Example

* Add a custom data extension to report designer

{% highlight html %}
 
<div id="container"></div> 
<script>
    $("#container").ejReportDesigner({
       reportDataExtensions: [{
        className: 'WebAPIDataSource',
        name: 'WebAPI',
        imageClass: 'e-reportdesigner-datasource-webapi',
        displayName: 'WebAPI'
    }]
  });
</script>

{% endhighlight %}

* Add multiple custom data extensions to report designer

{% highlight html %}
 
<div id="container"></div> 
<script>
    $("#container").ejReportDesigner({
       reportDataExtensions: [
         {
        className: 'WebAPIDataSource',
        name: 'WebAPI',
        imageClass: 'e-reportdesigner-datasource-webapi',
        displayName: 'WebAPI'
        },
        {
        className: 'PSQLDataSource',
        name: 'PostgreSQL',
        imageClass: 'e-reportdesigner-datasource-psql',
        displayName: 'PostgreSQL'
       }]
  });
</script>

{% endhighlight %}

### reportItemExtensions `array`
{:#members:reportitemextensions}

Gets or sets the list of custom report items.

#### Default Value

* []

### reportItemExtensions.name `string`
{:#members:reportitemextensions-name}

Gets or sets the name for the report item.

#### Default Value

* empty

### reportItemExtensions.className `string`
{:#members:reportitemextensions-classname}

Gets or sets the class name of the report item.

#### Default Value

* empty

### reportItemExtensions.imageClass `string`
{:#members:reportitemextensions-imageclass}

Gets or sets the image class name to load image in widgets pane tile.

#### Default Value

* empty

### reportItemExtensions.displayName `string`
{:#members:reportitemextensions-displayname}

Gets or sets the name for custom report item to display in the widgets pane tile.

#### Default Value

* empty

### reportItemExtensions.category `string`
{:#members:reportitemextensions-category}

Gets or sets the category name for the report item.

#### Default Value

* empty

### reportItemExtensions.toolTip `object`
{:#members:reportitemextensions-tooltip}

Gets information to provide content for custom report item tooltip.

<table class="params">
<thead>
<tr>
<th>Name</th>
<th>Description</th>
</tr>
</thead>
<tbody>
<tr>
<td class="name">requirements</td>
<td class="description">Gets or sets the minimum values required for the report item .</td>
</tr>
<tr>
<td class="name">description</td>
<td class="description">Gets or sets the description content for the report item.</td>
</tr>
<tr>
<td class="name">title</td>
<td class="description">Gets or sets the title for report item.</td>
</tr>
</tbody>
</table>

#### Default Value

* null

#### Example

* Add a custom report item

{% highlight html %}
 
<div id="container"></div> 
<script>
    $("#container").ejReportDesigner({ 
      reportItemExtensions: [{
        name: 'barcode',
        className: 'EJBarcode',
        imageClass: 'customitem-barcode',
        displayName: 'Barcode',
        category: 'Custom report item',
        toolTip: {
            requirements: 'Add a report item to the designer area.',
            description: 'Display the barcode lines as report item.',
            title: 'Barcode'
        }
    }]
  });
</script>

{% endhighlight %}

* Add multiple custom report items

{% highlight html %}
 
<div id="container"></div> 
<script>
    $("#container").ejReportDesigner({ 
      reportItemExtensions: [
        {
        name: 'barcode',
        className: 'EJBarcode',
        imageClass: 'customitem-barcode',
        displayName: 'Barcode',
        category: 'Barcodes',
        toolTip: {
            requirements: 'Add a report item to the designer area.',
            description: 'Display the barcode lines as report item.',
            title: 'Barcode'
          }
        },
       {
        name: 'qrbarcode',
        className: 'EJQRBarcode',
        imageClass: 'customitem-qrbarcode',
        displayName: 'QR Barcode',
        category: 'Barcodes',
        toolTip: <IItemTooltip>{
            requirements: 'Add a report item to the designer area.',
            description: 'Display the barcode lines as report item.',
            title: 'QR Barcode'
        }
      }]
  });
</script>

{% endhighlight %}

### reportPath  `string`	
{:#members:reportpath}

Gets or sets the report path of server.

#### Default Value 

* null

#### Example 

{% highlight js %}

<div id="container"></div>
<script>
    $("#container").ejReportDesigner({
        reportPath: "/Sample Reports/invoice"
    });
</script>

{% endhighlight %}

### reportType  `string`	
{:#members:reporttype}

Gets or sets the report type.

<table class="params">
<thead>
<tr>
<th>Name</th>
<th>Description</th>
</tr>
</thead>
<tbody>
<tr>
<td class="name">RDL</td>
<td class="description">Renders designer in RDL mode.</td>
</tr>
<tr>
<td class="name">RDLC</td>
<td class="description">Renders designer in RDLC mode.</td>
</tr>
</tbody>
</table>

#### Default Value 

* ej.ReportDesigner.ReportType.RDL

#### Example 

{% highlight js %}

<div id="container"></div>
<script>
    $("#container").ejReportDesigner({
        reportType: ej.ReportDesigner.ReportType.RDLC
    });
</script>

{% endhighlight %}

### reportServerUrl `string`	
{:#members:reportserverurl}

Gets or sets the reports server URL.

#### Default Value 

* null

#### Example 

{% highlight js %}

<div id="container"></div>
<script>
    $("#container").ejReportDesigner({
        reportServerUrl: "https://reportserver.syncfusion.com/"
    });
</script>

{% endhighlight %}

### serviceAuthorizationToken `string`
{:#members:serviceauthorizationtoken}

Gets or sets the serviceAuthorizationToken to access the Report Server API services.

#### Default Value 

* empty

#### Example 

{% highlight js %}

<div id="container"></div>
<script>
   $("#container").ejReportDesigner({ 
     serviceAuthorizationToken: token['token_type'] + ' ' + token['access_token'] 
    });
</script>

{% endhighlight %}

### serviceUrl `string`
{:#members:serviceurl}

Gets or sets the URL of the  WebAPI service; it will be used for processing the report.

#### Default Value

<li>null</li> 

#### Example 

{% highlight js %}

<div id="container"></div>
<script>
    $("#container").ejReportDesigner({
        serviceUrl: '../../api/ReportingService'
    });
</script>

{% endhighlight %}

### tenantName  `string`	
{:#members:tenantname}

Gets or sets the tenant name of the user groups; it will be used when integrating report designer with server.

#### Default Value 

* null

#### Example 

{% highlight js %}

<div id="container"></div>
<script>
    $("#container").ejReportDesigner({
        tenantName: "site"
    });
</script>

{% endhighlight %}

### toolbarSettings `object`
{:#members:toolbarsettings}

Defines the settings of the ReportDesigner toolbar.

### toolbarSettings.items `enum`
{:#members:toolbarsettings-items}

<ts name="ej.ReportDesigner.ToolbarItems"/>

Shows or hides the grouped items in the toolbar with the help of enum ej.ReportDesigner.ToolbarItems.

<table class="params">
  <thead>
    <tr>
      <th>Name</th>
      <th>Description</th>
    </tr>
  </thead>
  <tbody>
    <tr>
      <td class="name">New</td>
      <td class="description">Creates a new, blank report.</td>
    </tr>
    <tr>
      <td class="name">Open</td>
      <td class="description">Displays the Open dialog box to retrieve an existing report.</td>
    </tr>
    <tr>
      <td class="name">Save</td>
      <td class="description">Saves the active report to a specified location.</td>
    </tr>
    <tr>
      <td class="name">Cut</td>
      <td class="description">Removes the selected item from the active report.</td>
    </tr>
    <tr>
      <td class="name">Copy</td>
      <td class="description">Copies selected text or object to the clipboard.</td>
    </tr>
    <tr>
      <td class="name">Paste</td>
      <td class="description">Pastes the item that cut or copied into (the position of the insertion point) the report from the clipboard.</td>
    </tr>
    <tr>
      <td class="name">Delete</td>
      <td class="description">Deletes the selected item or text from the report.</td>
    </tr>
    <tr>
      <td class="name">Undo</td>
      <td class="description">Reverses the last action or deletes the last entry that is typed.</td>
    </tr>
    <tr>
      <td class="name">Redo</td>
      <td class="description">Reverses the action of the last Undo command.</td>
    </tr>
    <tr>
      <td class="name">Zoom</td>
      <td class="description">Used to "zoom in" to get a close-up view of a report or "zoom out" to see more of the page at a reduced size.</td>
    </tr>
    <tr>
      <td class="name">Order</td>
      <td class="description">Used to change the layout order of report items in design area surface.</td>
    </tr>
    <tr>
      <td class="name">Center</td>
      <td class="description">Aligns all report items to the center position of design surface in horizontal or vertical direction.</td>
    </tr>
    <tr>
      <td class="name">Alignment</td>
      <td class="description">Aligns the selected report item in the design surface.</td>
    </tr>
    <tr>
      <td class="name">Distribute</td>
      <td class="description">Distributes selected report items at equal intervals from each other.</td>
    </tr>
    <tr>
      <td class="name">Sizing</td>
      <td class="description">Equally size the selected report items in the design surface.</td>
    </tr>
       <tr>
      <td class="name">AlignGrid</td>
      <td class="description">Snaps the selected report items to the closest gridline.</td>
    </tr>
    <tr>
      <td class="name">EditDesign</td>
      <td class="description">Switches from preview to design view of the report.</td>
    </tr>
    <tr>
      <td class="name">View</td>
      <td class="description">Contains options to show or hide `Header`, `Footer`, `Grid Lines`, `Snap To Shape` in the report design.</td>
    </tr>
    <tr>
      <td class="name">Preview</td>
      <td class="description">Previews the active report in report viewer.</td>
    </tr>
     <tr>
      <td class="name">All</td>
      <td class="description">Shows all the toolbar items.</td>
    </tr>
  </tbody>
</table>

#### Default Value

<li>ej.ReportDesigner.ToolbarItems.All</li>

#### Example

* Show all toolbar items

{% highlight html %}
 
<div id="container"></div>
<script>
    $("#container").ejReportDesigner({
        toolbarSettings: { items: ej.ReportDesigner.ToolbarItems.All }
    });
</script>

{% endhighlight %}

* Hide all toolbar items

{% highlight html %}
 
<div id="container"></div>
<script>
    $("#container").ejReportDesigner({
        toolbarSettings: { items: ~ej.ReportDesigner.ToolbarItems.All }
    });
</script>

{% endhighlight %}

* Hide **Zoom** option from toolbar

{% highlight html %}
 
<div id="container"></div>
<script>
    $("#container").ejReportDesigner({
        toolbarSettings: { items: ej.ReportDesigner.ToolbarItems.All & ~ej.ReportDesigner.ToolbarItems.Zoom }
    });
</script>

{% endhighlight %}

* Hide **Open** and **Save** option from toolbar

{% highlight html %}
 
<div id="container"></div>
<script>
    $("#container").ejReportDesigner({
        toolbarSettings: { items: ej.ReportDesigner.ToolbarItems.All & ~ej.ReportDesigner.ToolbarItems.Open & ~ej.ReportDesigner.ToolbarItems.Save }
    });
</script>

{% endhighlight %}

### toolbarSettings.showToolbar `boolean`
{:#members:toolbarsettings-showtoolbar}

Shows or hides the toolbar.

#### Default Value 

* true

* Show report designer toolbar.

{% highlight html %}

<div id="container"></div>
<script>
    $("#container").ejReportDesigner({
        toolbarSettings: { showToolbar: true }
    });
</script>

{% endhighlight %}

* Hide report designer toolbar.

{% highlight html %}

<div id="container"></div>
<script>
    $("#container").ejReportDesigner({
        toolbarSettings: { showToolbar: false }
    });
</script>

{% endhighlight %}

### toolbarSettings.templateId `string`
{:#members:toolbarsettings-templateid}

Specifies the toolbar template ID.

#### Default Value 

* empty

#### Example

{% highlight html %}
 
<div id="container"></div>
<script>          
   $("#container").ejReportDesigner(
       {
           toolbarSettings:{templateId: "customtoolbarId"}
       });         
</script>

{% endhighlight %}

## Methods

### addDataSet(dataset)
{:#methods:adddataset}

Add a dataset to the report at runtime.

<table>
  <thead>
    <tr>
      <th>Name</th>
      <th>Type</th>
      <th>Description</th>
    </tr>
  </thead>
  <tbody>
    <tr>
      <td class='name'>dataset</td>
      <td class='type'>object</td>
      <td class='description'>a JSON to define a connection properties for dataset.</td>
    </tr>
  </tbody>
</table>

#### Example

* Add embedded dataset to the report 

{% highlight html %}

<div id="container"></div>
<script>
    //Create Report Designer Instance
    $("#container").ejReportDesigner();
    var designerObj = $("#container").data("ejReportDesigner");
    var dataset = 
    { 
     __type:'Syncfusion.RDL.DOM.DataSet',
     Name:'DataSet1',
     Fields:[
          { __type: "Syncfusion.RDL.DOM.Field",DataField: "DepartmentID",Name: "DepartmentID",TypeName: "System.Int16",Value: null},
          { __type: "Syncfusion.RDL.DOM.Field",DataField: "Name",Name: "Name",TypeName: "System.String",Value: null},
          { __type: "Syncfusion.RDL.DOM.Field",DataField: "GroupName",Name: "GroupName",TypeName: "System.String",Value: null },
          { __type: "Syncfusion.RDL.DOM.Field",DataField: "ModifiedDate",Name: "ModifiedDate",TypeName: "System.DateTime",Value: null}
        ],
     Query: {
          __type: "Syncfusion.RDL.DOM.Query",
          CommandText: "SELECT [HumanResources].[Department].[DepartmentID],\n[HumanResources].[Department].[Name],\n[HumanResources].[Department].[GroupName],\n[HumanResources].[Department].[ModifiedDate] FROM [HumanResources].[Department]",
          CommandType: 0,
          DataSourceName: "DataSource1",
          QueryDesignerState: {
              __type: "Syncfusion.RDL.DOM.QueryDesignerState",
              Expressions: null,
              Filters: null,
              Joins: null,
              StoredProcedure: null,
              Tables: [
                {
                  __type: "Syncfusion.RDL.DOM.Table",
                  Columns: [
                    { __type: "Syncfusion.RDL.DOM.Column",AggregateTye: undefined,AliasName: null,IsDuplicate: false,
                    IsSelected: true, Name: "DepartmentID"
                    },
                    {__type: "Syncfusion.RDL.DOM.Column",AggregateTye: undefined,AliasName: null,IsDuplicate: false,
                    IsSelected: true,Name: "Name"
                    },
                    {__type: "Syncfusion.RDL.DOM.Column",AggregateTye: undefined,AliasName: null,IsDuplicate: false,
                    IsSelected: true,Name: "GroupName"
                    },
                    {__type: "Syncfusion.RDL.DOM.Column",AggregateTye: undefined,AliasName: null,IsDuplicate: false,
                    IsSelected: true,Name: "ModifiedDate"
                    }
                  ],
                  Name: "Department", 
                  Schema: "HumanResources",
                  SchemaLevels: [
                    { Name: "HumanResources",SchemaType: "Schema"},
                    {Name: "Tables",SchemaType: "Category"},
                    { Name: "Department",SchemaType: "Table"}
                  ]
                }
              ]
          },
          QueryParameters: [],
          Timeout: 0
          },
     CaseSensitivity:0,
     Collation:null,
     AccentSensitivity:0,
     KanatypeSensitivity:0,
     WidthSensitvity:0,
     Filters:[],
     SharedDataSet:null,
     InterpretSubtotalsAsDetails:0,
     DataSetInfo:null,
     DataSetObject:null
     };

    designerObj.addDataSet(dataset);
</script>

{% endhighlight %}

* Add shared dataset to the report 

{% highlight html %}

<div id="container"></div>
<script>
    //Create Report Designer Instance
    $("#container").ejReportDesigner();
    var designerObj = $("#container").data("ejReportDesigner");
 
    var dataset = 
    { 
     __type:'Syncfusion.RDL.DOM.DataSet',
     Name:'DataSet1',
     Fields:[
          { __type: "Syncfusion.RDL.DOM.Field",DataField: "ProdCat",Name: "ProdCat",TypeName: "System.String",Value: null},
          { __type: "Syncfusion.RDL.DOM.Field",DataField: "SubCat",Name: "SubCat",TypeName: "System.String",Value: null},
          { __type: "Syncfusion.RDL.DOM.Field",DataField: "OrderYear",Name: "OrderYear",TypeName: "System.Int32",Value: null },
          { __type: "Syncfusion.RDL.DOM.Field",DataField: "OrderQtr",Name: "OrderQtr",TypeName: "System.String",Value: null},
          { __type: "Syncfusion.RDL.DOM.Field",DataField: "Sales",Name: "Sales",TypeName: "System.Decimal",Value: null}
        ],
     Query:null,
     CaseSensitivity:0,
     Collation:null,
     AccentSensitivity:0,
     KanatypeSensitivity:0,
     WidthSensitvity:0,
     Filters:[],
     SharedDataSet: {
            __type: "Syncfusion.RDL.DOM.SharedDataSet",
            QueryParameters: [],
            SharedDataSetReference: 'Sales'
     },
     InterpretSubtotalsAsDetails:0,
     DataSetInfo:null,
     DataSetObject:null
     };

    designerObj.addDataSet(dataset);
</script>

{% endhighlight %}

### addDataSource(datasource)
{:#methods:adddatasource}

Add a datasource to the report at runtime.

<table>
  <thead>
    <tr>
      <th>Name</th>
      <th>Type</th>
      <th>Description</th>
    </tr>
  </thead>
  <tbody>
    <tr>
      <td class='name'>datasource</td>
      <td class='type'>object</td>
      <td class='description'>a JSON to define a connection properties for datasource.</td>
    </tr>
  </tbody>
</table>

#### Example

{% highlight html %}

<div id="container"></div>
<script>
    //Create Report Designer Instance
    $("#container").ejReportDesigner();
    var designerObj = $("#container").data("ejReportDesigner");
    var datasource = 
    { 
      __type:'Syncfusion.RDL.DOM.DataSource',
      Name:'DataSource1',
      Transaction:false,
      DataSourceReference:null,
      SecurityType:'DataBase',
      ConnectionProperties:{
            __type:'Syncfusion.RDL.DOM.ConnectionProperties', 
            ConnectString:'Data Source=mvc.syncfusion.com;Initial Catalog=AdventureWorks;',
            EmbedCredentials:false,
            DataProvider:'SQL',
            IsDesignState:false,
            IntegratedSecurity:false,
            UserName:'',
            PassWord:'',
            Prompt:'Specify the Username and password for DataSource DataSource1',
            CustomProperties:[]
        } 
    };

    designerObj.addDataSource(datasource);
</script>

{% endhighlight %}

* Add shared datasource to the report

{% highlight html %}

<div id="container"></div>
<script>
    //Create Report Designer Instance
    $("#container").ejReportDesigner();
    var designerObj = $("#container").data("ejReportDesigner");
    var datasource = 
    { 
      __type:'Syncfusion.RDL.DOM.DataSource',
      Name:'DataSource1',
      Transaction:false,
      DataSourceReference: 'AdventureWorks',
      SecurityType:'None',
      ConnectionProperties:null
    };

    designerObj.addDataSource(datasource);
</script>

{% endhighlight %}

### addItem(item)
{:#methods:additem}

Add a report item to the report at runtime.

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
			<td class="name">item</td>
			<td class="type">object</td>
			<td class="description last">JSON for the new report item to be added</td>
		</tr>
	</tbody>
</table>

#### Example

* Add a report item to report body

{% highlight html %}

<div id="container"></div>
<script>
    //Create Report Designer Instance
    $("#container").ejReportDesigner();
    var designerObj = $("#container").data("ejReportDesigner");
    var item =  { left: 300, top: 100, itemType: 'Tablix', container: { name: 'Body' } };
    designerObj.addItem(item);
</script>

{% endhighlight %}

* Add a report item to report header

{% highlight html %}

<div id="container"></div>
<script>
    //Create Report Designer Instance
    $("#container").ejReportDesigner();
    var designerObj = $("#container").data("ejReportDesigner");
    var item =  { left: 100, top: 30, itemType: 'Image', container: { name: 'Header' } };
    designerObj.addItem(item);
</script>

{% endhighlight %}

* Add a report item to report footer

{% highlight html %}

<div id="container"></div>
<script>
    //Create Report Designer Instance
    $("#container").ejReportDesigner();
    var designerObj = $("#container").data("ejReportDesigner");
    var item =  { left: 50, top: 50, itemType: 'TextBox', container: { name: 'Footer' } };
    designerObj.addItem(item);
</script>

{% endhighlight %}

* Add a report item into a tablix cell

{% highlight html %}

<div id="container"></div>
<script>
    //Create Report Designer Instance
    $("#container").ejReportDesigner();
    var designerObj = $("#container").data("ejReportDesigner");
    //Add image report item into tablix cell
    var item =  { left: 50, top: 50, itemType: 'Image', container: { name: 'Tablix1',rowIndex:0,colIndex:0 } };
    designerObj.addItem(item);
</script>

{% endhighlight %}

* Add a report item into a rectangle report item

{% highlight html %}

<div id="container"></div>
<script>
    //Create Report Designer Instance
    $("#container").ejReportDesigner();
    var designerObj = $("#container").data("ejReportDesigner");
    //Add rectangle item
    var item =  { left: 50, top: 50, itemType: 'Rectangle', container: { name: 'Body' } };
    designerObj.addItem(item);
    //Add image report item into rectangle item
    var item =  { left: 10, top: 20, itemType: 'Image', container: { name: 'Rectangle1'} };
    designerObj.addItem(item);
</script>

{% endhighlight %}

### bringForward()
{:#methods:bringforward}

Visually move the selected report item over its closest intersected report items.

#### Example

{% highlight html %}

<div id="container"></div>
<script>
    //Create ReportDesigner Instance
    $("#container").ejReportDesigner();
    var designerObj = $("#container").data("ejReportDesigner");
    designerObj.bringForward();
</script>

{% endhighlight %}

### bringToFront()
{:#methods:bringtofront}

Visually move the selected report item over all other intersected report items.

#### Example

{% highlight html %}

<div id="container"></div>
<script>
    //Create ReportDesigner Instance
    $("#container").ejReportDesigner();
    var designerObj = $("#container").data("ejReportDesigner");
    designerObj.bringToFront();
</script>

{% endhighlight %}

### canCopy()
{:#methods:cancopy}

Determines whether a copy operation is possible.

#### Returns

* boolean

#### Example

{% highlight html %}

<div id="container"></div>
<script>
    // Create ReportDesigner Instance
    $("#container").ejReportDesigner();
    var designerObj = $("#container").data("ejReportDesigner");
    designerObj.canCopy();
</script>

{% endhighlight %}

### canCut()
{:#methods:cancut}

Determines whether a cut operation is possible.

#### Returns

* boolean

#### Example

{% highlight html %}

<div id="container"></div>
<script>
    // Create ReportDesigner Instance
    $("#container").ejReportDesigner();
    var designerObj = $("#container").data("ejReportDesigner");
    designerObj.canCut();
</script>

{% endhighlight %}

### canPaste()
{:#methods:canpaste}

Determines whether a paste operation is possible.

#### Returns

* boolean

#### Example

{% highlight html %}

<div id="container"></div>
<script>
    // Create ReportDesigner Instance
    $("#container").ejReportDesigner();
    var designerObj = $("#container").data("ejReportDesigner");
    designerObj.canPaste();
</script>

{% endhighlight %}

### canRedo()
{:#methods:canredo}

Returns the boolean value indicating whether the user can redo the previous action in the report.

#### Returns

* boolean

#### Example

{% highlight html %}

<div id="container"></div>
<script>
    // Create ReportDesigner Instance
    $("#container").ejReportDesigner();
    var designerObj = $("#container").data("ejReportDesigner");
    designerObj.canRedo();
</script>

{% endhighlight %}

### canRemove()
{:#methods:canremove}

Determines whether a delete operation is possible.

#### Returns

* boolean

#### Example

{% highlight html %}

<div id="container"></div>
<script>
    // Create ReportDesigner Instance
    $("#container").ejReportDesigner();
    var designerObj = $("#container").data("ejReportDesigner");
    designerObj.canRemove();
</script>

{% endhighlight %}

### canUndo()
{:#methods:canundo}

Returns a boolean value indicating whether the user can undo the previous action in the report.

#### Returns

* boolean

#### Example

{% highlight html %}

<div id="container"></div>
<script>
    // Create ReportDesigner Instance
    $("#container").ejReportDesigner();
    var designerObj = $("#container").data("ejReportDesigner");
    designerObj.canUndo();
</script>

{% endhighlight %}

### cloneDataSet(name)
{:#methods:clonedataset}

Clone the existing dataset in the report at runtime.

<table>
  <thead>
    <tr>
      <th>Name</th>
      <th>Type</th>
      <th>Description</th>
    </tr>
  </thead>
  <tbody>
    <tr>
      <td class='name'>name</td>
      <td class='type'>string</td>
      <td class='description'>Name of the existing dataset.</td>
    </tr>
  </tbody>
</table>

#### Example

{% highlight html %}

<div id="container"></div>
<script>
    //Create ReportDesigner Instance
    $("#container").ejReportDesigner();
    var designerObj = $("#container").data("ejReportDesigner");
    designerObj.cloneDataSet('DataSet1');
</script>

{% endhighlight %}

### cloneDataSource(name)
{:#methods:clonedatasource}

Clone the existing datasource in the report at runtime.

<table>
  <thead>
    <tr>
      <th>Name</th>
      <th>Type</th>
      <th>Description</th>
    </tr>
  </thead>
  <tbody>
    <tr>
      <td class='name'>name</td>
      <td class='type'>string</td>
      <td class='description'>Name of the existing datasource.</td>
    </tr>
  </tbody>
</table>

#### Example

{% highlight html %}

<div id="container"></div>
<script>
    //Create ReportDesigner Instance
    $("#container").ejReportDesigner();
    var designerObj = $("#container").data("ejReportDesigner");
    designerObj.cloneDataSource('DataSource1');
</script>

{% endhighlight %}

### copy()
{:#methods:copy}

Copies the selected report item from design panel to the Report Designer internal clipboard.

#### Example

{% highlight html %}

<div id="container"></div>
<script>
    // Create ReportDesigner Instance
    $("#container").ejReportDesigner();
    var designerObj = $("#container").data("ejReportDesigner");
    designerObj.copy();
</script>

{% endhighlight %}

### cut()
{:#methods:cut}

Cuts the selected report item from design panel to the Report Designer internal clipboard.

#### Example

{% highlight html %}

<div id="container"></div>
<script>
    // Create ReportDesigner Instance
    $("#container").ejReportDesigner();
    var designerObj = $("#container").data("ejReportDesigner");
    designerObj.cut();
</script>

{% endhighlight %}

### hasReportChanges()
{:#methods:hasreportchanges}

Returns the boolean value that specifies whether the report has changes or not.

#### Returns

* boolean

#### Example

{% highlight html %}

<div id="container"></div>
<script>
    // Create ReportDesigner Instance
    $("#container").ejReportDesigner();
    var designerObj = $("#container").data("ejReportDesigner");
    designerObj.hasReportChanges();
</script>

{% endhighlight %}

### isNewReport()
{:#methods:isnewreport}

Returns the boolean value that specifies whether the currently processing report is a new report or not.

#### Returns

* boolean

#### Example

{% highlight html %}

<div id="container"></div> 
<script>
    // Create ReportDesigner Instance
    $("#container").ejReportDesigner();
    var designerObj = $("#container").data("ejReportDesigner");
    designerObj.isNewReport();
</script>

{% endhighlight %}

### isNewServerReport()
{:#methods:isnewserverreport}

Returns the boolean value that specifies whether the currently processing report is a new server report or not.

#### Returns

* boolean

#### Example

{% highlight html %}

<div id="container"></div>
<script>
    // Create ReportDesigner Instance
    $("#container").ejReportDesigner();
    var designerObj = $("#container").data("ejReportDesigner");
    designerObj.isNewServerReport();
</script>

{% endhighlight %}

### isServerReport()
{:#methods:isserverreport}

Returns the boolean value that specifies whether the currently processing report is obtained from the server or local.

#### Returns

* boolean

#### Example

{% highlight html %}

<div id="container"></div>
<script>
    // Create ReportDesigner Instance
    $("#container").ejReportDesigner();
    var designerObj = $("#container").data("ejReportDesigner");
    designerObj.isServerReport();
</script>

{% endhighlight %}

### newReport()
{:#methods:newreport}

To create a new report.

<table>
  <thead>
    <tr>
      <th>Name</th>
      <th>Type</th>
      <th>Description</th>
    </tr>
  </thead>
  <tbody>
    <tr>
      <td class='name'>name</td>
      <td class='type'>string(optional)</td>
      <td class='description'>Name of the new report.</td>
    </tr>
    <tr>
      <td class='name'>dataSetPath</td>
      <td class='type'>string(optional)</td>
      <td class='description'>Name of the shared dataset.</td>
    </tr>
  </tbody>
</table>

#### Example

{% highlight html %}

<div id="container"></div>
<script>
    // Create ReportDesigner Instance
    $("#container").ejReportDesigner();
    var designerObj = $("#container").data("ejReportDesigner");
    designerObj.newReport();
</script>

{% endhighlight %}

### newServerReport()
{:#methods:newserverreport}

To create a new report in the server.

<table>
  <thead>
    <tr>
      <th>Name</th>
      <th>Type</th>
      <th>Description</th>
    </tr>
  </thead>
  <tbody>
    <tr>
      <td class='name'>name</td>
      <td class='type'>string(optional)</td>
      <td class='description'>Name of the new report.</td>
    </tr>
    <tr>
      <td class='name'>dataSetPath</td>
      <td class='type'>string(optional)</td>
      <td class='description'>Name of the shared dataset.</td>
    </tr>
  </tbody>
</table>

#### Example

{% highlight html %}

<div id="container"></div>
<script>
   // Create ReportDesigner Instance
   $("#container").ejReportDesigner();
   var designerObj = $("#container").data("ejReportDesigner");
   designerObj.newServerReport('Test1', 'ab018ae7-f747-49a1-9e26-759e35c0a0db');
</script>

{% endhighlight %}

### openReport()
{:#methods:openreport}

This method opens the report from the server.

<table>
  <thead>
    <tr>
      <th>Name</th>
      <th>Type</th>
      <th>Description</th>
    </tr>
  </thead>
  <tbody>
    <tr>
      <td class='name'>reportPath</td>
      <td class='type'>string(optional)</td>
      <td class='description'>Path of the server report</td>
    </tr>
    <tr>
      <td class='name'>serverUrl</td>
      <td class='type'>string(optional)</td>
      <td class='description'>Reports server URL</td>
    </tr>
  </tbody>
</table>

#### Example

{% highlight html %}

<div id="container"></div>
<script>
    // Create ReportDesigner Instance
    $("#container").ejReportDesigner();
    var designerObj = $("#container").data("ejReportDesigner");
    designerObj.openReport();
</script>

{% endhighlight %}

### openReportDefinition()
{:#methods:openreportdefinition}

This method opens the report using raw report data.

<table>
  <thead>
    <tr>
      <th>Name</th>
      <th>Type</th>
      <th>Description</th>
    </tr>
  </thead>
  <tbody>
    <tr>
      <td class='name'>rdlData</td>
      <td class='type'>JSON &#124; string &#124; XML</td>
      <td class='description'>Provide the report definition in the JSON or string or XML format</td>
    </tr>
  </tbody>
</table>

#### Example

{% highlight html %}

<div id="container"></div>
<script>
    // Create ReportDesigner Instance
    $("#container").ejReportDesigner();
    var designerObj = $("#container").data("ejReportDesigner");
    var rdlData = ''; // Assign a report data in JSON, string or XML format
    designerObj.openReportDefinition(rdlData);
</script>

{% endhighlight %}

### openReportFromDevice()
{:#methods:openreportfromdevice}

Opens the client browse dialog to browse the report.

#### Example

{% highlight html %}

<div id="container"></div>
<script>
    // Create ReportDesigner Instance
    $("#container").ejReportDesigner();
    var designerObj = $("#container").data("ejReportDesigner");
    designerObj.openReportFromDevice();
</script>

{% endhighlight %}

### openServerReportDialog()
{:#methods:openserverreportdialog}

Opens the report designer browse dialog to browse the available reports in the reportserver.

#### Example

{% highlight html %}

<div id="container"></div>
<script>
    // Create ReportDesigner Instance
    $("#container").ejReportDesigner();
    var designerObj = $("#container").data("ejReportDesigner");
    designerObj.openServerReportDialog();
</script>

{% endhighlight %}

### paste()
{:#methods:paste}

Pastes the selected report item from the Report Designer internal clipboard to design panel.

#### Example

{% highlight html %}

<div id="container"></div>
<script>
    // Create ReportDesigner Instance
    $("#container").ejReportDesigner();
    var designerObj = $("#container").data("ejReportDesigner");
    designerObj.paste();
</script>

{% endhighlight %}

### redo()
{:#methods:redo}

Reverses the action of the last Undo command.

#### Example

{% highlight html %}

<div id="container"></div>
<script>
    // Create ReportDesigner Instance
    $("#container").ejReportDesigner();
    var designerObj = $("#container").data("ejReportDesigner");
    designerObj.redo();
</script>

{% endhighlight %}

### remove()
{:#methods:remove}

Deletes the selected report item from the report.

#### Example

{% highlight html %}

<div id="container"></div>
<script>
    // Create ReportDesigner Instance
    $("#container").ejReportDesigner();
    var designerObj = $("#container").data("ejReportDesigner");
    designerObj.remove();
</script>

{% endhighlight %}

### removeDataSet(dataset)
{:#methods:removedataset}

Remove a dataset from the report at runtime.

<table>
  <thead>
    <tr>
      <th>Name</th>
      <th>Type</th>
      <th>Description</th>
    </tr>
  </thead>
  <tbody>
    <tr>
      <td class='name'>dataset</td>
      <td class='type'>string</td>
      <td class='description'>Name of the dataset.</td>
    </tr>
  </tbody>
</table>

#### Example

{% highlight html %}

<div id="container"></div>
<script>
    //Create ReportDesigner Instance
    $("#container").ejReportDesigner();
    var designerObj = $("#container").data("ejReportDesigner");
    designerObj.removeDataSet('DataSet1');
</script>

{% endhighlight %}

### removeDatasource(datasource)
{:#methods:removedatasource}

Remove a datasource from the report at runtime.

<table>
  <thead>
    <tr>
      <th>Name</th>
      <th>Type</th>
      <th>Description</th>
    </tr>
  </thead>
  <tbody>
    <tr>
      <td class='name'>datasource</td>
      <td class='type'>string</td>
      <td class='description'>Name of the datasource.</td>
    </tr>
  </tbody>
</table>

#### Example

{% highlight html %}

<div id="container"></div>
<script>
    //Create ReportDesigner Instance
    $("#container").ejReportDesigner();
    var designerObj = $("#container").data("ejReportDesigner");
    designerObj.removeDatasource('DataSource1');
</script>

{% endhighlight %}

### removeItem(itemName)
{:#methods:removeitem}

Remove the given report item from the report.

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
			<td class="name">itemName</td>
			<td class="type">string</td>
			<td class="description last">Name of the report item to be removed from report</td>
		</tr>
	</tbody>
</table>

#### Example

{% highlight html %}

<div id="container"></div>
<script>
    //Create ReportDesigner Instance
    $("#container").ejReportDesigner();
    var designerObj = $("#container").data("ejReportDesigner");
    designerObj.removeItem('Tablix1');
</script>

{% endhighlight %}

### saveReport()
{:#methods:savereport}

This method saves the report into the server.

<table>
  <thead>
    <tr>
      <th>Name</th>
      <th>Type</th>
      <th>Description</th>
    </tr>
  </thead>
  <tbody>
    <tr>
      <td class='name'>reportPath</td>
      <td class='type'>string(optional)</td>
      <td class='description'>Path of the ReportServer report</td>
    </tr>
  </tbody>
</table>

#### Example

{% highlight html %}

<div id="container"></div>
<script>
    // Create ReportDesigner Instance
    $("#container").ejReportDesigner();
    var designerObj = $("#container").data("ejReportDesigner");
    designerObj.saveReport();
</script>

{% endhighlight %}


### saveReportDefinition()
{:#methods:savereportdefinition}

This method returns the report in JSON or XML format.

<table>
  <thead>
    <tr>
      <th>Name</th>
      <th>Type</th>
      <th>Description</th>
    </tr>
  </thead>
  <tbody>
    <tr>
      <td class='name'>callback</td>
      <td class='type'>function</td>
      <td class='description'>Callback method to return the report data</td>
    </tr>
    <tr>
      <td class='name'>type</td>
      <td class='type'>string(optional)</td>
      <td class='string'>Specify the format as JSON or XML to save the report.</td>
    </tr>
  </tbody>
</table>

#### Example

{% highlight html %}

<div id="container"></div>
<script>
    // Create ReportDesigner Instance
    $("#container").ejReportDesigner();
    var designerObj = $("#container").data("ejReportDesigner");
    designerObj.saveReportDefinition((args: any) => {},'JSON');
</script>

{% endhighlight %}

### saveServerReportDialog()
{:#methods:saveserverreportdialog}

Opens the report designer browse dialog to save the report into server.

#### Example

{% highlight html %}

<div id="container"></div>
<script>
    // Create ReportDesigner Instance
    $("#container").ejReportDesigner();
    var designerObj = $("#container").data("ejReportDesigner");
    designerObj.saveServerReportDialog();
</script>

{% endhighlight %}

### saveToDevice()
{:#methods:savetodevice}

To download the designed report.

#### Example

{% highlight html %}

<div id="container"></div>
<script>
    // Create ReportDesigner Instance
    $("#container").ejReportDesigner();
    var designerObj = $("#container").data("ejReportDesigner");
    designerObj.saveToDevice();
</script>

{% endhighlight %}

### selectItems(itemNames)
{:#methods:selectitems}

Update the selection to report items at runtime.

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
			<td class="name">itemNames</td>
			<td class="type">array</td>
			<td class="description last">Name of the report items as string array.</td>
		</tr>
	</tbody>
</table>

#### Example

{% highlight html %}

<div id="container"></div>
<script>
    //Create ReportDesigner Instance
    $("#container").ejReportDesigner();
    var designerObj = $("#container").data("ejReportDesigner");
    var itemNames = ['Tablix1','Chart1','Rectangle2']
    designerObj.selectItems(itemNames);
</script>

{% endhighlight %}

### sendBackward()
{:#methods:sendbackward}

Visually move the selected report item behind its closest intersected report item.

#### Example

{% highlight html %}

<div id="container"></div>
<script>
    //Create ReportDesigner Instance
    $("#container").ejReportDesigner();
    var designerObj = $("#container").data("ejReportDesigner");
    designerObj.sendBackward();
</script>

{% endhighlight %}

### sendToBack()
{:#methods:sendtoback}

Visually move the selected report item behind all other intersected report items.

#### Example

{% highlight html %}

<div id="container"></div>
<script>
    //Create ReportDesigner Instance
    $("#container").ejReportDesigner();
    var designerObj = $("#container").data("ejReportDesigner");
    designerObj.sendToBack();
</script>

{% endhighlight %}

### showDesign()
{:#methods:showdesign}

Performs switch action from viewer to designer at runtime.

#### Example

{% highlight html %}

<div id="container"></div>
<script>
    // Create ReportDesigner Instance
    $("#container").ejReportDesigner();
    var designerObj = $("#container").data("ejReportDesigner");
    designerObj.showDesign();
</script>

{% endhighlight %}

### showNewReportDialog()
{:#methods:shownewreportdialog}

To open the new report dialog.

<table>
  <thead>
    <tr>
      <th>Name</th>
      <th>Type</th>
      <th>Description</th>
    </tr>
  </thead>
  <tbody>
    <tr>
      <td class='name'>callback</td>
      <td class='type'>function</td>
      <td class='description'>Callback method of new report dialog actions.</td>
    </tr>
  </tbody>
</table>

#### Example

{% highlight html %}

<div id="container"></div>
<script>
   // Create ReportDesigner Instance
   $("#container").ejReportDesigner();
   var designerObj = $("#container").data("ejReportDesigner");
   designerObj.showNewReportDialog((args: any) => {
   });
</script>

{% endhighlight %}

### showOpenSaveReportDialog()
{:#methods:showopensavereportdialog}

To open the server browse dialog.

<table>
  <thead>
    <tr>
      <th>Name</th>
      <th>Type</th>
      <th>Description</th>
    </tr>
  </thead>
  <tbody>
    <tr>
      <td class='name'>browseType</td>
      <td class='type'>enum(Open/Save)</td>
      <td class='description'>Open/Save the dialog type.</td>
    </tr>
    <tr>
      <td class='name'>callback</td>
      <td class='type'>function</td>
      <td class='description'>Callback method of open/save  dialog actions.</td>
    </tr>
    <tr>
      <td class='name'>reportName</td>
      <td class='type'>string(optional)</td>
      <td class='description'>Name of the report to save.</td>
    </tr>
  </tbody>
</table>

#### Example

{% highlight html %}

<div id="container"></div>
<script>
   // Create ReportDesigner Instance
   $("#container").ejReportDesigner();
   var designerObj = $("#container").data("ejReportDesigner");
   designerObj.showOpenSaveReportDialog(browseType, (args: any) => {
   });
</script>

{% endhighlight %}

### showPreview()
{:#methods:showpreview}

Performs switch action from designer to viewer at runtime.

#### Example

{% highlight html %}

<div id="container"></div>
<script>
    // Create ReportDesigner Instance
    $("#container").ejReportDesigner();
    var designerObj = $("#container").data("ejReportDesigner");
    designerObj.showPreview();
</script>

{% endhighlight %}

### undo()
{:#methods:undo}

Reverses the last action that was performed.

#### Example

{% highlight html %}

<div id="container"></div>
<script>
    //Create ReportDesigner Instance
    $("#container").ejReportDesigner();
    var designerObj = $("#container").data("ejReportDesigner");
    designerObj.undo();
</script>

{% endhighlight %}

### updateDataset(datasetName,dataset)
{:#methods:updatedataset}

Update the dataset in the report at runtime.

<table>
  <thead>
    <tr>
      <th>Name</th>
      <th>Type</th>
      <th>Description</th>
    </tr>
  </thead>
  <tbody>
    <tr>
      <td class='name'>datasetName</td>
      <td class='type'>string</td>
      <td class='description'>Name of the existing dataset.</td>
    </tr>
    <tr>
      <td class='name'>dataset</td>
      <td class='type'>object</td>
      <td class='description'>a JSON to define a connection properties for dataset.</td>
    </tr>
  </tbody>
</table>

#### Example

* Update embedded dataset

{% highlight html %}

<div id="container"></div>
<script>
    //Create ReportDesigner Instance
    $("#container").ejReportDesigner();
    var designerObj = $("#container").data("ejReportDesigner");
    var dataset = 
    { 
     __type:'Syncfusion.RDL.DOM.DataSet',
     Name:'DataSet2',
     Fields:[
          { __type: "Syncfusion.RDL.DOM.Field",DataField: "DepartmentID",Name: "DepartmentID",TypeName: "System.Int16",Value: null},
          { __type: "Syncfusion.RDL.DOM.Field",DataField: "Name",Name: "Name",TypeName: "System.String",Value: null},
          { __type: "Syncfusion.RDL.DOM.Field",DataField: "GroupName",Name: "GroupName",TypeName: "System.String",Value: null },
          { __type: "Syncfusion.RDL.DOM.Field",DataField: "ModifiedDate",Name: "ModifiedDate",TypeName: "System.DateTime",Value: null}
        ],
     Query: {
          __type: "Syncfusion.RDL.DOM.Query",
          CommandText: "SELECT [HumanResources].[Department].[DepartmentID],\n[HumanResources].[Department].[Name],\n[HumanResources].[Department].[GroupName],\n[HumanResources].[Department].[ModifiedDate] FROM [HumanResources].[Department]",
          CommandType: 0,
          DataSourceName: "DataSource1",
          QueryDesignerState: {
              __type: "Syncfusion.RDL.DOM.QueryDesignerState",
              Expressions: null,
              Filters: null,
              Joins: null,
              StoredProcedure: null,
              Tables: [
                {
                  __type: "Syncfusion.RDL.DOM.Table",
                  Columns: [
                    { __type: "Syncfusion.RDL.DOM.Column",AggregateTye: undefined,AliasName: null,IsDuplicate: false,
                    IsSelected: true, Name: "DepartmentID"
                    },
                    {__type: "Syncfusion.RDL.DOM.Column",AggregateTye: undefined,AliasName: null,IsDuplicate: false,
                    IsSelected: true,Name: "Name"
                    },
                    {__type: "Syncfusion.RDL.DOM.Column",AggregateTye: undefined,AliasName: null,IsDuplicate: false,
                    IsSelected: true,Name: "GroupName"
                    },
                    {__type: "Syncfusion.RDL.DOM.Column",AggregateTye: undefined,AliasName: null,IsDuplicate: false,
                    IsSelected: true,Name: "ModifiedDate"
                    }
                  ],
                  Name: "Department", 
                  Schema: "HumanResources",
                  SchemaLevels: [
                    { Name: "HumanResources",SchemaType: "Schema"},
                    {Name: "Tables",SchemaType: "Category"},
                    { Name: "Department",SchemaType: "Table"}
                  ]
                }
              ]
          },
          QueryParameters: [],
          Timeout: 0
          },
     CaseSensitivity:0,
     Collation:null,
     AccentSensitivity:0,
     KanatypeSensitivity:0,
     WidthSensitvity:0,
     Filters:[],
     SharedDataSet:null,
     InterpretSubtotalsAsDetails:0,
     DataSetInfo:null,
     DataSetObject:null
     };

designerObj.updateDataset('DataSet1',dataset);
</script>

{% endhighlight %}

* Update shared dataset

{% highlight html %}

<div id="container"></div>
<script>
    //Create Report Designer Instance
    $("#container").ejReportDesigner();
    var designerObj = $("#container").data("ejReportDesigner");
 
    var dataset = 
    { 
     __type:'Syncfusion.RDL.DOM.DataSet',
     Name:'DataSet2',
     Fields:[
          { __type: "Syncfusion.RDL.DOM.Field",DataField: "ProdCat",Name: "ProdCat",TypeName: "System.String",Value: null},
          { __type: "Syncfusion.RDL.DOM.Field",DataField: "SubCat",Name: "SubCat",TypeName: "System.String",Value: null},
          { __type: "Syncfusion.RDL.DOM.Field",DataField: "OrderYear",Name: "OrderYear",TypeName: "System.Int32",Value: null },
          { __type: "Syncfusion.RDL.DOM.Field",DataField: "OrderQtr",Name: "OrderQtr",TypeName: "System.String",Value: null},
          { __type: "Syncfusion.RDL.DOM.Field",DataField: "Sales",Name: "Sales",TypeName: "System.Decimal",Value: null}
        ],
     Query:null,
     CaseSensitivity:0,
     Collation:null,
     AccentSensitivity:0,
     KanatypeSensitivity:0,
     WidthSensitvity:0,
     Filters:[],
     SharedDataSet: {
            __type: "Syncfusion.RDL.DOM.SharedDataSet",
            QueryParameters: [],
            SharedDataSetReference: 'Sales'
     },
     InterpretSubtotalsAsDetails:0,
     DataSetInfo:null,
     DataSetObject:null
     };

    designerObj.updateDataset('DataSet1',dataset);
</script>

{% endhighlight %}

### updateDatasource(datasourceName,datasource)
{:#methods:updatedatasource}

Update the datasource in the report at runtime.

<table>
  <thead>
    <tr>
      <th>Name</th>
      <th>Type</th>
      <th>Description</th>
    </tr>
  </thead>
  <tbody>
    <tr>
      <td class='name'>datasourceName</td>
      <td class='type'>string</td>
      <td class='description'>Name of the existing datasource.</td>
    </tr>
    <tr>
      <td class='name'>datasource</td>
      <td class='type'>object</td>
      <td class='description'>a JSON to define a connection properties for datasource.</td>
    </tr>
  </tbody>
</table>

#### Example

{% highlight html %}

<div id="container"></div>
<script>
    //Create ReportDesigner Instance
    $("#container").ejReportDesigner();
    var designerObj = $("#container").data("ejReportDesigner");
    var datasource = { 
      __type:'Syncfusion.RDL.DOM.DataSource',
       Name:'DataSource2',
        Transaction:false,
         DataSourceReference:null,
         SecurityType:'DataBase',
         ConnectionProperties:{
            __type:'Syncfusion.RDL.DOM.ConnectionProperties', 
            ConnectString:'Data Source=mvc.syncfusion.com;Initial Catalog=AdventureWorks;',
             EmbedCredentials:false,
              DataProvider:'SQL',
             IsDesignState:false,
             IntegratedSecurity:false,
             UserName:'',
             PassWord:'',
             Prompt:'Specify the Username and password for DataSource DataSource2',
             CustomProperties:[]
              } 
         };

    designerObj.updateDatasource('DataSource1',datasource);
</script>

{% endhighlight %}


* Update shared datasource

{% highlight html %}

<div id="container"></div>
<script>
    //Create Report Designer Instance
    $("#container").ejReportDesigner();
    var designerObj = $("#container").data("ejReportDesigner");
    var datasource = 
    { 
      __type:'Syncfusion.RDL.DOM.DataSource',
      Name:'DataSource2',
      Transaction:false,
      DataSourceReference: 'AdventureWorks',
      SecurityType:'None',
      ConnectionProperties:null
    };

    designerObj.updateDatasource('DataSource1',datasource);
</script>

{% endhighlight %}

## Events

### ajaxBeforeLoad
{:#events:ajaxbeforeload}

This event will be triggered before AJAX loads.

<table>
  <thead>
    <tr>
      <th>Name</th>
      <th>Type</th>
      <th>Description</th>
    </tr>
  </thead>
  <tbody>
    <tr>
      <td class='name'>{% highlight html %}headers{% endhighlight %}</td>
      <td class='type'>array</td>
      <td class='description'>AJAX headers, we can pass any custom header through this property.</td>
    </tr>
    <tr>
      <td class='name'>{% highlight html %}data{% endhighlight %}</td>
      <td class='type'>object</td>
      <td class='description'>To pass the custom data while AJAX post back.</td>
    </tr>
    <tr>
      <td class='name'>{% highlight html %}reportDesignerToken{% endhighlight %}</td>
      <td class='type'>String</td>
      <td class='description'>Token of report designer.</td>
    </tr>
    <tr>
      <td class='name'>{% highlight html %}serviceAuthorizationToken{% endhighlight %}</td>
      <td class='type'>string</td>
      <td class='description'>Token of ReportingService.</td>
    </tr>
    <tr>
      <td class='name'>{% highlight html %}actionType{% endhighlight %}</td>
      <td class='type'>String</td>
      <td class='description'>Action type of AJAX call back.</td>
    </tr>
  </tbody>
</table>

#### Example 

{% highlight js %}

    $("#container").ejReportDesigner({
        ajaxBeforeLoad: function(args) {
            if (args && args.headers) {
                args.headers.push({ 'Key': 'keyCode', 'Value': ("Authorization") });
            }
        }
    });

{% endhighlight %}

### ajaxError
{:#events:ajaxerror}

This event will be triggered when AJAX result is failed.

#### Example 

{% highlight js %}

    $("#container").ejReportDesigner({
        ajaxError: function(args) {
            // Write your block of code
        }
    });

{% endhighlight %}

### ajaxSuccess
{:#events:ajaxsuccess}

This event will be triggered when AJAX result is succeeded.

#### Example 
 
{% highlight js %}

    $("#container").ejReportDesigner({
        ajaxSuccess: function(args) {
            // Write your block of code
        }
    });

{% endhighlight %}

### create
{:#events:create}

This event will be triggered when the Report Designer widget is created.

#### Example 

{% highlight js %}

    $("#container").ejReportDesigner({
        create: function(args) {
            // Write your block of code 
        }
    });

{% endhighlight %}

### destroy
{:#events:destroy}

This event will be triggered when the Report Designer widget is destroyed.

#### Example 

{% highlight js %}

    $("#container").ejReportDesigner({
        destroy: function(args) {
            // Write your block of code
        }
    });

{% endhighlight %}

### newDataClick
{:#events:newdataclick}

This event will be triggered while initiating new data click action. You can suppress the new data creation panel and perform custom actions.

#### Example 

{% highlight js %}

    $("#container").ejReportDesigner({
        newDataClick: function(args) {
            // Write your block of code
        }
    });

{% endhighlight %}

### openReportClick
{:#events:openreportclick}

This event will be triggered while clicking open menu items.

<table>
  <thead>
    <tr>
      <th>Name</th>
      <th>Type</th>
      <th>Description</th>
    </tr>
  </thead>
  <tbody>
    <tr>
      <td class='name'>{% highlight html %}target{% endhighlight %}</td>
      <td class='type'>jQuery</td>
      <td class='description'>DOM of the clicked target.</td>
    </tr>
    <tr>
      <td class='name'>{% highlight html %}select{% endhighlight %}</td>
      <td class='type'>string</td>
      <td class='description'>Name of selected item.</td>
    </tr>
  </tbody>
</table>

#### Example 

{% highlight js %}

    $("#container").ejReportDesigner({
        openReportClick: function(args) {
            // Write your block of code
        }
    });

{% endhighlight %}

### previewReport
{:#events:previewreport}

This event will be triggered while previewing the report in RDLC mode. It can be used to suppress the preview data dialog in RDLC mode.

<table>
  <thead>
    <tr>
      <th>Name</th>
      <th>Type</th>
      <th>Description</th>
    </tr>
  </thead>
  <tbody>
    <tr>
      <td class='name'>{% highlight html %}reportViewer{% endhighlight %}</td>
      <td class='type'>object</td>
      <td class='description'>Contains the instance of Report Viewer component.</td>
    </tr>
    <tr>
      <td class='name'>{% highlight html %}cancelDataInputDialog{% endhighlight %}</td>
      <td class='type'>boolean</td>
      <td class='description'>Specifies whether to show or hide preview data dialog.</td>
    </tr>
    <tr>
      <td class='name'>{% highlight html %}dataSets{% endhighlight %}</td>
      <td class='type'>array</td>
      <td class='description'>Contains the required data to load the report.</td>
    </tr>
  </tbody>
</table>

#### Example 

{% highlight js %}

    $("#container").ejReportDesigner({
        previewReport: function(args) {
            // Write your block of code
        }
    });

{% endhighlight %}

### reportModified
{:#events:reportmodified}

This event will be triggered when the report is modified.

<table>
  <thead>
    <tr>
      <th>Name</th>
      <th>Type</th>
      <th>Description</th>
    </tr>
  </thead>
  <tbody>
    <tr>
      <td class='name'>{% highlight html %}isModified{% endhighlight %}</td>
      <td class='type'>boolean</td>
      <td class='description'>Specifies whether the report is modified or not.</td>
    </tr>
    <tr>
      <td class='name'>{% highlight html %}reportName{% endhighlight %}</td>
      <td class='type'>string</td>
      <td class='description'>Name of Opened Report.</td>
    </tr>
  </tbody>
</table>

#### Example 

{% highlight js %}

    $("#container").ejReportDesigner({
        reportModified: function(args) {
            // Write your block of code
        }
    });

{% endhighlight %}

### reportOpened
{:#events:reportopened}
   
This event will be triggered when the report is opened.

<table>
  <thead>
    <tr>
      <th>Name</th>
      <th>Type</th>
      <th>Description</th>
    </tr>
  </thead>
  <tbody>
    <tr>
      <td class='name'>{% highlight html %}isServerReport{% endhighlight %}</td>
      <td class='type'>boolean</td>
      <td class='description'>
        Specifies whether report opened from device or server.
      </td>
    </tr>
    <tr>
      <td class='name'>{% highlight html %}reportName{% endhighlight %}</td>
      <td class='type'>string</td>
      <td class='description'>Name of Opened Report.</td>
    </tr>
  </tbody>
</table>

#### Example 

{% highlight js %}

    $("#container").ejReportDesigner({
        reportOpened: function(args) {
            // Write your block of code
        }
    });

{% endhighlight %}

### reportSaved
{:#events:reportsaved}

This event will be triggered when the report is saved.

<table>
  <thead>
    <tr>
      <th>Name</th>
      <th>Type</th>
      <th>Description</th>
    </tr>
  </thead>
  <tbody>
    <tr>
      <td class='name'>{% highlight html %}isServerReport{% endhighlight %}</td>
      <td class='type'>boolean</td>
      <td class='description'>
        Specifies whether report opened from device or server.
      </td>
    </tr>
    <tr>
      <td class='name'>{% highlight html %}reportAction{% endhighlight %}</td>
      <td class='type'>string</td>
      <td class='description'>States whether report is downloaded from ReportServer.</td>
    </tr>
  </tbody>
</table>

#### Example 

{% highlight js %}

    $("#container").ejReportDesigner({ 
        reportSaved: function (args) {
                // Write your block of code
        }
    });

{% endhighlight %}

### saveReportClick
{:#events:savereportclick}

This event will be triggered when the save menu items are clicked.

<table>
  <thead>
    <tr>
      <th>Name</th>
      <th>Type</th>
      <th>Description</th>
    </tr>
  </thead>
  <tbody>
    <tr>
      <td class='name'>{% highlight html %}target{% endhighlight %}</td>
      <td class='type'>jQuery</td>
      <td class='description'>
        DOM of the clicked target.
      </td>
    </tr>
    <tr>
      <td class='name'>{% highlight html %}select{% endhighlight %}</td>
      <td class='type'>string</td>
      <td class='description'>Name of selected item.</td>
    </tr>
  </tbody>
</table>

#### Example 

{% highlight js %}

    $("#container").ejReportDesigner({
        saveReportClick: function(args) {
            // Write your block of code
        }
    });

{% endhighlight %}

### toolbarClick
{:#events:toolbarclick}

This event will be triggered while clicking the toolbar items.

<table>
  <thead>
    <tr>
      <th>Name</th>
      <th>Type</th>
      <th>Description</th>
    </tr>
  </thead>
  <tbody>
    <tr>
      <td class='name'>{% highlight html %}target{% endhighlight %}</td>
      <td class='type'>jQuery</td>
      <td class='description'>
        DOM of the clicked target.
      </td>
    </tr>
    <tr>
      <td class='name'>{% highlight html %}click{% endhighlight %}</td>
      <td class='type'>string</td>
      <td class='description'>Name of clicked item.</td>
    </tr>
  </tbody>
</table>

#### Example 

{% highlight js %}

    $("#container").ejReportDesigner({
        toolbarClick: function(args) {
            // Write your block of code
        }
    });

{% endhighlight %}

### toolbarRendering
{:#events:toolbarrendering}

This event will be triggered on rendering the Report Designer toolbar.

#### Example 

{% highlight js %}

    $("#container").ejReportDesigner({
        toolbarRendering: function(args) {
            // Write your block of code 
        }
    });

{% endhighlight %}