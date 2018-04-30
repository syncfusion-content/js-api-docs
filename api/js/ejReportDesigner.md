---
layout: post
title: Properties, Methods and Events of ejReportDesigner Widget
description: Public API, Events documentation for ejReportDesigner
platform: js-api
metaname: 
metacontent: 
---

# ejReportDesigner

Report Designer allows to design the report that can be published in the Report Server or downloaded in the local physical path.

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

* module:ej.reportViewer.js

* module:ej.chart.js

* module:ej.circulargauge.js

* module:ej.lineargauge.js

* module:ej.bulletgraph.js

## Members

### locale `string`
{:#members:locale}

Specifies the locale for report designer.

#### Default Value

* "en-US"

#### Example

{% highlight html %}
 
<div id="container"></div> 
<script>          
    $("#container").ejReportDesigner(
        {
            locale: "fr-FR"
        });             
</script>

{% endhighlight %}

### reportPath  `string`	
{:#members:reportpath}

Gets or Sets the report path of server.

#### Default value 

<li>null</li>

#### Example 

{% highlight js %}

<div id="container"></div>
<script>
    $("#container").ejReportDesigner({
        reportPath: "/Sample Reports/invoice.rdl"
    });
</script>

{% endhighlight %}

### reportServerUrl `string`	
{:#members:reportserverurl}

Gets or Sets the reports server URL.

#### Default value 

<li>null</li>

#### Example 

{% highlight js %}

<div id="container"></div>
<script>
    $("#container").ejReportDesigner({
        reportServerUrl: "https://rsdev.syncfusion.com"
    });
</script>

{% endhighlight %}

### serviceAuthorizationToken `string`
{:#members:serviceauthorizationtoken}

Gets or sets the serviceAuthorizationToken to access the Report Server API services.

#### Default value 

<li>empty</li>

#### Example 

{% highlight js %}

<div id="container"></div>
<script type="text/javascript">
   $("#container").ejReportDesigner({ 
     serviceAuthorizationToken: token['token_type'] + ' ' + token['access_token'] 
     });
</script>

{% endhighlight %}

### serviceUrl `string`
{:#members:serviceurl}

Gets or Sets the URL of the  WebAPI service; it will be used for processing the report.

#### Default value

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

### toolbarSettings `object`
{:#members:toolbarsettings}

Specifies the toolbar settings.

### toolbarSettings.ToolbarItems `enum`
{:#members:toolbarsettings-toolbaritems}

Shows or hides the grouped items in the toolbar with the help of enum ej.ReportDesigner.ToolbarItems.

<ts name = "ej.ReportDesigner.ToolbarItems"/>
Specifies the toolbar items.
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
      <td class="name">Preview</td>
      <td class="description">Previews the active report in report viewer.</td>
    </tr>
    <tr>
      <td class="name">GridLine</td>
      <td class="description">Enables/Disables the gridline in active report.</td>
    </tr>
    <tr>
      <td class="name">Header</td>
      <td class="description">Enables header area in the report.</td>
    </tr>
    <tr>
      <td class="name">Footer</td>
      <td class="description">Enables footer area in the report.</td>
    </tr>
    <tr>
      <td class="name">EditDesign</td>
      <td class="description">Switches from preview to design view of the report.</td>
    </tr>
     <tr>
      <td class="name">All</td>
      <td class="description">Shows all the toolbar items.</td>
    </tr>
  </tbody>
</table>

#### Default value 

<li>ej.ReportDesigner.ToolbarItems.All</li>

#### Example

{% highlight html %}
 
<div id="container"></div>
<script>
    $("#container").ejReportDesigner({
        toolbarSettings: { items: ej.ReportDesigner.ToolbarItems.All }
    });
</script>

{% endhighlight %}

### toolbarSettings.showToolbar `boolean`
{:#members:toolbarsettings-showtoolbar}

Shows or hides the toolbar.

#### Default value 

<li>true</li>

#### Example

{% highlight html %}
 
<div id="container"></div>
<script>
    $("#container").ejReportDesigner({
        toolbarSettings: { showToolbar: true }
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

### canCopy()
{:#methods:cancopy}

Determines whether a copy operation is possible.

#### Returns

* boolean

#### Example

{% highlight html %}

<div id="container">ReportDesigner</div>
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

<div id="container">ReportDesigner</div>
<script>
    // Create ReportDesigner Instance
    $("#container").ejReportDesigner();
    var designerObj = $("#container").data("ejReportDesigner");
    designerObj.canCut();
</script>

{% endhighlight %}

### canDelete()
{:#methods:candelete}

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
    designerObj.canDelete();
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

Returns the bool value indicating whether the user can redo the previous action in the report.

#### Returns

* boolean

#### Example

{% highlight html %}

<div id="container">ReportDesigner</div>
<script>
    // Create ReportDesigner Instance
    $("#container").ejReportDesigner();
    var designerObj = $("#container").data("ejReportDesigner");
    designerObj.canRedo();
</script>

{% endhighlight %}

### canUndo()
{:#methods:canundo}

Returns a bool value indicating whether the user can undo the previous action in the report.

#### Returns

* boolean

#### Example

{% highlight html %}

<div id="container">ReportDesigner</div>
<script>
    // Create ReportDesigner Instance
    $("#container").ejReportDesigner();
    var designerObj = $("#container").data("ejReportDesigner");
    designerObj.canUndo();
</script>

{% endhighlight %}

### copy()
{:#methods:copy}

Copies the selected ReportItem from design panel to Report Designer internal clipboard.

#### Example

{% highlight html %}

<div id="container">ReportDesigner</div>
<script>
    // Create ReportDesigner Instance
    $("#container").ejReportDesigner();
    var designerObj = $("#container").data("ejReportDesigner");
    designerObj.copy();
</script>

{% endhighlight %}

### cut()
{:#methods:cut}

Cuts the selected ReportItem from design panel to Report Designer internal clipboard.

#### Example

{% highlight html %}

<div id="container">ReportDesigner</div>
<script>
    // Create ReportDesigner Instance
    $("#container").ejReportDesigner();
    var designerObj = $("#container").data("ejReportDesigner");
    designerObj.cut();
</script>

{% endhighlight %}

### delete()
{:#methods:delete}

Deletes the selected item from the report.

#### Example

{% highlight html %}

<div id="container">ReportDesigner</div>
<script>
    // Create ReportDesigner Instance
    $("#container").ejReportDesigner();
    var designerObj = $("#container").data("ejReportDesigner");
    designerObj.delete();
</script>

{% endhighlight %}

### hasReportChanges()
{:#methods:hasreportchanges}

Returns the bool value that specifies whether the report has changes or not.

#### Returns

* boolean

#### Example

{% highlight html %}

<div id="container">ReportDesigner</div>
<script>
    // Create ReportDesigner Instance
    $("#container").ejReportDesigner();
    var designerObj = $("#container").data("ejReportDesigner");
    designerObj.hasReportChanges();
</script>

{% endhighlight %}

### isNewReport()
{:#methods:isnewreport}

Returns the bool value that specifies whether the currently processing report is a new report or not.

#### Returns

* boolean

#### Example

{% highlight html %}

<div id="container">ReportDesigner</div> 
<script>
    // Create ReportDesigner Instance
    $("#container").ejReportDesigner();
    var designerObj = $("#container").data("ejReportDesigner");
    designerObj.isNewReport();
</script>

{% endhighlight %}

### isNewServerReport()
{:#methods:isnewserverreport}

Returns the bool value that specifies whether the currently processing report is a new server report or not.

#### Returns

* boolean

#### Example

{% highlight html %}

<div id="container">ReportDesigner</div>
<script>
    // Create ReportDesigner Instance
    $("#container").ejReportDesigner();
    var designerObj = $("#container").data("ejReportDesigner");
    designerObj.isNewServerReport();
</script>

{% endhighlight %}

### isServerReport()
{:#methods:isserverreport}

Returns the bool value that specifies whether the currently processing report is obtained from the server or local.

#### Returns

* boolean

#### Example

{% highlight html %}

<div id="container">ReportDesigner</div>
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

<div id="container">ReportDesigner</div>
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

<div id="container">ReportDesigner</div>
<script>
   // Create ReportDesigner Instance
   $("#container").ejReportDesigner();
   var designerObj = $("#container").data("ejReportDesigner");
   designerObj.newServerReport('Test1', 'ab018ae7-f747-49a1-9e26-759e35c0a0db');
</script>

{% endhighlight %}

### openReport()
{:#methods:openreport}

This method opens the report from the ReportServer.

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

### openReportFromDevice()
{:#methods:openreportfromdevice}

To open the report client browse dialog.

#### Example

{% highlight html %}

<div id="container">ReportDesigner</div>
<script>
    // Create ReportDesigner Instance
    $("#container").ejReportDesigner();
    var designerObj = $("#container").data("ejReportDesigner");
    designerObj.openReportFromDevice();
</script>

{% endhighlight %}

### openServerReportDialog()
{:#methods:openserverreportdialog}

To open the report open server browse dialog. 

#### Example

{% highlight html %}

<div id="container">ReportDesigner</div>
<script>
    // Create ReportDesigner Instance
    $("#container").ejReportDesigner();
    var designerObj = $("#container").data("ejReportDesigner");
    designerObj.openServerReportDialog();
</script>

{% endhighlight %}

### paste()
{:#methods:paste}

Pastes the selected ReportItem from Report Designer internal clipboard to design panel.

#### Example

{% highlight html %}

<div id="container">ReportDesigner</div>
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

<div id="container">ReportDesigner</div>
<script>
    // Create ReportDesigner Instance
    $("#container").ejReportDesigner();
    var designerObj = $("#container").data("ejReportDesigner");
    designerObj.redo();
</script>

{% endhighlight %}

### saveReport()
{:#methods:savereport}

This method saves the report into the ReportServer.

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

### saveServerReportDialog()
{:#methods:saveserverreportdialog}

To open the report save server browse dialog.

#### Example

{% highlight html %}

<div id="container">ReportDesigner</div>
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

<div id="container">ReportDesigner</div>
<script>
    // Create ReportDesigner Instance
    $("#container").ejReportDesigner();
    var designerObj = $("#container").data("ejReportDesigner");
    designerObj.saveToDevice();
</script>

{% endhighlight %}

### showDesign()
{:#methods:showdesign}

To show the report design.

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

<div id="container">ReportDesigner</div>
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

<div id="container">ReportDesigner</div>
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

To show the report preview.

#### Example

{% highlight html %}

<div id="container">ReportDesigner</div>
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

<div id="container">ReportDesigner</div>
<script>
    //Create ReportDesigner Instance
    $("#container").ejReportDesigner();
    var designerObj = $("#container").data("ejReportDesigner");
    designerObj.undo();
</script>

{% endhighlight %}

## Events

### ajaxBeforeLoad
{:#events:ajaxbeforeload}

This event will be triggered before AJAX loads.

#### Example 

{% highlight js %}

    $("#container").ejReportDesigner({
        ajaxBeforeLoad: function(args) {
            // Write your block of code
        }
    });

{% endhighlight %}

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
      <td class='type'>object array</td>
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

### openReportClick
{:#events:openreportclick}

This event will be triggered while clicking open menu items.

#### Example 

{% highlight js %}

    $("#container").ejReportDesigner({
        openReportClick: function(args) {
            // Write your block of code
        }
    });

{% endhighlight %}

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
      <td class='type'>name</td>
      <td class='description'>Name of selected item.</td>
    </tr>
  </tbody>
</table>

### reportModified
{:#events:reportmodified}

This event will be triggered when the report is modified.

#### Example 

{% highlight js %}

    $("#container").ejReportDesigner({
        reportModified: function(args) {
            // Write your block of code
        }
    });

{% endhighlight %}

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

### reportOpened
{:#events:reportopened}
   
This event will be triggered when the report is opened.

#### Example 

{% highlight js %}

    $("#container").ejReportDesigner({
        reportOpened: function(args) {
            // Write your block of code
        }
    });

{% endhighlight %}

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

### reportSaved
{:#events:reportsaved}

This event will be triggered when the report is saved.

#### Example 

{% highlight js %}

    $("#container").ejReportDesigner({ 
        reportSaved: function (args) {
                // Write your block of code
        }
    });

{% endhighlight %}

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

### saveReportClick
{:#events:savereportclick}

This event will be triggered when the save menu items are clicked.

#### Example 

{% highlight js %}

    $("#container").ejReportDesigner({
        saveReportClick: function(args) {
            // Write your block of code
        }
    });

{% endhighlight %}

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
      <td class='type'>name</td>
      <td class='description'>Name of selected item.</td>
    </tr>
  </tbody>
</table>

### toolbarClick
{:#events:toolbarclick}

This event will be triggered while clicking the toolbar items.

#### Example 

{% highlight js %}

    $("#container").ejReportDesigner({
        toolbarClick: function(args) {
            // Write your block of code
        }
    });

{% endhighlight %}

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
      <td class='type'>name</td>
      <td class='description'>Name of clicked item.</td>
    </tr>
  </tbody>
</table>

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