---
layout: post
title: Properties, Methods and Events of ejFileExplorer Widget
description: API reference for ejFileExplorer that provides a Windows Explorer-like functionality for any web application.
documentation: API
platform: js-api
keywords: FileExplorer, ejFileExplorer, syncfusion, FileExplorer api
---

# ejFileExplorer


FileExplorer provides a Windows Explorer-like functionality for any web application. It allows end-users to browse, select and upload files or change the folder structure by renaming, moving and deleting files or folders. File and folder management capabilities are fully customizable and can be disabled when necessary.



#### Syntax

{% highlight javascript %}

        $(element).ejFileExplorer(options)

{% endhighlight %}




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
options</td>
<td class="type"><span class="param-type">object</span></td>
<td class="description">settings for FileExplorer.</td>
</tr>
</tbody>
</table>




#### Example



{% highlight html %}
 
<div id="fileExplorer"></div> 
 
<script>
// Create FileExplorer
$('#fileExplorer').ejFileExplorer({ 
path: "http://js.syncfusion.com/demos/ejServices/Content/FileBrowser/",           
ajaxAction: "http://js.syncfusion.com/demos/ejServices/api/FileExplorer/FileOperations",
});
</script>

{% endhighlight %}







#### Requires


* module:jQuery


* module:jsrender.min.js


* module:ej.core.js


* module:ej.data.js


* module:ej.globalize.js


* module:ej.scroller.js


* module:ej.draggable.js


* module:ej.button.js


* module:ej.treeview.js


* module:ej.uploadbox.js


* module:ej.waitingpopup.js


* module:ej.dialog.js


* module:ej.splitter.js


* module:ej.toolbar.js


* module:ej.tooltip.js


* module:ej.menu.js


* module:ej.fileexplorer.js


* module:ej.checkbox.js


* module:ej.splitbutton.js


* module:ej.grid.edit.js


* module:ej.grid.filter.js


* module:ej.grid.selection.js


* module:ej.gridresize.js


* module:ej.grid.sort.js


* module:ej.grid.dragAndDrop.js


* module:ej.grid.common.js


* module:ej.grid.base.js




## Members



### ajaxAction `string`
{:#members:ajaxaction}



Sets the URL of server side AJAX handling method that handles file operation like Read, Remove, Rename, Create, Upload, Download, Copy and Move in FileExplorer.




#### Default Value







* ""








#### Example



{% highlight html %}
        
        <div id="fileExplorer"></div> 
        
        <script>
        // Initialize the FileExplorer with ajaxAction value specified.
        $('#fileExplorer').ejFileExplorer({            
        path: "http://js.syncfusion.com/demos/ejServices/Content/FileBrowser/",           
        ajaxAction: "http://js.syncfusion.com/demos/ejServices/api/FileExplorer/FileOperations"
        });
        </script>

{% endhighlight %}



### ajaxDataType `string`
{:#members:ajaxdatatype}

Specifies the data type of server side AJAX handling method. 

#### Default Value


* "json"

#### Example



{% highlight html %}
 
        <div id="fileExplorer"></div> 
        
        <script>
        // Initialize the FileExplorer with ajaxDataType value specified.
        $('#fileExplorer').ejFileExplorer({
        ajaxDataType: "jsonp",            
        path: "http://js.syncfusion.com/demos/ejServices/Content/FileBrowser/",           
        ajaxAction: "http://js.syncfusion.com/demos/ejServices/api/FileExplorer/FileOperations"
        });
        </script>

{% endhighlight %}



### ajaxSettings `object`
{:#members:ajaxsettings}








By using ajaxSettings property, you can customize the AJAX configurations. Normally you can customize the following option in AJAX handling data, URL, type, async, contentType, dataType and success. For upload, download and getImage API, you can only customize URL.




#### Default Value







* { read: {}, createFolder: {}, remove: {}, rename: {}, paste: {}, getDetails: {}, download: {}, upload: {}, getImage: {}, search: {}}








#### Example



{% highlight html %}
 
        <div id="fileExplorer"></div> 
        
        <script>
        // Initialize the FileExplorer with ajaxSettings value specified.
        $('#fileExplorer').ejFileExplorer({            
        path: "http://js.syncfusion.com/demos/ejServices/Content/FileBrowser/",           
        ajaxAction: "http://js.syncfusion.com/demos/ejServices/api/FileExplorer/FileOperations",      
        ajaxSettings: {
            read: {
                url: "http://js.syncfusion.com/demos/ejServices/api/FileExplorer/FileOperations",
                dataType: "jsonp"
            }
        }
        });
        </script>

{% endhighlight %}



### allowDragAndDrop `boolean`
{:#members:allowdraganddrop}

The FileExplorer allows to move the files from one folder to another folder of FileExplorer by using drag and drop option. Also it supports to upload a file by dragging it from windows explorer to the necessary folder of ejFileExplorer.  

#### Default Value


* true

#### Example



{% highlight html %}
 
        <div id="fileExplorer"></div> 
        
        <script>
        // Initialize the FileExplorer with allowDragAndDrop value specified.
        $('#fileExplorer').ejFileExplorer({
        allowDragAndDrop: false,            
        path: "http://js.syncfusion.com/demos/ejServices/Content/FileBrowser/",           
        ajaxAction: "http://js.syncfusion.com/demos/ejServices/api/FileExplorer/FileOperations"
        });
        </script>
        
{% endhighlight %}


### allowKeyboardNavigation `boolean`
{:#members:allowkeyboardnavigation}

Gets or sets a value that indicates whether to enable keyboard support for FileExplorer actions.

#### Default Value


* true

#### Example



{% highlight html %}
 
        <div id="fileExplorer"></div> 
        
        <script>
        // Initialize the FileExplorer with allowKeyboardNavigation value specified.
        $('#fileExplorer').ejFileExplorer({
        allowKeyboardNavigation: false,            
        path: "http://js.syncfusion.com/demos/ejServices/Content/FileBrowser/",           
        ajaxAction: "http://js.syncfusion.com/demos/ejServices/api/FileExplorer/FileOperations"
        });
        </script>
        
{% endhighlight %}




### allowMultiSelection `boolean`
{:#members:allowmultiselection}

The FileExplorer allows to select multiple files by enabling the allowMultiSelection property. You can perform multi selection by pressing the Ctrl key or Shift key. 

#### Default Value


* true

#### Example



{% highlight html %}
 
        <div id="fileExplorer"></div> 
        
        <script>
        // Initialize the FileExplorer with allowMultiSelection value specified.
        $('#fileExplorer').ejFileExplorer({
        allowMultiSelection: false,            
        path: "http://js.syncfusion.com/demos/ejServices/Content/FileBrowser/",           
        ajaxAction: "http://js.syncfusion.com/demos/ejServices/api/FileExplorer/FileOperations"
        });
        </script>
        
{% endhighlight %}




### contextMenuSettings `object`
{:#members:contextmenusettings}

By using the contextMenuSettings property, you can customize the ContextMenu in the FileExplorer control.


### contextMenuSettings.items `object`
{:#members:contextmenusettings-items}

The items property is used to configure and group the required ContextMenu items in FileExplorer control.

#### Default Value

* {% highlight javascript %} 
        {
        navbar: ["NewFolder", "Upload", "|", "Delete", "Rename", "|", "Cut", "Copy", "Paste", "|", "Getinfo"],
        cwd: ["Refresh", "Paste","|", "SortBy", "|", "NewFolder", "Upload", "|", "Getinfo"],
        files: ["Open", "Download", "|", "Upload", "|", "Delete", "Rename", "|", "Cut", "Copy", "Paste", "|", "OpenFolderLocation", "Getinfo"]
        }
{% endhighlight %}

#### Example


{% highlight html %}
 
        <div id="fileExplorer"></div> 
        
        <script>
        // Initialize the FileExplorer with the items value specified.
        $('#fileExplorer').ejFileExplorer({ 
        contextMenuSettings:{
                //define the ContextMenu items
                items:{
                        // removed the "NewFolder" item from NavigationPane ContextMenu
                        navbar: ["Upload", "|", "Delete", "Rename", "|", "Cut", "Copy", "Paste", "|", "Getinfo"],
                        // added the custom menu item (View) to Current working directory ContextMenu
                        cwd: ["Refresh", "Paste","|", "SortBy", "|", "NewFolder", "Upload", "|", "Getinfo", "View"],
                        // removed "Upload" item from Selected files/ folder's ContextMenu
                        files: ["Open", "Download", "|", "Delete", "Rename", "|", "Cut", "Copy", "Paste", "|", "OpenFolderLocation", "Getinfo"]
                },
        },
        path: "http://js.syncfusion.com/demos/ejServices/Content/FileBrowser/",           
        ajaxAction: "http://js.syncfusion.com/demos/ejServices/api/FileExplorer/FileOperations"               
        }); 
        </script>

{% endhighlight %}


### contextMenuSettings.customMenuFields `array`
{:#members:contextmenusettings-custommenufields}

The customMenuFields property is used to define custom functionality for custom ContextMenu item's which are defined in `items` property.

#### Default Value

* []


#### Example



{% highlight html %}
 
        <div id="fileExplorer"></div> 
        
        <script>
        // Initialize the FileExplorer with the customMenuFields value specified.
        $('#fileExplorer').ejFileExplorer({ 
        contextMenuSettings:{
                //define the ContextMenu items
                items:{
                        // removed the "NewFolder" item from NavigationPane ContextMenu
                        navbar: ["Upload", "|", "Delete", "Rename", "|", "Cut", "Copy", "Paste", "|", "Getinfo"],
                        // added the custom ContextMenu item (View) to Current working directory ContextMenu
                        cwd: ["Refresh", "Paste","|", "SortBy", "|", "NewFolder", "Upload", "|", "Getinfo", "View"],
                        // removed "Upload" item from Selected files/ folder's ContextMenu
                        files: ["Open", "Download", "|", "Delete", "Rename", "|", "Cut", "Copy", "Paste", "|", "OpenFolderLocation", "Getinfo"]
                },
                //added the custom ContextMenu item's (View) functionality
                customMenuFields: [
                {
                        id: "View",
                        text: "View",
                        child: [
                        {
                                id: "Tile",
                                text: "Tile view",
                                action: "onLayout"
                        },
                        {
                                id: "Grid",
                                text: "Grid view",
                                action: "onLayout"
                        },
                        {
                                id: "LargeIcons",
                                text: "Large icons view",
                                action: "onLayout"
                        },]
                },]
        },
        path: "http://js.syncfusion.com/demos/ejServices/Content/FileBrowser/",           
        ajaxAction: "http://js.syncfusion.com/demos/ejServices/api/FileExplorer/FileOperations"               
        });
        
        //define the action for custom ContextMenu item
        function onLayout(args) {
                var fileExplorerObj = $('#fileExplorer').data("ejFileExplorer");
                fileExplorerObj.option("layout", args.ID);
        }
        </script>

{% endhighlight %}




### cssClass `string`
{:#members:cssclass}








Sets the root class for FileExplorer theme. This cssClass API allows to use custom skinning option for File Explorer control. By defining the root class by using this API, you have to include this root class in CSS.




#### Default Value







* ""








#### Example



{% highlight html %}
 
        <div id="fileExplorer"></div> 
        
        <script>
        // Initialize the FileExplorer with cssClass value specified.
        $('#fileExplorer').ejFileExplorer({ 
        cssClass: 'gradient-lime',
        path: "http://js.syncfusion.com/demos/ejServices/Content/FileBrowser/",           
        ajaxAction: "http://js.syncfusion.com/demos/ejServices/api/FileExplorer/FileOperations"      
        });
        </script>

{% endhighlight %}







### enablePersistence `boolean`
{:#members:enablepersistence}








Specify the enablePersistence to FileExplorer to save the current model value in browser cookies for state maintains.




#### Default Value







* false








#### Example



{% highlight html %}
 
        <div id="fileExplorer"></div> 
        
        <script>
        // Initialize the FileExplorer with enablePersistence value specified.
        $('#fileExplorer').ejFileExplorer({ 
        enablePersistence: true,
        path: "http://js.syncfusion.com/demos/ejServices/Content/FileBrowser/",           
        ajaxAction: "http://js.syncfusion.com/demos/ejServices/api/FileExplorer/FileOperations"                   
        });
        </script>

{% endhighlight %}







### enableResize `boolean`
{:#members:enableresize}








Enables or disables the resize support in FileExplorer control.




#### Default Value







* false








#### Example



{% highlight html %}
 
        <div id="fileExplorer"></div> 
        
        <script>
        // Initialize the FileExplorer with enableResize value specified.
        $('#fileExplorer').ejFileExplorer({ 
        enableResize: true,
        path: "http://js.syncfusion.com/demos/ejServices/Content/FileBrowser/",           
        ajaxAction: "http://js.syncfusion.com/demos/ejServices/api/FileExplorer/FileOperations"                   
        });
        </script>

{% endhighlight %}







### enableRTL `boolean`
{:#members:enablertl}








Enables or disables the Right to Left alignment support in FileExplorer control.




#### Default Value







* false








#### Example



{% highlight html %}
 
        <div id="fileExplorer"></div> 
        
        <script>
        // Initialize the FileExplorer with enableRTL value specified.
        $('#fileExplorer').ejFileExplorer({ 
        enableRTL: true,
        path: "http://js.syncfusion.com/demos/ejServices/Content/FileBrowser/",           
        ajaxAction: "http://js.syncfusion.com/demos/ejServices/api/FileExplorer/FileOperations"                
        });
        </script>

{% endhighlight %}



### enableThumbnailCompress `boolean`
{:#members:enablethumbnailcompress}








Enables or disables the thumbnail image compression option in FileExplorer control. By enabling this option, you can reduce the thumbnail image size while loading. 




#### Default Value







* false








#### Example



{% highlight html %}
 
        <div id="fileExplorer"></div> 
        
        <script>
        // Initialize the FileExplorer with enableThumbnailCompress value specified.
        $('#fileExplorer').ejFileExplorer({ 
        enableThumbnailCompress: true,
        path: "http://js.syncfusion.com/demos/ejServices/Content/FileBrowser/",           
        ajaxAction: "http://js.syncfusion.com/demos/ejServices/api/FileExplorer/FileOperations"                
        });
        </script>

{% endhighlight %}







### fileTypes `string`
{:#members:filetypes}








Allows specified type of files only to display in FileExplorer control.




#### Default Value







* "* . *"








#### Example



{% highlight html %}
 
        <div id="fileExplorer"></div> 
        
        <script>
        // Specifies the file types that one needs to allow in FileExplorer control
        $('#fileExplorer').ejFileExplorer({ 
        fileTypes: "*.png,*.gif,*.jpg,*.jpeg,*.docx",
        path: "http://js.syncfusion.com/demos/ejServices/Content/FileBrowser/",           
        ajaxAction: "http://js.syncfusion.com/demos/ejServices/api/FileExplorer/FileOperations"               
        });
        </script>

{% endhighlight %}







### filterSettings `object`
{:#members:filtersettings}








By using filterSettings property, you can customize the search functionality of the search bar in FileExplorer control.











### filterSettings.allowSearchOnTyping `boolean`
{:#members:filtersettings-allowsearchontyping}
 
 
It allows to search the text given in search Textbox in every keyup event. When this property was set as false, searching will works only on Enter key and searchbar blur.

#### Default Value


* true


#### Example


{% highlight html %}
 
        <div id="fileExplorer"></div> 
        
        <script>
        // Initialize the FileExplorer with selectedFolder value specified.
        $('#fileExplorer').ejFileExplorer({
        path: "http://js.syncfusion.com/demos/ejServices/Content/FileBrowser/",           
        ajaxAction: "http://js.syncfusion.com/demos/ejServices/api/FileExplorer/FileOperations",
        filterSettings: {allowSearchOnTyping: false},
        });
        </script>

{% endhighlight %}








### filterSettings.caseSensitiveSearch `boolean`
{:#members:filtersettings-casesensitivesearch}








Enables or disables to perform the filter operation with case sensitive.




#### Default Value







* false








#### Example



{% highlight html %}
 
        <div id="fileExplorer"></div> 
        
        <script>
        // Specifies the case sensitive for searching operation
        $('#fileExplorer').ejFileExplorer({ 
        filterSettings: {
        caseSensitiveSearch: true,
        },
        path: "http://js.syncfusion.com/demos/ejServices/Content/FileBrowser/",           
        ajaxAction: "http://js.syncfusion.com/demos/ejServices/api/FileExplorer/FileOperations"     
        });
        </script>

{% endhighlight %}







### filterSettings.filterType `enum`
{:#members:filtersettings-filtertype}



<ts name="ej.FilterType" />




Sets the search filter type. There are several filter types available such as "startswith", "contains", "endswith". See filterType.


<table class="props">
<thead>
<tr>
<th>Name</th>
<th>Type</th>
<th>Default</th>
<th class="last">Description</th>
</tr>
</thead>
<tbody>
<tr>
<td class="name">
StartsWith</td>
<td class="type">string</td>
<td class="default">startswith</td>
<td class="description">Enum for filter type startswith</td>
</tr>
<tr>
<td class="name">
Contains</td>
<td class="type">string</td>
<td class="default">contains</td>
<td class="description">Enum for filter type contains</td>
</tr>
<td class="name">
EndsWith</td>
<td class="type">string</td>
<td class="default">endswith</td>
<td class="description">Enum for filter type endswith</td>
</tr>
</tbody>
</table>

#### Default Value







* ej.FileExplorer.filterType.Contains








#### Example



{% highlight html %}
 
        <div id="fileExplorer"></div> 
        
        <script>
        // Specifies the filter types that are used to filter the grid or list elements
        $('#fileExplorer').ejFileExplorer({
        filterSettings: { 
        filterType: "startswith",
        },
        path: "http://js.syncfusion.com/demos/ejServices/Content/FileBrowser/",           
        ajaxAction: "http://js.syncfusion.com/demos/ejServices/api/FileExplorer/FileOperations"     
        });
        </script>

{% endhighlight %}







### gridSettings `object`
{:#members:gridsettings}








By using the gridSettings property, you can customize the grid behavior in the FileExplorer control.











### gridSettings.allowResizing `boolean`
{:#members:gridsettings-allowresizing}








Allows to Resize the width of the columns by simply click and move the particular column header line.



#### Default Value







* true








#### Example



{% highlight html %}
 
        <div id="fileExplorer" ></div> 
        
        <script>
        // Initialize the FileExplorer with the allowSorting value specified for grid.
        $('#fileExplorer').ejFileExplorer({ 
        gridSettings:{allowResizing:false},
        path: "http://js.syncfusion.com/demos/ejServices/Content/FileBrowser/",           
        ajaxAction: "http://js.syncfusion.com/demos/ejServices/api/FileExplorer/FileOperations"               
        }); 
        </script>

{% endhighlight %}







### gridSettings.allowSorting `boolean`
{:#members:gridsettings-allowsorting}








Gets or sets a value that indicates whether to enable the dynamic sorting behavior on grid data. Sorting can be done through clicking on particular column header.




#### Default Value







* true








#### Example



{% highlight html %}
 
        <div id="fileExplorer" ></div> 
        
        <script>
        // Initialize the FileExplorer with the allowSorting value specified for grid.
        $('#fileExplorer').ejFileExplorer({ 
        gridSettings:{allowSorting:false},
        path: "http://js.syncfusion.com/demos/ejServices/Content/FileBrowser/",           
        ajaxAction: "http://js.syncfusion.com/demos/ejServices/api/FileExplorer/FileOperations"               
        }); 
        </script>

{% endhighlight %}







### gridSettings.columns `array`
{:#members:gridsettings-columns}








Gets or sets an object that indicates to render the grid with specified columns. You can use this property same as the column property in Grid control.




#### Default Value







* [{ field: "name", headerText: "Name", width: "30%" }, { field: "dateModified", headerText: "Date Modified", width: "30%" }, { field: "type", headerText: "Type", width: "15%" }, { field: "size", headerText: "Size", width: "12%", textAlign: "right", headerTextAlign: "left" }]








#### Example



{% highlight html %}
 
        <div id="fileExplorer"></div> 
        
        <script>
        // Initialize the FileExplorer with the columns value specified for grid.
        $('#fileExplorer').ejFileExplorer({ 
        gridSettings:{columns:[{ field: "name", headerText: "Name", width: 90 }, { field: "type", headerText: "Type", width: 95 }, { field: "size", headerText: "Size", width: 90 }]},
        path: "http://js.syncfusion.com/demos/ejServices/Content/FileBrowser/",           
        ajaxAction: "http://js.syncfusion.com/demos/ejServices/api/FileExplorer/FileOperations"               
        }); 
        </script>

{% endhighlight %}







### height `string | number`
{:#members:height}








Specifies the height of FileExplorer control.




#### Default Value







* 400








#### Example



{% highlight html %}
 
        <div id="fileExplorer"></div> 
        
        <script>
        // Initialize the FileExplorer with the height value specified.
        $('#fileExplorer').ejFileExplorer({   
        height: 450,
        path: "http://js.syncfusion.com/demos/ejServices/Content/FileBrowser/",           
        ajaxAction: "http://js.syncfusion.com/demos/ejServices/api/FileExplorer/FileOperations"            
        });
        </script>

{% endhighlight %}







### isResponsive `boolean`
{:#members:isresponsive}








Enables or disables the responsive support for FileExplorer control during the window resizing time.




#### Default Value







* false








#### Example



{% highlight html %}
 
        <div id="fileExplorer"></div> 
        
        <script>
        // Initialize the FileExplorer with isResponsive value specified.
        $('#fileExplorer').ejFileExplorer({
        isResponsive: true,
        width: "70%",
        height: "50%",
        path: "http://js.syncfusion.com/demos/ejServices/Content/FileBrowser/",
        ajaxAction: "http://js.syncfusion.com/demos/ejServices/api/FileExplorer/FileOperations"
        });
        </script>

{% endhighlight %}







### layout `enum`
{:#members:layout}



<ts name="ej.FileExplorer.layoutType"/>




Sets the file view type. There are three view types available such as Grid, Tile and Large icons. See layoutType.


<table class="props">
<thead>
<tr>
<th>Name</th>
<th class="last">Description</th>
</tr>
</thead>
<tbody>
<tr>
<td class="name">
Tile</td>
<td class="description">Supports to display files in tile view</td>
</tr>
<tr>
<td class="name">
Grid</td>
<td class="description">Supports to display files in grid view </td>
</tr>
<tr>
<td class="name">
LargeIcons</td>
<td class="description">Supports to display files as large icons</td>
</tr>
</tbody>
</table>

#### Default Value







* ej.FileExplorer.layoutType.Grid








#### Example



{% highlight html %}
 
        <div id="fileExplorer"></div> 
        
        <script>
        // Initialize the FileExplorer with the layout value specified.
        $('#fileExplorer').ejFileExplorer({ 
        layout: "tile",
        path: "http://js.syncfusion.com/demos/ejServices/Content/FileBrowser/",           
        ajaxAction: "http://js.syncfusion.com/demos/ejServices/api/FileExplorer/FileOperations"                 
        }); 
        </script>

{% endhighlight %}







### locale `string`
{:#members:locale}








Sets the culture in FileExplorer.




#### Default Value







* "en-US"








#### Example



{% highlight html %}
 
        <div id="fileExplorer"></div> 
        
        <script>
        // Initialize the FileExplorer with the culture value specified.
        $('#fileExplorer').ejFileExplorer({ 
        locale: "en-US",
        path: "http://js.syncfusion.com/demos/ejServices/Content/FileBrowser/",           
        ajaxAction: "http://js.syncfusion.com/demos/ejServices/api/FileExplorer/FileOperations"               
        });
        </script>

{% endhighlight %}



### maxHeight `string | number`
{:#members:maxheight}

Sets the maximum height of FileExplorer control. 

#### Default Value


* null

#### Example



{% highlight html %}
 
        <div id="fileExplorer"></div> 
        
        <script>
        // Initialize the FileExplorer with maxHeight value specified.
        $('#fileExplorer').ejFileExplorer({
        maxHeight: 500,            
        path: "http://js.syncfusion.com/demos/ejServices/Content/FileBrowser/",           
        ajaxAction: "http://js.syncfusion.com/demos/ejServices/api/FileExplorer/FileOperations"
        });
        </script>

{% endhighlight %}


### maxWidth `string | number`
{:#members:maxwidth}

Sets the maximum width of FileExplorer control. 

#### Default Value


* null

#### Example



{% highlight html %}
 
        <div id="fileExplorer"></div> 
        
        <script>
        // Initialize the FileExplorer with maxWidth value specified.
        $('#fileExplorer').ejFileExplorer({
        maxWidth: 1000,            
        path: "http://js.syncfusion.com/demos/ejServices/Content/FileBrowser/",           
        ajaxAction: "http://js.syncfusion.com/demos/ejServices/api/FileExplorer/FileOperations"
        });
        </script>

{% endhighlight %}


### minHeight `string | number`
{:#members:minheight}

Sets the minimum height of FileExplorer control. 

#### Default Value


* "250px"

#### Example



{% highlight html %}
 
        <div id="fileExplorer"></div> 
        
        <script>
        // Initialize the FileExplorer with minHeight value specified.
        $('#fileExplorer').ejFileExplorer({
        minHeight: 300,            
        path: "http://js.syncfusion.com/demos/ejServices/Content/FileBrowser/",           
        ajaxAction: "http://js.syncfusion.com/demos/ejServices/api/FileExplorer/FileOperations"
        });
        </script>

{% endhighlight %}


### minWidth `string | number`
{:#members:minwidth}

Sets the minimum width of FileExplorer control. 

#### Default Value


* "400px"

#### Example



{% highlight html %}
 
        <div id="fileExplorer"></div> 
        
        <script>
        // Initialize the FileExplorer with minWidth value specified.
        $('#fileExplorer').ejFileExplorer({
        minWidth: 300,            
        path: "http://js.syncfusion.com/demos/ejServices/Content/FileBrowser/",           
        ajaxAction: "http://js.syncfusion.com/demos/ejServices/api/FileExplorer/FileOperations"
        });
        </script>

{% endhighlight %}



### path `string`
{:#members:path}








The property path denotes the filesystem path that are to be explored. The path for the filesystem can be physical path or relative path, but it has to be relevant to where the Web API is hosted.




#### Default Value







* ""








#### Example



{% highlight html %}
 
        <div id="fileExplorer"></div> 
        
        <script>
        // Specifies the root folder path that has to be specified in FileExplorer control
        $('#fileExplorer').ejFileExplorer({            
        path: "http://js.syncfusion.com/demos/ejServices/Content/FileBrowser/",           
        ajaxAction: "http://js.syncfusion.com/demos/ejServices/api/FileExplorer/FileOperations"                                 
        });
        </script>

{% endhighlight %}


### rootFolderName `string`
{:#members:rootfoldername}

Sets the alias name of root folder name in FileExplorer. It is used to replace the actual root folder name in FileExplorer.

#### Default Value

* ""

#### Example

{% highlight html %}
        
        <div id="fileExplorer"></div> 
        
        <script>
        // Initialize the FileExplorer with ajaxAction value specified.
        $('#fileExplorer').ejFileExplorer({            
        path: "http://js.syncfusion.com/demos/ejServices/Content/FileBrowser/",           
        ajaxAction: "http://js.syncfusion.com/demos/ejServices/api/FileExplorer/FileOperations",
        rootFolderName: "This PC", // The name to replace your actual root folder name(FileBrowser).
        });
        </script>

{% endhighlight %}


### selectedFolder `string`
{:#members:selectedfolder}

The selectedFolder is used to select the specified folder of FileExplorer control. 

#### Default Value


* ""

#### Example



{% highlight html %}
 
        <div id="fileExplorer"></div> 
        
        <script>
        // Initialize the FileExplorer with selectedFolder value specified.
        $('#fileExplorer').ejFileExplorer({
        selectedFolder: "http://js.syncfusion.com/demos/ejServices/Content/FileBrowser/Food",            
        path: "http://js.syncfusion.com/demos/ejServices/Content/FileBrowser/",           
        ajaxAction: "http://js.syncfusion.com/demos/ejServices/api/FileExplorer/FileOperations"
        });
        </script>

{% endhighlight %}



### selectedItems `string | array`
{:#members:selecteditems}

The selectedItems is used to select the specified items (file, folder) of FileExplorer control. 

#### Default Value


* ""

#### Example



{% highlight html %}
 
        <div id="fileExplorer"></div> 
        
        <script>
        // Initialize the FileExplorer with selectedItems value specified.
        $('#fileExplorer').ejFileExplorer({
        selectedItems: ["Food", "Nature"],            
        path: "http://js.syncfusion.com/demos/ejServices/Content/FileBrowser/",           
        ajaxAction: "http://js.syncfusion.com/demos/ejServices/api/FileExplorer/FileOperations"
        });
        </script>

{% endhighlight %}


### showCheckbox `boolean`
{:#members:showcheckbox}


Enables or disables the checkbox option in FileExplorer control.


#### Default Value


* true


#### Example



{% highlight html %}
 
        <div id="fileExplorer"></div> 
        
        <script>
        // Initialize the FileExplorer with the showCheckbox value specified.
        $('#fileExplorer').ejFileExplorer({ 
        showCheckbox: false,
        path: "http://js.syncfusion.com/demos/ejServices/Content/FileBrowser/",           
        ajaxAction: "http://js.syncfusion.com/demos/ejServices/api/FileExplorer/FileOperations"                     
        });
        </script>

{% endhighlight %}




### showContextMenu `boolean`
{:#members:showcontextmenu}








Enables or disables the context menu option in FileExplorer control.




#### Default Value







* true








#### Example



{% highlight html %}
 
        <div id="fileExplorer"></div> 
        
        <script>
        // Initialize the FileExplorer with the showContextMenu value specified.
        $('#fileExplorer').ejFileExplorer({ 
        showContextMenu: false,
        path: "http://js.syncfusion.com/demos/ejServices/Content/FileBrowser/",           
        ajaxAction: "http://js.syncfusion.com/demos/ejServices/api/FileExplorer/FileOperations"                     
        });
        </script>

{% endhighlight %}







### showFooter `boolean`
{:#members:showfooter}








Enables or disables the footer in FileExplorer control. The footer element displays the details of the current selected files and folders. And also the footer having the switcher to change the layout view.




#### Default Value







* true








#### Example



{% highlight html %}
 
        <div id="fileExplorer"></div> 
        
        <script>
        // Initialize the FileExplorer with the showFooter value specified.
        $('#fileExplorer').ejFileExplorer({ 
        showFooter: false,
        path: "http://js.syncfusion.com/demos/ejServices/Content/FileBrowser/",           
        ajaxAction: "http://js.syncfusion.com/demos/ejServices/api/FileExplorer/FileOperations"                   
        });
        </script>

{% endhighlight %}



### showRoundedCorner `boolean`
{:#members:showroundedcorner}


FileExplorer control is displayed with rounded corner when this property is set to true.


#### Default Value


* false


#### Example



{% highlight html %}
 
        <div id="fileExplorer" ></div> 
        
        <script>
        // Initialize the FileExplorer with the showRoundedCorner value specified.
        $('#fileExplorer').ejFileExplorer({ 
        showRoundedCorner: true,
        path: "http://js.syncfusion.com/demos/ejServices/Content/FileBrowser/",           
        ajaxAction: "http://js.syncfusion.com/demos/ejServices/api/FileExplorer/FileOperations"                
        });
        </script>

{% endhighlight %}



### showThumbnail `boolean`
{:#members:showthumbnail}


FileExplorer control is rendered with thumbnail preview of images in Tile and LargeIcons layout when this property set to true.


#### Default Value


* true


#### Example


{% highlight html %}
 
        <div id="fileExplorer" ></div> 
        
        <script>
        // Initialize the FileExplorer with the showThumbnail value specified.
        $('#fileExplorer').ejFileExplorer({ 
        showThumbnail: false,
        path: "http://js.syncfusion.com/demos/ejServices/Content/FileBrowser/",           
        ajaxAction: "http://js.syncfusion.com/demos/ejServices/api/FileExplorer/FileOperations"                
        });
        </script>

{% endhighlight %}



### showToolbar `boolean`
{:#members:showtoolbar}








Shows or disables the toolbar in FileExplorer control.




#### Default Value







* true








#### Example



{% highlight html %}
 
        <div id="fileExplorer" ></div> 
        
        <script>
        // Initialize the FileExplorer with the showToolbar value specified.
        $('#fileExplorer').ejFileExplorer({ 
        showToolbar: false,
        path: "http://js.syncfusion.com/demos/ejServices/Content/FileBrowser/",           
        ajaxAction: "http://js.syncfusion.com/demos/ejServices/api/FileExplorer/FileOperations"                
        });
        </script>

{% endhighlight %}







### showNavigationPane `boolean`
{:#members:shownavigationpane}








Enables or disables the navigation pane in FileExplorer control. The navigation pane contains a tree view element that displays all the folders from the filesystem in a hierarchical manner. This is useful to a quick navigation of any folder in the filesystem.




#### Default Value







* true








#### Example



{% highlight html %}
 
        <div id="fileExplorer" ></div> 
        
        <script>
        // Initialize the FileExplorer with the showNavigationPane value specified.
        $('#fileExplorer').ejFileExplorer({ 
        showNavigationPane: false,
        path: "http://js.syncfusion.com/demos/ejServices/Content/FileBrowser/",           
        ajaxAction: "http://js.syncfusion.com/demos/ejServices/api/FileExplorer/FileOperations"                 
        }); 
        </script>

{% endhighlight %}







### tools `object`
{:#members:tools}








The tools property is used to configure and group required toolbar items in FileExplorer control.




#### Default Value







* { creation: ["NewFolder"], navigation: ["Back", "Forward", "Upward"], addressBar: ["Addressbar"], editing: ["Refresh", "Upload", "Delete", "Rename", "Download"], copyPaste: ["Cut", "Copy", "Paste"], getProperties: ["Details"], searchBar: ["Searchbar"], layout: ["Layout"], sortBy: ["SortBy"]}








#### Example



{% highlight html %}
            
            <div id="fileExplorer" ></div> 
            
            <script>
            // Initialize the FileExplorer with toolbar tools value specified.
            $('#fileExplorer').ejFileExplorer({ 
            tools: {
            creation:["NewFolder", "Open"],
            navigation: ["Back", "Forward", "Upward"],
            addressBar: ["Addressbar"],
            editing: ["Refresh", "Upload", "Delete", "Rename", "Download"],
            copyPaste: ["Cut", "Copy", "Paste"],
            getProperties: ["Details"],
            searchBar: ["Searchbar"]
            },
            path: "http://js.syncfusion.com/demos/ejServices/Content/FileBrowser/",           
            ajaxAction: "http://js.syncfusion.com/demos/ejServices/api/FileExplorer/FileOperations"        
            });
            </script>

{% endhighlight %}







### toolsList `array`
{:#members:toolslist}








The toolsList property is used to arrange the toolbar items in the FileExplorer control.




#### Default Value







* ["layout", "creation", "navigation", "addressBar", "editing", "copyPaste", "sortBy", "getProperties", "searchBar"]








#### Example



{% highlight html %}
        
        <div id="fileExplorer"></div> 
        
        <script>
        // Initialize the FileExplorer with toolsList value specified.
        $('#fileExplorer').ejFileExplorer({ 
        toolsList: ["navigation", "creation", "addressBar", "editing", "copyPaste", "getProperties", "searchBar"],
        path: "http://js.syncfusion.com/demos/ejServices/Content/FileBrowser/",           
        ajaxAction: "http://js.syncfusion.com/demos/ejServices/api/FileExplorer/FileOperations"                 
        }); 
        </script>

{% endhighlight %}







### uploadSettings `object`
{:#members:uploadsettings}








Gets or sets an object that indicates whether to customize the upload behavior in the FileExplorer.





### uploadSettings.allowMultipleFile `boolean`
{:#members:uploadsettings-allowmultiplefile}








Enables or disables the multiple files upload. When it is enabled, you can upload multiple files at a time and when disabled, you can upload only one file at a time.




#### Default Value







* true








#### Example



{% highlight html %}
 
        <div id="fileExplorer"></div> 
        
        <script>
        // Initialize the FileExplorer with the multipleFilesSelection value specified for uploadbox.
        $('#fileExplorer').ejFileExplorer({ 
        uploadSettings:{allowMultipleFile:false},
        path: "http://js.syncfusion.com/demos/ejServices/Content/FileBrowser/",           
        ajaxAction: "http://js.syncfusion.com/demos/ejServices/api/FileExplorer/FileOperations"                
        }); 
        </script>

{% endhighlight %}





### uploadSettings.autoUpload `boolean`
{:#members:uploadsettings-autoupload}








Enables or disables the auto upload option while uploading files in FileExplorer control.




#### Default Value







* false








#### Example



{% highlight html %}
 
        <div id="fileExplorer"></div> 
        
        <script>
        // Initialize the FileExplorer with auto upload option as true.
        $('#fileExplorer').ejFileExplorer({ 
        uploadSettings:{autoUpload:true},
        path: "http://js.syncfusion.com/demos/ejServices/Content/FileBrowser/",           
        ajaxAction: "http://js.syncfusion.com/demos/ejServices/api/FileExplorer/FileOperations"                
        }); 
        </script>

{% endhighlight %}





### uploadSettings.dialogAction `object`
{:#members:uploadsettings-dialogaction}








Specifies the actions for upload dialog during initialization.




#### Default Value







* { modal:false, closeOnComplete:false, content:null, drag:true }








#### Example



{% highlight html %}
 
        <div id="fileExplorer"></div> 
        
        <script>
        // Sets the  dialogAction API value
        $('#fileExplorer').ejFileExplorer({ 
        dialogAction:{ modal:false, closeOnComplete:false,resize: false, drag:true, content:"#controlId" },
        path: "http://js.syncfusion.com/demos/ejServices/Content/FileBrowser/",           
        ajaxAction: "http://js.syncfusion.com/demos/ejServices/api/FileExplorer/FileOperations"                
        }); 
        </script>

{% endhighlight %}





### uploadSettings.dialogPosition `object`
{:#members:uploadsettings-dialogposition}








Specifies the position at which the upload dialog is displayed using X and Y values. X: Sets the left position value for dialog. Y: Sets the top position value for dialog.




#### Default Value







* null








#### Example



{% highlight html %}
 
        <div id="fileExplorer"></div> 
        
        <script>
        // Sets the dialogPosition API value during initialization
        $('#fileExplorer').ejFileExplorer({ 
        dialogPosition: { X: 200, Y: 30 },
        path: "http://js.syncfusion.com/demos/ejServices/Content/FileBrowser/",           
        ajaxAction: "http://js.syncfusion.com/demos/ejServices/api/FileExplorer/FileOperations"                
        }); 
        </script>

{% endhighlight %}





### uploadSettings.maxFileSize `number`
{:#members:uploadsettings-maxfilesize}








Specifies the maximum file size allowed to upload. It accepts the value in bytes.




#### Default Value







* 31457280








#### Example



{% highlight html %}
 
        <div id="fileExplorer"></div> 
        
        <script>
        // Initialize the FileExplorer with the maxFileSize value specified for uploadbox.
        $('#fileExplorer').ejFileExplorer({ 
        uploadSettings:{maxFileSize:10000},
        path: "http://js.syncfusion.com/demos/ejServices/Content/FileBrowser/",           
        ajaxAction: "http://js.syncfusion.com/demos/ejServices/api/FileExplorer/FileOperations"                
        }); 
        </script>

{% endhighlight %}





### uploadSettings.showFileDetails `boolean`
{:#members:uploadsettings-showfiledetails}








Specifies the file details which are to be displayed when selected for upload by setting the `showFileDetails` to true.




#### Default Value







* true








#### Example



{% highlight html %}
 
        <div id="fileExplorer"></div> 
        
        <script>
        // Sets the showFileDetails API value during initialization
        $('#fileExplorer').ejFileExplorer({ 
        showFileDetails: false,
        path: "http://js.syncfusion.com/demos/ejServices/Content/FileBrowser/",           
        ajaxAction: "http://js.syncfusion.com/demos/ejServices/api/FileExplorer/FileOperations"                
        }); 
        </script>

{% endhighlight %}




### virtualItemCount `number`
{:#members:virtualitemcount}








Specifies the virtual item count for virtual support.




#### Default Value







* 0








#### Example



{% highlight html %}
 
        <div id="fileExplorer"></div> 
        
        <script>
        // Initialize the FileExplorer with the virtualItemCount value specified.
        $('#fileExplorer').ejFileExplorer({
        virtualItemCount: 40,
        path: "http://js.syncfusion.com/demos/ejServices/Content/FileBrowser/",           
        ajaxAction: "http://js.syncfusion.com/demos/ejServices/api/FileExplorer/FileOperations"                     
        });
        </script>

{% endhighlight %}






### width `string | number`
{:#members:width}








Specifies the width of FileExplorer control.




#### Default Value







* 850








#### Example



{% highlight html %}
 
        <div id="fileExplorer"></div> 
        
        <script>
        // Initialize the FileExplorer with the width value specified.
        $('#fileExplorer').ejFileExplorer({   
        width: 800,
        path: "http://js.syncfusion.com/demos/ejServices/Content/FileBrowser/",           
        ajaxAction: "http://js.syncfusion.com/demos/ejServices/api/FileExplorer/FileOperations"                     
        });
        </script>

{% endhighlight %}





## Methods



### adjustSize()
{:#methods:adjustsize}


Refresh the size of FileExplorer control.

#### Example



{% highlight html %}
 
        <div id="fileExplorer"></div> 
        
        <script>
        // refresh the size of FileExplorer 
        $('#fileExplorer').ejFileExplorer({      
        path: "http://js.syncfusion.com/demos/ejServices/Content/FileBrowser/",           
        ajaxAction: "http://js.syncfusion.com/demos/ejServices/api/FileExplorer/FileOperations"           
        });
        // Create FileExplorer instance
        var fileExplorerObj = $("#fileExplorer").data("ejFileExplorer");
        fileExplorerObj.adjustSize(); // refresh the size of file explorer               
        </script>

{% endhighlight %}



### disableMenuItem(item)
{:#methods:disablemenuitem}


Disable the particular context menu item.

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
item</td>
<td class="type"><span class="param-type">string | element</span></td>
<td class="description">Id of the menu item/ Menu element to be disabled </td>
</tr>
</tbody>
</table>

#### Example



{% highlight html %}
 
        <div id="fileExplorer"></div> 
        
        <script>
        // disable the context menu item 
        $('#fileExplorer').ejFileExplorer({      
        path: "http://js.syncfusion.com/demos/ejServices/Content/FileBrowser/",           
        ajaxAction: "http://js.syncfusion.com/demos/ejServices/api/FileExplorer/FileOperations"           
        });
        // Create FileExplorer instance
        var fileExplorerObj = $("#fileExplorer").data("ejFileExplorer");
        fileExplorerObj.disableMenuItem("Upload"); // disable upload option                         
        </script>

{% endhighlight %}



### disableToolbarItem(item)
{:#methods:disabletoolbaritem}








Disable the particular toolbar item.


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
item</td>
<td class="type"><span class="param-type">string | element</span></td>
<td class="description">Id of the toolbar item/ Tool item element to be disabled </td>
</tr>
</tbody>
</table>


#### Example



{% highlight html %}
 
        <div id="fileExplorer" ></div> 
        
        <script>
        // disable the toolbar tool 
        $('#fileExplorer').ejFileExplorer({      
        path: "http://js.syncfusion.com/demos/ejServices/Content/FileBrowser/",           
        ajaxAction: "http://js.syncfusion.com/demos/ejServices/api/FileExplorer/FileOperations"           
        });
        // Create FileExplorer instance
        var fileExplorerObj = $("#fileExplorer").data("ejFileExplorer");
        fileExplorerObj.disableToolbarItem("Searchbar"); // disable search bar                           
        </script>

{% endhighlight %}




### enableMenuItem(item)
{:#methods:enablemenuitem}

Enable the particular context menu item.

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
item</td>
<td class="type"><span class="param-type">string | Element</span></td>
<td class="description">Id of the menu item/ Menu element to be Enabled </td>
</tr>
</tbody>
</table>

#### Example



{% highlight html %}
 
        <div id="fileExplorer" ></div> 
        
        <script>
        // enable the context menu item 
        $('#fileExplorer').ejFileExplorer({      
        path: "http://js.syncfusion.com/demos/ejServices/Content/FileBrowser/",           
        ajaxAction: "http://js.syncfusion.com/demos/ejServices/api/FileExplorer/FileOperations"            
        });
        // Create FileExplorer instance
        var fileExplorerObj = $("#fileExplorer").data("ejFileExplorer");
        fileExplorerObj.enableMenuItem("Upload"); // enable upload option in context menu                     
        </script>

{% endhighlight %}



### enableToolbarItem(item)
{:#methods:enabletoolbaritem}








Enable the particular toolbar item


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
item</td>
<td class="type"><span class="param-type">string | Element</span></td>
<td class="description">Id of the tool item/ Tool item element to be Enabled </td>
</tr>
</tbody>
</table>



#### Example



{% highlight html %}
 
        <div id="fileExplorer" ></div> 
        
        <script>
        // enable the toolbar tool 
        $('#fileExplorer').ejFileExplorer({      
        path: "http://js.syncfusion.com/demos/ejServices/Content/FileBrowser/",           
        ajaxAction: "http://js.syncfusion.com/demos/ejServices/api/FileExplorer/FileOperations"            
        });
        // Create FileExplorer instance
        var fileExplorerObj = $("#fileExplorer").data("ejFileExplorer");
        fileExplorerObj.enableToolbarItem("Searchbar"); // enable search bar                     
        </script>

{% endhighlight %}



### refresh()
{:#methods:refresh}


Refresh the content of the selected folder in FileExplorer control.

#### Example



{% highlight html %}
 
        <div id="fileExplorer"></div> 
        
        <script>
        // refresh the content of selected folder 
        $('#fileExplorer').ejFileExplorer({      
        path: "http://js.syncfusion.com/demos/ejServices/Content/FileBrowser/",           
        ajaxAction: "http://js.syncfusion.com/demos/ejServices/api/FileExplorer/FileOperations"           
        });
        // Create FileExplorer instance
        var fileExplorerObj = $("#fileExplorer").data("ejFileExplorer");
        fileExplorerObj.refresh(); // refresh the content of selected folder               
        </script>

{% endhighlight %}



### removeToolbarItem(item)
{:#methods:removetoolbaritem}








Remove the particular toolbar item.

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
item</td>
<td class="type"><span class="param-type">string | Element</span></td>
<td class="description">Id of the tool item/ tool item element to be removed </td>
</tr>
</tbody>
</table>



#### Example



{% highlight html %}
 
        <div id="fileExplorer" ></div> 
        
        <script>
        // remove the toolbar tool 
        $('#fileExplorer').ejFileExplorer({      
        path: "http://js.syncfusion.com/demos/ejServices/Content/FileBrowser/",           
        ajaxAction: "http://js.syncfusion.com/demos/ejServices/api/FileExplorer/FileOperations"            
        });
        // Create FileExplorer instance
        var fileExplorerObj = $("#fileExplorer").data("ejFileExplorer");
        fileExplorerObj.removeToolbarItem("Searchbar"); // remove search bar                     
        </script>

{% endhighlight %}



## Events



### beforeAjaxRequest
{:#events:beforeajaxrequest}

Fires before the AJAX request is performed.

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
argument</td>
<td class="type"><span class="param-type">Object</span></td>
<td class="description">Event parameters from FileExplorer
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
cancel</td>
<td class="type"><span class="param-type">boolean</span></td>
<td class="description">Set to true when the event has to be canceled, else false.</td>
</tr>
<tr>
<td class="name">
data</td>
<td class="type"><span class="param-type">object</span></td>
<td class="description">returns the AJAX request data</td>
</tr>
<tr>
<td class="name">
model</td>
<td class="type"><ts ref="ej.FileExplorer.Model"/>
<span class="param-type">object</span></td>
<td class="description">returns the FileExplorer model</td>
</tr>
<tr>
<td class="name">
type</td>
<td class="type"><span class="param-type">string</span></td>
<td class="description">returns the name of the event</td>
</tr>
</tbody>
</table>
</td>
</tr>
</tbody>
</table>



#### Example



{% highlight html %}
 
        <div id="fileExplorer" ></div> 
        
        <script>
        // beforeAjaxRequest event for FileExplorer
        $('#fileExplorer').ejFileExplorer({            
        path: "http://js.syncfusion.com/demos/ejServices/Content/FileBrowser/",         
        ajaxAction: "http://js.syncfusion.com/demos/ejServices/api/FileExplorer/FileOperations",      
        beforeAjaxRequest: function (args) {}
        });
        </script>

{% endhighlight %}



### beforeDownload
{:#events:beforedownload}



Fires before downloading the files.

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
argument</td>
<td class="type"><span class="param-type">Object</span></td>
<td class="description">Event parameters from FileExplorer
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
cancel</td>
<td class="type"><span class="param-type">boolean</span></td>
<td class="description">Set to true when the event has to be canceled, else false.</td>
</tr>
<tr>
<td class="name">
files</td>
<td class="type"><span class="param-type">string[]</span></td>
<td class="description">returns the downloaded file names.</td>
</tr>
<tr>
<td class="name">
model</td>
<td class="type"><ts ref="ej.FileExplorer.Model"/>
<span class="param-type">object</span></td>
<td class="description">returns the FileExplorer model.</td>
</tr>
<tr>
<td class="name">
path</td>
<td class="type"><span class="param-type">string</span></td>
<td class="description">returns the path of currently opened item.</td>
</tr>
<tr>
<td class="name">
selectedItems</td>
<td class="type"><span class="param-type">object</span></td>
<td class="description">returns the selected item details.</td>
</tr>
<tr>
<td class="name">
type</td>
<td class="type"><span class="param-type">string</span></td>
<td class="description">returns the name of the event.</td>
</tr>
</tbody>
</table>
</td>
</tr>
</tbody>
</table>



#### Example



{% highlight html %}
 
        <div id="fileExplorer" ></div> 
        
        <script>
        // beforeDownload event for FileExplorer
        $('#fileExplorer').ejFileExplorer({            
        path: "http://js.syncfusion.com/demos/ejServices/Content/FileBrowser/",         
        ajaxAction: "http://js.syncfusion.com/demos/ejServices/api/FileExplorer/FileOperations",      
        beforeDownload: function (args) {}
        });
        </script>

{% endhighlight %}





### beforeGetImage
{:#events:beforegetimage}



Fires before getting a requested image from server. Also this event will be triggered when you have enabled thumbnail image compression option in FileExplorer. 
Using this event, you can customize the image compression size.


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
path</td>
<td class="type"><span class="param-type">String</span></td>
<td class="description"> Image path
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
cancel</td>
<td class="type"><span class="param-type">boolean</span></td>
<td class="description">set to true when the event has to be canceled, else false.</td>
</tr>
<tr>
<td class="name">
canCompress</td>
<td class="type"><span class="param-type">boolean</span></td>
<td class="description">enable or disable the image compress option.</td>
</tr>
<tr>
<td class="name">
model</td>
<td class="type"><ts ref="ej.FileExplorer.Model"/>
<span class="param-type">object</span></td>
<td class="description">returns the FileExplorer model.</td>
</tr>
<tr>
<td class="name">
size</td>
<td class="type"><span class="param-type">object</span></td>
<td class="description">returns the expected image size.</td>
</tr>
<tr>
<td class="name">
selectedItems</td>
<td class="type"><span class="param-type">object</span></td>
<td class="description">returns the selected item details.</td>
</tr>
<tr>
<td class="name">
type</td>
<td class="type"><span class="param-type">string</span></td>
<td class="description">returns the name of the event.</td>
</tr>
</tbody>
</table>
</td>
</tr>
</tbody>
</table>



#### Example



{% highlight html %}
 
        <div id="fileExplorer" ></div> 
        
        <script>
        // beforeGetImage event for FileExplorer
        $('#fileExplorer').ejFileExplorer({            
        path: "http://js.syncfusion.com/demos/ejServices/Content/FileBrowser/",         
        ajaxAction: "http://js.syncfusion.com/demos/ejServices/api/FileExplorer/FileOperations",      
        beforeGetImage: function (args) {}
        });
        </script>

{% endhighlight %}





### beforeOpen
{:#events:beforeopen}



Fires before files or folders open.

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
argument</td>
<td class="type"><span class="param-type">Object</span></td>
<td class="description">Event parameters from FileExplorer
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
cancel</td>
<td class="type"><span class="param-type">boolean</span></td>
<td class="description">Set to true when the event has to be canceled, else false.</td>
</tr>
<tr>
<td class="name">
itemType</td>
<td class="type"><span class="param-type">string</span></td>
<td class="description">returns the opened item type.</td>
</tr>
<tr>
<td class="name">
model</td>
<td class="type"><ts ref="ej.FileExplorer.Model"/>
<span class="param-type">object</span></td>
<td class="description">returns the FileExplorer model.</td>
</tr>
<tr>
<td class="name">
path</td>
<td class="type"><span class="param-type">string</span></td>
<td class="description">returns the path of currently opened item.</td>
</tr>
<tr>
<td class="name">
selectedItems</td>
<td class="type"><span class="param-type">object</span></td>
<td class="description">returns the selected item details.</td>
</tr>
<tr>
<td class="name">
type</td>
<td class="type"><span class="param-type">string</span></td>
<td class="description">returns the name of the event.</td>
</tr>
</tbody>
</table>
</td>
</tr>
</tbody>
</table>
</tr>
</tbody>
</table>




#### Example



{% highlight html %}
 
        <div id="fileExplorer" ></div> 
        
        <script>
        // beforeOpen event for FileExplorer
        $('#fileExplorer').ejFileExplorer({            
        path: "http://js.syncfusion.com/demos/ejServices/Content/FileBrowser/",         
        ajaxAction: "http://js.syncfusion.com/demos/ejServices/api/FileExplorer/FileOperations",      
        beforeOpen: function (args) {}
        });
        </script>

{% endhighlight %}



### beforeUpload
{:#events:beforeupload}



Fires before uploading the files.

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
argument</td>
<td class="type"><span class="param-type">Object</span></td>
<td class="description">Event parameters from FileExplorer
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
cancel</td>
<td class="type"><span class="param-type">boolean</span></td>
<td class="description">Set to true when the event has to be canceled, else false.</td>
</tr>
<tr>
<td class="name">
model</td>
<td class="type"><ts ref="ej.FileExplorer.Model"/>
<span class="param-type">object</span></td>
<td class="description">returns the FileExplorer model.</td>
</tr>
<tr>
<td class="name">
path</td>
<td class="type"><span class="param-type">string</span></td>
<td class="description">returns the path of currently opened item.</td>
</tr>
<tr>
<td class="name">
selectedItems</td>
<td class="type"><span class="param-type">object</span></td>
<td class="description">returns the selected item details.</td>
</tr>
<tr>
<td class="name">
uploadItemDetails</td>
<td class="type"><span class="param-type">object</span></td>
<td class="description">returns the upload item details.</td>
</tr>
<tr>
<td class="name">
type</td>
<td class="type"><span class="param-type">string</span></td>
<td class="description">returns the name of the event.</td>
</tr>
</tbody>
</table>
</td>
</tr>
</tbody>
</table>




#### Example



{% highlight html %}
 
        <div id="fileExplorer" ></div> 
        
        <script>
        // beforeUpload event for FileExplorer
        $('#fileExplorer').ejFileExplorer({            
        path: "http://js.syncfusion.com/demos/ejServices/Content/FileBrowser/",         
        ajaxAction: "http://js.syncfusion.com/demos/ejServices/api/FileExplorer/FileOperations",      
        beforeUpload: function (args) {}
        });
        </script>

{% endhighlight %}

### beforeUploadDialogOpen
{:#events:beforeuploaddialogopen}








Fires before opening the upload dialog.

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
<td class="name">files</td>
<td class="type"><span class="param-type">object</span></td>
<td class="description">returns Selected FileList objects</td>
</tr>
<tr>
<td class="name">model</td>
<td class="type"><span class="param-type">object</span></td>
<td class="description">returns the FileExplorer model</td>
</tr>
<tr>
<td class="name">type</td>
<td class="type"><span class="param-type">string</span></td>
<td class="description">returns the name of the event.</td>
</tr>
</tbody>
</table>


#### Example

{% highlight html %}
 
        <div id="fileExplorer" ></div> 
        
        <script>
        // beforeUploadboxOpen event for FileExplorer
        $('#fileExplorer').ejFileExplorer({            
        path: "http://js.syncfusion.com/demos/ejServices/Content/FileBrowser/",         
        ajaxAction: "http://js.syncfusion.com/demos/ejServices/api/FileExplorer/FileOperations",      
        beforeUploadDialogOpen: function (args) {}
        });
        </script>

{% endhighlight %}

### beforeUploadSend
{:#events:beforeuploadsend}








Event is fired before the upload progress is started.

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
<td class="description">if the event is cancelled; otherwise, false</td>
</tr>
<tr>
<td class="name">files</td>
<td class="type"><span class="param-type">object</span></td>
<td class="description">selected FileList Object</td>
</tr>
<tr>
<td class="name">model</td>
<td class="type"><span class="param-type">object</span></td>
<td class="description">returns the upload model</td>
</tr>
<tr>
<td class="name">type</td>
<td class="type"><span class="param-type">string</span></td>
<td class="description">returns the name of the event</td>
</tr>
<tr>
<td class="name">xhr</td>
<td class="type"><span class="param-type">object</span></td>
<td class="description">XHR-AJAX Object for reference</td>
</tr>
</tbody>
</table>


#### Example

{% highlight html %}
 
        <div id="fileExplorer" ></div> 
        
        <script>
        // beforeUploadSend event for FileExplorer
        $('#fileExplorer').ejFileExplorer({            
        path: "http://js.syncfusion.com/demos/ejServices/Content/FileBrowser/",         
        ajaxAction: "http://js.syncfusion.com/demos/ejServices/api/FileExplorer/FileOperations",      
        beforeUploadSend: function (args) {}
        });
        </script>

{% endhighlight %}


### create
{:#events:create}


Fires when FileExplorer control was created




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
cancel</td>
<td class="type"><span class="param-type">boolean</span></td>
<td class="description">Set to true when the event has to be canceled, else false.</td>
</tr>
<tr>
<td class="name">
model</td>
<td class="type"><ts ref="ej.FileExplorer.Model"/><span class="param-type">object</span></td>
<td class="description">returns the FileExplorer model.</td>
</tr>
<tr>
<td class="name">
type</td>
<td class="type"><span class="param-type">string</span></td>
<td class="description">returns the name of the event.</td>
</tr>
</tbody>
</table>



### Example



{% highlight html %}
 
        <div id="fileExplorer" ></div> 
        
        <script>
        // copy event for FileExplorer
        $('#fileExplorer').ejFileExplorer({            
        path: "http://js.syncfusion.com/demos/ejServices/Content/FileBrowser/",           
        ajaxAction: "http://js.syncfusion.com/demos/ejServices/api/FileExplorer/FileOperations",      
        create: function (args) {}
        });
        </script>

{% endhighlight %}





### copy
{:#events:copy}



Fires when file or folder is copied successfully.

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
argument</td>
<td class="type"><span class="param-type">Object</span></td>
<td class="description">Event parameters from FileExplorer
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
cancel</td>
<td class="type"><span class="param-type">boolean</span></td>
<td class="description">Set to true when the event has to be canceled, else false.</td>
</tr>
<tr>
<td class="name">
model</td>
<td class="type"><ts ref="ej.FileExplorer.Model"/>
<span class="param-type">object</span></td>
<td class="description">returns the FileExplorer model.</td>
</tr>
<tr>
<td class="name">
name</td>
<td class="type">
<span class="param-type">string[]</span></td>
<td class="description">returns the name of copied file/folder.</td>
</tr>
<tr>
<td class="name">
selectedItems</td>
<td class="type"><span class="param-type">object</span></td>
<td class="description">returns the selected item details.</td>
</tr>
<tr>
<td class="name">
sourcePath</td>
<td class="type"><span class="param-type">string</span></td>
<td class="description">returns the source path.</td>
</tr>
<tr>
<td class="name">
type</td>
<td class="type"><span class="param-type">string</span></td>
<td class="description">returns the name of the event.</td>
</tr>
</tbody>
</table>
</td>
</tr>
</tbody>
</table>




#### Example



{% highlight html %}
 
        <div id="fileExplorer" ></div> 
        
        <script>
        // copy event for FileExplorer
        $('#fileExplorer').ejFileExplorer({            
        path: "http://js.syncfusion.com/demos/ejServices/Content/FileBrowser/",           
        ajaxAction: "http://js.syncfusion.com/demos/ejServices/api/FileExplorer/FileOperations",      
        copy: function (args) {}
        });
        </script>

{% endhighlight %}



### createFolder
{:#events:createfolder}



Fires when new folder is created successfully in file system.

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
argument</td>
<td class="type"><span class="param-type">Object</span></td>
<td class="description">Event parameters from FileExplorer
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
cancel</td>
<td class="type"><span class="param-type">boolean</span></td>
<td class="description">Set to true when the event has to be canceled, else false.</td>
</tr>
<tr>
<td class="name">
data</td>
<td class="type"><span class="param-type">object</span></td>
<td class="description">returns the AJAX response data</td>
</tr>
<tr>
<td class="name">
model</td>
<td class="type"><ts ref="ej.FileExplorer.Model"/>
<span class="param-type">object</span></td>
<td class="description">returns the FileExplorer model</td>
</tr>
<tr>
<td class="name">
selectedItems</td>
<td class="type"><span class="param-type">object</span></td>
<td class="description">returns the selected item details</td>
</tr>
<tr>
<td class="name">
type</td>
<td class="type"><span class="param-type">string</span></td>
<td class="description">returns the name of the event.</td>
</tr>
</tbody>
</table>
</td>
</tr>
</tbody>
</table>



#### Example



{% highlight html %}
 
        <div id="fileExplorer" ></div> 
        
        <script>
        // createFolder event for FileExplorer
        $('#fileExplorer').ejFileExplorer({            
        path: "http://js.syncfusion.com/demos/ejServices/Content/FileBrowser/",           
        ajaxAction: "http://js.syncfusion.com/demos/ejServices/api/FileExplorer/FileOperations",      
        createFolder: function (args) {}
        });
        </script>

{% endhighlight %}



### cut
{:#events:cut}



Fires when file or folder is cut successfully.

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
argument</td>
<td class="type"><span class="param-type">Object</span></td>
<td class="description">Event parameters from FileExplorer
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
cancel</td>
<td class="type"><span class="param-type">boolean</span></td>
<td class="description">Set to true when the event has to be canceled, else false.</td>
</tr>
<tr>
<td class="name">
model</td>
<td class="type"><ts ref="ej.FileExplorer.Model"/>
<span class="param-type">object</span></td>
<td class="description">returns the FileExplorer model.</td>
</tr>
<tr>
<td class="name">
name</td>
<td class="type"><span class="param-type">string[]</span></td>
<td class="description">returns the name of moved file or folder.</td>
</tr>
<tr>
<td class="name">
selectedItems</td>
<td class="type"><span class="param-type">object</span></td>
<td class="description">returns the selected item details.</td>
</tr>
<tr>
<td class="name">
sourcePath</td>
<td class="type"><span class="param-type">string</span></td>
<td class="description">returns the source path.</td>
</tr>
<tr>
<td class="name">
type</td>
<td class="type"><span class="param-type">string</span></td>
<td class="description">returns the name of the event.</td>
</tr>
</tbody>
</table>
</td>
</tr>
</tbody>
</table>




#### Example



{% highlight html %}
 
        <div id="fileExplorer" ></div> 
        
        <script>
        // cut event for FileExplorer
        $('#fileExplorer').ejFileExplorer({            
        path: "http://js.syncfusion.com/demos/ejServices/Content/FileBrowser/",           
        ajaxAction: "http://js.syncfusion.com/demos/ejServices/api/FileExplorer/FileOperations",      
        cut: function (args) {}
        });
        </script>

{% endhighlight %}



### destroy
{:#events:destroy}








Fires when the FileExplorer is destroyed successfully.

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
cancel</td>
<td class="type"><span class="param-type">boolean</span></td>
<td class="description">Set to true when the event has to be canceled, else false.</td>
</tr>
<tr>
<td class="name">
model</td>
<td class="type"><ts ref="ej.FileExplorer.Model"/><span class="param-type">object</span></td>
<td class="description">returns the FileExplorer model.</td>
</tr>
<tr>
<td class="name">
type</td>
<td class="type"><span class="param-type">string</span></td>
<td class="description">returns the name of the event.</td>
</tr>
</tbody>
</table>




#### Example



{% highlight html %}
 
        <div id="fileExplorer" ></div> 
        
        <script>
        // destroy event for FileExplorer
        $('#fileExplorer').ejFileExplorer({            
        path: "http://js.syncfusion.com/demos/ejServices/Content/FileBrowser/",           
        ajaxAction: "http://js.syncfusion.com/demos/ejServices/api/FileExplorer/FileOperations",      
        
        destroy: function (args) {}
        });
        </script>

{% endhighlight %}








### dragStart
{:#events:dragstart}








Fires when the files or directory has been started to drag over on the FileExplorer

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
cancel</td>
<td class="type"><span class="param-type">boolean</span></td>
<td class="description">set to true when the event has to be canceled, else false.</td>
</tr>
<tr>
<td class="name">
model</td>
<td class="type"><ts ref="ej.FileExplorer.Model"/><span class="param-type">object</span></td>
<td class="description">returns the FileExplorer model.</td>
</tr>
<tr>
<td class="name">
type</td>
<td class="type"><span class="param-type">string</span></td>
<td class="description">returns the name of the event.</td>
</tr>
<tr>
<td class="name">
target</td>
<td class="type"><span class="param-type">object</span></td>
<td class="description">returns the dragging element.</td>
</tr>
<tr>
<td class="name">
targetPath</td>
<td class="type"><span class="param-type">string</span></td>
<td class="description">returns the path of dragging element.</td>
</tr>
<tr>
<td class="name">
selectedItems</td>
<td class="type"><span class="param-type">object</span></td>
<td class="description">returns the dragging file details.</td>
</tr>
</tbody>
</table>




#### Example



{% highlight html %}
 
        <div id="fileExplorer" ></div> 
        
        <script>
        // dragStart event for FileExplorer
        $('#fileExplorer').ejFileExplorer({            
        path: "http://js.syncfusion.com/demos/ejServices/Content/FileBrowser/",           
        ajaxAction: "http://js.syncfusion.com/demos/ejServices/api/FileExplorer/FileOperations",      
        dragStart: function (args) {}
        });
        </script>

{% endhighlight %}





### drag
{:#events:drag}








Fires when the files or directory is dragging over on the FileExplorer.

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
cancel</td>
<td class="type"><span class="param-type">boolean</span></td>
<td class="description">set to true when the event has to be canceled, else false.</td>
</tr>
<tr>
<td class="name">
model</td>
<td class="type"><ts ref="ej.FileExplorer.Model"/><span class="param-type">object</span></td>
<td class="description">returns the FileExplorer model.</td>
</tr>
<tr>
<td class="name">
type</td>
<td class="type"><span class="param-type">string</span></td>
<td class="description">returns the name of the event.</td>
</tr>
<tr>
<td class="name">
target</td>
<td class="type"><span class="param-type">object</span></td>
<td class="description">returns the target element.</td>
</tr>
<tr>
<td class="name">
targetElementName</td>
<td class="type"><span class="param-type">string</span></td>
<td class="description">returns the name of target element.</td>
</tr>
<tr>
<td class="name">
targetPath</td>
<td class="type"><span class="param-type">string</span></td>
<td class="description">returns the path of target element.</td>
</tr>
</tbody>
</table>




#### Example



{% highlight html %}
 
        <div id="fileExplorer" ></div> 
        
        <script>
        // drag event for FileExplorer
        $('#fileExplorer').ejFileExplorer({            
        path: "http://js.syncfusion.com/demos/ejServices/Content/FileBrowser/",           
        ajaxAction: "http://js.syncfusion.com/demos/ejServices/api/FileExplorer/FileOperations",      
        drag: function (args) {}
        });
        </script>

{% endhighlight %}











### dragStop
{:#events:dragstop}








Fires when the files or directory has been stopped to drag over on FileExplorer

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
cancel</td>
<td class="type"><span class="param-type">boolean</span></td>
<td class="description">set to true when the event has to be canceled, else false.</td>
</tr>
<tr>
<td class="name">
model</td>
<td class="type"><ts ref="ej.FileExplorer.Model"/><span class="param-type">object</span></td>
<td class="description">returns the FileExplorer model.</td>
</tr>
<tr>
<td class="name">
type</td>
<td class="type"><span class="param-type">string</span></td>
<td class="description">returns the name of the event.</td>
</tr>
<tr>
<td class="name">
target</td>
<td class="type"><span class="param-type">object</span></td>
<td class="description">returns the target element.</td>
</tr>
<tr>
<td class="name">
targetPath</td>
<td class="type"><span class="param-type">string</span></td>
<td class="description">returns the path of target element.</td>
</tr>
<tr>
<td class="name">
targetElementName</td>
<td class="type"><span class="param-type">string</span></td>
<td class="description">returns the name of target element</td>
</tr>
<tr>
<td class="name">
dropAction</td>
<td class="type"><span class="param-type">string</span></td>
<td class="description">returns the action, which is performed after dropping the files (upload/ move).</td>
</tr>
<tr>
<td class="name">
fileInfo</td>
<td class="type"><span class="param-type">object</span></td>
<td class="description">returns the dragging file details</td>
</tr>
</tbody>
</table>




#### Example



{% highlight html %}
 
        <div id="fileExplorer" ></div> 
        
        <script>
        // dragStop event for FileExplorer
        $('#fileExplorer').ejFileExplorer({            
        path: "http://js.syncfusion.com/demos/ejServices/Content/FileBrowser/",           
        ajaxAction: "http://js.syncfusion.com/demos/ejServices/api/FileExplorer/FileOperations",      
        dragStop: function (args) {}
        });
        </script>

{% endhighlight %}







### drop
{:#events:drop}








Fires when the files or directory is dropped to the target folder of FileExplorer

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
cancel</td>
<td class="type"><span class="param-type">boolean</span></td>
<td class="description">set to true when the event has to be canceled, else false.</td>
</tr>
<tr>
<td class="name">
model</td>
<td class="type"><ts ref="ej.FileExplorer.Model"/><span class="param-type">object</span></td>
<td class="description">returns the FileExplorer model.</td>
</tr>
<tr>
<td class="name">
type</td>
<td class="type"><span class="param-type">string</span></td>
<td class="description">returns the name of the event.</td>
</tr>
<tr>
<td class="name">
target</td>
<td class="type"><span class="param-type">object</span></td>
<td class="description">returns the target element.</td>
</tr>
<tr>
<td class="name">
targetFolder</td>
<td class="type"><span class="param-type">string</span></td>
<td class="description">returns the name of target folder.</td>
</tr>
<tr>
<td class="name">
targetPath</td>
<td class="type"><span class="param-type">string</span></td>
<td class="description">returns the path of target folder.</td>
</tr>
<tr>
<td class="name">
fileInfo</td>
<td class="type"><span class="param-type">object</span></td>
<td class="description">returns the dragging element details.</td>
</tr>
<tr>
<td class="name">
dropAction</td>
<td class="type"><span class="param-type">string</span></td>
<td class="description">returns the action, which is performed after dropping the files (upload/ move).</td>
</tr>
</tbody>
</table>




#### Example



{% highlight html %}
 
        <div id="fileExplorer" ></div> 
        
        <script>
        // drop event for FileExplorer
        $('#fileExplorer').ejFileExplorer({            
        path: "http://js.syncfusion.com/demos/ejServices/Content/FileBrowser/",           
        ajaxAction: "http://js.syncfusion.com/demos/ejServices/api/FileExplorer/FileOperations",      
        drop: function (args) {}
        });
        </script>

{% endhighlight %}






### getImage
{:#events:getimage}



Fires after loading the requested image from server. Using this event, you can get the details of loaded image.



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
cancel</td>
<td class="type"><span class="param-type">boolean</span></td>
<td class="description">set to true when the event has to be canceled, else false.</td>
</tr>
<tr>
<td class="name">
path</td>
<td class="type"><span class="param-type">string</span></td>
<td class="description">loaded image path.</td>
</tr>
<tr>
<td class="name">
element</td>
<td class="type"><span class="param-type">object</span></td>
<td class="description">loaded image element</td>
</tr>
<tr>
<td class="name">
model</td>
<td class="type"><ts ref="ej.FileExplorer.Model"/>
<span class="param-type">object</span></td>
<td class="description">returns the FileExplorer model.</td>
</tr>
<tr>
<td class="name">
originalArgs</td>
<td class="type"><span class="param-type">object</span></td>
<td class="description">original arguments of image load or error event</td>
</tr>
<tr>
<td class="name">
action</td>
<td class="type"><span class="param-type">string</span></td>
<td class="description">returns the action type, which specifies thumbnail preview or opening image.</td>
</tr>
<tr>
<td class="name">
type</td>
<td class="type"><span class="param-type">string</span></td>
<td class="description">returns the name of the event.</td>
</tr>
</tbody>
</table>
</td>
</tr>
</tbody>
</table>



#### Example



{% highlight html %}
 
        <div id="fileExplorer" ></div> 
        
        <script>
        // getImage event for FileExplorer
        $('#fileExplorer').ejFileExplorer({            
        path: "http://js.syncfusion.com/demos/ejServices/Content/FileBrowser/",         
        ajaxAction: "http://js.syncfusion.com/demos/ejServices/api/FileExplorer/FileOperations",      
        getImage: function (args) {}
        });
        </script>

{% endhighlight %}







### keydown
{:#events:keydown}



Fires when keydown in FileExplorer control.

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
cancel</td>
<td class="type"><span class="param-type">boolean</span></td>
<td class="description">Set to true when the event has to be canceled, else false.</td>
</tr>
<tr>
<td class="name">
keyCode</td>
<td class="type"><span class="param-type">number</span></td>
<td class="description">returns the downed key keyCode value</td>
</tr>
<tr>
<td class="name">
altKey</td>
<td class="type"><span class="param-type">boolean</span></td>
<td class="description">returns altKey value.</td>
</tr>
<tr>
<td class="name">
shiftKey</td>
<td class="type"><span class="param-type">boolean</span></td>
<td class="description">returns shiftKey value.</td>
</tr>
<tr>
<td class="name">
ctrlKey</td>
<td class="type"><span class="param-type">boolean</span></td>
<td class="description">returns ctrlKey value.</td>
</tr>
<tr>
<td class="name">
originalArgs</td>
<td class="type"><span class="param-type">object</span></td>
<td class="description">returns the event object.</td>
</tr>
<tr>
<td class="name">
model</td>
<td class="type"><ts ref="ej.FileExplorer.Model"/>
<span class="param-type">object</span></td>
<td class="description">returns the FileExplorer model.</td>
</tr>
<tr>
<td class="name">
type</td>
<td class="type"><span class="param-type">string</span></td>
<td class="description">returns the name of the event.</td>
</tr>
</tbody>
</table>
</td>
</tr>
</tbody>
</table>




#### Example



{% highlight html %}
 
        <div id="fileExplorer" ></div> 
        
        <script>
        // keydown event for FileExplorer
        $('#fileExplorer').ejFileExplorer({            
        path: "http://js.syncfusion.com/demos/ejServices/Content/FileBrowser/",           
        ajaxAction: "http://js.syncfusion.com/demos/ejServices/api/FileExplorer/FileOperations",      
        keydown: function (args) {}
        });
        </script>

{% endhighlight %}





### layoutChange
{:#events:layoutchange}



Fires when the file view type is changed.

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
argument</td>
<td class="type"><span class="param-type">Object</span></td>
<td class="description">Event parameters from FileExplorer
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
cancel</td>
<td class="type"><span class="param-type">boolean</span></td>
<td class="description">Set to true when the event has to be canceled, else false.</td>
</tr>
<tr>
<td class="name">
isInteraction</td>
<td class="type"><ts ref="ej.FileExplorer.Model"/>
<span class="param-type">boolean</span></td>
<td class="description">return true when we change the layout via interaction, else false.</td>
</tr>
<tr>
<td class="name">
layoutType</td>
<td class="type"><span class="param-type">string</span></td>
<td class="description">returns the current view type.</td>
</tr>
<tr>
<td class="name">
model</td>
<td class="type"><span class="param-type">object</span></td>
<td class="description">returns the FileExplorer model.</td>
</tr>
<tr>
<td class="name">
type</td>
<td class="type"><span class="param-type">string</span></td>
<td class="description">returns the name of the event.</td>
</tr>
</tbody>
</table>
</td>
</tr>
</tbody>
</table>




#### Example



{% highlight html %}
 
        <div id="fileExplorer" ></div> 
        
        <script>
        // layoutChange event for FileExplorer
        $('#fileExplorer').ejFileExplorer({            
        path: "http://js.syncfusion.com/demos/ejServices/Content/FileBrowser/",           
        ajaxAction: "http://js.syncfusion.com/demos/ejServices/api/FileExplorer/FileOperations",      
        layoutChange: function (args) {}
        });
        </script>

{% endhighlight %}




### menuBeforeOpen
{:#events:menubeforeopen}


Fires when before the ContextMenu opening.


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
<td class="description">Event parameters from FileExplorer
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
<td class="description">set to true when the event has to be canceled, else false.</td>
</tr>
<tr>
<td class="name">contextMenu</td>
<td class="type"><span class="param-type">string</span></td>
<td class="description">returns the name of ContextMenu items group.</td>
</tr>
<tr>
<td class="name">dataSource</td>
<td class="type"><span class="param-type">array</span></td>
<td class="description">returns the dataSource of ContextMenu.</td>
</tr>
<tr>
<td class="name">element</td>
<td class="type"><span class="param-type">object</span></td>
<td class="description">returns the element of ContextMenu.</td>
</tr>
<tr>
<td class="name">events</td>
<td class="type"><span class="param-type">object</span></td>
<td class="description">returns the event of ContextMenu.</td>
</tr>
<tr>
<td class="name">model</td>
<td class="type"><ts ref="ej.FileExplorer.Model"/>
<span class="param-type">object</span></td>
<td class="description">returns the FileExplorer model.</td>
</tr>
<tr>
<td class="name">target</td>
<td class="type"><span class="param-type">object</span></td>
<td class="description">returns the target element.</td>
</tr>
<tr>
<td class="name">type</td>
<td class="type"><span class="param-type">string</span></td>
<td class="description">returns the name of the event.</td>
</tr>
</tbody>
</table>
</td>
</tr>
</tbody>
</table>


#### Example


{% highlight html %}
        
        <div id="fileExplorer"></div> 
        
        <script>
        // menuBeforeOpen event of ContextMenu for FileExplorer
        $('#fileExplorer').ejFileExplorer({            
        path: "http://js.syncfusion.com/demos/ejServices/Content/FileBrowser/",         
        ajaxAction: "http://js.syncfusion.com/demos/ejServices/api/FileExplorer/FileOperations",      
        menuBeforeOpen: function (args) {}
        });
        </script>

{% endhighlight %}



### menuClick
{:#events:menuclick}


Fires when click the ContextMenu item.


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
<td class="description">Event parameters from FileExplorer
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
<td class="name">ID</td>
<td class="type"><span class="param-type">string</span></td>
<td class="description">returns the ID of clicked ContextMenu item.</td>
</tr>
<tr>
<td class="name">cancel</td>
<td class="type"><span class="param-type">boolean</span></td>
<td class="description">set to true when the event has to be canceled, else false.</td>
</tr>
<tr>
<td class="name">contextMenu</td>
<td class="type"><span class="param-type">string</span></td>
<td class="description">returns the name of ContextMenu items group.</td>
</tr>
<tr>
<td class="name">element</td>
<td class="type"><span class="param-type">object</span></td>
<td class="description">returns the element of clicked ContextMenu item.</td>
</tr>
<tr>
<td class="name">event</td>
<td class="type"><span class="param-type">object</span></td>
<td class="description">returns the event of ContextMenu.</td>
</tr>
<tr>
<td class="name">model</td>
<td class="type"><ts ref="ej.FileExplorer.Model"/>
<span class="param-type">object</span></td>
<td class="description">returns the FileExplorer model.</td>
</tr>
<tr>
<td class="name">parentId</td>
<td class="type"><span class="param-type">string</span></td>
<td class="description">returns the parent element ID of clicked ContextMenu item.</td>
</tr>
<tr>
<td class="name">parentText</td>
<td class="type"><span class="param-type">string</span></td>
<td class="description">returns the parent element text of clicked ContextMenu item.</td>
</tr>
<tr>
<td class="name">text</td>
<td class="type"><span class="param-type">string</span></td>
<td class="description">returns the text of clicked ContextMenu item.</td>
</tr>
<tr>
<td class="name">type</td>
<td class="type"><span class="param-type">string</span></td>
<td class="description">returns the name of the event.</td>
</tr>
</tbody>
</table>
</td>
</tr>
</tbody>
</table>


#### Example


{% highlight html %}
        
        <div id="fileExplorer"></div> 
        
        <script>
        // menuClick event of ContextMenu for FileExplorer
        $('#fileExplorer').ejFileExplorer({            
        path: "http://js.syncfusion.com/demos/ejServices/Content/FileBrowser/",         
        ajaxAction: "http://js.syncfusion.com/demos/ejServices/api/FileExplorer/FileOperations",      
        menuClick: function (args) {}
        });
        </script>

{% endhighlight %}



### menuOpen
{:#events:menuopen}


Fires when ContextMenu is successfully opened.


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
<td class="description">Event parameters from FileExplorer
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
<td class="description">set to true when the event has to be canceled, else false.</td>
</tr>
<tr>
<td class="name">contextMenu</td>
<td class="type"><span class="param-type">string</span></td>
<td class="description">returns the name of ContextMenu items group.</td>
</tr>
<tr>
<td class="name">element</td>
<td class="type"><span class="param-type">object</span></td>
<td class="description">returns the element of ContextMenu.</td>
</tr>
<tr>
<td class="name">model</td>
<td class="type"><ts ref="ej.FileExplorer.Model"/>
<span class="param-type">object</span></td>
<td class="description">returns the FileExplorer model.</td>
</tr>
<tr>
<td class="name">target</td>
<td class="type"><span class="param-type">object</span></td>
<td class="description">returns the target element.</td>
</tr>
<tr>
<td class="name">type</td>
<td class="type"><span class="param-type">string</span></td>
<td class="description">returns the name of the event.</td>
</tr>
</tbody>
</table>
</td>
</tr>
</tbody>
</table>


#### Example


{% highlight html %}
        
        <div id="fileExplorer"></div> 
        
        <script>
        // menuOpen event of ContextMenu for FileExplorer
        $('#fileExplorer').ejFileExplorer({            
        path: "http://js.syncfusion.com/demos/ejServices/Content/FileBrowser/",         
        ajaxAction: "http://js.syncfusion.com/demos/ejServices/api/FileExplorer/FileOperations",      
        menuOpen: function (args) {}
        });
        </script>

{% endhighlight %}




### open
{:#events:open}



Fires when files are successfully opened.
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
argument</td>
<td class="type"><span class="param-type">Object</span></td>
<td class="description">Event parameters from FileExplorer
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
cancel</td>
<td class="type"><span class="param-type">boolean</span></td>
<td class="description">Set to true when the event has to be canceled, else false.</td>
</tr>
<tr>
<td class="name">
itemType</td>
<td class="type"><span class="param-type">string</span></td>
<td class="description">returns the opened item type.</td>
</tr>
<tr>
<td class="name">
model</td>
<td class="type"><ts ref="ej.FileExplorer.Model"/>
<span class="param-type">object</span></td>
<td class="description">returns the FileExplorer model.</td>
</tr>
<tr>
<td class="name">
path</td>
<td class="type"><span class="param-type">string</span></td>
<td class="description">returns the path of currently opened item.</td>
</tr>
<tr>
<td class="name">
selectedItems</td>
<td class="type"><span class="param-type">object</span></td>
<td class="description">returns the selected item details.</td>
</tr>
<tr>
<td class="name">
type</td>
<td class="type"><span class="param-type">string</span></td>
<td class="description">returns the name of the event.</td>
</tr>
</tbody>
</table>
</td>
</tr>
</tbody>
</table>




#### Example



{% highlight html %}
        
        <div id="fileExplorer" ></div> 
        
        <script>
        // open event for FileExplorer
        $('#fileExplorer').ejFileExplorer({            
        path: "http://js.syncfusion.com/demos/ejServices/Content/FileBrowser/",         
        ajaxAction: "http://js.syncfusion.com/demos/ejServices/api/FileExplorer/FileOperations",      
        open: function (args) {}
        });
        </script>

{% endhighlight %}



### paste
{:#events:paste}



Fires when a file or folder is pasted successfully.

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
argument</td>
<td class="type"><span class="param-type">Object</span></td>
<td class="description">Event parameters from FileExplorer
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
cancel</td>
<td class="type"><span class="param-type">boolean</span></td>
<td class="description">Set to true when the event has to be canceled, else false.</td>
</tr>
<tr>
<td class="name">
model</td>
<td class="type"><ts ref="ej.FileExplorer.Model"/>
<span class="param-type">object</span></td>
<td class="description">returns the FileExplorer model.</td>
</tr>
<tr>
<td class="name">
name</td>
<td class="type"><span class="param-type">string[]</span></td>
<td class="description">returns the name of moved/copied file or folder.</td>
</tr>
<tr>
<td class="name">
selectedItems</td>
<td class="type"><span class="param-type">object</span></td>
<td class="description">returns the selected item details.</td>
</tr>
<tr>
<td class="name">
targetFolder</td>
<td class="type"><span class="param-type">object</span></td>
<td class="description">returns the target folder item details.</td>
</tr>
<tr>
<td class="name">
targetPath</td>
<td class="type"><span class="param-type">string</span></td>
<td class="description">returns the target path.</td>
</tr>
<tr>
<td class="name">
type</td>
<td class="type"><span class="param-type">string</span></td>
<td class="description">returns the name of the event.</td>
</tr>
</tbody>
</table>
</td>
</tr>
</tbody>
</table>


#### Example



{% highlight html %}
 
        <div id="fileExplorer" ></div> 
        
        <script>
        // paste event for FileExplorer
        $('#fileExplorer').ejFileExplorer({            
        path: "http://js.syncfusion.com/demos/ejServices/Content/FileBrowser/",           
        ajaxAction: "http://js.syncfusion.com/demos/ejServices/api/FileExplorer/FileOperations",      
        paste: function (args) {}
        });
        </script>

{% endhighlight %}



### remove
{:#events:remove}



Fires when file or folder is deleted successfully.

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
argument</td>
<td class="type"><span class="param-type">Object</span></td>
<td class="description">Event parameters from FileExplorer
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
cancel</td>
<td class="type"><span class="param-type">boolean</span></td>
<td class="description">Set to true when the event has to be canceled, else false.</td>
</tr>
<tr>
<td class="name">
data</td>
<td class="type"><span class="param-type">object</span></td>
<td class="description">returns the AJAX response data.</td>
</tr>
<tr>
<td class="name">
model</td>
<td class="type"><ts ref="ej.FileExplorer.Model"/>
<span class="param-type">object</span></td>
<td class="description">returns the FileExplorer model.</td>
</tr>
<tr>
<td class="name">
name</td>
<td class="type"><span class="param-type">string</span></td>
<td class="description">returns the names of deleted items.</td>
</tr>
<tr>
<td class="name">
path</td>
<td class="type"><span class="param-type">string</span></td>
<td class="description">returns the path of deleted item.</td>
</tr>
<tr>
<td class="name">
selectedItems</td>
<td class="type"><span class="param-type">object</span></td>
<td class="description">returns the removed item details.</td>
</tr>
<tr>
<td class="name">
type</td>
<td class="type"><span class="param-type">string</span></td>
<td class="description">returns the name of the event.</td>
</tr>
</tbody>
</table>
</td>
</tr>
</tbody>
</table>




#### Example



{% highlight html %}
 
        <div id="fileExplorer" ></div> 
        
        <script>
        // remove event for FileExplorer
        $('#fileExplorer').ejFileExplorer({            
        path: "http://js.syncfusion.com/demos/ejServices/Content/FileBrowser/",           
        ajaxAction: "http://js.syncfusion.com/demos/ejServices/api/FileExplorer/FileOperations",      
        remove: function (args) {}
        });
        </script>

{% endhighlight %}



### resize
{:#events:resize}


Fires when resizing is performed for FileExplorer.

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
argument</td>
<td class="type"><span class="param-type">Object</span></td>
<td class="description">Event parameters from FileExplorer
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
cancel</td>
<td class="type"><span class="param-type">boolean</span></td>
<td class="description">if the event should be canceled; otherwise, false.</td>
</tr>
<tr>
<td class="name">
event</td>
<td class="type"><span class="param-type">object</span></td>
<td class="description">returns the mouse move event args.</td>
</tr>
<tr>
<td class="name">
model</td>
<td class="type"><ts ref="ej.FileExplorer.Model"/>
<span class="param-type">object</span></td>
<td class="description">returns the FileExplorer model.</td>
</tr>
<tr>
<td class="name">
type</td>
<td class="type"><span class="param-type">string</span></td>
<td class="description">returns the name of the event.</td>
</tr>
</tbody>
</table>
</td>
</tr>
</tbody>
</table>





#### Example



{% highlight html %}
 
        <div id="fileExplorer" ></div> 
        
        <script>
        // resize event for FileExplorer
        $('#fileExplorer').ejFileExplorer({            
        path: "http://js.syncfusion.com/demos/ejServices/Content/FileBrowser/",         
        ajaxAction: "http://js.syncfusion.com/demos/ejServices/api/FileExplorer/FileOperations",      
        resize: function (args) {}
        });
        </script>

{% endhighlight %}



### resizeStart
{:#events:resizestart}


Fires when resizing is started for FileExplorer.

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
argument</td>
<td class="type"><span class="param-type">Object</span></td>
<td class="description">Event parameters from FileExplorer
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
cancel</td>
<td class="type"><span class="param-type">boolean</span></td>
<td class="description">Set to true when the event has to be canceled, else false.</td>
</tr>
<tr>
<td class="name">
event</td>
<td class="type"><span class="param-type">object</span></td>
<td class="description">returns the mouse down event args.</td>
</tr>
<tr>
<td class="name">
model</td>
<td class="type"><ts ref="ej.FileExplorer.Model"/>
<span class="param-type">object</span></td>
<td class="description">returns the FileExplorer model.</td>
</tr>
<tr>
<td class="name">
type</td>
<td class="type"><span class="param-type">string</span></td>
<td class="description">returns the name of the event.</td>
</tr>
</tbody>
</table>
</td>
</tr>
</tbody>
</table>



#### Example



{% highlight html %}
 
        <div id="fileExplorer" ></div> 
        
        <script>
        // resizeStart event for FileExplorer
        $('#fileExplorer').ejFileExplorer({            
        path: "http://js.syncfusion.com/demos/ejServices/Content/FileBrowser/",         
        ajaxAction: "http://js.syncfusion.com/demos/ejServices/api/FileExplorer/FileOperations",      
        resizeStart: function (args) {}
        });
        </script>

{% endhighlight %}



### resizeStop
{:#events:resizestop}


Fires this event when the resizing is stopped for FileExplorer.

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
argument</td>
<td class="type"><span class="param-type">Object</span></td>
<td class="description">Event parameters from FileExplorer
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
cancel</td>
<td class="type"><span class="param-type">boolean</span></td>
<td class="description">Set to true when the event has to be canceled, else false.</td>
</tr>
<tr>
<td class="name">
event</td>
<td class="type"><span class="param-type">object</span></td>
<td class="description">returns the mouse leave event args.</td>
</tr>
<tr>
<td class="name">
model</td>
<td class="type"><ts ref="ej.FileExplorer.Model"/>
<span class="param-type">object</span></td>
<td class="description">returns the FileExplorer model.</td>
</tr>
<tr>
<td class="name">
type</td>
<td class="type"><span class="param-type">string</span></td>
<td class="description">returns the name of the event.</td>
</tr>
</tbody>
</table>
</td>
</tr>
</tbody>
</table>





#### Example



{% highlight html %}
 
        <div id="fileExplorer" ></div> 
        
        <script>
        // resizeStop event for FileExplorer
        $('#fileExplorer').ejFileExplorer({            
        path: "http://js.syncfusion.com/demos/ejServices/Content/FileBrowser/",         
        ajaxAction: "http://js.syncfusion.com/demos/ejServices/api/FileExplorer/FileOperations",      
        resizeStop: function (args) {}
        });
        </script>

{% endhighlight %}



### select
{:#events:select}



Fires when the items from grid view or tile view of FileExplorer control is selected.

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
argument</td>
<td class="type"><span class="param-type">Object</span></td>
<td class="description">Event parameters from FileExplorer
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
cancel</td>
<td class="type"><span class="param-type">boolean</span></td>
<td class="description">Set to true when the event has to be canceled, else false.</td>
</tr>
<tr>
<td class="name">
model</td>
<td class="type"><ts ref="ej.FileExplorer.Model"/>
<span class="param-type">object</span></td>
<td class="description">returns the FileExplorer model.</td>
</tr>
<tr>
<td class="name">
name</td>
<td class="type"><span class="param-type">string[]</span></td>
<td class="description">returns the name of selected items.</td>
</tr>
<tr>
<td class="name">
path</td>
<td class="type"><span class="param-type">string</span></td>
<td class="description">returns the path of selected items.</td>
</tr>
<tr>
<tr>
<td class="name">
names</td>
<td class="type"><span class="param-type">string[]</span></td>
<td class="description">returns the name of selected items.</td>
</tr>
<td class="name">
selectedItems</td>
<td class="type"><span class="param-type">object</span></td>
<td class="description">returns the selected item details</td>
</tr>
<tr>
<td class="name">
type</td>
<td class="type"><span class="param-type">string</span></td>
<td class="description">returns the name of the event.</td>
</tr>
</tbody>
</table>
</td>
</tr>
</tbody>
</table>




#### Example



{% highlight html %}
 
        <div id="fileExplorer" ></div> 
        
        <script>
        // select event for FileExplorer
        $('#fileExplorer').ejFileExplorer({            
        path: "http://js.syncfusion.com/demos/ejServices/Content/FileBrowser/",           
        ajaxAction: "http://js.syncfusion.com/demos/ejServices/api/FileExplorer/FileOperations",        
        select: function (args) {}
        });
        </script>

{% endhighlight %}


### templateRefresh
{:#events:templaterefresh}



Triggered when refresh the template column elements in the grid view of FileExplorer control.

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
argument</td>
<td class="type"><span class="param-type">Object</span></td>
<td class="description">Event parameters from FileExplorer
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
cancel</td>
<td class="type"><span class="param-type">boolean</span></td>
<td class="description">Set to true when the event has to be canceled, else false.</td>
</tr>
<tr>
<td class="name">
cell</td>
<td class="type"><ts ref="ej.FileExplorer.Model"/>
<span class="param-type">object</span></td>
<td class="description">Returns the cell object.</td>
</tr>
<tr>
<td class="name">
column</td>
<td class="type"><span class="param-type">object</span></td>
<td class="description">Returns the column object.</td>
</tr>
<tr>
<td class="name">
data</td>
<td class="type"><span class="param-type">object</span></td>
<td class="description">Returns the current row data.</td>
</tr>
<tr>
<td class="name">
model</td>
<td class="type"><span class="param-type">object</span></td>
<td class="description">Returns the grid model of FileExplorer.</td>
</tr>
<tr>
<td class="name">
rowIndex</td>
<td class="type"><span class="param-type">number</span></td>
<td class="description">Returns the current row index.</td>
</tr>
<tr>
<td class="name">
type</td>
<td class="type"><span class="param-type">string</span></td>
<td class="description">returns the name of the event.</td>
</tr>
</tbody>
</table>
</td>
</tr>
</tbody>
</table>




#### Example



{% highlight html %}
 
        <div id="fileExplorer" ></div> 
        
        <script>
        // select event for FileExplorer
        $('#fileExplorer').ejFileExplorer({            
        path: "http://js.syncfusion.com/demos/ejServices/Content/FileBrowser/",           
        ajaxAction: "http://js.syncfusion.com/demos/ejServices/api/FileExplorer/FileOperations",        
        templateRefresh: function (args) {}
        });
        </script>

{% endhighlight %}

### unselect
{:#events:unselect}



Fires when the items from grid view or tile view or large icons view of FileExplorer control is unselected.

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
<td class="description">Event parameters from FileExplorer
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
<td class="name">model</td>
<td class="type"><ts ref="ej.FileExplorer.Model"/>
<span class="param-type">object</span></td>
<td class="description">Returns the FileExplorer model.</td>
</tr>
<tr>
<td class="name">name</td>
<td class="type"><span class="param-type">string</span></td>
<td class="description">Returns the name of unselected item.</td>
</tr>
<tr>
<td class="name">names</td>
<td class="type"><span class="param-type">string[]</span></td>
<td class="description">Returns the name of unselected items.</td>
</tr>
<tr>
<td class="name">nodeType</td>
<td class="type"><span class="param-type">string</span></td>
<td class="description">Returns the type of unselected item.</td>
</tr>
<tr>
<td class="name">path</td>
<td class="type"><span class="param-type">string</span></td>
<td class="description">Returns the path of unselected item.</td>
</tr>
<tr>
<td class="name">type</td>
<td class="type"><span class="param-type">string</span></td>
<td class="description">Returns the name of the event.</td>
</tr>
<tr>
<td class="name">unselectedItem</td>
<td class="type"><span class="param-type">object</span></td>
<td class="description">Returns the unselected item details.</td>
</tr>
<tr>
<td class="name">unselectedItems</td>
<td class="type"><span class="param-type">array</span></td>
<td class="description">Returns the unselected items details.</td>
</tr>
</tbody>
</table>
</td>
</tr>
</tbody>
</table>




#### Example



{% highlight html %}
 
<div id="fileExplorer"></div>

<script>
    // unselect event for FileExplorer
    $('#fileExplorer').ejFileExplorer({
        path: "http://js.syncfusion.com/demos/ejServices/Content/FileBrowser/",
        ajaxAction: "http://js.syncfusion.com/demos/ejServices/api/FileExplorer/FileOperations",
        unselect: function (args) { }
    });
</script>

{% endhighlight %}


### uploadComplete
{:#events:uploadcomplete}



Event is fired when the file upload progress gets completed.

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
<td class="name">e</td>
<td class="type"><span class="param-type">object</span></td>
<td class="description">AJAX event argument for reference</td>
</tr>
<tr>
<td class="name">error</td>
<td class="type"><span class="param-type">string</span></td>
<td class="description">details about the error information</td>
</tr>
<tr>
<td class="name">files</td>
<td class="type"><span class="param-type">object</span></td>
<td class="description">uploaded file list</td>
</tr>
<tr>
<td class="name">model</td>
<td class="type"><span class="param-type">object</span></td>
<td class="description">returns the Upload model</td>
</tr>
<tr>
<td class="name">responseText</td>
<td class="type"><span class="param-type">string</span></td>
<td class="description">response from the server</td>
</tr>
<tr>
<td class="name">success</td>
<td class="type"><span class="param-type">object</span></td>
<td class="description">successfully uploaded files list</td>
</tr>
<tr>
<td class="name">type</td>
<td class="type"><span class="param-type">string</span></td>
<td class="description">returns the name of the event</td>
</tr>
<tr>
<td class="name">xhr</td>
<td class="type"><span class="param-type">object</span></td>
<td class="description">XHR-AJAX Object for reference</td>
</tr>
</tbody>
</table>




#### Example



{% highlight html %}
 
        <div id="fileExplorer" ></div> 
        
        <script>
        // uploadComplete event for FileExplorer
        $('#fileExplorer').ejFileExplorer({            
        path: "http://js.syncfusion.com/demos/ejServices/Content/FileBrowser/",         
        ajaxAction: "http://js.syncfusion.com/demos/ejServices/api/FileExplorer/FileOperations",      
        uploadComplete: function (args) {}
        });
        </script>

{% endhighlight %}


### uploadError
{:#events:uploaderror}



Event is fired when the file upload fails due to some error.

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
<td class="name">action</td>
<td class="type"><span class="param-type">string</span></td>
<td class="description">error event action details</td>
</tr>
<tr>
<td class="name">error</td>
<td class="type"><span class="param-type">string</span></td>
<td class="description">details about the error information</td>
</tr>
<tr>
<td class="name">files</td>
<td class="type"><span class="param-type">object</span></td>
<td class="description">returns the details of the uploaded files</td>
</tr>
<tr>
<td class="name">type</td>
<td class="type"><span class="param-type">string</span></td>
<td class="description">returns the name of the event</td>
</tr>
</tbody>
</table>




#### Example



{% highlight html %}
 
        <div id="fileExplorer" ></div> 
        
        <script>
        // uploadError event for FileExplorer
        $('#fileExplorer').ejFileExplorer({            
        path: "http://js.syncfusion.com/demos/ejServices/Content/FileBrowser/",         
        ajaxAction: "http://js.syncfusion.com/demos/ejServices/api/FileExplorer/FileOperations",      
        uploadError: function (args) {}
        });
        </script>

{% endhighlight %}


### uploadSuccess
{:#events:uploadsuccess}



Event is fired when the file upload progress gets succeeded.

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
<td class="name">e</td>
<td class="type"><span class="param-type">object</span></td>
<td class="description">AJAX event argument for reference</td>
</tr>
<tr>
<td class="name">files</td>
<td class="type"><span class="param-type">object</span></td>
<td class="description">uploaded file list</td>
</tr>
<tr>
<td class="name">model</td>
<td class="type"><span class="param-type">object</span></td>
<td class="description">returns the Upload model</td>
</tr>
<tr>
<td class="name">responseText</td>
<td class="type"><span class="param-type">string</span></td>
<td class="description">response from the server</td>
</tr>
<tr>
<td class="name">type</td>
<td class="type"><span class="param-type">string</span></td>
<td class="description">returns the name of the event</td>
</tr>
<tr>
<td class="name">xhr</td>
<td class="type"><span class="param-type">object</span></td>
<td class="description">XHR-AJAX Object for reference</td>
</tr>
</tbody>
</table>




#### Example



{% highlight html %}
 
        <div id="fileExplorer" ></div> 
        
        <script>
        // uploadSuccess event for FileExplorer
        $('#fileExplorer').ejFileExplorer({            
        path: "http://js.syncfusion.com/demos/ejServices/Content/FileBrowser/",         
        ajaxAction: "http://js.syncfusion.com/demos/ejServices/api/FileExplorer/FileOperations",      
        uploadSuccess: function (args) {}
        });
        </script>

{% endhighlight %}

