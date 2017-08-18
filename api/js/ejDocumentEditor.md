---
layout: post
title: Properties, Methods and Events of ejDocumentEditor Widget
description: Properties, Methods and Events of ejDocumentEditor Widget
documentation: API
platform: js-api
keywords: ejDocumentEditor, API, Essential JS Document Editor
---

# ejDocumentEditor

Document Editor JS is an editor component to view and print DOCX, DOC, RTF and Text documents.

#### Syntax

{% highlight html %}
  $(element).ejDocumentEditor(
            importExportSetting: {
                importUrl: "../api/DocumentEditor/ImportDocument",
            });
{% endhighlight %}

#### Example

{% highlight html %}
<div id="container"></div>
    <script>
        $("#container").ejDocumentEditor({
            importExportSetting: {
                importUrl: "http://js.syncfusion.com/demos/ejservices/api/DocumentEditor/ImportDocument",
            }
        });
    </script>
{% endhighlight %}

#### Document Editor requires the following script files

* Module: jquery.js
* Module: ej.data.js 
* Module: ej.core.js
* Module: ej.documenteditor.js
* Module: ej.scroller.js

## Members

### importExportSettings `Object`
{:#members:importexportsettings}

Gets or sets an object that indicates initialization of importing and exporting documents in document editor.

### importExportSettings.importUrl `string`
{:#members:importexportsettings-importurl}

Gets or sets URL of Web API that should be used to parse the document while loading.

#### Example

{% highlight html %}
<div id="container"></div>
    <script>
        $("#container").ejDocumentEditor({
            importExportSetting: {
                importUrl: "http://js.syncfusion.com/demos/ejservices/api/DocumentEditor/ImportDocument",
            }
        });
    </script>
{% endhighlight %}

N> Create a controller class and write service for import document. Mention the controller name and action name in **import url**

## Methods

### load(path)
{:#methods:load}

Loads the document from specified path using web API provided by importUrl.

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
<td>
path
</td>
<td>
string
</td>
<td>
Specifies the file path.
</td>
</tr>
</tbody>
</table>

#### Example

{% highlight html %}
<script>
	var documentEditorObj = $("#container").data("ejDocumentEditor");
	documentEditorObj.load(event.target.files[0]);// specify the file path.
</script>
{% endhighlight %}

### getCurrentPageNumber()
{:#methods:getcurrentpagenumber}

Gets the page number of current selection in the document.

N> This method does not accept any arguments.

#### Returns:

number

#### Example

{% highlight html %}
<script>
	var documentEditorObj = $("#container").data("ejDocumentEditor");
	alert("current Page number in a document is"+documentEditorObj.getCurrentPageNumber());
</script>
{% endhighlight %}

### getPageCount()
{:#methods:getpagecount}

Gets the total number of pages in the document.

N> This method does not accept any arguments.

#### Returns:

number

#### Example

{% highlight html %}
<script>
	var documentEditorObj = $("#container").data("ejDocumentEditor");
	alert("Total page count in document is"+ documentEditorObj.getPageCount());
</script>
{% endhighlight %}

### getSelectedText()
{:#methods:getselectedtext}

Gets the text of current selection in the document.

N> This method does not accept any arguments.

#### Returns:

string

#### Example

{% highlight html %}
<script>
	var documentEditorObj = $("#container").data("ejDocumentEditor");
	alert("Selected Text: "+ documentEditorObj.getSelectedText());
</script>
{% endhighlight %}

### getZoomFactor()
{:#methods:getzoomfactor}

Gets the current zoom factor value of the document editor.

N> This method does not accept any arguments.

#### Returns:

number

#### Example

{% highlight html %}
<script>
	var documentEditorObj = $("#container").data("ejDocumentEditor");
	alert("zoom value of the container is"+documentEditorObj.getZoomFactor());
</script>
{% endhighlight %}

### setZoomFactor(factor)
{:#methods:setzoomfactor}

Scales the document editor with the specified zoom factor. The range of zoom factor should be 0.10 to 5.00 (10 - 500 %).

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
<td>
factor
</td>
<td>
number
</td>
<td>
Specifies the factor for zooming.
</td>
</tr>
</tbody>
</table>

#### Example

{% highlight html %}
<script>
	var documentEditorObj = $("#container").data("ejDocumentEditor");
	var zoomVal = 120;// specify the zoom percentage value to scale the container in detail
	documentEditorObj.setZoomFactor(zoomVal/100);
</script>
{% endhighlight %}

### print()
{:#methods:print}

Prints the document content as page by page.

N> This method does not accept any arguments.

#### Example

{% highlight html %}
<script>
	var documentEditorObj = $("#container").data("ejDocumentEditor");
	documentEditorObj.print();
</script>
{% endhighlight %}

### find(text)
{:#methods:find}

Finds the first occurrence of specified text from current selection and  highlights the result. If the document end is reached, find operation will occur from the document start position.

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
<td>
text
</td>
<td>
string 
</td>
<td>
Specifies the text to search in a document.
</td>
</tr>
</tbody>
</table>

#### Example

{% highlight html %}
<script>
	var documentEditorObj = $("#container").data("ejDocumentEditor");
	documentEditorObj.find("abc"); //specify the text to find in a document.
</script>
{% endhighlight %}

## Events

### onDocumentChange
{:#events:ondocumentchange}

Triggers when the document changes.

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
<td>
Argument
</td>
<td>
Object
</td>
<td>
Event parameters from Document Editor.
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
<td>
cancel
</td>
<td>
boolean
</td>
<td>
True, if the event should be canceled; otherwise, false.
</td>
</tr>
<tr>
<td>
model
</td>
<td>
object
</td>
<td>
Returns the document editor model.
</td>
</tr>
<tr>
<td>
type
</td>
<td>
string
</td>
<td>
Returns the name of the event.
</td>
</tr>
</tbody>
</table>
</td>
</tr>
</tbody>
</table>

#### Example

{% highlight html %}
<div id="container"></div>
<span id="pageCountSpan"></span>
<script>
    $("#container").ejDocumentEditor({
        importExportSetting: {
            importUrl: "http://js.syncfusion.com/demos/ejservices/api/DocumentEditor/ImportDocument",
            },
            documentChange: "onDocumentChange",
        });
    function onDocumentChange(args) {
		var documentEditorObj = $("#container").data("ejDocumentEditor");
		$("#pageCountSpan").text(documentEditorObj.getPageCount());
	}
</script>
{% endhighlight %}

### onSelectionChange
{:#events:onselectionchange}

Triggers when the selection changes.

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
<td>
Argument
</td>
<td>
Object
</td>
<td>
Event parameters from Document Editor.
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
<td>
cancel
</td>
<td>
boolean
</td>
<td>
True, if the event should be canceled; otherwise, false.
</td>
</tr>
<tr>
<td>
model
</td>
<td>
object
</td>
<td>
Returns the document editor model.
</td>
</tr>
<tr>
<td>
type
</td>
<td>
string
</td>
<td>
Returns the name of the event.
</td>
</tr>
</tbody>
</table>
</td>
</tr>
</tbody>
</table>

#### Example

{% highlight html %}
<div id="container"></div>
<span id="pageNumberSpan"></span>
<script>
    $("#container").ejDocumentEditor({
        importExportSetting: {
            importUrl: "http://js.syncfusion.com/demos/ejservices/api/DocumentEditor/ImportDocument",
        },
        selectionChange: "onSelectionChange",
    });
    function onSelectionChange(args) {
		var documentEditorObj = $("#container").data("ejDocumentEditor");
		$("#pageNumberSpan").text(documentEditorObj.getCurrentPageNumber());
    }
    </script>
{% endhighlight %}

### onZoomFactorChange
{:#events:onzoomfactorchange}

Triggers when the zoom factor changes.

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
<td>
Argument
</td>
<td>
Object
</td>
<td>
Event parameters from Document Editor.
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
<td>
cancel
</td>
<td>
boolean
</td>
<td>
True, if the event should be canceled; otherwise, false.
</td>
</tr>
<tr>
<td>
model
</td>
<td>
object
</td>
<td>
Returns the document editor model.
</td>
</tr>
<tr>
<td>
type
</td>
<td>
string
</td>
<td>
Returns the name of the event.
</td>
</tr>
</tbody>
</table>
</td>
</tr>
</tbody>
</table>

#### Example

{% highlight html %}
<div id="container"></div>
<span id="zoomFactorSpan"></span>
<script>
    $("#container").ejDocumentEditor({
        importExportSetting: {
            importUrl: "http://js.syncfusion.com/demos/ejservices/api/DocumentEditor/ImportDocument",
        },
        zoomFactorChange: "onZoomFactorChange",
    });
    function onZoomFactorChange(args) {
		var documentEditorObj = $("#container").data("ejDocumentEditor");
		$("#zoomFactorSpan").text(documentEditorObj.getZoomFactor()*100+"%")
    }
</script>
{% endhighlight %}

### onRequestNavigate
{:#events:onrequestnavigate}

Triggers when the hyperlink is clicked.

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
<td>
Argument
</td>
<td>
Object
</td>
<td>
Event parameters from Document Editor.
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
<td>
cancel
</td>
<td>
boolean
</td>
<td>
true, if the event should be canceled; otherwise, false.
</td>
</tr>
<tr>
<td>
model
</td>
<td>
object
</td>
<td>
Returns the document editor model.
</td>
</tr>
<tr>
<td>
hyperlink
</td>
<td>
object
</td>
<td>
Returns the link type and navigation link.
</td>
</tr>
<tr>
<td>
type
</td>
<td>
string
</td>
<td>
Returns the name of the event.
</td>
</tr>
</tbody>
</table>
</td>
</tr>
</tbody>
</table>

#### Example

{% highlight html %}
<div id="container"></div>
<script>
     $("#container").ejDocumentEditor({
        importExportSetting: {
        importUrl: "http://js.syncfusion.com/demos/ejservices/api/DocumentEditor/ImportDocument",
        },
        requestNavigate: "onRequestNavigate",
    });
    function onRequestNavigate(args) {
        if (args.hyperlink.linkType == "webpage" || args.hyperlink.linkType == "email" || args.hyperlink.linkType == "file")
            window.open(args.hyperlink.navigationLink);
    }
</script>
{% endhighlight %}
