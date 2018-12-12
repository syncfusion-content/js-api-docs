---
title: Properties, Methods and Events of Syncfusion ejPdfViewer Widget
description: Methods,members and events available in ejPdfViewer
platform: js-api
control: ejPdfViewer
documentation: UG
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
* module:ej.data.js
* module:ej.globalize.js
* module:ej.draggable.js
* module:ej.pdfviewer.js
* module:ej.dropdownlist.js
* module:ej.toolbar.js
* module:ej.button.js
* module:ej.waitingpopup.js
* module:ej.scroller.js
* module:ej.checkbox.js
* module:ej.tooltip.js
* module:ej.maskedit.js
* module:ej.dialog.js
* module:ej.tab.js
* module:ej.colorpicker.js
* module:ej.splitbutton.js
* module:ej.menu.js
* module:ej.slider.js

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
TextSearchTool
</td>
<td class="description">
Shows only text search tool in the toolbar.
</td>
</tr>
<tr>
<td class="name">
TextMarkupAnnotationTools
</td>
<td class="description">
Shows only text markup annotation tools in the toolbar.
</td>
</tr>
<tr>
<td class="name">
SignatureTool
</td>
<td class="description">
Shows only signature tool in the toolbar.
</td>
</tr>
<tr>
<td class="name">
SelectionTool
</td>
<td class="description">
Shows only selection tool in the toolbar.
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

{:#members:serveractionsettings}

Specifies the name of the action method in the server.

### serverActionSettings.load `string`

{:#members:serveractionsettings-load}

Specifies the name of the action method used for loading the PDF document.

**Default Value**: Load

### serverActionSettings.fileUpload `string`

{:#members:serveractionsettings-fileupload}

Specifies the name of the action method used for uploading the PDF document to the PDF viewer control.

**Default Value**: FileUpload

### serverActionSettings.print `string`

{:#members:serveractionsettings-print}

Specifies the name of the action method used for printing the PDF document in the PDF viewer control.

**Default Value**: Load

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

{:#members:documentpath}

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

### enableTextMarkupAnnotations `boolean`

{:#members:enabletextmarkupannotations}

Enables or disables the text markup annotations.

**Default Value**: true

#### Example:

{% highlight html %}
<div id="viewer"></div>
<script type="text/javascript">
        $(function () {
            $("#viewer").ejPdfViewer({ serviceUrl: '../api/PdfViewer', enableTextMarkupAnnotations: true });
        });
</script>
{% endhighlight %}

### enableHighlightAnnotation `boolean`

{:#members:enablehighlightannotation}

Enables or disables the highlight annotation.

**Default Value**: true

#### Example:

{% highlight html %}
<div id="viewer"></div>
<script type="text/javascript">
        $(function () {
            $("#viewer").ejPdfViewer({ serviceUrl: '../api/PdfViewer', enableHighlightAnnotation: true });
        });
</script>
{% endhighlight %}

### enableUnderlineAnnotation `boolean`

{:#members:enableunderlineannotation}

Enables or disables the underline annotation.

**Default Value**: true

#### Example:

{% highlight html %}
<div id="viewer"></div>
<script type="text/javascript">
        $(function () {
            $("#viewer").ejPdfViewer({ serviceUrl: '../api/PdfViewer', enableUnderlineAnnotation: true });
        });
</script>
{% endhighlight %}

### enableStrikethroughAnnotation `boolean`

{:#members:enablestrikethroughannotation}

Enables or disables the strikethrough annotation.

**Default Value**: true

#### Example:

{% highlight html %}
<div id="viewer"></div>
<script type="text/javascript">
        $(function () {
            $("#viewer").ejPdfViewer({ serviceUrl: '../api/PdfViewer', enableStrikethroughAnnotation: true });
        });
</script>
{% endhighlight %}

### enableSignature `boolean`

{:#members:enablesignature}

 Enables or disables the adding of handwritten signature over the PDF document.

**Default Value**: true

#### Example:

{% highlight html %}
<div id="viewer"></div>
<script type="text/javascript">
        $(function () {
            $("#viewer").ejPdfViewer({ serviceUrl: '../api/PdfViewer', enableSignature: true });
        });
</script>
{% endhighlight %}

### strikethroughSettings `object`

{:#members:strikethroughsettings}

Gets/sets the settings of the strikethrough annotation.

### strikethroughSettings.color `string`

{:#members:strikethroughsettings-color}

Gets/sets the color of the strikethrough annotation.

**Default Value**: "#ff0000"

### strikethroughSettings.author `string`

{:#members:strikethroughsettings-author}

Gets/sets the author of the strikethrough annotation.

**Default Value**: "Guest"

### strikethroughSettings.opacity `number`

{:#members:strikethroughsettings-opacity}

Gets/sets the opacity of the strikethrough annotation.

**Default Value**: 1

### strikethroughSettings.subject `string`

{:#members:strikethroughsettings-subject}

Gets/sets the subject of the strikethrough annotation.

**Default Value**: "Strikethrough"

### strikethroughSettings.modifiedDate `string`

{:#members:strikethroughsettings-modifieddate}

Gets/sets the modified Date of the strikethrough annotation.

**Default Value**: null

### strikethroughSettings.isLocked `boolean`

{:#members:strikethroughsettings-islocked}

Gets/sets the locked property of the strikethrough annotation.

**Default Value**: false

#### Example:

{% highlight html %}
<div id="viewer"></div>
<script type="text/javascript">
        $(function () {
            $("#viewer").ejPdfViewer({ serviceUrl: '../api/PdfViewer', strikethroughSettings: {
				color: "#ff0000", author: "Guest", opacity: 0.5, subject: "strikethrough", modifiedDate: "2017-03-27 12:00:51", isLocked: true
			} });
        });
</script>
{% endhighlight %}

### underlineSettings `object`

{:#members:underlinesettings}

Gets/sets the settings of the underline annotation.

### underlineSettings.color `string`

{:#members:underlinesettings-color}

Gets/sets the color of the underline annotation.

**Default Value**: "#00ff00" 

### underlineSettings.author `string`

{:#members:underlinesettings-author}

Gets/sets the author of the underline annotation.

**Default Value**: "Guest"

### underlineSettings.opacity `number`

{:#members:underlinesettings-opacity}

Gets/sets the opacity of the underline annotation.

**Default Value**: 1

### underlineSettings.subject `string`

{:#members:underlinesettings-subject}

Gets/sets the subject of the underline annotation.

**Default Value**: "Underline"

### underlineSettings.modifiedDate `string`

{:#members:underlinesettings-modifieddate}

Gets/sets the modified Date of the underline annotation.

**Default Value**: null

### underlineSettings.isLocked `boolean`

{:#members:underlinesettings-islocked}

Gets/sets the locked property of the underline annotation.

**Default Value**: false

#### Example:

{% highlight html %}
<div id="viewer"></div>
<script type="text/javascript">
        $(function () {
            $("#viewer").ejPdfViewer({ serviceUrl: '../api/PdfViewer', underlineSettings: {
				color: "#00ff00", author: "Guest", opacity: 0.5, subject: "underline", modifiedDate: "2017-03-27 12:00:51", isLocked: true
			} });
        });
</script>
{% endhighlight %}

### highlightSettings `object`

{:#members:highlightsettings}

Gets/sets the settings of the highlight annotation.

### highlightSettings.color `string`

{:#members:highlightsettings-color}

Gets/sets the color of the highlight  annotation.

**Default Value**: "#ffff00"

### highlightSettings.author `string`

{:#members:highlightsettings-author}

Gets/sets the author of the highlight annotation.

**Default Value**: "Guest"

### highlightSettings.opacity `number`

{:#members:highlightsettings-opacity}

Gets/sets the opacity of the highlight annotation.

**Default Value**: 1

### highlightSettings.subject `string`

{:#members:highlightsettings-subject}

Gets/sets the subject of the highlight annotation.

**Default Value**: "Highlight"

### highlightSettings.modifiedDate `string`

{:#members:highlightsettings-modifieddate}

Gets/sets the modified Date of the highlight annotation.

**Default Value**: null

### highlightSettings.isLocked `boolean`

{:#members:highlightsettings-islocked}

Gets/sets the locked property of the highlight annotation.

**Default Value**: false

#### Example:

{% highlight html %}
<div id="viewer"></div>
<script type="text/javascript">
        $(function () {
            $("#viewer").ejPdfViewer({ serviceUrl: '../api/PdfViewer', highlightSettings: {
				color: "#ffff00", author: "Guest", opacity: 0.5, subject: "highlight", modifiedDate: "2017-03-27 12:00:51", isLocked: true
			} });
        });
</script>
{% endhighlight %}

### signatureSettings `object`

{:#members:signaturesettings}

Gets/sets the settings of the handwritten signature.

### signatureSettings.color `string`

{:#members:signaturesettings-color}

Gets/sets the color of the handwritten signature.

**Default Value**: "#000000"

### signatureSettings.opacity `number`

{:#members:signaturesettings-opacity}

Gets/sets the opacity of the handwritten signature.

**Default Value**: 1

#### Example:

{% highlight html %}
<div id="viewer"></div>
<script type="text/javascript">
        $(function () {
            $("#viewer").ejPdfViewer({ serviceUrl: '../api/PdfViewer', signatureSettings: {
				color: "#000000", opacity: 1
			} });
        });
</script>
{% endhighlight %}

### textSelectionContextMenu `object`

{:#members:textselectioncontextmenu}

Enables/ disables the text selection context menu.

### textSelectionContextMenu.isEnable `boolean`

{:#members:textselectioncontextmenu-isenable}

Enables/ disables the text selection context menu.

**Default Value**: true

### textSelectionContextMenu.isCopyEnable `boolean`

{:#members:textselectioncontextmenu-iscopyenable}

Enables/disables the copy menu in the text selection context menu.

**Default Value**: true

### textSelectionContextMenu.isSearchEnable `boolean`

{:#members:textselectioncontextmenu-issearchenable }

Enables/disables the search menu in the text selection context menu.

**Default Value**: true

### textSelectionContextMenu.isHighlightEnable `boolean`

{:#members:textselectioncontextmenu-ishighlightenable }

Enables/disables the highlight annotation menu in the text selection context menu.

**Default Value**: true

### textSelectionContextMenu.isStrikeoutEnable `boolean`

{:#members:textselectioncontextmenu-isstrikeoutenable }

Enables/disables the strikeout annotation menu in the text selection context menu.

**Default Value**: true

#### Example:

{% highlight html %}
<div id="viewer"></div>
<script type="text/javascript">
        $(function () {
            $("#viewer").ejPdfViewer({ serviceUrl: '../api/PdfViewer', textSelectionContextMenu: {
				isSearchEnable : false , isHighlightEnable: false
			} });
        });
</script>
{% endhighlight %}

### annotationContextMenu `object`

{:#members:annotationcontextmenu}

Enables/disables the annotation context menu.

### annotationContextMenu.isEnable `boolean`

{:#members:annotationcontextmenu-isenable}

Enables/disables the annotation context menu.

**Default Value**: true

### annotationContextMenu.isPopupEnable  `boolean`

{:#members:annotationcontextmenu-ispopupenable }

Enables/disables the popup menu in the annotation context menu.

**Default Value**: true

### annotationContextMenu.isDeleteEnable  `boolean`

{:#members:annotationcontextmenu-isdeleteenable  }

Enables/disables the delete menu in the annotation context menu.

**Default Value**: true

### annotationContextMenu.isPropertiesEnable `boolean`

{:#members:annotationcontextmenu-ispropertiesenable }

Enables/disables the properties menu in the annotation context menu.

**Default Value**: true

#### Example:

{% highlight html %}
<div id="viewer"></div>
<script type="text/javascript">
        $(function () {
            $("#viewer").ejPdfViewer({ serviceUrl: '../api/PdfViewer', annotationContextMenu: {
				isPopupEnable  : false ,isDeleteEnable:false
			} });
        });
</script>
{% endhighlight %}

### annotationType `enum`

{:#members:annotationtype}

<ts name="ej.PdfViewer.AnnotationType"/>

Specifies the type of the annotations.

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
Underline
</td>
<td class="description">
Specifies the underline annotation.
</td>
</tr>
<tr>
<td class="name">
Strikethrough
</td>
<td class="description">
Specifies the strikethrough annotation.
</td>
</tr>
<tr>
<td class="name">
Highlight
</td>
<td class="description">
Specifies the highlight annotation.
</td>
</tr>
</tbody>
</table>

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

### interactionMode `enum`

{:#members:interactionmode}

<ts name="ej.PdfViewer.InteractionMode"/>

Specifies the viewer interaction mode.

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
TextSelection
</td>
<td class="description">
To set the text selection mode to the PDF viewer control.
</td>
</tr>
<tr>
<td class="name">
Pan
</td>
<td class="description">
To set the panning mode to the PDF viewer control.
</td>
</tr>
</tbody>
</table>

**Default value:** ej.PdfViewer.InteractionMode.TextSelection

#### Example:

The below code snippet shows to set the Panning mode to the PDF viewer control.


{% highlight javascript %}
<div id="viewer"></div>
<script type="text/javascript">
        $(function () {
           $("#viewer").ejPdfViewer({ serviceUrl: '../api/PdfViewer', interactionMode: ej.PdfViewer.InteractionMode.Pan});
        });
</script>
{% endhighlight %}

### bufferingMode  `enum`

{:#members:bufferingmode }

<ts name="ej.PdfViewer.BufferingMode"/>

Gets or sets the buffering mode of the PDF viewer control when allowClientBuffering is set to true. 

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
Retrieves details to render first two pages in a request and rest of the pages in other request. 
</td>
</tr>
<tr>
<td class="name">
Complete 
</td>
<td class="description">
Retrieves complete details to render all the pages in a single request. 
</td>
</tr>
</tbody>
</table>

**Default value:** ej.PdfViewer.BufferingMode.Default 

#### Example:

The below code snippet shows to set the Buffering mode to the PDF viewer control.


{% highlight javascript %}
<div id="viewer"></div>
<script type="text/javascript">
        $(function () {
           $("#viewer").ejPdfViewer({ serviceUrl: '../api/PdfViewer', allowClientBuffering: true, bufferingMode: ej.PdfViewer.BufferingMode.Complete});
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
{:#members:enabletextselection}

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
{:#members:isresponsive}

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
{:#members:isdocumentedited}

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
{:#members:allowclientbuffering}

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

### abortDownload()
{:#methods:abortdownload}

Aborts the download operation.

#### Example:

{% highlight javascript %}
var pdfviewerObj = $("#viewer").data("ejPdfViewer");
pdfviewerObj.abortDownload();
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

### showTextMarkupAnnotationTools(show)
{:#methods:showtextmarkupannotationtools}

Shows/hides the text markup annotation tools in the toolbar.

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
<td class="description">shows/hides text markup annotation tools in the toolbar</td>
</tr>
</tbody>
</table>

#### Example:

{% highlight javascript %}
var pdfviewerObj = $("#viewer").data("ejPdfViewer");
pdfviewerObj.showTextMarkupAnnotationTools(false);
{% endhighlight %}

### showSignatureTool(show)
{:#methods:showsignaturetool}

Shows/hides the signature tool in the toolbar.

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
<td class="description">shows/hides signature tool in the toolbar</td>
</tr>
</tbody>
</table>

#### Example:

{% highlight javascript %}
var pdfviewerObj = $("#viewer").data("ejPdfViewer");
pdfviewerObj.showSignatureTool(false);
{% endhighlight %}

### showSelectionTool(show)
{:#methods:showselectiontool}

Shows/hides the selection tool in the toolbar.

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
<td class="description">shows/hides selection tool in the toolbar</td>
</tr>
</tbody>
</table>

#### Example:

{% highlight javascript %}
var pdfviewerObj = $("#viewer").data("ejPdfViewer");
pdfviewerObj.showSelectionTool(false);
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

### showTextSearchTool(show)

{:#methods:showtextsearchtool}

Shows/hides the search tool in the toolbar.

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
<td class="description">shows/hides search tool in the toolbar</td>
</tr>
</tbody>
</table>

#### Example:

{% highlight javascript %}
var pdfviewerObj = $("#viewer").data("ejPdfViewer");
pdfviewerObj.showTextSearchTool(false);
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

### updateViewerSize()

{:#methods:updateviewersize}

Resize the viewer based on the parent element height.

#### Example:

{% highlight javascript %}
var pdfviewerObj = $("#viewer").data("ejPdfViewer");
pdfviewerObj.updateViewerSize();
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

### searchText(targetText)

{:#methods:searchtext}

Searches the target text in the PDF document and highlights the occurrences in the pages.

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
targetText</td>
<td class="type"><span class="param-type">string</span></td>
<td class="description">The text to be searched in the pages in the PDF viewer.</td>
</tr>
</tbody>
</table>

#### Example:

{% highlight javascript %}
var pdfviewerObj = $("#viewer").data("ejPdfViewer");
pdfviewerObj.searchText("name");
{% endhighlight %}

### searchNext()

{:#methods:searchnext}

Searches the next occurrence of the searched text from the current occurrence in the PDF viewer control.

#### Example:

{% highlight javascript %}
var pdfviewerObj = $("#viewer").data("ejPdfViewer");
pdfviewerObj.searchNext();
{% endhighlight %}

### searchPrevious()

{:#methods:searchprevious}

Searches the previous occurrence of the searched text from the current occurrence in the PDF viewer control.

#### Example:

{% highlight javascript %}
var pdfviewerObj = $("#viewer").data("ejPdfViewer");
pdfviewerObj.searchPrevious();
{% endhighlight %}

### setJSONData(jsonData)

{:#methods:setjsondata}

Set the JSON data that are formed for rendering the document content in PDF viewer. 

N> The JSON data format should be formed as mentioned [here](https://help.syncfusion.com/js/webapi/pdfviewer#response-information)

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
jsonData</td>
<td class="type"><span class="param-type">object</span></td>
<td class="description">Set the JSON data that are formed for rendering the document content.</td>
</tr>
</tbody>
</table>

#### Example:

{% highlight javascript %}
<script type="text/javascript">
        $(function () {
            $("#viewer").ejPdfViewer({ serviceUrl: '../api/PdfViewer', ajaxRequestSuccess: "ajaxRequestSucceed" });
        });
         function ajaxRequestSucceed(args){           
            var pdfviewerObj = $("#container").data("ejPdfViewer");            
            pdfviewerObj.setJSONData(args.responseData);
        }
</script>
{% endhighlight %}

### matchCase(enableMatchCase)

{:#methods:matchcase}

Searches the target text with its casing.

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
enableMatchCase</td>
<td class="type"><span class="param-type">boolean</span></td>
<td class="description">Specifies whether the text search must be performed with match case or not.</td>
</tr>
</tbody>
</table>

#### Example:

{% highlight javascript %}
var pdfviewerObj = $("#viewer").data("ejPdfViewer");
pdfviewerObj.matchCase(true);
{% endhighlight %}

### cancelSearchText()

{:#methods:cancelsearchtext}

Cancels the text search and removes the highlighted occurrences from the PDF viewer.

#### Example:

{% highlight javascript %}
var pdfviewerObj = $("#viewer").data("ejPdfViewer");
pdfviewerObj.cancelSearchText();
{% endhighlight %}

### addAnnotation(annotationType)
{:#methods:addannotation}

Adds annotations to the PDF document.

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
annotationType
</td>
<td class="type"><ts ref="ej.PdfViewer.AnnotationType"/>enum</td>
<td class="description">type of the annotation to be added in the PDF document.</td>
</tr>
</tbody>
</table>

#### Example:

{% highlight javascript %}
var pdfviewerObj = $("#viewer").data("ejPdfViewer");
pdfviewerObj.addAnnotation(ej.PdfViewer.AnnotationType.Underline);
{% endhighlight %}

### undo()

{:#methods:undo}

Performs undo function for the included annotations in the PDF document.
 
#### Example:

{% highlight javascript %}
var pdfviewerObj = $("#viewer").data("ejPdfViewer");
pdfviewerObj.undo();
{% endhighlight %}

### redo()

{:#methods:redo}

Performs redo function for the included annotations in the PDF document.
 
#### Example:

{% highlight javascript %}
var pdfviewerObj = $("#viewer").data("ejPdfViewer");
pdfviewerObj.redo();
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
Returns the cancel option value.
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
Returns the cancel option value.
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
Returns the cancel option value.
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


### ajaxRequestFailure

{:#events:ajaxrequestfailure}

Triggers when the AJAX request is failed.
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
Returns the cancel option value.
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
message
</td>
<td class="type">
string
</td>
<td class="description">
Returns the exception details.
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
            var obj = $("#viewer").ejPdfViewer({ serviceUrl: '../api/PdfViewer', ajaxRequestFailure:"ajaxRequestFailed" });
        });
        function ajaxRequestFailed(args) {
            alert("Please find the Exception details"+ args.message);
        }
</script>
{% endhighlight %}

### ajaxRequestSuccess

{:#events:ajaxrequestsuccess}

Triggers when the ajax request is Success.
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
responseData
</td>
<td class="type">
string
</td>
<td class="description">
Returns the response data on ajax success.
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
            var obj = $("#viewer").ejPdfViewer({ serviceUrl: '../api/PdfViewer', ajaxRequestSuccess:"ajaxRequestSucceed" });
        });
        function ajaxRequestSucceed(args) {
            alert("Please find the response data"+ args.responseData);
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
Returns the cancel option value.
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
Returns the cancel option value.
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
Returns the cancel option value.
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
            var obj = $("#viewer").ejPdfViewer({ serviceUrl: '../api/PdfViewer', beforePrint: "beforePrint" });
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
Returns the cancel option value.
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
Returns the cancel option value.
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
            var obj = $("#viewer").ejPdfViewer({ serviceUrl: '../api/PdfViewer', pageClick: "onPageClicked" });
        });
          function onPageClicked(args) {
            alert("X-coordinate :" + args.XCoordinate + "  Y-coordinate :" + args.YCoordinate);
        }
</script>
{% endhighlight %}

### annotationAdd

{:#events:annotationadd}

Triggers when an annotation is added over the page of the PDF document.
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
Returns the cancel option value.
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
annotationSettings
</td>
<td class="type">
object
</td>
<td class="description">
Returns the settings of the annotation added to the PDF document.
</td>
</tr>
<tr>
<td class="name">
annotationID
</td>
<td class="type">
number
</td>
<td class="description">
Returns the id of the annotation added in the page of the PDF document.
</td>
</tr>
<tr>
<td class="name">
annotationBound
</td>
<td class="type">
array
</td>
<td class="description">
Returns the bounds of the annotation added in the page of the PDF document.
</td>
</tr>
<tr>
<td class="name">
pageID
</td>
<td class="type">
number
</td>
<td class="description">
Returns the page number in which the annotation is added.
</td>
</tr>
<tr>
<td class="name">
annotationType
</td>
<td class="type">
string
</td>
<td class="description">
Returns the type of the annotation added in the page of the PDF document.
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
            var obj = $("#viewer").ejPdfViewer({ serviceUrl: '../api/PdfViewer', annotationAdd: "annotationAdd" });
        });
        function annotationAdd(args) {
            alert("The annotation is added to the PDF document successfully");
        }
</script>
{% endhighlight %}

### annotationRemove

{:#events:annotationremove}

Triggers when an annotation is removed from the page of the PDF document.
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
Returns the cancel option value.
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
annotationID
</td>
<td class="type">
number
</td>
<td class="description">
Returns the id of the annotation removed from the page of the PDF document.
</td>
</tr>
<tr>
<td class="name">
pageID
</td>
<td class="type">
number
</td>
<td class="description">
Returns the page number in which the annotation is removed.
</td>
</tr>
<tr>
<td class="name">
annotationType
</td>
<td class="type">
string
</td>
<td class="description">
Returns the type of the annotation removed from the page of the PDF document.
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
            var obj = $("#viewer").ejPdfViewer({ serviceUrl: '../api/PdfViewer', annotationRemove: "annotationRemove" });
        });
        function annotationRemove(args) {
            alert("The annotation is removed from the PDF document successfully");
        }
</script>
{% endhighlight %}

### annotationPropertiesChange

{:#events:annotationpropertieschange}

Triggers when the property of the annotation is changed in the page of the PDF document.
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
Returns the cancel option value.
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
annotationID
</td>
<td class="type">
number
</td>
<td class="description">
Returns the id of the annotation added in the page of the PDF document.
</td>
</tr>
<tr>
<td class="name">
pageID
</td>
<td class="type">
number
</td>
<td class="description">
Returns the page number in which the annotation is added.
</td>
</tr>
<tr>
<td class="name">
annotationType
</td>
<td class="type">
string
</td>
<td class="description">
Returns the type of the annotation added in the page of the PDF document.
</td>
</tr>
<tr>
<td class="name">
isColorChanged
</td>
<td class="type">
boolean
</td>
<td class="description">
Specifies that the color of the annotation is changed.
</td>
</tr>
<tr>
<td class="name">
isOpacityChanged
</td>
<td class="type">
boolean
</td>
<td class="description">
Specifies that the opacity of the annotation is changed.
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
            var obj = $("#viewer").ejPdfViewer({ serviceUrl: '../api/PdfViewer', annotationAdd: "annotationAdd" });
        });
        function annotationAdd(args) {
            alert("The annotation is added to the PDF document successfully");
        }
</script>
{% endhighlight %}

### signatureAdd

{:#events:signatureadd}

Triggers when a handwritten signature is added over the page of the PDF document.
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
Returns the cancel option value.
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
signatureSettings
</td>
<td class="type">
object
</td>
<td class="description">
Returns the settings of the signature added to the PDF document.
</td>
</tr>
<tr>
<td class="name">
signatureBound
</td>
<td class="type">
array
</td>
<td class="description">
Returns the bounds of the signature added in the page of the PDF document.
</td>
</tr>
<tr>
<td class="name">
pageNumber
</td>
<td class="type">
number
</td>
<td class="description">
Returns the page number in which the signature is added.
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
            var obj = $("#viewer").ejPdfViewer({ serviceUrl: '../api/PdfViewer', signatureAdd: "signatureAdd" });
        });
        function signatureAdd(args) {
            alert("The signature is added to the PDF document successfully");
        }
</script>
{% endhighlight %}

### signatureDelete

{:#events:signaturedelete}

Triggers when a handwritten signature is removed from the page of the PDF document.
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
Returns the cancel option value.
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
pageNumber
</td>
<td class="type">
number
</td>
<td class="description">
Returns the page number in which the signature is removed.
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
            var obj = $("#viewer").ejPdfViewer({ serviceUrl: '../api/PdfViewer', signatureDelete: "signatureDelete" });
        });
        function signatureDelete(args) {
            alert("The signature is removed from the page of the PDF document successfully");
        }
</script>
{% endhighlight %}

### signaturePropertiesChange

{:#events:signaturepropertieschange}

Triggers when a handwritten signature properties is changed in the PDF document.
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
Returns the cancel option value.
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
pageID
</td>
<td class="type">
number
</td>
<td class="description">
Returns the page number in which the signature properties is changed.
</td>
</tr>
<tr>
<td class="name">
isColorChange
</td>
<td class="type">
boolean
</td>
<td class="description">
Specifies that the color of the signature is changed.
</td>
</tr>
<tr>
<td class="name">
isOpacityChange
</td>
<td class="type">
boolean
</td>
<td class="description">
Specifies that the opacity of the signature is changed.
</td>
</tr>
<tr>
<td class="name">
previousColor
</td>
<td class="type">
string
</td>
<td class="description">
Returns the previous color of the signature.
</td>
</tr>
<tr>
<td class="name">
currentColor
</td>
<td class="type">
string
</td>
<td class="description">
Returns the current color of the signature.
</td>
</tr>
<tr>
<td class="name">
previousOpacity
</td>
<td class="type">
number
</td>
<td class="description">
Returns the previous opacity of the signature.
</td>
</tr>
<tr>
<td class="name">
currentOpacity
</td>
<td class="type">
number
</td>
<td class="description">
Returns the current opacity of the signature.
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
            var obj = $("#viewer").ejPdfViewer({ serviceUrl: '../api/PdfViewer', signaturePropertiesChange: "signaturePropertiesChange" });
        });
        function signaturePropertiesChange(args) {
            alert("The signature properties is changed from the page of the PDF document successfully");
        }
</script>
{% endhighlight %}

### signatureResize

{:#events:signatureresize}

Triggers when a handwritten signature is resized in the PDF document.
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
Returns the cancel option value.
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
signatureSettings
</td>
<td class="type">
object
</td>
<td class="description">
Returns the settings of the signature added to the PDF document.
</td>
</tr>
<tr>
<td class="name">
pageNumber
</td>
<td class="type">
number
</td>
<td class="description">
Returns the page number in which the signature is added.
</td>
</tr>
<tr>
<td class="name">
signatureCurrentBound
</td>
<td class="type">
array
</td>
<td class="description">
Returns the current bounds of the signature resized in the page of the PDF document.
</td>
</tr>
<tr>
<td class="name">
signaturePreviousBound
</td>
<td class="type">
array
</td>
<td class="description">
Returns the previous bounds of the signature resized in the page of the PDF document.
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
            var obj = $("#viewer").ejPdfViewer({ serviceUrl: '../api/PdfViewer', signatureResize: "signatureResize" });
        });
        function signatureResize(args) {
            alert("The signature is resized to the PDF document successfully");
        }
</script>
{% endhighlight %}

### bufferStart

{:#events:bufferstart}

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
Returns the cancel option value.
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

{:#events:bufferend}

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
Returns the cancel option value.
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

### downloadStart

{:#events:downloadStart}

Triggers when the download is started.
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
true, if the event should be canceled; otherwise, false
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
Returns the name of the file being displayed in the PDF viewer.
</td>
</tr>
<tr>
<td class="name">
status
</td>
<td class="type">
string
</td>
<td class="description">
Returns the status about the download is started.
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
            var obj = $("#viewer").ejPdfViewer({ serviceUrl: '../api/PdfViewer', downloadStart: "downloadStart" });
        });
        function downloadStart(args) {
             alert(args.fileName + " file download process " + args.status);
        }
</script>
{% endhighlight %}

### downloadEnd

{:#events:downloadEnd}

Triggers when the download is completed or aborted.
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
true, if the event should be canceled; otherwise, false
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
Returns the name of the file being displayed in the PDF viewer.
</td>
</tr>
<tr>
<td class="name">
status
</td>
<td class="type">
string
</td>
<td class="description">
Returns the status about the download is completed or aborted.
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
            var obj = $("#viewer").ejPdfViewer({ serviceUrl: '../api/PdfViewer', downloadEnd: "downloadEnd" });
        });
        function downloadEnd(args) {
             alert(args.fileName + " file download process " + args.status);
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
Returns the cancel option value.
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

