---
title: ejPdfViewer
description: API reference for ejPdfViewer
platform: js-api
control: ejPdfViewer
documentation: API
keywords: pdfviewer, ejPdfViewer, pdfviewer api, syncfusion, pdf viewer
---

# ejPdfViewer

PDF viewer JS is visualization component to view PDF documents. It is powered by HTML5/JavaScript and provides various control customizations.

#### Syntax

$(element).ejPdfViewer({serviceUrl: ‘../api/PdfViewer’});

#### Example


{% highlight html %}
<div id="viewer"></div>
<script type="text/javascript">
        $(function () {
            $("#viewer").ejPdfViewer({ serviceUrl: '../api/PdfViewer'});
});
</script>
{% endhighlight %}


#### Requires

* module:jquery.js
* module:jquery.easing.min.js
* module:ej.core.js
* module:ej.pdfviewer.js
* module:ej.dropdownlist.js
* module:ej.toolbar.js
* module:ej.button.js
* module:ej.waitingpopup.js
* module:ej.scroller.js

## Members

### locale `string`

{:#members:locale}

Specifies the locale information of the PDF viewer.

**Default Value**: “en-US”

#### Example:

{% highlight html %}
<div id="viewer"></div>
<script type="text/javascript">
        $(function () {
            $("#viewer").ejPdfViewer({ serviceUrl: '../api/PdfViewer', locale:"fr-FR" });
        });
</script>
{% endhighlight %}


### toolbarSettings `object`

{:#members:toolbarsettings}

Specifies the toolbar settings.

### toolbarSettings.showToolTip `boolean`

{:#members:toolbarsettings-showtooltip}

Shows or hides the tooltip of the toolbar items.

**Default Value**: true

#### Example:

{% highlight html %}
<div id="viewer"></div>
<script type="text/javascript">
        $(function () {
            $("#viewer").ejPdfViewer({ serviceUrl: '../api/PdfViewer', toolbarSettings: { showTooltip: false } });
        });
</script>
{% endhighlight %}


### toolbarSettings.toolbarItem `enum`

{:#members:toolbarsettings-toolbaritem}

<ts name="ej.PdfViewer.ToolbarItems"/>

Shows or hides the grouped items in the toolbar with the help of enum ej.PdfViewer.ToolbarItems

<table class="params">
<thead>
<tr>
<th>
Name
</th>
<th>
Description
</th>
</tr>
</thead>
<tbody>
<tr>
<td class="name">
MagnificationTools
</td>
<td class="description">
Shows only magnification tools in the toolbar.
</td>
</tr>
<tr>
<td class="name">
PageNavigationTools
</td>
<td class="description">
Shows only page navigation tools in the toolbar.
</td>
</tr>
<tr>
<td class="name">
PrintTools
</td>
<td class="description">
Shows only print tool in the toolbar.
</td>
</tr>
<tr>
<td class="name">
DownloadTool
</td>
<td class="description">
Shows only download tool in the toolbar.
</td>
</tr>
<tr>
<td class="name">
All
</td>
<td class="description">
Shows all the toolbar items.
</td>
</tr>
</tbody>
</table>

**Default value:** ej.PdfViewer.ToolbarItems.All

#### Example:

Below code snippet shows only the magnification tools in the toolbar.

{% highlight html %}
<div id="viewer"></div>
<script type="text/javascript">
        $(function () {
           $("#viewer").ejPdfViewer({ serviceUrl: '../api/PdfViewer', toolbarSettings: { toolbarItem: ej.PdfViewer.ToolbarItems.MagnificationTools } });
        });
</script>
{% endhighlight %}

### serverActionSettings `object`

{:#members:serverActionSettings}

Specifies the name of the action method in the server.

### serverActionSettings.load `string`

{:#members:serverActionSettings-load}

Specifies the name of the action method used for loading the PDF document.

**Default Value**: Load

### serverActionSettings.fileUpload `string`

{:#members:serverActionSettings-fileUpload}

Specifies the name of the action method used for uploading the PDF document to the PDF viewer control.

**Default Value**: FileUpload

### serverActionSettings.print `string`

{:#members:serverActionSettings-print}

Specifies the name of the action method used for printing the PDF document in the PDF viewer control.

**Default Value**: Print

### serverActionSettings.download `string`

{:#members:serverActionSettings-download}

Specifies the name of the action method used for downloading the PDF document from the PDF viewer control.

**Default Value**: Download

#### Example:

{% highlight html %}
<div id="viewer"></div>
<script type="text/javascript">
        $(function () {
            $("#viewer").ejPdfViewer({ serviceUrl: '../api/PdfViewer', serverActionSettings: { load: "Load", fileUpload: "FileUpload", print: "Print", download: "Download" } });
        });
</script>
{% endhighlight %}

### serviceUrl `string`

{:#members:serviceurl}

Sets the PDF Web API service URL

### documentPath `string`

{:#members:documentPath}

Sets the PDF document path for initial loading.

#### Example:

{% highlight html %}
<div id="viewer"></div>
<script type="text/javascript">
        $(function () {
            $("#viewer").ejPdfViewer({ serviceUrl: '../api/PdfViewer', documentPath: "HTTP Succinctly.pdf" });
        });
</script>
{% endhighlight %}

### pageCount `number`

{:#members:pagecount}

Gets the total number of pages in PDF document.

#### Example:

{% highlight javascript %}
var pdfviewerObj = $("#viewer").data("ejPdfViewer");
var totalPages = pdfviewerObj.pageCount;
{% endhighlight %}


### currentPageNumber `number`

{:#members:currentpagenumber}

Gets the number of the page being displayed in the PDF viewer.

#### Example:

{% highlight javascript %}
var pdfviewerObj = $("#viewer").data("ejPdfViewer");
var currentPage = pdfviewerObj.currentPageNumber;
{% endhighlight %}


### zoomPercentage `number`

{:#members:zoompercentage}

Gets the current zoom percentage of the PDF document in viewer.

#### Example:

{% highlight javascript %}
var pdfviewerObj = $("#viewer").data("ejPdfViewer");
var currentZoom = pdfviewerObj.zoomPercentage;
{% endhighlight %}


### pdfService `enum`

{:#members:pdfservice}

<ts name="ej.PdfViewer.PdfService"/>

Specifies the location of the supporting PDF service

<table class="params">
<thead>
<tr>
<th>
Name
</th>
<th>
Description
</th>
</tr>
</thead>
<tbody>
<tr>
<td class="name">
Local
</td>
<td class="description">
Denotes that the service is located in the local project
</td>
</tr>
<tr>
<td class="name">
Remote
</td>
<td class="description">
Denotes that the service is hosted in the remote server
</td>
</tr>
</tbody>
</table>

**Default value:** ej.PdfViewer.PdfService.Local

#### Example:

The below code snippet shows the service accessed from remote server.


{% highlight javascript %}
<div id="viewer"></div>
<script type="text/javascript">
        $(function () {
           $("#viewer").ejPdfViewer({serviceUrl: 'http://mvc.syncfusion.com/PDFViewer/pdfviewer.asmx/PostViewerAction', pdfService : ej.PdfViewer.PdfService.Remote});
        });
</script>
{% endhighlight %}


### hyperlinkOpenState `enum`

{:#members:hyperlinkopenstate}

<ts name="ej.PdfViewer.LinkTarget"/>

Specifies the open state of the hyperlink in the PDF document.

<table class="params">
<thead>
<tr>
<th>
Name
</th>
<th>
Description
</th>
</tr>
</thead>
<tbody>
<tr>
<td class="name">
Default
</td>
<td class="description">
Opens the hyperlink in the same tab of the browser. 
</td>
</tr>
<tr>
<td class="name">
NewTab
</td>
<td class="description">
Opens the hyperlink in a new tab of the browser.
</td>
</tr>
<tr>
<td class="name">
NewWindow
</td>
<td class="description">
Opens the hyperlink in a new window of the browser.
</td>
</tr>
</tbody>
</table>

**Default value:** ej.PdfViewer.LinkTarget.Default

#### Example:

The below code snippet shows the hyperlink opened in a new tab.


{% highlight javascript %}
<div id="viewer"></div>
<script type="text/javascript">
        $(function () {
           $("#viewer").ejPdfViewer({ serviceUrl: '../api/PdfViewer', hyperlinkOpenState : ej.PdfViewer.LinkTarget.NewTab});
        });
</script>
{% endhighlight %}


### enableHyperlink `boolean`
{:#members:enablehyperlink}

Enables or disables the hyperlinks in PDF document.

**Default Value**: true

##### Example:

{% highlight javascript %}
<div id="viewer"></div>
<script type="text/javascript">
        $(function () {
            $("#viewer").ejPdfViewer({ serviceUrl: '../api/PdfViewer', enableHyperlink: false });
        });
</script>	
{% endhighlight %}

### enableTextSelection `boolean`
{:#members:enableTextSelection}

Enables or disables the text selection in PDF document.

**Default Value**: true

##### Example:

{% highlight javascript %}
<div id="viewer"></div>
<script type="text/javascript">
        $(function () {
            $("#viewer").ejPdfViewer({ serviceUrl: '../api/PdfViewer', enableTextSelection: false });
        });
</script>	
{% endhighlight %}

### isResponsive `boolean`
{:#members:isResponsive}

Enables or disables the responsiveness of the PDF viewer control during the window resize.

**Default Value**: true

#### Example

{% highlight javascript %}

<div id="viewer"></div>
<script type="text/javascript">
        $(function () {
            $("#viewer").ejPdfViewer({ serviceUrl: '../api/PdfViewer', isResponsive: false });
        });
</script>	

{% endhighlight %}

### isDocumentEdited `boolean`
{:#members:isDocumentEdited}

Checks whether the PDF document is edited. 

**Default Value**: false

#### Example

{% highlight javascript %}

<div id="viewer"></div>
<script type="text/javascript">
var pdfviewerObj = $("#viewer").data("ejPdfViewer");
var isEdited = pdfviewerObj.isDocumentEdited;
</script>	

{% endhighlight %}

### allowClientBuffering `boolean`
{:#members:allowClientBuffering}

Enables or disables the buffering of the PDF pages in the client side.

**Default Value**: false

##### Example:

{% highlight javascript %}
<div id="viewer"></div>
<script type="text/javascript">
        $(function () {
            $("#viewer").ejPdfViewer({ serviceUrl: '../api/PdfViewer', allowClientBuffering: true });
        });
</script>	
{% endhighlight %}

### fileName `string`

{:#members:filename}

Gets the name of the PDF document which loaded in the ejPdfViewer control for downloading. 

#### Example:

{% highlight javascript %}
<div id="viewer"></div>
<script type="text/javascript">
var pdfviewerObj = $("#viewer").data("ejPdfViewer");
var fileName = pdfviewerObj.fileName;
</script>	
{% endhighlight %}


## Methods

### load(fileName)

{:#methods:load}

Loads the document with the filename and displays it in PDF viewer.

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
fileName</td>
<td class="type"><span class="param-type">string</span></td>
<td class="description">File name to be loaded</td>
</tr>
</tbody>
</table>

#### Example:

{% highlight javascript %}
var pdfviewerObj = $("#viewer").data("ejPdfViewer");
pdfviewerObj.load("Manual");
{% endhighlight %}

### showToolbar(show)

{:#methods:showtoolbar}

Shows/hides the toolbar in the PDF viewer.

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
show</td>
<td class="type"><span class="param-type">boolean</span></td>
<td class="description">shows/hides the toolbar</td>
</tr>
</tbody>
</table>

#### Example:

{% highlight javascript %}
var pdfviewerObj = $("#viewer").data("ejPdfViewer");
pdfviewerObj.showToolbar(false);
{% endhighlight %}

### print()

{:#methods:print}

Prints the PDF document.

#### Example:

{% highlight javascript %}
var pdfviewerObj = $("#viewer").data("ejPdfViewer");
pdfviewerObj.print();
{% endhighlight %}

### abortPrint()
{:#methods:abortprint}

Abort the printing function and restores the PDF viewer.

#### Example:

{% highlight javascript %}
var pdfviewerObj = $("#viewer").data("ejPdfViewer");
pdfviewerObj.abortPrint();
{% endhighlight %}


### showPrintTools(show)
{:#methods:showprinttools}

Shows/hides the print icon in the toolbar.

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
show</td>
<td class="type"><span class="param-type">boolean</span></td>
<td class="description">shows/hides print button in the toolbar</td>
</tr>
</tbody>
</table>

#### Example:

{% highlight javascript %}
var pdfviewerObj = $("#viewer").data("ejPdfViewer");
pdfviewerObj.showPrintTools(false);
{% endhighlight %}


### download()
{:#methods:download}

Downloads the PDF document being loaded in the ejPdfViewer control.

#### Example:

{% highlight javascript %}
var pdfviewerObj = $("#viewer").data("ejPdfViewer");
pdfviewerObj.download();
{% endhighlight %}


### showDownloadTool(show)
{:#methods:showdownloadtool}

Shows/hides the download tool in the toolbar.

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
show</td>
<td class="type"><span class="param-type">boolean</span></td>
<td class="description">shows/hides download button in the toolbar</td>
</tr>
</tbody>
</table>

#### Example:

{% highlight javascript %}
var pdfviewerObj = $("#viewer").data("ejPdfViewer");
pdfviewerObj.showDownloadTool(false);
{% endhighlight %}

### showPageNavigationTools(show)

{:#methods:showpagenavigationtools}

Shows/hides the page navigation tools in the toolbar

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
show</td>
<td class="type"><span class="param-type">boolean</span></td>
<td class="description">shows/hides navigation tools in the toolbar</td>
</tr>
</tbody>
</table>

#### Example:

{% highlight javascript %}
var pdfviewerObj = $("#viewer").data("ejPdfViewer");
pdfviewerObj.showPageNavigationTools(false);
{% endhighlight %}

### goToPage(pageNumber)

{:#methods:gotopage}

Navigates to the specific page in the PDF document. If the page is not available for the given pageNumber, PDF viewer retains the existing page in view.

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
pageNumber</td>
<td class="type"><span class="param-type">number</span></td>
<td class="description">navigates to the page number in the PDF document</td>
</tr>
</tbody>
</table>

#### Example:

{% highlight javascript %}
var pdfviewerObj = $("#viewer").data("ejPdfViewer");
pdfviewerObj.goToPage(4);
{% endhighlight %}


### goToLastPage()

{:#methods:gotolastpage}

Navigates to the last page of the PDF document.

#### Example:

{% highlight javascript %}
var pdfviewerObj = $("#viewer").data("ejPdfViewer");
pdfviewerObj.goToLastPage();
{% endhighlight %}


### goToFirstPage()

{:#methods:gotofirstpage}

Navigates to the first page of PDF document.

#### Example:

{% highlight javascript %}
var pdfviewerObj = $("#viewer").data("ejPdfViewer");
pdfviewerObj.goToFirstPage();
{% endhighlight %}


### goToNextPage()

{:#methods:gotonextpage}

Navigates to the next page of the PDF document.

#### Example:

{% highlight javascript %}
var pdfviewerObj = $("#viewer").data("ejPdfViewer");
pdfviewerObj.goToNextPage();
{% endhighlight %}


### goToPreviousPage()

{:#methods:gotopreviouspage}

Navigates to the previous page of the PDF document.

#### Example:

{% highlight javascript %}
var pdfviewerObj = $("#viewer").data("ejPdfViewer");
pdfviewerObj.goToPreviousPage();
{% endhighlight %}

### showMagnificationTools(show)

{:#methods:showmagnificationtools}

Shows/hides the zoom tools in the toolbar.

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
show</td>
<td class="type"><span class="param-type">boolean</span></td>
<td class="description">shows/hides zoom tools in the toolbar</td>
</tr>
</tbody>
</table>

#### Example:

{% highlight javascript %}
var pdfviewerObj = $("#viewer").data("ejPdfViewer");
pdfviewerObj.showMagnificationTools(false);
{% endhighlight %}


### fitToPage()

{:#methods:fittopage}

Scales the page to fit the page in the container in the control.

#### Example:

{% highlight javascript %}
var pdfviewerObj = $("#viewer").data("ejPdfViewer");
pdfviewerObj.fitToPage();
{% endhighlight %}


### fitToWidth()

{:#methods:fittowidth}

Scales the page to fit the page width to the width of the container in the control.

#### Example:

{% highlight javascript %}
var pdfviewerObj = $("#viewer").data("ejPdfViewer");
pdfviewerObj.fitToWidth();
{% endhighlight %}


### zoomIn()

{:#methods:zoomin}

Magnifies the page to the next value in the zoom drop down list.

#### Example:

{% highlight javascript %}
var pdfviewerObj = $("#viewer").data("ejPdfViewer");
pdfviewerObj.zoomIn();
{% endhighlight %}


### zoomOut()

{:#methods:zoomout}

Shrinks the page to the previous value in the magnification in the drop down list.

#### Example:

{% highlight javascript %}
var pdfviewerObj = $("#viewer").data("ejPdfViewer");
pdfviewerObj.zoomOut();
{% endhighlight %}


### zoomTo(zoomValue)

{:#methods:zoomto}

Scales the page to the specified percentage ranging from 50 to 400. If the given zoomValue is less than 50 or greater than 400; the PDF viewer scales the page to 50 and 400 respectively.

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
zoomValue</td>
<td class="type"><span class="param-type">number</span></td>
<td class="description">zoom value for scaling the pages in the PDF Viewer</td>
</tr>
</tbody>
</table>

#### Example:

{% highlight javascript %}
var pdfviewerObj = $("#viewer").data("ejPdfViewer");
pdfviewerObj.zoomTo(130);
{% endhighlight %}


### unload()

{:#methods:unload}

Unloads the PDF document being displayed in the PDF viewer.
 
#### Example:

{% highlight javascript %}
var pdfviewerObj = $("#viewer").data("ejPdfViewer");
pdfviewerObj.unload();
{% endhighlight %}



## Events

### documentLoad

{:#events:documentload}

Triggers when the PDF document gets loaded and is ready to view in the Control.
<table>
<thead>
<tr>
<th>
{{'**Name**'| markdownify }}
</th>
<th>
{{'**Type**'| markdownify }}
</th>
<th>
{{'**Description**'| markdownify }}
</th>
</tr>
</thead>
<tbody>
<tr>
<td class="name">
argument
</td>
<td class="type">
object
</td>
<td class="description">
Event parameters from PDF viewer
<table>
<thead>
<tr>
<th>
{{'**Name**'| markdownify }}
</th>
<th>
{{'**Type**'| markdownify }}
</th>
<th>
{{'**Description**'| markdownify }}
</th>
</tr>
</thead>
<tbody>
<tr>
<td class="name">
cancel
</td>
<td class="type">
boolean
</td>
<td class="description">
true, if the event should be canceled; otherwise, false.
</td>
</tr>
<tr>
<td class="name">
model
</td>
<td class="type">
object
</td>
<td class="description">
Returns the PDF viewer model
</td>
</tr>
<tr>
<td class="name">
type
</td>
<td class="type">
string
</td>
<td class="description">
Returns the name of the event
</td>
</tr>
<tr>
<td class="name">
fileName
</td>
<td class="type">
string
</td>
<td class="description">
Returns the PDF document name displaying in the PDF viewer.
</td>
</tr>
</tbody>
</table>
</td>
</tr>
</tbody>
</table>

#### Example:

{% highlight html %}
<script type="text/javascript">
        $(function () {
            var obj = $("#viewer").ejPdfViewer({ serviceUrl: '../api/PdfViewer', documentLoad:"documentLoaded" });
        });
        function documentLoaded(args) {
            alert("The document" +args.fileName + "is ready to view");
        }
</script>
{% endhighlight %}


### documentUnload

{:#events:documentunload}

Triggers when the PDF document gets unloaded from the PDF viewer.
<table>
<thead>
<tr>
<th>
{{'**Name**'| markdownify }}
</th>
<th>
{{'**Type**'| markdownify }}
</th>
<th>
{{'**Description**'| markdownify }}
</th>
</tr>
</thead>
<tbody>
<tr>
<td class="name">
argument
</td>
<td class="type">
object
</td>
<td class="description">
Event parameters from PDF viewer
<table>
<thead>
<tr>
<th>
{{'**Name**'| markdownify }}
</th>
<th>
{{'**Type**'| markdownify }}
</th>
<th>
{{'**Description**'| markdownify }}
</th>
</tr>
</thead>
<tbody>
<tr>
<td class="name">
cancel
</td>
<td class="type">
boolean
</td>
<td class="description">
true, if the event should be canceled; otherwise, false.
</td>
</tr>
<tr>
<td class="name">
model
</td>
<td class="type">
object
</td>
<td class="description">
Returns the PDF viewer model
</td>
</tr>
<tr>
<td class="name">
type
</td>
<td class="type">
string
</td>
<td class="description">
Returns the name of the event
</td>
</tr>
</tbody>
</table>
</td>
</tr>
</tbody>
</table>

#### Example:

{% highlight html %}
<script type="text/javascript">
        $(function () {
            var obj = $("#viewer").ejPdfViewer({ serviceUrl: '../api/PdfViewer', documentUnload:"documentUnloaded" });
        });
        function documentUnloaded(args) {
            alert("The PDF document is unloaded from the PDF viewer");
        }
</script>
{% endhighlight %}


### pageChange

{:#events:pagechange}

Triggers when there is change in current page number.
<table>
<thead>
<tr>
<th>
{{'**Name**'| markdownify }}
</th>
<th>
{{'**Type**'| markdownify }}
</th>
<th>
{{'**Description**'| markdownify }}
</th>
</tr>
</thead>
<tbody>
<tr>
<td class="name">
argument
</td>
<td class="type">
object
</td>
<td class="description">
Event parameters from PDF viewer
<table>
<thead>
<tr>
<th>
{{'**Name**'| markdownify }}
</th>
<th>
{{'**Type**'| markdownify }}
</th>
<th>
{{'**Description**'| markdownify }}
</th>
</tr>
</thead>
<tbody>
<tr>
<td class="name">
cancel
</td>
<td class="type">
boolean
</td>
<td class="description">
true, if the event should be canceled; otherwise, false.
</td>
</tr>
<tr>
<td class="name">
model
</td>
<td class="type">
object
</td>
<td class="description">
Returns the PDF viewer model
</td>
</tr>
<tr>
<td class="name">
type
</td>
<td class="type">
string
</td>
<td class="description">
Returns the name of the event
</td>
</tr>
<tr>
<td class="name">
currentPageNumber
</td>
<td class="type">
number
</td>
<td class="description">
Returns the current page number in view.
</td>
</tr>
</tbody>
</table>
</td>
</tr>
</tbody>
</table>

#### Example:

{% highlight html %}
<script type="text/javascript">
        $(function () {
            var obj = $("#viewer").ejPdfViewer({ serviceUrl: '../api/PdfViewer', pageChange:"currentPageChanged" });
        });
        function currentPageChanged(args) {
            alert("The current page number is " + args.currentPageNumber);
        }
</script>
{% endhighlight %}


### zoomChange

{:#events:zoomchange}

Triggers when there is change in the magnification value.
<table>
<thead>
<tr>
<th>
{{'**Name**'| markdownify }}
</th>
<th>
{{'**Type**'| markdownify }}
</th>
<th>
{{'**Description**'| markdownify }}
</th>
</tr>
</thead>
<tbody>
<tr>
<td class="name">
Argument
</td>
<td class="type">
object
</td>
<td class="description">
Event parameters from PDF viewer
<table>
<thead>
<tr>
<th>
{{'**Name**'| markdownify }}
</th>
<th>
{{'**Type**'| markdownify }}
</th>
<th>
{{'**Description**'| markdownify }}
</th>
</tr>
</thead>
<tbody>
<tr>
<td class="name">
cancel
</td>
<td class="type">
boolean
</td>
<td class="description">
true, if the event should be canceled; otherwise, false.
</td>
</tr>
<tr>
<td class="name">
model
</td>
<td class="type">
object
</td>
<td class="description">
Returns the PDF viewer model
</td>
</tr>
<tr>
<td class="name">
type
</td>
<td class="type">
string
</td>
<td class="description">
Returns the name of the event.
</td>
</tr>
<tr>
<td class="name">
previousZoomPercentage
</td>
<td class="type">
number
</td>
<td class="description">
Returns the previous zoom percentage of the PDF viewer control
</td>
</tr>
<tr>
<td class="name">
currentZoomPercentage
</td>
<td class="type">
number
</td>
<td class="description">
Returns the current zoom percentage of the PDF viewer control
</td>
</tr>
</tbody>
</table>
</td>
</tr>
</tbody>
</table>

#### Example:

{% highlight html %}
<script type="text/javascript">
        $(function () {
            var obj = $("#viewer").ejPdfViewer({ serviceUrl: '../api/PdfViewer', zoomChange: "zoomChanged" });
        });
        function zoomChanged(args) {
            alert("The magnification changes from " + args.previousZoomPercentage + " to" + args.currentZoomPercentage);
        }
</script>
{% endhighlight %}


### hyperlinkClick

{:#events:hyperlinkclick}

Triggers when hyperlink in the PDF Document is clicked
<table>
<thead>
<tr>
<th>
{{'**Name**'| markdownify }}
</th>
<th>
{{'**Type**'| markdownify }}
</th>
<th>
{{'**Description**'| markdownify }}
</th>
</tr>
</thead>
<tbody>
<tr>
<td class="name">
argument
</td>
<td class="type">
object
</td>
<td class="description">
Event parameters from PDF viewer
<table>
<thead>
<tr>
<th>
{{'**Name**'| markdownify }}
</th>
<th>
{{'**Type**'| markdownify }}
</th>
<th>
{{'**Description**'| markdownify }}
</th>
</tr>
</thead>
<tbody>
<tr>
<td class="name">
cancel
</td>
<td class="type">
boolean
</td>
<td class="description">
true, if the event should be canceled; otherwise, false.
</td>
</tr>
<tr>
<td class="name">
model
</td>
<td class="type">
object
</td>
<td class="description">
Returns the PDF viewer model
</td>
</tr>
<tr>
<td class="name">
type
</td>
<td class="type">
string
</td>
<td class="description">
Returns the name of the event
</td>
</tr>
<tr>
<td class="name">
hyperlink
</td>
<td class="type">
string
</td>
<td class="description">
Returns the clicked hyperlink
</td>
</tr>
</tbody>
</table>
</td>
</tr>
</tbody>
</table>

#### Example:

{% highlight html %}
<script type="text/javascript">
        $(function () {
       $("#viewer").ejPdfViewer({ serviceUrl: '../api/PdfViewer', hyperlinkClick:"onHyperlinkClicked" });
        });
        function onHyperlinkClicked(args) {
            alert("The hyperlink is " + args.hyperlink);
        }
</script>
{% endhighlight %}


### beforePrint

{:#events:beforeprint}

Triggers before the printing starts.
<table>
<thead>
<tr>
<th>
{{'**Name**'| markdownify }}
</th>
<th>
{{'**Type**'| markdownify }}
</th>
<th>
{{'**Description**'| markdownify }}
</th>
</tr>
</thead>
<tbody>
<tr>
<td class="name">
argument
</td>
<td class="type">
object
</td>
<td class="description">
Event parameters from PDF viewer
<table>
<thead>
<tr>
<th>
{{'**Name**'| markdownify }}
</th>
<th>
{{'**Type**'| markdownify }}
</th>
<th>
{{'**Description**'| markdownify }}
</th>
</tr>
</thead>
<tbody>
<tr>
<td class="name">
cancel
</td>
<td class="type">
boolean
</td>
<td class="description">
True, if the event should be canceled; otherwise, false.
</td>
</tr>
<tr>
<td class="name">
model
</td>
<td class="type">
object
</td>
<td class="description">
Returns the PDF viewer model
</td>
</tr>
<tr>
<td class="name">
type
</td>
<td class="type">
string
</td>
<td class="description">
Returns the name of the event
</td>
</tr>
</tbody>
</table>
</td>
</tr>
</tbody>
</table>

#### Example:

{% highlight html %}
<script type="text/javascript">
        $(function () {
            var obj = $("#viewer").ejPdfViewer({ serviceUrl: '../api/PdfViewer', brforePrint: "beforePrint" });
        });
        function beforePrint() {
            alert("Printing started successfully");
        }
</script>
{% endhighlight %}

{:#events:}

### afterPrint

{:#events:afterprint}

Triggers after the printing is completed.
<table>
<thead>
<tr>
<th>
{{'**Name**'| markdownify }}
</th>
<th>
{{'**Type**'| markdownify }}
</th>
<th>
{{'**Description**'| markdownify }}
</th>
</tr>
</thead>
<tbody>
<tr>
<td class="name">
argument
</td>
<td class="type">
object
</td>
<td class="description">
Event parameters from PDF viewer
<table>
<thead>
<tr>
<th>
{{'**Name**'| markdownify }}
</th>
<th>
{{'**Type**'| markdownify }}
</th>
<th>
{{'**Description**'| markdownify }}
</th>
</tr>
</thead>
<tbody>
<tr>
<td class="name">
cancel
</td>
<td class="type">
boolean
</td>
<td class="description">
True, if the event should be canceled; otherwise, false.
</td>
</tr>
<tr>
<td class="name">
model
</td>
<td class="type">
object
</td>
<td class="description">
Returns the PDF viewer model
</td>
</tr>
<tr>
<td class="name">
type
</td>
<td class="type">
string
</td>
<td class="description">
Returns the name of the event
</td>
</tr>
</tbody>
</table>
</td>
</tr>
</tbody>
</table>

#### Example:

{% highlight html %}
<script type="text/javascript">
        $(function () {
            var obj = $("#viewer").ejPdfViewer({ serviceUrl: '../api/PdfViewer', afterPrint: "afterPrint" });
        });
        function afterPrint() {
            alert("Printing completed successfully");
        }
</script>
{% endhighlight %}


### pageClick

{:#events:pageclick}

Triggers when the mouse click is performed over the page of the PDF document.
<table>
<thead>
<tr>
<th>
{{'**Name**'| markdownify }}
</th>
<th>
{{'**Type**'| markdownify }}
</th>
<th>
{{'**Description**'| markdownify }}
</th>
</tr>
</thead>
<tbody>
<tr>
<td class="name">
argument
</td>
<td class="type">
object
</td>
<td class="description">
Event parameters from PDF viewer
<table>
<thead>
<tr>
<th>
{{'**Name**'| markdownify }}
</th>
<th>
{{'**Type**'| markdownify }}
</th>
<th>
{{'**Description**'| markdownify }}
</th>
</tr>
</thead>
<tbody>
<tr>
<td class="name">
cancel
</td>
<td class="type">
boolean
</td>
<td class="description">
True, if the event should be canceled; otherwise, false.
</td>
</tr>
<tr>
<td class="name">
model
</td>
<td class="type">
object
</td>
<td class="description">
Returns the PDF viewer model
</td>
</tr>
<tr>
<td class="name">
type
</td>
<td class="type">
string
</td>
<td class="description">
Returns the name of the event
</td>
</tr>
<tr>
<td class="name">
offsetX
</td>
<td class="type">
number
</td>
<td class="description">
Returns the current X position
</td>
</tr>
<tr>
<td class="name">
offsetY
</td>
<td class="type">
number
</td>
<td class="description">
Returns the current Y position
</td>
</tr>
</tbody>
</table>
</td>
</tr>
</tbody>
</table>

#### Example:

{% highlight html %}
<script type="text/javascript">
        $(function () {
            var obj = $("#viewer").ejPdfViewer({ serviceUrl: '../api/PdfViewer', destroy: "destroy" });
        });
        function destroy(args) {
            alert("The control is destroyed successfully");
        }
</script>
{% endhighlight %}

### bufferStart

{:#events:bufferStart}

Triggers when the client buffering process starts.
<table>
<thead>
<tr>
<th>
{{'**Name**'| markdownify }}
</th>
<th>
{{'**Type**'| markdownify }}
</th>
<th>
{{'**Description**'| markdownify }}
</th>
</tr>
</thead>
<tbody>
<tr>
<td class="name">
argument
</td>
<td class="type">
object
</td>
<td class="description">
Event parameters from PDF viewer
<table>
<thead>
<tr>
<th>
{{'**Name**'| markdownify }}
</th>
<th>
{{'**Type**'| markdownify }}
</th>
<th>
{{'**Description**'| markdownify }}
</th>
</tr>
</thead>
<tbody>
<tr>
<td class="name">
cancel
</td>
<td class="type">
boolean
</td>
<td class="description">
True, if the event should be canceled; otherwise, false.
</td>
</tr>
<tr>
<td class="name">
model
</td>
<td class="type">
object
</td>
<td class="description">
Returns the PDF viewer model
</td>
</tr>
<tr>
<td class="name">
type
</td>
<td class="type">
string
</td>
<td class="description">
Returns the name of the event
</td>
</tr>
<tr>
<td class="name">
isBuffering
</td>
<td class="type">
boolean
</td>
<td class="description">
Specifies the state of the buffering
</td>
</tr>
</tbody>
</table>
</td>
</tr>
</tbody>
</table>

#### Example:

{% highlight html %}
<script type="text/javascript">
        $(function () {
            var obj = $("#viewer").ejPdfViewer({ serviceUrl: '../api/PdfViewer', allowClientBuffering: true, bufferStart: "bufferStart" });
        });
        function bufferStart(args) {
            alert("The buffering process is started");
        }
</script>
{% endhighlight %}

### bufferEnd

{:#events:bufferEnd}

Triggers when the client buffering process ends.
<table>
<thead>
<tr>
<th>
{{'**Name**'| markdownify }}
</th>
<th>
{{'**Type**'| markdownify }}
</th>
<th>
{{'**Description**'| markdownify }}
</th>
</tr>
</thead>
<tbody>
<tr>
<td class="name">
argument
</td>
<td class="type">
object
</td>
<td class="description">
Event parameters from PDF viewer
<table>
<thead>
<tr>
<th>
{{'**Name**'| markdownify }}
</th>
<th>
{{'**Type**'| markdownify }}
</th>
<th>
{{'**Description**'| markdownify }}
</th>
</tr>
</thead>
<tbody>
<tr>
<td class="name">
cancel
</td>
<td class="type">
boolean
</td>
<td class="description">
True, if the event should be canceled; otherwise, false.
</td>
</tr>
<tr>
<td class="name">
model
</td>
<td class="type">
object
</td>
<td class="description">
Returns the PDF viewer model
</td>
</tr>
<tr>
<td class="name">
type
</td>
<td class="type">
string
</td>
<td class="description">
Returns the name of the event
</td>
</tr>
<tr>
<td class="name">
isBuffering
</td>
<td class="type">
boolean
</td>
<td class="description">
Specifies the state of the buffering
</td>
</tr>
</tbody>
</table>
</td>
</tr>
</tbody>
</table>

#### Example:

{% highlight html %}
<script type="text/javascript">
        $(function () {
            var obj = $("#viewer").ejPdfViewer({ serviceUrl: '../api/PdfViewer', allowClientBuffering: true, bufferEnd: "bufferEnd" });
        });
        function bufferEnd(args) {
            alert("The buffering process is ended");
        }
</script>
{% endhighlight %}

### destroy

{:#events:destroy}

Triggers when PDF viewer control is destroyed successfully.
<table>
<thead>
<tr>
<th>
{{'**Name**'| markdownify }}
</th>
<th>
{{'**Type**'| markdownify }}
</th>
<th>
{{'**Description**'| markdownify }}
</th>
</tr>
</thead>
<tbody>
<tr>
<td class="name">
argument
</td>
<td class="type">
object
</td>
<td class="description">
Event parameters from PDF viewer
<table>
<thead>
<tr>
<th>
{{'**Name**'| markdownify }}
</th>
<th>
{{'**Type**'| markdownify }}
</th>
<th>
{{'**Description**'| markdownify }}
</th>
</tr>
</thead>
<tbody>
<tr>
<td class="name">
cancel
</td>
<td class="type">
boolean
</td>
<td class="description">
True, if the event should be canceled; otherwise, false.
</td>
</tr>
<tr>
<td class="name">
model
</td>
<td class="type">
object
</td>
<td class="description">
Returns the PDF viewer model
</td>
</tr>
<tr>
<td class="name">
type
</td>
<td class="type">
string
</td>
<td class="description">
Returns the name of the event
</td>
</tr>
</tbody>
</table>
</td>
</tr>
</tbody>
</table>

#### Example:

{% highlight html %}
<script type="text/javascript">
        $(function () {
            var obj = $("#viewer").ejPdfViewer({ serviceUrl: '../api/PdfViewer', destroy: "destroy" });
        });
        function destroy(args) {
            alert("The control is destroyed successfully");
        }
</script>
{% endhighlight %}

