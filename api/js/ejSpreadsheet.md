---
layout: post
title: Properties, Methods and Events of Syncfusion ejSpreadsheet Widget
description: What are the options, methods and events available in the Essential JavaScript ejSpreadsheet Widget.
documentation: UG
platform: js-api
keywords: ejSpreadsheet, API, Essential JS Spreadsheet
---

# Essential JS Spreadsheet

The Spreadsheet can be easily configured to the DOM element, such as div. you can create a Spreadsheet with a highly customizable look and feel.

#### Syntax

{% highlight javascript %}

$(element).ejSpreadsheet(options)

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
{% highlight html %} 
options
{% endhighlight %}
</td>
<td class="type"><ts ref= "ej.Spreadsheet.Model"/><span class="param-type">Object</span></td>
<td class="description">Settings for Spreadsheet.</td>
</tr>
</tbody>
</table>

#### Example

{% highlight html %}
<div id="Spreadsheet"></div> 
<script>
// Create Spreadsheet
$('#Spreadsheet').ejSpreadsheet();
</script>

{% endhighlight %}

#### Requires

* jQuery.js
* jsrender.js
* jQuery.validate.js
* ej.globalize.js
* ej.core.js
* ej.data.js
* ej.scroller.js
* ej.ribbon.js
* ej.chart.js
* ej.listbox.js
* ej.menu.js
* ej.colorpicker.js
* ej.slider.js
* ej.excelfilter.js
* ej.treeview.js
* ej.button.js
* ej.checkbox.js
* ej.draggable.js
* ej.waitingpopup.js
* ej.radiobutton.js
* ej.autocomplete.js
* ej.dropdownlist.js
* ej.datepicker.js
* ej.dialog.js
* ej.editor.js
* ej.pager.js
* ej.ribbon.js
* ej.uploadbox.js
* ej.togglebutton.js
* ej.calculate.js
* ej.tab.js
* ej.toolbar.js

## Members

### activeSheetIndex `number`
{:#members:activesheetindex}


Gets or sets an active sheet index in the Spreadsheet. By defining this value, you can specify which sheet should be active in workbook.

#### Default Value
* 1


#### Example

{% highlight html %}
<div id="Spreadsheet"></div>
<script>
$('#Spreadsheet').ejSpreadsheet({
    sheetCount: 5,
    activeSheetIndex: 3
});         
</script>

{% endhighlight %}

### allowAutoCellType `boolean`
{:#members:allowautocelltype}

Gets or sets a value that indicates whether to enable or disable auto rendering of cell type in the Spreadsheet. 

#### Default Value
* false


N> [`allowCellType`](https://help.syncfusion.com/api/js/ejspreadsheet#members:allowcelltype "allowCellType") must be `true` while using this property.

#### Example

{% highlight html %}
<div id="Spreadsheet"></div> 
<script>
$('#Spreadsheet').ejSpreadsheet({   
    allowCellType: true,
    allowAutoCellType:true
});        
</script>

{% endhighlight %}

### allowAutoFill `boolean`
{:#members:allowautofill}

Gets or sets a value that indicates whether to enable or disable auto fill feature in the Spreadsheet. 

#### Default Value
* true

#### Example
{% highlight html %}
<div id="Spreadsheet"></div> 
<script>
$('#Spreadsheet').ejSpreadsheet({   
    allowAutoFill: true
});        
</script>


{% endhighlight %}

### allowAutoSum `boolean`
{:#members:allowautosum}

Gets or sets a value that indicates whether to enable or disable auto sum feature in the Spreadsheet.

#### Default Value
* true


#### Example
{% highlight html %}
<div id="Spreadsheet"></div>
<script>
$('#Spreadsheet').ejSpreadsheet({ 
    allowAutoSum: true
});         
</script>


{% endhighlight %}

### allowCellFormatting `boolean`
{:#members:allowcellformatting}

Gets or sets a value that indicates whether to enable or disable cell format feature in the Spreadsheet. By enabling this, you can customize styles and number formats.

#### Default Value
* true


#### Example
{% highlight html %}
<div id="Spreadsheet"></div> 
<script>
$('#Spreadsheet').ejSpreadsheet({ 
    allowCellFormatting : true
});                     
</script>

{% endhighlight %}

### allowCellType `boolean`
{:#members:allowcelltype}

Gets or sets a value that indicates whether to enable or disable cell type feature in the Spreadsheet.

#### Default Value
* false

#### Example
{% highlight html %}
<div id="Spreadsheet"></div> 
<script>
$('#Spreadsheet').ejSpreadsheet({ 
    allowCellType : true
});                     
</script>

{% endhighlight %}

### allowCharts `boolean`
{:#members:allowcharts}

Gets or sets a value that indicates whether to enable or disable chart feature in the Spreadsheet. By enabling this feature, you can create and customize charts in Spreadsheet.

#### Default Value
* true


#### Example
{% highlight html %}
<div id="Spreadsheet"></div> 
<script>
$('#Spreadsheet').ejSpreadsheet({ 
    allowCharts: false
}); 
</script>

{% endhighlight %}

### allowClear `boolean`
{:#members:allowclear}

Gets or sets a value that indicates whether to enable or disable clear feature in the Spreadsheet.
 
#### Default Value
* true


#### Example
{% highlight html %}
<div id="Spreadsheet"></div> 
<script>
$('#Spreadsheet').ejSpreadsheet({ 
allowClear: false
}); 
</script>
 
{% endhighlight %}

### allowClipboard `boolean`
{:#members:allowclipboard}

Gets or sets a value that indicates whether to enable or disable clipboard feature in the Spreadsheet. By enabling this feature, you can perform cut/copy and paste operations in Spreadsheet.

#### Default Value
* true


#### Example
{% highlight html %}
<div id="Spreadsheet"></div> 
<script>
$('#Spreadsheet').ejSpreadsheet({ 
    allowClipboard : true                  
});
</script>


{% endhighlight %}

### allowComments `boolean`
{:#members:allowcomments}

Gets or sets a value that indicates whether to enable or disable comment feature in the Spreadsheet. By enabling this, you can add/delete/modify comments in Spreadsheet.

#### Default Value
* true

#### Example
{% highlight html %}
<div id="Spreadsheet"></div> 
<script>
$('#Spreadsheet').ejSpreadsheet({ 
    allowComments: true
});         
</script>


{% endhighlight %}

### allowConditionalFormats `boolean`
{:#members:allowconditionalformats}

Gets or sets a value that indicates whether to enable or disable Conditional Format feature in the Spreadsheet. By enabling this, you can apply formatting to the selected range of cells based on the provided conditions (Greater than, Less than, Equal, Between, Contains, etc.).

N> [`allowConditionalFormats`](https://help.syncfusion.com/api/js/ejspreadsheet#members:allowconditionalformats "allowConditionalFormats") must be `true` while using conditional formatting.

#### Default Value
* true


#### Example
{% highlight html %}
<div id="Spreadsheet"></div> 
<script>
$('#Spreadsheet').ejSpreadsheet({
    allowCellFormatting : true,
    allowConditionalFormats : true        
});
</script>


{% endhighlight %}

### allowDataValidation `boolean`
{:#members:allowdatavalidation}

Gets or sets a value that indicates whether to enable or disable data validation feature in the Spreadsheet.

#### Default Value
* true


#### Example
{% highlight html %}
<div id="Spreadsheet"></div> 
<script>
$('#Spreadsheet').ejSpreadsheet({ 
    allowDataValidation: true                   
});
</script>


{% endhighlight %}

### allowDelete `boolean`
{:#members:allowdelete}

Gets or sets a value that indicates whether to enable or disable the delete action in the Spreadsheet. By enabling this feature, you can delete existing rows, columns, cells and sheet.
 
#### Default Value
* true


#### Example
{% highlight html %}
<div id="Spreadsheet"></div> 
<script>
$('#Spreadsheet').ejSpreadsheet({ 
    allowDelete: true
});         
</script>


{% endhighlight %}

### allowDragAndDrop `boolean`
{:#members:allowdraganddrop}

Gets or sets a value that indicates whether to enable or disable drag and drop feature in the Spreadsheet.

#### Default Value
* true


#### Example
{% highlight html %}
<div id="Spreadsheet"></div> 
<script>
$('#Spreadsheet').ejSpreadsheet({ 
    allowDragAndDrop: true
});         
</script>


{% endhighlight %}

### allowEditing `boolean`
{:#members:allowediting}

Gets or sets a value that indicates whether to enable or disable the edit action in the Spreadsheet.

#### Default Value
* true


#### Example
{% highlight html %}
<div id="Spreadsheet"></div> 
<script>
$('#Spreadsheet').ejSpreadsheet({ 
    allowEditing: true
});         
</script>


{% endhighlight %}

### allowFiltering `boolean`
{:#members:allowfiltering}

Gets or sets a value that indicates whether to enable or disable filtering feature in the Spreadsheet. Filtering can be used to limit the data displayed using required criteria.

#### Default Value
* true


#### Example
{% highlight html %}
<div id="Spreadsheet"></div> 
<script>
$('#Spreadsheet').ejSpreadsheet({ 
    allowFiltering: true
});         
</script>


{% endhighlight %}

### allowFormatAsTable `boolean`
{:#members:allowformatastable}

Gets or sets a value that indicates whether to enable or disable table feature in the Spreadsheet. By enabling this, you can render table in selected range.

N> [`allowCellFormatting`](https://help.syncfusion.com/api/js/ejspreadsheet#members:allowcellformatting "allowCellFormatting") and [`allowFiltering`](https://help.syncfusion.com/api/js/ejspreadsheet#members:allowfiltering "allowFiltering") must be `true` while using format as table.

#### Default Value
* true


#### Example
{% highlight html %}
<div id="Spreadsheet"></div> 
<script>
$('#Spreadsheet').ejSpreadsheet({ 
    allowCellFormatting  :true,
    allowFiltering:true,
    allowFormatAsTable: true
});         
</script>


{% endhighlight %}

### allowFormatPainter `boolean`
{:#members:allowformatpainter}

Get or sets a value that indicates whether to enable or disable format painter feature in the Spreadsheet. By enabling this feature, you can copy the format from the selected range and apply it to another range.

N> [`allowCellFormatting`](https://help.syncfusion.com/api/js/ejspreadsheet#members:allowcellformatting "allowCellFormatting") must be `true` while enable this feature.

#### Default Value
* true


#### Example
{% highlight html %}
<div id="Spreadsheet"></div>  
<script>
$('#Spreadsheet').ejSpreadsheet({ 
    allowCellFormatting: true,
    allowFormatPainter: true
});         
</script>


{% endhighlight %}

### allowFormulaBar `boolean`
{:#members:allowformulabar}

Gets or sets a value that indicates whether to enable or disable formula bar in the Spreadsheet.

#### Default Value
* true


#### Example
{% highlight html %}
<div id="Spreadsheet"></div>  
<script>
$('#Spreadsheet').ejSpreadsheet({ 
    allowFormulaBar: false
});         
</script>


{% endhighlight %}

### allowFreezing `boolean`
{:#members:allowfreezing}

Gets or sets a value that indicates whether to enable or disable freeze pane support in Spreadsheet. By enabling this feature, you can use freeze top row, freeze first column and freeze panes options.

#### Default Value
* true


#### Example
{% highlight html %}
<div id="Spreadsheet"></div> 
<script>
$('#Spreadsheet').ejSpreadsheet({
    allowFreezing : false
});
</script>


{% endhighlight %}

### allowHyperlink `boolean`
{:#members:allowhyperlink}

Gets or sets a value that indicates whether to enable or disable hyperlink feature in the Spreadsheet. By enabling this feature, you can add hyperlink which is used to easily navigate to the cell reference from one sheet to another or a web page.

#### Default Value
* true


#### Example
{% highlight html %}
<div id="Spreadsheet"></div> 
<script>
$('#Spreadsheet').ejSpreadsheet({ 
    allowHyperlink: true
});         
</script>


{% endhighlight %}

### allowImport `boolean`
{:#members:allowimport}

Gets or sets a value that indicates whether to enable or disable import feature in the Spreadsheet. By enabling this feature, you can open existing Spreadsheet documents. 

N> Need to specify [`importMapper`](https://help.syncfusion.com/api/js/ejspreadsheet#members:importsettings-importmapper "importMapper") while enabling this feature.Import feature supports XLS, XLSX file formats.

#### Default Value
* true


#### Example
{% highlight html %}
<div id="Spreadsheet"></div> 
<script>
$('#Spreadsheet').ejSpreadsheet({ 
    allowImport: true,
    importSettings:
        {
            importMapper: "http://js.syncfusion.com/demos/ejservices/api/Spreadsheet/Import"
        }
});         
</script>


{% endhighlight %}

### allowInsert `boolean`
{:#members:allowinsert}

Gets or sets a value that indicates whether to enable or disable the insert action in the Spreadsheet. By enabling this feature, you can insert new rows, columns, cells and sheet.

#### Default Value
* true


#### Example
{% highlight html %}
<div id="Spreadsheet"></div> 
<script>
$('#Spreadsheet').ejSpreadsheet({
    allowInsert: true
});         
</script>


{% endhighlight %}

### allowKeyboardNavigation `boolean`
{:#members:allowkeyboardnavigation}

Gets or sets a value that indicates whether to enable or disable keyboard navigation feature in the Spreadsheet.

#### Default Value
* true


#### Example
{% highlight html %}
<div id="Spreadsheet"></div> 
<script>
$('#Spreadsheet').ejSpreadsheet({
    allowKeyboardNavigation: true
});         
</script>


{% endhighlight %}

### allowLockCell `boolean`
{:#members:allowlockcell}

Gets or sets a value that indicates whether to enable or disable lock cell feature in the Spreadsheet. 

#### Default Value
* true

#### Example

{% highlight html %}
<div id="Spreadsheet"></div> 
<script>
$('#Spreadsheet').ejSpreadsheet({ 
    allowLockCell: true                    
});
</script>
{% endhighlight %}

### allowMerging `boolean`
{:#members:allowmerging}

Gets or sets a value that indicates whether to enable or disable merge feature in the Spreadsheet.

#### Default Value
* true

#### Example

{% highlight html %}
<div id="Spreadsheet"></div> 
<script>
$('#Spreadsheet').ejSpreadsheet({
    allowMerging: true
});         
</script>

{% endhighlight %}

### allowOverflow `boolean`
{:#members:allowoverflow}

Gets or sets a value that indicates whether to enable or disable overflow feature in the Spreadsheet.

#### Default Value
* true

#### Example

{% highlight html %}
<div id="Spreadsheet"></div> 
<script>
$('#Spreadsheet').ejSpreadsheet({
allowOverflow: false
});         
</script>

{% endhighlight %}

### allowResizing `boolean`
{:#members:allowresizing}

Gets or sets a value that indicates whether to enable or disable resizing feature in the Spreadsheet. By enabling this feature, you can change the column width and row height by dragging its header boundaries.

#### Default Value
* true

#### Example

{% highlight html %}
<div id="Spreadsheet"></div> 
<script>
$('#Spreadsheet').ejSpreadsheet({
    allowResizing: true
});         
</script>

{% endhighlight %}

### allowSearching `boolean`
{:#members:allowsearching}

Gets or sets a value that indicates whether to enable or disable find and replace feature in the Spreadsheet. By enabling this, you can easily find and replace a specific value in the sheet or workbook. By using goto behavior, you can select and highlight all cells that contains specific data or data types.

#### Default Value
* true

#### Example

{% highlight html %}
<div id="Spreadsheet"></div> 
<script>
$('#Spreadsheet').ejSpreadsheet({
    allowSearching : true
});        
</script>

{% endhighlight %}

### allowSelection `boolean`
{:#members:allowselection}

Gets or sets a value that indicates whether to enable or disable selection in the Spreadsheet. By enabling this feature, selected items will be highlighted.

#### Default Value
* true

#### Example
{% highlight html %}
<div id="Spreadsheet"></div>
 
<script>
$('#Spreadsheet').ejSpreadsheet({ 
    allowSelection: true
});         
</script>

{% endhighlight %}

### allowSorting `boolean`
{:#members:allowsorting}

Gets or sets a value that indicates whether to enable the sorting feature in the Spreadsheet. 

#### Default Value
* true

#### Example

{% highlight html %}
<div id="Spreadsheet"></div> 
<script>
$('#Spreadsheet').ejSpreadsheet({ 
    allowSorting: true
});         
</script>

{% endhighlight %}

### allowSparkline `boolean`
{:#members:allowsparkline}

Gets or sets a value that indicates whether to enable the sparkline feature in the Spreadsheet. 

#### Default Value
* false

#### Example

{% highlight html %}
<div id="Spreadsheet"></div> 
<script>
$('#Spreadsheet').ejSpreadsheet({ 
    allowSparkline: true
});         
</script>

{% endhighlight %}

### allowUndoRedo `boolean`
{:#members:allowundoredo}

Gets or sets a value that indicates whether to enable or disable undo and redo feature in the Spreadsheet.

#### Default Value
* true

#### Example

{% highlight html %}
<div id="Spreadsheet"></div> 
<script>
$('#Spreadsheet').ejSpreadsheet({ 
    allowUndoRedo: true                    
});
</script>

{% endhighlight %}

### allowWrap `boolean`
{:#members:allowwrap}

Gets or sets a value that indicates whether to enable or disable wrap text feature in the Spreadsheet. By enabling this, cell content can wrap to the next line, if the cell content exceeds the boundary of the cell.

#### Default Value
* true

#### Example

{% highlight html %}
<div id="Spreadsheet"></div> 
<script>
$('#Spreadsheet').ejSpreadsheet({ 
    allowWrap: true                     
});
</script>

{% endhighlight %}

### apWidth `number`
{:#members:apwidth}

Gets or sets a value that indicates to define the width of the activation panel in Spreadsheet.

#### Default Value
* 300

#### Example

{% highlight html %}
<div id="Spreadsheet"></div>
<script>
$('#Spreadsheet').ejSpreadsheet({ 
    apWidth: 100
});         
</script>

{% endhighlight %}

### autoFillSettings `Object`
{:#members:autofillsettings}

Gets or sets an object that indicates to customize the auto fill behavior in the Spreadsheet.

### autoFillSettings.fillType `enum` 
{:#members:autofillsettings-filltype}

<ts name="ej.Spreadsheet.AutoFillOptions"/>

This property is used to set fillType unit in Spreadsheet. It has five types which are CopyCells, FillSeries, FillFormattingOnly, FillWithoutFormatting and FlashFill.

N> [`allowAutoFill`](https://help.syncfusion.com/api/js/ejspreadsheet#members:allowautofill "allowAutoFill") must be `true` while using this property.

<table class="params">
<thead>
<tr>
<th>Name</th>
<th>Description</th>
</tr>
</thead>
<tbody>
<tr>
<td class="name">CopyCells</td>
<td class="description">Specifies the CopyCells property in AutoFillOptions.</td>
</tr>
<tr>
<td class="name">FillSeries</td>
<td class="description">Specifies the FillSeries property in AutoFillOptions.</td>
</tr>
<tr>
<td class="name">FillFormattingOnly</td>
<td class="description">Specifies the FillFormattingOnly property in AutoFillOptions.</td>
</tr>
<tr>
<td class="name">FillWithoutFormatting</td>
<td class="description">Specifies the FillWithoutFormatting property in AutoFillOptions.</td>
</tr>
<tr>
<td class="name">FlashFill</td>
<td class="description">Specifies the FlashFill property in AutoFillOptions.</td>
</tr>
</tbody>
</table>

#### Default Value
* ej.Spreadsheet.AutoFillOptions.FillSeries



#### Example

{% highlight html %}
<div id="Spreadsheet"></div> 
<script>
$('#Spreadsheet').ejSpreadsheet({
    allowAutoFill: true,
    autoFillSettings:{
        fillType: ej.Spreadsheet.AutoFillOptions.CopyCells
    }
});  
</script>

{% endhighlight %}

### autoFillSettings.showFillOptions `boolean`
{:#members:autofillsettings-showfilloptions}

Gets or sets a value that indicates to enable or disable auto fill options in the Spreadsheet.

N> [`allowAutoFill`](https://help.syncfusion.com/api/js/ejspreadsheet#members:allowautofill "allowAutoFill") must be `true` while enabling this property.

#### Default Value
* true

#### Example

{% highlight html %}
<div id="Spreadsheet"></div> 
<script>
$('#Spreadsheet').ejSpreadsheet({
    allowAutoFill: true,
    autoFillSettings:{
        showFillOptions: true
    }
});  
</script>

{% endhighlight %}

### chartSettings `Object`
{:#members:chartsettings}

Gets or sets an object that indicates to customize the chart behavior in the Spreadsheet.

### chartSettings.height `number`
{:#members:chartsettings-height}

Gets or sets a value that defines the chart height in Spreadsheet.

N> [`allowCharts`](https://help.syncfusion.com/api/js/ejspreadsheet#members:allowcharts "allowCharts") must be `true` while using this property.

#### Default Value
* 220

#### Example

{% highlight html %}
<div id="Spreadsheet"></div> 
<script>
$('#Spreadsheet').ejSpreadsheet({ 
    allowCharts: true,
    chartSettings: {
        height : 300
    }
}); 
</script>

{% endhighlight %}

### chartSettings.width `number`
{:#members:chartsettings-width}

Gets or sets a value that defines the chart width in the Spreadsheet.

N> [`allowCharts`](https://help.syncfusion.com/api/js/ejspreadsheet#members:allowcharts "allowCharts") must be `true` while using this property.

#### Default Value
* 440

#### Example

{% highlight html %}
<div id="Spreadsheet"></div> 
<script>
$('#Spreadsheet').ejSpreadsheet({ 
    allowCharts: true,
    chartSettings: {
        width : 500
    }
}); 
</script>

{% endhighlight %}

### columnCount `number`
{:#members:columncount}

Gets or sets a value that defines the number of columns displayed in the sheet.

#### Default Value
* 21


#### Example
{% highlight html %}
<div id="Spreadsheet"></div>
<script>
$('#Spreadsheet').ejSpreadsheet({ 
    columnCount: 30
});         
</script>

{% endhighlight %}

### columnWidth `number`
{:#members:columnwidth}

Gets or sets a value that indicates to define the common width for each column in the Spreadsheet.

#### Default Value
* 64

#### Example
{% highlight html %}
<div id="Spreadsheet"></div>
<script>
$('#Spreadsheet').ejSpreadsheet({ 
    columnWidth: 100
});         
</script>

{% endhighlight %}

### cssClass `string`
{:#members:cssclass}

Gets or sets a value to add root CSS class for customizing Spreadsheet skins.

#### Default Value
* ""

#### Example

{% highlight html %}
<div id="Spreadsheet"></div>
<script>
// Set the CSS class during initialization. 
$('#Spreadsheet').ejSpreadsheet({
    cssClass: "gradient-lime"
});        
</script>

{% endhighlight %}

### customFormulas `Array`
{:#members:customformulas}

Gets or sets a value that indicates custom formulas in Spreadsheet.

#### Default Value
* []

#### Example

{% highlight html %}
<div id="Spreadsheet"></div>
<script>
// Set the custom formula
$('#Spreadsheet').ejSpreadsheet({
    customFormulas: [{
	    formulaName:"CUSTOMTOTAL",
	    functionName:"customTotal"
    }]
});   
function customTotal(args){}//args-It uses the value given by the user while using custom formula in Spreadsheet.
</script>

{% endhighlight %}

### enableContextMenu `boolean`
{:#members:enablecontextmenu}

Gets or sets a value that indicates whether to enable or disable context menu in the Spreadsheet.

#### Default Value
* true

#### Example

{% highlight html %}
<div id="Spreadsheet"></div> 
<script>
$('#Spreadsheet').ejSpreadsheet({ 
    enableContextMenu: true
});                   
</script>

{% endhighlight %}

### enablePivotTable `boolean`
{:#members:enablepivottable}

Gets or sets a value that indicates whether to enable or disable pivot table in the Spreadsheet.

#### Default Value
* false

#### Example

{% highlight html %}
<div id="Spreadsheet"></div> 
<script>
$('#Spreadsheet').ejSpreadsheet({ 
    enablePivotTable: false
});                   
</script>

{% endhighlight %}

### enableTouch `boolean`
{:#members:enabletouch}

Gets or sets a value that indicates whether to enable or disable touch support in the Spreadsheet.

#### Default Value
* true

#### Example

{% highlight html %}
<div id="Spreadsheet"></div> 
<script>
$('#Spreadsheet').ejSpreadsheet({ 
    enableTouch: true
});                   
</script>

{% endhighlight %}

### exportSettings `Object`
{:#members:exportsettings}

Gets or sets an object that indicates to customize the exporting behavior in Spreadsheet.

### exportSettings.allowExporting `boolean`
{:#members:exportsettings-allowexporting}

Gets or sets a value that indicates whether to enable or disable save feature in Spreadsheet. By enabling this feature, you can save existing Spreadsheet.

N> User must specify [`excelUrl`](https://help.syncfusion.com/api/js/ejspreadsheet#members:exportsettings-excelurl "excelUrl") or [`pdfUrl`](https://help.syncfusion.com/api/js/ejspreadsheet#members:exportsettings-pdfurl "pdfUrl") or [`csvUrl`](https://help.syncfusion.com/api/js/ejspreadsheet#members:exportsettings-csvurl "csvUrl") while enabling this feature

#### Default Value
* true

#### Example
{% highlight html %}

<div id="Spreadsheet"></div> 
<script>
$('#Spreadsheet').ejSpreadsheet({
    exportSettings:{
        allowExporting: true,
        csvUrl: "http://js.syncfusion.com/demos/ejservices/api/Spreadsheet/CsvExport", // It is used to set the url of the csv export.
        excelUrl: "http://js.syncfusion.com/demos/ejservices/api/Spreadsheet/ExcelExport", //It is used to set the url of the excel export.
        pdfUrl: "http://js.syncfusion.com/demos/ejservices/api/Spreadsheet/PdfExport", //It is used to set the url of the pdf export.
    }
});        
</script>

{% endhighlight %}

### exportSettings.enableFormulaCalculation `boolean`
{:#members:exportsettings-enableFormulaCalculation}

Gets or sets a value that indicates whether to enable or disable formula calculation in Spreadsheet. By enabling this feature, formula calculated while export the Spreadsheet in protected mode.

#### Default Value
* false

#### Example
{% highlight html %}

<div id="Spreadsheet"></div> 
<script>
$('#Spreadsheet').ejSpreadsheet({
    exportSettings:{
        enableFormulaCalculation: true,
        csvUrl: "http://js.syncfusion.com/demos/ejservices/api/Spreadsheet/CsvExport", // It is used to set the url of the csv export.
        excelUrl: "http://js.syncfusion.com/demos/ejservices/api/Spreadsheet/ExcelExport", //It is used to set the url of the excel export.
        pdfUrl: "http://js.syncfusion.com/demos/ejservices/api/Spreadsheet/PdfExport", //It is used to set the url of the pdf export.
    }
});        
</script>

{% endhighlight %}

### exportSettings.csvUrl `string`
{:#members:exportsettings-csvurl}

Gets or sets a value that indicates to define csvUrl for export to CSV format.

N> User must specify [`allowExporting`](https://help.syncfusion.com/api/js/ejspreadsheet#members:exportsettings-allowexporting "allowExporting") `true` while using this property.

#### Default Value
* null

#### Example

{% highlight html %}
<div id="Spreadsheet"></div> 
<script>
$('#Spreadsheet').ejSpreadsheet({
    exportSettings:{
        allowExporting: true,
        csvUrl: "http://js.syncfusion.com/demos/ejservices/api/Spreadsheet/CsvExport", // It is used to set the url of the csv export.
    }
});        
</script>

{% endhighlight %}

### exportSettings.excelUrl `string`
{:#members:exportsettings-excelurl}

Gets or sets a value that indicates to define excelUrl for export to excel format.

N> User must specify [`allowExporting`](https://help.syncfusion.com/api/js/ejspreadsheet#members:exportsettings-allowexporting "allowExporting") `true` while using this property.

#### Default Value
* null

#### Example

{% highlight html %}
<div id="Spreadsheet"></div> 
<script>
$('#Spreadsheet').ejSpreadsheet({
    exportSettings:{
        allowExporting: true,
        excelUrl: "http://js.syncfusion.com/demos/ejservices/api/Spreadsheet/ExcelExport", //It is used to set the url of the excel export.
    }
});        
</script>

{% endhighlight %}

### exportSettings.password `string`
{:#members:exportsettings-password}

Gets or sets a value that indicates to define password while export to excel format.

N> User must specify [`allowExporting`](https://help.syncfusion.com/api/js/ejspreadsheet#members:exportsettings-allowexporting "allowExporting") `true` while using this property.

#### Default Value
* null

#### Example

{% highlight html %}
<div id="Spreadsheet"></div> 
<script>
$('#Spreadsheet').ejSpreadsheet({
    exportSettings:{
        allowExporting: true,
        excelUrl: "http://js.syncfusion.com/demos/ejservices/api/Spreadsheet/ExcelExport", //It is used to set the url of the excel export
        password :"Spreadsheet"
    }
});        
</script>

{% endhighlight %}

### exportSettings.pdfUrl `string`
{:#members:exportsettings-pdfurl}

Gets or sets a value that indicates to define pdfUrl for export to PDF format.

N> User must specify [`allowExporting`](https://help.syncfusion.com/api/js/ejspreadsheet#members:exportsettings-allowexporting "allowExporting") `true` while using this property.

#### Default Value
* null

#### Example

{% highlight html %}
<div id="Spreadsheet"></div> 
<script>
$('#Spreadsheet').ejSpreadsheet({
    exportSettings:{
        allowExporting: true,
        pdfUrl: "http://js.syncfusion.com/demos/ejservices/api/Spreadsheet/PdfExport", //It is used to set the url of the pdf export.
    }
});        
</script>

{% endhighlight %}

### formatSettings `Object`
{:#members:formatsettings}

Gets or sets an object that indicates to customize the format behavior in the Spreadsheet.

### formatSettings.allowCellBorder `boolean`
{:#members:formatsettings-allowcellborder}

Gets or sets a value that indicates whether to enable or disable cell border feature in the Spreadsheet.

N> [`allowCellFormatting`](https://help.syncfusion.com/api/js/ejspreadsheet#members:allowcellformatting "allowCellFormatting") must be `true` while using this property.

#### Default Value
* true

#### Example
{% highlight html %}
<div id="Spreadsheet"></div> 
<script>
$('#Spreadsheet').ejSpreadsheet({
    allowCellFormatting: true,
    formatSettings:{
        allowCellBorder: true
    }
});  
</script>

{% endhighlight %}

### formatSettings.allowDecimalPlaces `boolean`
{:#members:formatsettings-allowdecimalplaces}

Gets or sets a value that indicates whether to enable or disable decimal places in the Spreadsheet.

N> [`allowCellFormatting`](https://help.syncfusion.com/api/js/ejspreadsheet#members:allowcellformatting "allowCellFormatting") must be `true` while using this property.

#### Default Value
* true

#### Example

{% highlight html %}
<div id="Spreadsheet"></div> 
<script>
$('#Spreadsheet').ejSpreadsheet({
    allowCellFormatting: true,
    formatSettings:{
        allowDecimalPlaces: true
    }
});  
</script>

{% endhighlight %}

### formatSettings.allowFontFamily `boolean`
{:#members:formatsettings-allowfontfamily}

Gets or sets a value that indicates whether to enable or disable font family feature in Spreadsheet.

N> [`allowCellFormatting`](https://help.syncfusion.com/api/js/ejspreadsheet#members:allowcellformatting "allowCellFormatting") must be `true` while using this property. 

#### Default Value
* true

#### Example

{% highlight html %}
<div id="Spreadsheet"></div> 
<script>
$('#Spreadsheet').ejSpreadsheet({
    allowCellFormatting : true,
    formatSettings:{
        allowFontFamily: true
    }
});  
</script>

{% endhighlight %}

### importSettings `Object`
{:#members:importsettings}

Gets or sets an object that indicates to customize the import behavior in the Spreadsheet.

### importSettings.importMapper `string`
{:#members:importsettings-importmapper}

Sets import mapper to perform import feature in Spreadsheet.

N> [`allowImport`](https://help.syncfusion.com/api/js/ejspreadsheet#members:allowimport "allowImport") must be `true` while using this property.

#### Default Value
* ""

#### Example

{% highlight html %}
<div id="Spreadsheet"></div> 
<script>
$('#Spreadsheet').ejSpreadsheet({
    allowImport: true,
    importSettings:{
        importMapper: "http://js.syncfusion.com/demos/ejservices/api/Spreadsheet/Import"
    }
});        
</script>

{% endhighlight %}

### importSettings.importOnLoad `boolean`
{:#members:importsettings-importonload}

Gets or sets a value that indicates whether to enable or disable import while initial loading.

#### Default Value
* false

#### Example

{% highlight html %}

<div id="Spreadsheet"></div>

<script>
$('#Spreadsheet').ejSpreadsheet({ 
    importSettings: {
        importOnLoad: true            
    }
});                   
</script>

{% endhighlight %}

### importSettings.importUrl `string`
{:#members:importsettings-importurl}

Sets import URL to access the online files in the Spreadsheet.

N> [`allowImport`](https://help.syncfusion.com/api/js/ejspreadsheet#members:allowimport "allowImport") must be `true` while using this property.

#### Default Value
* ""

#### Example

{% highlight html %}
<div id="Spreadsheet"></div> 
<script>
$('#Spreadsheet').ejSpreadsheet({
    allowImport: true,
    importSettings:{
        importUrl: "http://mvc.syncfusion.com/Spreadsheet/Spreadsheet.xlsx", //It is used to access the online files in Spreadsheet.
    }
});        
</script>

{% endhighlight %}

### importSettings.password `string`
{:#members:importsettings-password}

Gets or sets a value that indicates to define password while importing in the Spreadsheet.

N> [`allowImport`](https://help.syncfusion.com/api/js/ejspreadsheet#members:allowimport "allowImport") must be `true` while using this property.

#### Default Value
* ""

#### Example

{% highlight html %}
<div id="Spreadsheet"></div> 
<script>
$('#Spreadsheet').ejSpreadsheet({
    allowImport: true,
    importSettings:{
        importMapper: "http://js.syncfusion.com/demos/ejservices/api/Spreadsheet/Import",
        password: "Spreadsheet" //It opens the excel file using this password.
    }
});        
</script>

{% endhighlight %}

### isImport `boolean`
{:#members:isImport}

Gets a value that indicates whether importing or not while loading the sheets in Spreadsheet.

#### Default Value
* false

#### Example

{% highlight html %}
<div id="Spreadsheet"></div> 
<script>
$('#Spreadsheet').ejSpreadsheet({ 
    loadComplete: "loadComplete"
});         
function loadComplete(args) {
    if (!this.model.isImport)
        this.setWidthToColumns([140, 128, 105, 100, 100, 110, 120, 120, 100]);
}         
</script>

{% endhighlight %}

### isReadOnly `boolean`
{:#members:isreadonly}

Gets or sets a value that indicates whether to enable or disable readonly support in the Spreadsheet.

#### Default Value
* false

#### Example
{% highlight html %}
<div id="Spreadsheet"></div>
 
<script>
$('#Spreadsheet').ejSpreadsheet({ 
    isReadOnly: true
});         
</script>

{% endhighlight %}

### locale `string`
{:#members:locale}

Gets or sets a value that indicates whether to customizing the user interface (UI) as locale-specific in order to display regional data (i.e.) in a language and culture specific to a particular country or region.

#### Default Value
* "en-US"

#### Example

{% highlight html %}
<div id="Spreadsheet"></div>
<script>
ej.Spreadsheet.locale["es-ES"] = {
Sheet: "Hoja"
};             
$('#Spreadsheet').ejSpreadsheet({ 
    locale: "es-ES"
});         
</script>

{% endhighlight %}

### nameManager `Array`
{:#members:namemanager}

Gets or sets a value that indicates name manager in Spreadsheet.

### nameManager.name `string`
{:#members:namemanager-name}

Specifies the name for the cell or a range.

#### Default Value
* ""

#### Example

{% highlight html %}
<div id="Spreadsheet"></div> 
<script>
$('#Spreadsheet').ejSpreadsheet({
    nameManager:[{
        name: "inputRange",
		refersto: "=Sheet1!$A$1:$A$2"
    }]
});    
</script>

{% endhighlight %}

### nameManager.refersto `string`
{:#members:namemanager-refersto}

Specifies the address for the cell or a range.

#### Default Value
* ""

#### Example

{% highlight html %}
<div id="Spreadsheet"></div> 
<script>
$('#Spreadsheet').ejSpreadsheet({
    nameManager:[{
        name: "inputRange",
		refersto: "=Sheet1!$A$1:$A$2"
    }]
});    
</script>

{% endhighlight %}

### pictureSettings `Object`
{:#members:picturesettings}

Gets or sets an object that indicates to customize the picture behavior in the Spreadsheet.

### pictureSettings.allowPictures `boolean`
{:#members:picturesettings-allowpictures}

Gets or sets a value that indicates whether to enable or disable picture feature in Spreadsheet. By enabling this, you can add pictures in Spreadsheet.

#### Default Value
* true

#### Example

{% highlight html %}
<div id="Spreadsheet"></div> 
<script>
$('#Spreadsheet').ejSpreadsheet({
    pictureSettings:{
        allowPictures: true
    }
});    
</script>

{% endhighlight %}

### pictureSettings.height `number`
{:#members:picturesettings-height}

Gets or sets a value that indicates to define height to picture in the Spreadsheet.

N> [`allowPictures`](https://help.syncfusion.com/api/js/ejspreadsheet#members:picturesettings-allowpictures "allowPictures") must be `true` while using this property.

#### Default Value
* 220

#### Example

{% highlight html %}
<div id="Spreadsheet"></div> 
<script>
$('#Spreadsheet').ejSpreadsheet({
    pictureSettings:{
        allowPictures: true,
        height: 300
    }
});    
</script>

{% endhighlight %}

### pictureSettings.width `number`
{:#members:picturesettings-width}

Gets or sets a value that indicates to define width to picture in the Spreadsheet.

N> [`allowPictures`](https://help.syncfusion.com/api/js/ejspreadsheet#members:picturesettings-allowpictures "allowPictures") must be `true` while using this property.

#### Default Value
* 440

#### Example

{% highlight html %}
<div id="Spreadsheet"></div> 
<script>
$('#Spreadsheet').ejSpreadsheet({
    pictureSettings:{
        allowPictures: true,
        width: 500
    }
});    
</script>

{% endhighlight %}

### printSettings `Object`
{:#members:printsettings}

Gets or sets an object that indicates to customize the print option in Spreadsheet.

### printSettings.allowPageSetup `boolean`
{:#members:printsettings-allowpagesetup}

Gets or sets a value that indicates whether to enable or disable page setup support for printing in Spreadsheet. 

N> [`allowPrinting`](https://help.syncfusion.com/api/js/ejspreadsheet#members:printsettings-allowprinting "allowPrinting") must be `true` while enabling this property.

#### Default Value
* true

#### Example

{% highlight html %}
<div id="Spreadsheet"></div> 
<script>
$('#Spreadsheet').ejSpreadsheet({
    allowPrinting: true,
    printSettings:{
        allowPageSetup: true
    }
});   
</script>

{% endhighlight %}

### printSettings.allowPageSize `boolean`
{:#members:printsettings-allowpagesize}

Gets or sets a value that indicates whether to enable or disable page size support for printing in Spreadsheet.

N> [`allowPrinting`](https://help.syncfusion.com/api/js/ejspreadsheet#members:printsettings-allowprinting "allowPrinting") must be `true` while enabling this property.

#### Default Value
* false

#### Example

{% highlight html %}
<div id="Spreadsheet"></div> 
<script>
$('#Spreadsheet').ejSpreadsheet({
    allowPrinting: true,
    printSettings:{
        allowPageSize: true
    }
});   
</script>

{% endhighlight %}

### printSettings.allowPrinting `boolean`
{:#members:printsettings-allowprinting}

Gets or sets a value that indicates whether to enable or disable print feature in the Spreadsheet.

#### Default Value
* true

#### Example

{% highlight html %}
<div id="Spreadsheet"></div> 
<script>
$('#Spreadsheet').ejSpreadsheet({
    printSettings:{
        allowPrinting: true
    }
});   
</script>

{% endhighlight %}

### ribbonSettings `Object`
{:#members:ribbonsettings}

Gets or sets an object that indicates to customize the ribbon settings in Spreadsheet.

### ribbonSettings.applicationTab `Object`
{:#members:ribbonsettings-applicationtab}

Gets or sets an object that indicates application tab settings in Spreadsheet.

N>[`showRibbon`](https://help.syncfusion.com/api/js/ejspreadsheet#members:showribbon "showRibbon") must be `true` while using this property.

### ribbonSettings.applicationTab.type `enum`
{:#members:ribbonsettings-applicationtab-type}

<ts ref="ej.Ribbon.ApplicationTabType"/>

Gets or sets a value that indicates to set application tab type in Spreadsheet. It has two types, Menu and Backstage.

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
<td class="description">To enable menu type in ribbon.</td>
</tr>
<tr>
<td class="name">Backstage</td>
<td class="description">To enable back stage type in ribbon.</td>
</tr>
</tbody>
</table>

#### Default Value
* ej.Ribbon.ApplicationTabType.Backstage

#### Example

{% highlight html %}
<div id="Spreadsheet"></div> 
<script>
$('#Spreadsheet').ejSpreadsheet({
    ribbonSettings: {
        applicationTab: {
            type: ej.Ribbon.ApplicationTabType.Menu
        }
    }
    });   
</script>

{% endhighlight %}

### ribbonSettings.applicationTab.menuSettings `Object`
{:#members:ribbonsettings-applicationtab-menusettings}

Gets or sets an object that indicates menu settings for application tab in Spreadsheet.

N> `ApplicationTabType` should be `Menu` while using this property.

### ribbonSettings.applicationTab.menuSettings.isAppend `boolean`
{:#members:ribbonsettings-applicationtab-menusettings-isappend}

Gets or sets a value that indicates whether to enable or disable isAppend property in ribbon settings.

#### Default Value
* false

#### Example

{% highlight html %}
<div id="Spreadsheet"></div> 
<script>
$('#Spreadsheet').ejSpreadsheet({
    ribbonSettings:{
        applicationTab:{
            type: ej.Ribbon.ApplicationTabType.Menu
            menuSettings:{
                isAppend:true
            }
        }
    }   
});   
</script>

{% endhighlight %}

### ribbonSettings.applicationTab.menuSettings.dataSource `Array`
{:#members:ribbonsettings-applicationtab-menusettings-datasource}

Specifies the data source to append in application tab.

#### Default Value
* []

#### Example

{% highlight html %}
<div id="Spreadsheet"></div> 
<script>
$('#Spreadsheet').ejSpreadsheet({
    ribbonSettings:{
        applicationTab:{
            type: ej.Ribbon.ApplicationTabType.Menu,
            menuSettings:{                
                isAppend:true,
                dataSource:[{ id: "File", text: "File" }]
            }
        }
    }
});   
</script>

{% endhighlight %}

### rowCount `number`
{:#members:rowcount}

Gets or sets a value that indicates whether to define the number of rows to be displayed in the sheet.

#### Default Value
* 20

#### Example

{% highlight html %}
<div id="Spreadsheet"></div> 
<script>
$('#Spreadsheet').ejSpreadsheet({ 
    rowCount: 30
});         
</script>

{% endhighlight %}

### rowHeight `number`
{:#members:rowheight}

Gets or sets a value that indicates to define the common height for each row in the sheet.

#### Default Value
* 20

#### Example

{% highlight html %}
<div id="Spreadsheet"></div> 
<script>
$('#Spreadsheet').ejSpreadsheet({ 
    rowHeight: 30
});         
</script>

{% endhighlight %}

### scrollSettings `Object`
{:#members:scrollsettings}

Gets or sets an object that indicates to customize the scroll options in the Spreadsheet.

### scrollSettings.allowScrolling `boolean`
{:#members:scrollsettings-allowscrolling}

Gets or sets a value that indicates whether to enable or disable scrolling in Spreadsheet.

#### Default Value
* true

#### Example
{% highlight html %}
<div id="Spreadsheet"></div> 
<script>
$('#Spreadsheet').ejSpreadsheet({
    scrollSettings:{
        allowScrolling: true,
    }
});    
</script>

{% endhighlight %}

### scrollSettings.allowSheetOnDemand `boolean`
{:#members:scrollsettings-allowsheetondemand}

Gets or sets a value that indicates whether to enable or disable sheet on demand. By enabling this, it render only the active sheet element while paging remaining sheets are created one by one.

#### Default Value
* false

#### Example

{% highlight html %}
<div id="Spreadsheet"></div> 
<script>
$('#Spreadsheet').ejSpreadsheet({
    scrollSettings:{
        allowScrolling: true,
        allowSheetOnDemand: true
    }
});    
</script>

{% endhighlight %}

### scrollSettings.allowVirtualScrolling `boolean`
{:#members:scrollsettings-allowvirtualscrolling}

Gets or sets a value that indicates whether to enable or disable virtual scrolling feature in the Spreadsheet.

N> [`allowScrolling`](https://help.syncfusion.com/api/js/ejspreadsheet#members:scrollsettings-allowscrolling "allowScrolling") must be `true` while enabling this property.

#### Default Value
* true

#### Example

{% highlight html %}
<div id="Spreadsheet"></div> 
<script>
$('#Spreadsheet').ejSpreadsheet({
    scrollSettings:{
        allowScrolling: true,
        allowVirtualScrolling: true
    }
});    
</script>

{% endhighlight %}

### scrollSettings.height  `number|string`
{:#members:scrollsettings-height}

Gets or sets the value that indicates to define the height of spreadsheet.

#### Default Value
* 100%

#### Example

{% highlight html %}
<div id="Spreadsheet"></div> 
<script>
$('#Spreadsheet').ejSpreadsheet({
    scrollSettings:{
        allowScrolling: true,
        height: 600
    }
});    
</script>

{% endhighlight %}

### scrollSettings.isResponsive `boolean`
{:#members:scrollsettings-isresponsive}

Gets or sets the value that indicates whether to enable or disable responsive mode in the Spreadsheet.

#### Default Value
* true

#### Example

{% highlight html %}
<div id="Spreadsheet"></div> 
<script>
$('#Spreadsheet').ejSpreadsheet({
    scrollSettings:{
        allowScrolling: true,
        width: "100%",
        height: "100%",
        isResponsive: true
    }
});    
</script>

{% endhighlight %}

### scrollSettings.scrollMode `enum`
{:#members:scrollsettings-scrollmode}

<ts name="ej.Spreadsheet.scrollMode"/>

Gets or sets a value that indicates to set scroll mode in Spreadsheet. It has two scroll modes, Normal and Infinite.

N> [`allowScrolling`](https://help.syncfusion.com/api/js/ejspreadsheet#members:scrollsettings-allowscrolling "allowScrolling") must be `true` while enabling this property.

<table class="params">
<thead>
<tr>
<th>Name</th>
<th>Description</th>
</tr>
</thead>
<tbody>
<tr>
<td class="name">Infinite</td>
<td class="description">To enable Infinite scroll mode for Spreadsheet.</td>
</tr>
<tr>
<td class="name">Normal</td>
<td class="description">To enable Normal scroll mode for Spreadsheet.</td>
</tr>
</tbody>
</table>

#### Default Value
* ej.Spreadsheet.scrollMode.Infinite



#### Example

{% highlight html %}
<div id="Spreadsheet"></div> 
<script>
$('#Spreadsheet').ejSpreadsheet({
    scrollSettings:{
        allowScrolling: true,
        height: "100%",
        width: "100%",
        scrollmode: ej.Spreadsheet.scrollMode.Infinite,
    }
});    
</script>

{% endhighlight %}

### scrollSettings.width `number|string`
{:#members:scrollsettings-width}

Gets or sets the value that indicates to define the height of the spreadsheet.

#### Default Value
* 100%

#### Example

{% highlight html %}
<div id="Spreadsheet"></div> 
<script>
$('#Spreadsheet').ejSpreadsheet({
    scrollSettings:{
        allowScrolling: true,
        width: 1300,
        scrollmode: ej.Spreadsheet.scrollMode.Infinite
    }
});    
</script>

{% endhighlight %}

### selectionSettings `Object`
{:#members:selectionsettings}

Gets or sets an object that indicates to customize the selection options in the Spreadsheet.

### selectionSettings.activeCell `string`
{:#members:selectionsettings-activecell}

Gets or sets a value that indicates to define active cell in spreadsheet.

N> [`allowSelection`](https://help.syncfusion.com/api/js/ejspreadsheet#members:allowselection "allowSelection") must be `true` while using this property.

#### Default Value
* ""

#### Example

{% highlight html %}
<div id="Spreadsheet"></div> 
<script>
$('#Spreadsheet').ejSpreadsheet({
    allowSelection: true,
    selectionSettings:{
        activeCell: "A1"
    }
});
</script>

{% endhighlight %}

### selectionSettings.animationTime `number`
{:#members:selectionsettings-animationtime}

Gets or sets a value that indicates to define animation time while selection in the Spreadsheet.

N> [`allowSelection`](https://help.syncfusion.com/api/js/ejspreadsheet#members:allowselection "allowSelection") must be `true` while using this property.

#### Default Value
* 0.001

#### Example

{% highlight html %}
<div id="Spreadsheet"></div> 
<script>
$('#Spreadsheet').ejSpreadsheet({
    allowSelection: true,
    selectionSettings:{
        enableAnimation: true,
        animationTime: 0.002
    }
});
</script>

{% endhighlight %}

### selectionSettings.enableAnimation `boolean`
{:#members:selectionsettings-enableanimation}

Gets or sets a value that indicates to enable or disable animation while selection.

N> [`allowSelection`](https://help.syncfusion.com/api/js/ejspreadsheet#members:allowselection "allowSelection") must be `true` while using this property

#### Default Value
* false

#### Example

{% highlight html %}
<div id="Spreadsheet"></div> 
<script>
$('#Spreadsheet').ejSpreadsheet({
    allowSelection: true,
    selectionSettings:{
        enableAnimation: true
    }
});
</script>

{% endhighlight %}

### selectionSettings.selectionType `enum`
{:#members:selectionsettings-selectiontype}

<ts name="ej.Spreadsheet.SelectionType"/>

Gets or sets a value that indicates to set selection type in Spreadsheet. It has three types which are Column, Row and Default.

N> [`allowSelection`](https://help.syncfusion.com/api/js/ejspreadsheet#members:allowselection "allowSelection") must be `true` while using this property

<table class="params">
<thead>
<tr>
<th>Name</th>
<th>Description</th>
</tr>
</thead>
<tbody>
<tr>
<td class="name">Column</td>
<td class="description">To select only Column in Spreadsheet.</td>
</tr>
<tr>
<td class="name">Row</td>
<td class="description">To select only Row in Spreadsheet.</td>
</tr>
<tr>
<td class="name">Default</td>
<td class="description">To select both Column/Row in Spreadsheet.</td>
</tr>
</tbody>
</table>

#### Default Value
* ej.Spreadsheet.SelectionType.Default

#### Example

{% highlight html %}
<div id="Spreadsheet"></div>

<script>
$('#Spreadsheet').ejSpreadsheet({
    allowSelection: true,
    selectionSettings:{
        selectionType: ej.Spreadsheet.SelectionType.Row,
        animationTime: 0.001,
        enableAnimation: true
    }
});
</script>
{% endhighlight %}

### selectionSettings.selectionUnit `enum`
{:#members:selectionsettings-selectionunit}

<ts name="ej.Spreadsheet.SelectionUnit"/>

Gets or sets a value that indicates to set selection unit in Spreadsheet. It has three types which are Single, Range and MultiRange.

N> [`allowSelection`](https://help.syncfusion.com/api/js/ejspreadsheet#members:allowselection "allowSelection") must be `true` while using this property
	
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
<td class="description">To enable Single selection in Spreadsheet</td>
</tr>
<tr>
<td class="name">Range</td>
<td class="description">To enable Range selection in Spreadsheet</td>
</tr>
<tr>
<td class="name">MultiRange</td>
<td class="description">To enable MultiRange selection in Spreadsheet</td>
</tr>
</tbody>
</table>

#### Default Value
* ej.Spreadsheet.SelectionUnit.MultiRange

#### Example

{% highlight html %}
<div id="Spreadsheet"></div>

<script>
$('#Spreadsheet').ejSpreadsheet({
    allowSelection: true,
    selectionSettings:{
        selectionUnit: ej.Spreadsheet.SelectionUnit.Single
    }
});  
</script>

{% endhighlight %}

### sheetCount `number`
{:#members:sheetcount}

Gets or sets a value that indicates to define the number of sheets to be created at the initial load.

#### Default Value
* 1

#### Example

{% highlight html %}
<div id="Spreadsheet"></div> 
<script>
$('#Spreadsheet').ejSpreadsheet({ 
    sheetCount: 5
});         
</script>

{% endhighlight %}

### sheets `Array`
{:#members:sheets}

Gets or sets an object that indicates to customize the sheet behavior in Spreadsheet.

### sheets.border `Array`
{:#members:sheets-border}

Specifies the border for the cell in the Spreadsheet.

#### Default Value:

* []

#### Example

{% highlight html %}
<div id="Spreadsheet"></div> 
<script>
$('#Spreadsheet').ejSpreadsheet({
    sheets:[{
        border: [{ type: ej.Spreadsheet.BorderType.AllBorder, color: "#456534", range: "C6:D9" }]
    }]
});    
</script>

{% endhighlight %}

### sheets.border.type `enum`
{:#members:sheets-border-type}

<ts name="ej.Spreadsheet.BorderType"/>

Specifies border type in the Spreadsheet.

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
<td class="description">To apply top border for the given range of cell.</td>
</tr>
<tr>
<td class="name">Left</td>
<td class="description">To apply left border for the given range of cell.</td>
</tr>
<tr>
<td class="name">Right</td>
<td class="description">To apply right border for the given range of cell.</td>
</tr>
<tr>
<td class="name">Bottom</td>
<td class="description">To apply bottom border for the given range of cell.</td>
</tr>
<tr>
<td class="name">OutSide</td>
<td class="description">To apply outside border for the given range of cell.</td>
</tr>
<tr>
<td class="name">AllBorder</td>
<td class="description">To apply all border for the given range of cell.</td>
</tr>
<tr>
<td class="name">ThickBox</td>
<td class="description">To apply thick box border for the given range of cell.</td>
</tr>
<tr>
<td class="name">ThickBottom</td>
<td class="description">To apply thick bottom border for the given range of cell.</td>
</tr>
<tr>
<td class="name">TopandBottom</td>
<td class="description">To apply top and bottom border for the given range of cell.</td>
</tr>
<tr>
<td class="name">TopandThickBottom</td>
<td class="description">To apply top and thick bottom border for the given range of cell.</td>
</tr>
</tbody>
</table>

#### Example

{% highlight html %}
<div id="Spreadsheet"></div> 
<script>
$('#Spreadsheet').ejSpreadsheet({
    sheets:[{
        border: [{ type: ej.Spreadsheet.BorderType.AllBorder, color: "#456534", range: "C6:D9" }]
    }]
});    
</script>

{% endhighlight %}

### sheets.border.color `string`
{:#members:sheets-border-color}

Specifies border color for range of cells in Spreadsheet.

#### Default Value:

* ""

#### Example

{% highlight html %}
<div id="Spreadsheet"></div> 
<script>
$('#Spreadsheet').ejSpreadsheet({
    sheets:[{
        border: [{ type: ej.Spreadsheet.BorderType.AllBorder, color: "#456534", range: "C6:D9" }]
    }]
});    
</script>

{% endhighlight %}

### sheets.border.range `string`
{:#members:sheets-border-range}

To apply border for the specified range of cell. 

#### Default Value:

* ""

#### Example

{% highlight html %}
<div id="Spreadsheet"></div> 
<script>
$('#Spreadsheet').ejSpreadsheet({
    sheets:[{
        border: [{ type: ej.Spreadsheet.BorderType.AllBorder, color: "#456534", range: "C6:D9" }]
    }]
});    
</script>

{% endhighlight %}

### sheets.cellTypes `Array`
{:#members:sheets-celltypes}

Specifies the cell types for a cell or range in Spreadsheet.

#### Default Value:

* []

#### Example

{% highlight html %}
<div id="Spreadsheet"></div> 
<script>
$('#Spreadsheet').ejSpreadsheet({
    sheets: [{
    cellTypes: [{ range: 'F5', settings: { type: ej.Spreadsheet.CustomCellType.Button, 'background-color': 'yellow', color: 'black', text: 'BUTTON' } }]
    }]
});    
</script>

{% endhighlight %}

### sheets.cFormatRule `Array`
{:#members:sheets-cformatrule}

Specifies the conditional formatting for the range of cell in Spreadsheet.

#### Default Value:

* []

#### Example

{% highlight html %}
<div id="Spreadsheet"></div> 
<script>
$('#Spreadsheet').ejSpreadsheet({
    sheets:[{
        cFormatRule: [{ action: ej.Spreadsheet.CFormatRule.LessThan, inputs: ["30"], color: ej.Spreadsheet.CFormatHighlightColor.RedFillwithDarkRedText, range: "A1:E1" }],
        rows:[
            {
                cells: [
                    { value: "20"},
				    { value: "30"},
				    { value: "15"},
				    { value: "40"},
				    { value: "50"}
                ]
            }
        ]
    }]
});    
</script>

{% endhighlight %}

### sheets.cFormatRule.action `enum`
{:#members:sheets-cformatrule-action}

<ts name="ej.Spreadsheet.CFormatRule"/>

Specifies the conditions to apply for the range of cells in Spreadsheet.

<table class="params">
<thead>
<tr>
<th>Name</th>
<th>Description</th>
</tr>
</thead>
<tbody>
<tr>
<td class="name">GreaterThan</td>
<td class="description">To identify greater than values in the given range of cells.</td>
</tr>
<tr>
<td class="name">LessThan</td>
<td class="description">To identify less than values in the given range of cells.</td>
</tr>
<tr>
<td class="name">Between</td>
<td class="description">To identify in between values in the given range of cells.</td>
</tr>
<tr>
<td class="name">EqualTo</td>
<td class="description">To identify the equal values in the given range of cells.</td>
</tr>
<tr>
<td class="name">TextContains</td>
<td class="description">To identify the specified text in the range of cells.</td>
</tr>
<tr>
<td class="name">DateOccurs</td>
<td class="description">To identify the specified date in the range of cells.</td>
</tr>
</tbody>
</table>

#### Example

{% highlight html %}
<div id="Spreadsheet"></div> 
<script>
$('#Spreadsheet').ejSpreadsheet({
    sheets:[{
        cFormatRule: [{ action: ej.Spreadsheet.CFormatRule.LessThan, inputs: ["30"], color: ej.Spreadsheet.CFormatHighlightColor.RedFillwithDarkRedText, range: "A1:E1" }],
        rows:[
            {
            cells: [
                    { value: "20"},
				    { value: "30"},
				    { value: "15"},
				    { value: "40"},
				    { value: "50"}
                ]
            }
        ]
    }]
});    
</script>

{% endhighlight %}

### sheets.cFormatRule.color `enum`
{:#members:sheets-cformatrule-color}

<ts name="ej.Spreadsheet.CFormatHighlightColor"/>

Specifies the color to apply for the range of cell while conditional formatting.

<table class="params">
<thead>
<tr>
<th>Name</th>
<th>Description</th>
</tr>
</thead>
<tbody>
<tr>
<td class="name">RedFillwithDarkRedText</td>
<td class="description">Highlights red with dark red text color.</td>
</tr>
<tr>
<td class="name">YellowFillwithDarkYellowText</td>
<td class="description">Highlights yellow with dark yellow text color.</td>
</tr>
<tr>
<td class="name">GreenFillwithDarkGreenText</td>
<td class="description">Highlights green with dark green text color.</td>
</tr>
<tr>
<td class="name">RedFill</td>
<td class="description">Highlights with red fill.</td>
</tr>
<tr>
<td class="name">RedText</td>
<td class="description">Highlights with red text.</td>
</tr>
</tbody>
</table>

#### Example

{% highlight html %}
<div id="Spreadsheet"></div> 
<script>
$('#Spreadsheet').ejSpreadsheet({
    sheets:[{
        cFormatRule: [{ action: ej.Spreadsheet.CFormatRule.LessThan, inputs: ["30"], color: ej.Spreadsheet.CFormatHighlightColor.RedFillwithDarkRedText, range: "A1:E1" }],
        rows:[
            {
            cells: [
                    { value: "20"},
				    { value: "30"},
				    { value: "15"},
				    { value: "40"},
				    { value: "50"}
                ]
            }
        ]
    }]
});    
</script>

{% endhighlight %}

### sheets.cFormatRule.inputs `Array`
{:#members:sheets-cformatrule-inputs}

Specifies the inputs for conditional formatting in Spreadsheet.

#### Default Value:

* []

#### Example

{% highlight html %}
<div id="Spreadsheet"></div> 
<script>
$('#Spreadsheet').ejSpreadsheet({
    sheets:[{
        cFormatRule: [{ action: ej.Spreadsheet.CFormatRule.LessThan, inputs: ["30"], color: ej.Spreadsheet.CFormatHighlightColor.RedFillwithDarkRedText, range: "A1:E1" }],
        rows:[
            {
                cells: [
                    { value: "20"},
				    { value: "30"},
				    { value: "15"},
				    { value: "40"},
				    { value: "50"}
                ]
            }
        ]
    }]
});    
</script>

{% endhighlight %}

### sheets.cFormatRule.range `string`
{:#members:sheets-cformatrule-range}

Specifies the range for conditional formatting in Spreadsheet.

#### Default Value:

* ""

#### Example

{% highlight html %}
<div id="Spreadsheet"></div> 
<script>
$('#Spreadsheet').ejSpreadsheet({
    sheets:[{
        cFormatRule: [{ action: ej.Spreadsheet.CFormatRule.LessThan, inputs: ["30"], color: ej.Spreadsheet.CFormatHighlightColor.RedFillwithDarkRedText, range: "A1:E1" }],
        rows:[
            {
            cells: [
                    { value: "20"},
				    { value: "30"},
				    { value: "15"},
				    { value: "40"},
				    { value: "50"}
                ]
            }
        ]
    }]
});    
</script>

{% endhighlight %}

### sheets.colCount `number`
{:#members:sheets-colcount}

Gets or sets a value that indicates to define column count in the Spreadsheet.

#### Default Value:

* 21

#### Example

{% highlight html %}
<div id="Spreadsheet"></div> 
<script>
$('#Spreadsheet').ejSpreadsheet({
    sheets:[{
        rangeSettings: [{dataSource: window.defaultData}],
        colCount: 25
    }]
});    
</script>

{% endhighlight %}

### sheets.columnWidth `number`
{:#members:sheets-columnwidth}

Gets or sets a value that indicates to define column width in the Spreadsheet.

#### Default Value:

* 64 

#### Example

{% highlight html %}
<div id="Spreadsheet"></div> 
<script>
$('#Spreadsheet').ejSpreadsheet({
    sheets:[{
            columnWidth: 100
        }]
});    
</script>

{% endhighlight %}

### sheets.dataSource `Object`
{:#members:sheets-datasource}

Gets or sets the data to render the Spreadsheet.

#### Default Value:

* null

#### Example

{% highlight html %}
<div id="Spreadsheet"></div>

<script>
$('#Spreadsheet').ejSpreadsheet({
    sheets:[{
        // the datasource "window.defaultData" is referred from 'http://js.syncfusion.com/demos/web/scripts/xljsondata.js'
        dataSource: window.defaultData
    }]
});    
</script>
{% endhighlight %}

### sheets.fieldAsColumnHeader `boolean`
{:#members:sheets-fieldascolumnheader}

Gets or sets a value that indicates whether to enable or disable field as column header in the Spreadsheet.

#### Default Value:

* false

#### Example

{% highlight html %}
<div id="Spreadsheet"></div> 
<script>
var dataManager = ej.DataManager("http://mvc.syncfusion.com/Services/Northwnd.svc/Orders/");
$('#Spreadsheet').ejSpreadsheet({
    sheets:[{
        dataSource: dataManager,
        query: ej.Query().take(50).select(["OrderID", "CustomerID", "EmployeeID", "ShipName", "ShipAddress", "ShipCity", "ShipCountry"]),
        fieldAsColumnHeader: true,
        primaryKey: "OrderID"
    }]
});    
</script>

{% endhighlight %}

### sheets.frozenRows `number`
{:#members:sheets-frozenrows}

Gets or sets a value to freeze rows in the Spreadsheet.

#### Default Value:

* 0

#### Example

{% highlight html %}
<div id="Spreadsheet"></div> 
<script>
$('#Spreadsheet').ejSpreadsheet({
    sheets:[{
            frozenRows: 3
        }]
});    
</script>

{% endhighlight %}

### sheets.frozenColumns `number`
{:#members:sheets-frozencolumns}

Gets or sets a value to freeze columns in the Spreadsheet.

#### Default Value:

* 0

#### Example

{% highlight html %}
<div id="Spreadsheet"></div> 
<script>
$('#Spreadsheet').ejSpreadsheet({
    sheets:[{
            frozenColumns: 3
        }]
});    
</script>

{% endhighlight %}

### sheets.headerStyles `Object`
{:#members:sheets-headerstyles}

Specifies the header styles for the headers in datasource range.

#### Default Value:

* null

#### Example

{% highlight html %}
<div id="Spreadsheet"></div> 
<script>
$('#Spreadsheet').ejSpreadsheet({
    sheets:[{
        dataSource: window.defaultData, showHeader: true, headerStyles: { "font-weight": "bold", "vertical-align": "middle", "text-align": "center", "background-color": "#559ad9", "color": "#FFFFFF" }}]
    });    
</script>

{% endhighlight %}

### sheets.hideColumns `Array`
{:#members:sheets-hidecolumns}

To hide the specified columns in Spreadsheet.

#### Default Value:

* []

#### Example

{% highlight html %}
<div id="Spreadsheet"></div> 
<script>
$('#Spreadsheet').ejSpreadsheet({
    sheets:[{
        hideColumns: [3, 4]
    }]
});    
</script>

{% endhighlight %}

### sheets.hideRows `Array`
{:#members:sheets-hiderows}

To hide the specified rows in Spreadsheet.

#### Default Value:

* []

#### Example

{% highlight html %}
<div id="Spreadsheet"></div> 
<script>
$('#Spreadsheet').ejSpreadsheet({
    sheets:[{
        hideRows: [2, 3]
    }]
});    
</script>

{% endhighlight %}

### sheets.mergeCells `Array`
{:#members:sheets-mergecells}

To merge specified ranges in Spreadsheet.

#### Default Value:

* []

#### Example

{% highlight html %}
<div id="Spreadsheet"></div> 
<script>
$('#Spreadsheet').ejSpreadsheet({
    sheets:[{
        mergeCells:["A1:A2","B2:C2"]
    }]
});    
</script>

{% endhighlight %}

### sheets.primaryKey `string`
{:#members:sheets-primarykey}

Specifies the primary key for the datasource in Spreadsheet.

#### Default Value:

* ""

#### Example

{% highlight html %}
<div id="Spreadsheet"></div> 
<script>
var dataManager = ej.DataManager("http://mvc.syncfusion.com/Services/Northwnd.svc/Orders/");
$('#Spreadsheet').ejSpreadsheet({
    sheets:[{
        dataSource: dataManager,
        query: ej.Query().take(50).select(["OrderID", "CustomerID", "EmployeeID", "ShipName", "ShipAddress", "ShipCity", "ShipCountry"]),
        primaryKey: "OrderID"
    }]
});    
</script>

{% endhighlight %}

### sheets.query `Object`
{:#members:sheets-query}

Specifies the query for the [`dataSource`](https://help.syncfusion.com/api/js/ejspreadsheet#members:sheets-datasource "dataSource") in Spreadsheet.

#### Default Value:

* null

#### Example

{% highlight html %}
<div id="Spreadsheet"></div> 

<script>
var dataManager = ej.DataManager("http://mvc.syncfusion.com/Services/Northwnd.svc/Orders/");
$('#Spreadsheet').ejSpreadsheet({
    sheets:[{
        dataSource: dataManager,
        query: ej.Query().take(50).select(["OrderID", "CustomerID", "EmployeeID", "ShipName", "ShipAddress", "ShipCity", "ShipCountry"]),
        primaryKey: "OrderID"
    }]
});    
</script>
{% endhighlight %}

### sheets.rangeSettings `Array`
{:#members:sheets-rangesettings}

Specifies single range or multiple range settings for a sheet in Spreadsheet.

#### Default Value:

* []

#### Example

{% highlight html %}
<div id="Spreadsheet"></div> 
<script>
$('#Spreadsheet').ejSpreadsheet({
    sheets:[{
        {rangeSettings: [{dataSource: window.defaultData, showHeader: true, startCell: "A1"}]},
        {rangeSettings: [{dataSource: window.personList, showHeader: true, startCell: "D1"}]}
    }]
});    
</script>

{% endhighlight %}

### sheets.rangeSettings.dataSource `Object`
{:#members:sheets-rangesettings-datasource}

Gets or sets the data to render the Spreadsheet.

#### Default Value:

* null

#### Example

{% highlight html %}
<div id="Spreadsheet"></div> 
<script>
$('#Spreadsheet').ejSpreadsheet({
    sheets:[{
        rangeSettings: [{dataSource: window.defaultData, showHeader: true}]}]
    });    
</script>

{% endhighlight %}

### sheets.rangeSettings.headerStyles `Object`
{:#members:sheets-rangesettings-headerstyles}

Specifies the header styles for the headers in datasource range.

#### Default Value:

* null

#### Example

{% highlight html %}
<div id="Spreadsheet"></div> 
<script>
$('#Spreadsheet').ejSpreadsheet({
    sheets:[{
        rangeSettings: [{dataSource: window.defaultData, showHeader: true, headerStyles: { "font-weight": "bold", "vertical-align": "middle", "text-align": "center", "background-color": "#559ad9", "color": "#FFFFFF" }}]
        }]
});    
</script>

{% endhighlight %}

### sheets.rangeSettings.primaryKey `string`
{:#members:sheets-rangesettings-primarykey}

Specifies the primary key for the datasource in Spreadsheet.

#### Default Value:

* ""

#### Example

{% highlight html %}
<div id="Spreadsheet"></div> 
<script>
var dataManager = ej.DataManager("http://mvc.syncfusion.com/Services/Northwnd.svc/Orders/");
$('#Spreadsheet').ejSpreadsheet({
    sheets:[{
        rangeSettings:[{
            dataSource: dataManager,
            query: ej.Query().take(50).select(["OrderID", "CustomerID", "EmployeeID", "ShipName", "ShipAddress", "ShipCity", "ShipCountry"]),
            primaryKey: "OrderID"
        }]
    }]
});    
</script>

{% endhighlight %}

### sheets.rangeSettings.query `Object`
{:#members:sheets-rangesettings-query}

Specifies the query for the datasource in Spreadsheet.

#### Default Value:

* null

#### Example

{% highlight html %}
<div id="Spreadsheet"></div> 
<script>
var dataManager = ej.DataManager("http://mvc.syncfusion.com/Services/Northwnd.svc/Orders/");
$('#Spreadsheet').ejSpreadsheet({
    sheets:[{
        rangeSettings:[{
	        dataSource: dataManager,
            query: ej.Query().take(50).select(["OrderID", "CustomerID", "EmployeeID", "ShipName", "ShipAddress", "ShipCity", "ShipCountry"]),
            primaryKey: "OrderID"
            }]
        }]
});    
</script>

{% endhighlight %}

### sheets.rangeSettings.showHeader `boolean`
{:#members:sheets-rangesettings-showheader}

Gets or sets a value that indicates whether to enable or disable the datasource header in Spreadsheet.

#### Default Value:

* true

#### Example

{% highlight html %}
<div id="Spreadsheet"></div> 
<script>
$('#Spreadsheet').ejSpreadsheet({
    sheets:[{
        rangeSettings: [{dataSource: window.defaultData, showHeader: true}]
        }]
});    
</script>

{% endhighlight %}

### sheets.rangeSettings.startCell `string`
{:#members:sheets-rangesettings-startcell}

Specifies the start cell for the datasource range in Spreadsheet.

#### Default Value:

* "A1"

#### Example

{% highlight html %}
<div id="Spreadsheet"></div> 
<script>
$('#Spreadsheet').ejSpreadsheet({
    sheets: [{
        rangeSettings: [{ dataSource: window.defaultData, startCell: "B1" }]
}]
});    
</script>

{% endhighlight %}

### sheets.rowCount `number`
{:#members:sheets-rowcount}

Gets or sets a value that indicates to define row count in the Spreadsheet.

#### Default Value:

* 20

#### Example

{% highlight html %}
<div id="Spreadsheet"></div> 
<script>
$('#Spreadsheet').ejSpreadsheet({
    sheets:[{
        rangeSettings: [{dataSource: window.defaultData}],
        rowCount: 30
    }]
});    
</script>

{% endhighlight %}

### sheets.rows `Array`
{:#members:sheets-rows}

Specifies the rows for a sheet in Spreadsheet.

#### Default Value:

* []

#### Example

{% highlight html %}
<div id="Spreadsheet"></div> 
<script>
$('#Spreadsheet').ejSpreadsheet({
    sheets:[{
        rows:[
            {
                height:30,
                cells:[
                     { value: "Item Name", style: { "font-weight": "bold", "color": "#FFFFFF", "background-color": "#428bca" }},
                     { value: "Quantity", style: { "font-weight": "bold", "color": "#FFFFFF", "background-color": "#428bca" }},
                ]
            }
        ]
    }],
});    
</script>

{% endhighlight %}

### sheets.rows.height `number`
{:#members:sheets-rows-height}

Gets or sets the height of a row in Spreadsheet.

#### Default Value:

* 20

#### Example

{% highlight html %}
<div id="Spreadsheet"></div> 
<script>
$('#Spreadsheet').ejSpreadsheet({
    sheets:[{
        rows:[
            {
                height:30,
			    cells: [
                            { value: "Item Name", style: { "font-weight": "bold", "color": "#FFFFFF", "background-color": "#428bca" }},
                            { value: "Quantity", style: { "font-weight": "bold", "color": "#FFFFFF", "background-color": "#428bca" } },
			    ]
            }
        ]
    }],    
});
</script>

{% endhighlight %}

### sheets.rows.cells `Array`
{:#members:sheets-rows-cells}

Specifies the cells of a row in Spreadsheet.

#### Default Value:

* []

#### Example

{% highlight html %}
<div id="Spreadsheet"></div> 
<script>
$('#Spreadsheet').ejSpreadsheet({
sheets: [{
    rows: [
        {
            cells: [
                { value: "Item Name", style: { "font-weight": "bold", "color": "#FFFFFF", "background-color": "#428bca" } },
                { value: "Quantity", style: { "font-weight": "bold", "color": "#FFFFFF", "background-color": "#428bca" } }
            ]
        }
    ]
}]   
});
</script>

{% endhighlight %}

### sheets.rows.cells.comment `Object`
{:#members:sheets-rows-cells-comment}

Specifies the comment for a cell in Spreadsheet.

#### Default Value:

* null

#### Example

{% highlight html %}
<div id="Spreadsheet"></div> 
<script>
$('#Spreadsheet').ejSpreadsheet({
    sheets: [{
    rows: [
        {
            cells: [
                { value: "Item Name", comment: { value: "Name of the item" } }
            ]
        }
    ]
}]    
});
</script>

{% endhighlight %}

### sheets.rows.cells.comment.isVisible `boolean`
{:#members:sheets-rows-cells-comment-isvisible}

Get or sets the value that indicates whether to show or hide comments in Spreadsheet.

#### Default Value:

* false

#### Example

{% highlight html %}
<div id="Spreadsheet"></div> 
<script>
$('#Spreadsheet').ejSpreadsheet({
    sheets:[{
        rows:[
            {
                cells: [
                    { value: "Item Name",comment: { value: "Name of the item" , isVisible:true}}
                ]
            }
        ]
    }]    
});
</script>

{% endhighlight %}

### sheets.rows.cells.comment.value `string`
{:#members:sheets-rows-cells-comment-value}

Specifies the value for the comment in Spreadsheet.

#### Default Value:

* "" 

#### Example

{% highlight html %}
<div id="Spreadsheet"></div> 
<script>
$('#Spreadsheet').ejSpreadsheet({
    sheets:[{
        rows:[
            {
                cells: [
                    { value: "Item Name",comment: { value: "Name of the item" , isVisible:true}}
                ]
            }
        ]
    }]    
});
</script>

{% endhighlight %}

### sheets.rows.cells.format `Object`
{:#members:sheets-rows-cells-format}

Specifies the format of a cell in Spreadsheet.

#### Default Value:
* null

#### Example

{% highlight html %}
<div id="Spreadsheet"></div> 
<script>
$('#Spreadsheet').ejSpreadsheet({
    sheets:[{
        rows:[
            {
                cells: [
                    { value: "20", format: { type: "currency" } }
                ]
            }
        ]
    }]    
});
</script>

{% endhighlight %}

### sheets.rows.cells.format.decimalPlaces `number`
{:#members:sheets-rows-cells-format-decimalplaces}

Specifies the number of decimal places for the given input.

#### Default Value:
* 2

#### Example

{% highlight html %}

<div id="Spreadsheet"></div> 
<script>
$('#Spreadsheet').ejSpreadsheet({
    sheets: [{
        rows: [
            { cells: [{ value: "200", format: { type: "currency", decimalPlaces: 3 } }] }
        ]
    }]
});
</script>

{% endhighlight %}

### sheets.rows.cells.format.formatStr `string`
{:#members:sheets-rows-cells-format-formatstr}

Specifies the string format for the given input.

#### Default Value:
* ""

#### Example

{% highlight html %}

<div id="Spreadsheet"></div> 
<script>
$('#Spreadsheet').ejSpreadsheet({
    sheets: [{
        rows: [
            { cells: [{ value: "20000", format: { type: "percentage", formatStr: "{0:P3}" } }] }
        ]
    }]
});
</script>

{% endhighlight %}

### sheets.rows.cells.format.thousandSeparator `boolean`
{:#members:sheets-rows-cells-format-thousandseparator}

Specifies the thousand separator for the given input.

#### Default Value:
* false

#### Example

{% highlight html %}

<div id="Spreadsheet"></div> 
<script>
$('#Spreadsheet').ejSpreadsheet({
    sheets: [{
        rows: [
            { cells: [{ value: "200000", format: { type: "number", thousandSeparator: true } }] }
        ]
    }]
});
</script>

{% endhighlight %}

### sheets.rows.cells.format.type `string`
{:#members:sheets-rows-cells-format-type}

Specifies the type of the format in Spreadsheet.

#### Default Value:
* ""

#### Example

{% highlight html %}
<div id="Spreadsheet"></div> 
<script>
$('#Spreadsheet').ejSpreadsheet({
    sheets:[{
        rows:[
            {
                cells: [
                    { value: "20", format: { type: "currency" } }
                ]
            }
        ]
    }]    
});
</script>

{% endhighlight %}

### sheets.rows.cells.hyperlink `Object`
{:#members:sheets-rows-cells-hyperlink}

Specifies the hyperlink for a cell in Spreadsheet.

#### Default Value:
* null

#### Example

{% highlight html %}
<div id="Spreadsheet"></div> 
<script>
$('#Spreadsheet').ejSpreadsheet({
    sheets:[{
        rows:[
            {
                cells: [
                    { value: "AliExpress", hyperlink: { webAddr: "www.aliexpress.com" } }
                ]
            }
        ]
    }]    
});
</script>

{% endhighlight %}

### sheets.rows.cells.hyperlink.webAddr `string`
{:#members:sheets-rows-cells-hyperlink-webaddr}

Specifies the web address for the hyperlink of a cell.

#### Default Value:
* ""

#### Example

{% highlight html %}
<div id="Spreadsheet"></div> 
<script>
$('#Spreadsheet').ejSpreadsheet({
    sheets:[{
        rows:[
            {
                cells: [
                    { value: "AliExpress", hyperlink: { webAddr: "www.aliexpress.com" } }
                ]
            }
        ]
    }]    
});
</script>

{% endhighlight %}

### sheets.rows.cells.hyperlink.cellAddr `string`
{:#members:sheets-rows-cells-hyperlink-celladdr}

Specifies the cell address for the hyperlink of a cell.

#### Default Value:
* ""

#### Example

{% highlight html %}
<div id="Spreadsheet"></div> 
<script>
$('#Spreadsheet').ejSpreadsheet({
    sheets:[{
        rows:[
            {
                cells: [
                    { value: "AliExpress", hyperlink: { cellAddr: "B2" } }
                ]
            }
        ]
    }]    
});
</script>

{% endhighlight %}

### sheets.rows.cells.hyperlink.sheetIndex `number`
{:#members:sheets-rows-cells-hyperlink-sheetindex}

Specifies the sheet index to which the cell is referred.

N> User must give `cellAddr` to use this property.

#### Default Value:
* 1

#### Example

{% highlight html %}
<div id="Spreadsheet"></div> 
<script>
$('#Spreadsheet').ejSpreadsheet({
    sheets:[{
        rows:[
            {
                cells: [
                    { value: "AliExpress", hyperlink: { cellAddr: "B2" , sheetIndex: 2} }
                ]
            }
        ]
    }]    
});
</script>

{% endhighlight %}

### sheets.rows.cells.index `number`
{:#members:sheets-rows-cells-index}

Specifies the index of a cell in Spreadsheet.

#### Default Value:

* 0

#### Example

{% highlight html %}
<div id="Spreadsheet"></div> 
<script>
$('#Spreadsheet').ejSpreadsheet({
    sheets:[{
        rows:[
            {
                cells: [
                    { index: 1, value: "Item Name", style: { "font-weight": "bold", "color": "#FFFFFF", "background-color": "#428bca" }},
                    { value: "Quantity", style: { "font-weight": "bold", "color": "#FFFFFF", "background-color": "#428bca" }}
                ]
            }
        ]
    }]    
});
</script>

{% endhighlight %}

### sheets.rows.cells.isLocked `boolean`
{:#members:sheets-rows-cells-islocked}

Specifies whether to lock or unlock a particular cell.

#### Default Value:

* false

#### Example

{% highlight html %}
<div id="Spreadsheet"></div> 
<script>
$('#Spreadsheet').ejSpreadsheet({
    sheets: [{
        rows: [{
            cells: [{ value: "Item Name", isLocked: true }]
        }]
    }]
});
</script>

{% endhighlight %}

### sheets.rows.cells.style `Object`
{:#members:sheets-rows-cells-style}

Specifies the styles of a cell in Spreadsheet.

#### Default Value:
* null

#### Example

{% highlight html %}
<div id="Spreadsheet"></div> 
<script>
$('#Spreadsheet').ejSpreadsheet({
    sheets:[{
        rows:[
            {
                cells: [
                    { value: "Item Name",style: { "font-weight": "bold", "color": "#FFFFFF", "background-color": "#428bca" }},
                    { value: "Quantity",style: { "font-weight": "bold", "color": "#FFFFFF", "background-color": "#428bca" }}
                ]
            }
        ]
    }]    
});
</script>

{% endhighlight %}

### sheets.rows.cells.style.backgroundColor `string`
{:#members:sheets-rows-cells-style-backgroundcolor}

Specifies the background color of a cell in the Spreadsheet.

#### Default Value:
* ""

#### Example

{% highlight html %}
<div id="Spreadsheet"></div> 
<script>
$('#Spreadsheet').ejSpreadsheet({
    sheets: [{
        rows: [
            {
                cells: [
                    { value: "Item Name", style: { "background-color": "#428bca" } }
                ]
            }
        ]
    }]
});
</script>

{% endhighlight %}

### sheets.rows.cells.style.color `string`
{:#members:sheets-rows-cells-style-color}

Specifies the font color of a cell in the Spreadsheet.

#### Default Value:
* ""

#### Example

{% highlight html %}
<div id="Spreadsheet"></div> 
<script>
$('#Spreadsheet').ejSpreadsheet({
    sheets: [{
        rows: [
            {
                cells: [
                    { value: "Item Name", style: { "color": "#428bca" } }
                ]
            }
        ]
    }]
});
</script>

{% endhighlight %}

### sheets.rows.cells.style.fontWeight `string`
{:#members:sheets-rows-cells-style-fontweight}

Specifies the font weight of a cell in the Spreadsheet.

#### Default Value:
* ""

#### Example

{% highlight html %}
<div id="Spreadsheet"></div> 
<script>
$('#Spreadsheet').ejSpreadsheet({
    sheets: [{
        rows: [
            {
                cells: [
                    { value: "Item Name", style: { "font-weight": "bold" } }
                ]
            }
        ]
    }]
});
</script>

{% endhighlight %}

### sheets.rows.cells.value `string`
{:#members:sheets-rows-cells-value}

Specifies the value for a cell in Spreadsheet.

#### Default Value:

* ""

#### Example

{% highlight html %}
<div id="Spreadsheet"></div> 
<script>
$('#Spreadsheet').ejSpreadsheet({
    sheets:[{
        rows:[
            {
                cells: [
                    { value: "Item Name"},
                    { value: "Quantity"}
                ]
            }
        ]
    }]    
});
</script>

{% endhighlight %}

### sheets.rows.index `number`
{:#members:sheets-rows-index}

Gets or sets the index of a row in Spreadsheet.

#### Default Value:

* 0

#### Example

{% highlight html %}
<div id="Spreadsheet"></div> 
<script>
$('#Spreadsheet').ejSpreadsheet({
    sheets:[{
        rows:[
            {   
                index:1,
                height:30,
			    cells: [
                            { value: "Item Name", style: { "font-weight": "bold", "color": "#FFFFFF", "background-color": "#428bca" }},
                            { value: "Quantity", style: { "font-weight": "bold", "color": "#FFFFFF", "background-color": "#428bca" }},
			    ]
            }
        ]
    }],    
});
</script>

{% endhighlight %}

### sheets.showGridlines `boolean`
{:#members:sheets-showgridlines}

Gets or sets a value that indicates whether to show or hide grid lines in the Spreadsheet.

#### Default Value
* true

#### Example

{% highlight html %}
<div id="Spreadsheet"></div> 
<script>
$('#Spreadsheet').ejSpreadsheet({
	sheets:[{
		showGridlines: true
	}]
});   
</script>

{% endhighlight %}


### sheets.showHeader `boolean`
{:#members:sheets-showheader}

Gets or sets a value that indicates whether to enable or disable the datasource header in Spreadsheet.

#### Default Value:

* true

#### Example

{% highlight html %}
<div id="Spreadsheet"></div> 
<script>
$('#Spreadsheet').ejSpreadsheet({
    sheets:[{
        dataSource: window.defaultData, showHeader: true
        }]
});    
</script>

{% endhighlight %}

### sheets.showHeadings `boolean`
{:#members:sheets-showheadings}

Gets or sets a value that indicates whether to show or hide headings in the Spreadsheet.

#### Default Value
* true

#### Example

{% highlight html %}
<div id="Spreadsheet"></div> 
<script>
$('#Spreadsheet').ejSpreadsheet({
	sheets:[{
		showHeadings: true
	}]
});   
</script>

{% endhighlight %}


### sheets.sheetName `string`
{:#members:sheets-sheetname}

Specifies the name for sheet in the Spreadsheet.

#### Default Value
* string

#### Example

{% highlight html %}
<div id="Spreadsheet"></div> 
<script>
$('#Spreadsheet').ejSpreadsheet({
	sheets:[{
		sheetName: "Sheet Name"
	}]
});   
</script>

{% endhighlight %}

### sheets.startCell `string`
{:#members:sheets-startcell}

Specifies the start cell for the datasource range in Spreadsheet.

#### Default Value:

* "A1"

#### Example

{% highlight html %}
<div id="Spreadsheet"></div> 
<script>
$('#Spreadsheet').ejSpreadsheet({
    sheets:[{
        dataSource: window.defaultData, startCell: "B1"
        }]
});    
</script>

{% endhighlight %}

### showPager `boolean`
{:#members:showpager}

Gets or sets a value that indicates whether to show or hide pager in the Spreadsheet.

#### Default Value
* true

#### Example

{% highlight html %}
<div id="Spreadsheet"></div> 
<script>
$('#Spreadsheet').ejSpreadsheet({ 
    showPager: true
});         
</script>

{% endhighlight %}

### showRibbon `boolean`
{:#members:showribbon}

Gets or sets a value that indicates whether to show or hide ribbon in the Spreadsheet.

#### Default Value
* true

#### Example

{% highlight html %}
<div id="Spreadsheet"></div> 
<script>
$('#Spreadsheet').ejSpreadsheet({ 
    showRibbon: true
});         
</script>

{% endhighlight %}

### undoRedoStep `number`
{:#members:undoredostep}

This is used to set the number of undo-redo steps in the Spreadsheet.

#### Default Value
* 20

#### Example

{% highlight html %}
<div id="Spreadsheet"></div>
<script>
$('#Spreadsheet').ejSpreadsheet({ 
    undoRedoStep: 15
});         
</script>

{% endhighlight %}

### userName `string`
{:#members:username}

Define the username for the Spreadsheet which is displayed in comment.

#### Default Value
* User Name

#### Example

{% highlight html %}
<div id="Spreadsheet"></div>
<script>
$('#Spreadsheet').ejSpreadsheet({ 
    userName: "User Name"
});         
</script>

{% endhighlight %}

## Methods

### addCustomFormula(formulaName, functionName)
{:#methods:addcustomformula}

This method is used to add custom formulas in Spreadsheet.
<table class="params">
<thead>
<tr>
<th>Name</th>
<th>Type</th>
<th>Description</th>
</tr>
</thead>
<tbody>
<tr>
<td class="name">formulaName</td>
<td class="type"><span class="param-type">string</span></td>
<td class="description">Pass the name of the formula.</td>
</tr>
<tr>
<td class="name">functionName</td>
<td class="type"><span class="param-type">string</span></td>
<td class="description">Pass the name of the function.</td>
</tr>
</tbody>
</table>

#### Example

{% highlight html %}
<script>
// Initialize the Spreadsheet object.
var excelObj = $("#Spreadsheet").data("ejSpreadsheet");
excelObj.addCustomFormula("CUSTOMTOTAL","customTotal"); // Sends a add custom formula request to the Spreadsheet.
function customTotal(args){}//args-It uses the value given by the user while using custom formula in Spreadsheet.
</script>

{% endhighlight %}

{% highlight html %}
<script>
// Sends a add custom formula request to the Spreadsheet.
$("#Spreadsheet").ejSpreadsheet("addCustomFormula","CUSTOMTOTAL","customTotal" );     
function customTotal(args){}//args-It uses the value given by the user while using custom formula in Spreadsheet.  
</script>

{% endhighlight %}

### addNewSheet()
{:#methods:addnewsheet}

This method is used to add a new sheet in the last position of the sheet container.

#### Example

{% highlight html %}
<script>
// Initialize the Spreadsheet object.
var excelObj = $("#Spreadsheet").data("ejSpreadsheet");
excelObj.addNewSheet(); // Sends a add new sheet request to the Spreadsheet.
</script>

{% endhighlight %}

{% highlight html %}
<script>
// Sends a add new sheet request to the Spreadsheet
$("#Spreadsheet").ejSpreadsheet("addNewSheet");        
</script>

{% endhighlight %}

### blankWorkbook()
{:#methods:blankworkbook}

This method is used to blank the workbook in Spreadsheet.

#### Example

{% highlight html %}
<script>
//initialize the Spreadsheet object
var excelObj = $("#Spreadsheet").data("ejSpreadsheet");
//To blank the workbook in Spreadsheet
excelObj.blankWorkbook();
</script>

{% endhighlight %}

### clearAll(\[range\])
{:#methods:clearall}

It is used to clear all the data and format in the specified range of cells in Spreadsheet.
<table class="params">
<thead>
<tr>
<th>Name</th>
<th>Type</th>
<th>Description</th>
</tr>
</thead>
<tbody>
<tr>
<td class="name">range</td>
<td class="type"><span class="param-type">string|Array</span></td>
<td class="description"><span class="optional">Optional.</span> If range is specified, then it will clear all content in the specified range else it will use the current selected range. </td>
</tr>
</tbody>
</table>

#### Example

{% highlight html %}
<script>
// Initialize the Spreadsheet object.
var excelObj = $("#Spreadsheet").data("ejSpreadsheet");
excelObj.clearAll("A2:A6"); // Sends a clear all request to the Spreadsheet.
</script>
{% endhighlight %}

{% highlight html %}
<script>
// Sends a clear all request to the Spreadsheet.
$("#Spreadsheet").ejSpreadsheet("clearAll", "A2:A6");        
</script>

{% endhighlight %}


### clearAllFormat(\[range\])
{:#methods:clearallformat}

This property is used to clear all the formats applied in the specified range in Spreadsheet.
<table class="params">
<thead>
<tr>
<th>Name</th>
<th>Type</th>
<th>Description</th>
</tr>
</thead>
<tbody>
<tr>
<td class="name">range</td>
<td class="type"><span class="param-type">string|Array</span></td>
<td class="description"><span class="optional">Optional.</span> If range is specified, then it will clear all format in the specified range else it will use the current selected range. </td>
</tr>
</tbody>
</table>

#### Example

{% highlight html %}
<script>
// Initialize the Spreadsheet object.
var excelObj = $("#Spreadsheet").data("ejSpreadsheet");
excelObj.clearAllFormat("A2:A6"); // Sends a clear all format request to the Spreadsheet.
</script>
{% endhighlight %}

{% highlight html %}
<script>
// Sends a clear all format request to the Spreadsheet
$("#Spreadsheet").ejSpreadsheet("clearAllFormat", "A2:A6");        
</script>

{% endhighlight %}

### clearBorder(\[range\])
{:#methods:clearborder}

Used to clear the applied border in the specified range in Spreadsheet.
<table class="params">
<thead>
<tr>
<th>Name</th>
<th>Type</th>
<th>Description</th>
</tr>
</thead>
<tbody>
<tr>
<td class="name">range</td>
<td class="type"><span class="param-type">string|Array</span></td>
<td class="description"><span class="optional">Optional.</span> If range is specified, then it will clear border in the specified range else it will use the current selected range.</td>
</tr>
</tbody>
</table>

#### Example

{% highlight html %}
<script>
// Initialize the Spreadsheet object.
var excelObj = $("#Spreadsheet").data("ejSpreadsheet");
excelObj.clearBorder("A2:A6"); // Sends a clear border request to the Spreadsheet.
</script>
{% endhighlight %}

{% highlight html %}
<script>
// Sends a clear border request to the Spreadsheet.
$("#Spreadsheet").ejSpreadsheet("clearBorder", "A2:A6");        
</script>

{% endhighlight %}

### clearContents(\[range\])
{:#methods:clearcontents}

This property is used to clear the contents in the specified range in Spreadsheet.
<table class="params">
<thead>
<tr>
<th>Name</th>
<th>Type</th>
<th>Description</th>
</tr>
</thead>
<tbody>
<tr>
<td class="name">range</td>
<td class="type"><span class="param-type">string|Array</span></td>
<td class="description"><span class="optional">Optional.</span> If the range is specified, then it will clear the content in the specified <br/>range else it will use the current selected range. </td>
</tr>
</tbody>
</table>

#### Example

{% highlight html %}
<script>
// Create Spreadsheet object.
var excelObj = $("#Spreadsheet").data("ejSpreadsheet");
excelObj.clearContents("A2:A6"); // Sends a clear content request to the Spreadsheet.
</script>

{% endhighlight %}

{% highlight html %}
<script>
// Sends a clear content request to the Spreadsheet
$("#Spreadsheet").ejSpreadsheet("clearContents", "A2:A6");        
</script>

{% endhighlight %}

### clearRange(rangeName)
{:#methods:clearrange}

This method is used to remove only the data in the range denoted by the specified range name.
<table class="params">
<thead>
<tr>
<th>Name</th>
<th>Type</th>
<th>Description</th>
</tr>
</thead>
<tbody>
<tr>
<td class="name">rangeName</td>
<td class="type"><span class="param-type">string</span></td>
<td class="description">Pass the defined rangeSettings property name.</td>
</tr>
</tbody>
</table>

#### Example

{% highlight html %}
<script>
// Initialize the Spreadsheet object.
var excelObj = $("#Spreadsheet").data("ejSpreadsheet");
excelObj.clearRange("updateTable"); // Sends a clear range request to the Spreadsheet.
</script>

{% endhighlight %}

{% highlight html %}
<div id="Spreadsheet"></div> 
<script>
// Sends a clear range request to the Spreadsheet.
$("#Spreadsheet").ejSpreadsheet("clearRange","updateTable");        
</script>

{% endhighlight %}

### clearRangeData(\[range\], \[property\],\[cells\],\[skipHiddenRow\],\[status\],\[skipCell\])
{:#methods:clearrangedata}

It is used to remove data in the specified range of cells based on the defined property.

<table class="params">
<thead>
<tr>
<th>Name</th>
<th>Type</th>
<th>Description</th>
</tr>
</thead>
<tbody>
<tr>
<td class="name">range</td>
<td class="type"><span class="param-type">Array|string</span></td>
<td class="description"><span class="optional">Optional.</span> If range is specified, it will clear data for the specified range else it will use the current selected range. </td>
</tr>
<tr>
<td class="name">property</td>
<td class="type"><span class="param-type">string</span></td>
<td class="description"><span class="optional">Optional.</span> If property is specified, it will remove the specified property in the range else it will remove default properties </td>
</tr>
<tr>
<td class="name">cells</td>
<td class="type"><span class="param-type">element</span></td>
<td class="description"><span class="optional">Optional.</span>
</td></tr>
<tr>
<td class="name">skipHiddenRow</td>
<td class="type"><span class="param-type">boolean</span></td>
<td class="description"><span class="optional">Optional.</span> pass {{'`true`' | markdownify}}, if you want to skip the hidden rows </td>
</tr>
<tr>
<td class="name">status</td>
<td class="type"><span class="param-type">string</span></td>
<td class="description"><span class="optional">Optional.</span> Pass the status to perform undo and redo operation.</td>
</tr>
<tr>
<td class="name">skipCell</td>
<td class="type"><span class="param-type">boolean</span></td>
<td class="description"><span class="optional">Optional.</span> It specifies whether to skip element processing or not.</td>
</tr>
</tbody>
</table>

#### Example

{% highlight html %}
<script>
// Initialize the Spreadsheet object.
var excelObj = $("#Spreadsheet").data("ejSpreadsheet");
excelObj.clearRangeData("A1:A5", ["value", "value2"], excelObj.getRange("A1:A5"), true);
</script>

{% endhighlight %}

{% highlight html %}
<script>
var excelObj = $("#Spreadsheet").data("ejSpreadsheet");
// Sends a clear range data request to the Spreadsheet.
$("#Spreadsheet").ejSpreadsheet("clearRangeData", "A1:A5", ["value", "value2"], excelObj.getRange("A1:A5"), false);        
</script>

{% endhighlight %}

### clearUndoRedo()
{:#methods:clearundoredo}

This method is used to clear undo and redo collections in the Spreadsheet.

#### Example

{% highlight html %}
<div id="Spreadsheet"></div>
<script>
// Initialize the Spreadsheet object.
var excelObj = $("#Spreadsheet").data("ejSpreadsheet");
excelObj.clearUndoRedo(); 
</script>

{% endhighlight %}

{% highlight html %}
<script>
// Sends a clear undo redo request to the Spreadsheet.
$("#Spreadsheet").ejSpreadsheet("clearUndoRedo");        
</script>

{% endhighlight %}

### copySheet(fromIdx, toIdx, isCopySheet)
{:#methods:copysheet}

This method is used to copy or move the sheets in Spreadsheet.
<table class="params">
<thead>
<tr>
<th>Name</th>
<th>Type</th>
<th>Description</th>
</tr>
</thead>
<tbody>
<tr>
<td class="name">fromIdx</td>
<td class="type"><span class="param-type">number</span></td>
<td class="description">Pass the sheet index that you want to copy or move.</td>
</tr>
<tr>
<td class="name">toIdx</td>
<td class="type"><span class="param-type">number</span></td>
<td class="description">Pass the position index where you want to copy or move.</td>
</tr>
<tr>
<td class="name">isCopySheet</td>
<td class="type"><span class="param-type">boolean</span></td>
<td class="description">Pass {{'`true`' | markdownify}},If you want to copy sheet or else it will move sheet.</td>
</tr>
</tbody>
</table>

#### Example

{% highlight html %}
<script>
// Initialize the Spreadsheet object.
var excelObj = $("#Spreadsheet").data("ejSpreadsheet");
excelObj.copySheet(2, 1, true); // Sends a copy sheet request to the Spreadsheet.
//excelObj.copySheet(2, 1, false); // Sends a move sheet request to the Spreadsheet.
</script>

{% endhighlight %}

{% highlight html %}
<script>
// Sends a copy sheet request to the Spreadsheet.
$("#Spreadsheet").ejSpreadsheet("copySheet", 2, 1, true);        
</script>

{% endhighlight %}


### deleteEntireColumn(startCol, endCol)
{:#methods:deleteentirecolumn}

This method is used to delete the entire column which is selected.

<table class="params">
<thead>
<tr>
<th>Name</th>
<th>Type</th>
<th>Description</th>
</tr>
</thead>
<tbody>
<tr>
<td class="name">startCol</td>
<td class="type"><span class="param-type">number</span></td>
<td class="description">Pass the start column index.</td>
</tr>
<tr>
<td class="name">endCol</td>
<td class="type"><span class="param-type">number</span></td>
<td class="description">Pass the end column index.</td>
</tr>
</tbody>
</table>

#### Example

{% highlight html %}
<script>
// Initialize the Spreadsheet object.
var excelObj = $("#Spreadsheet").data("ejSpreadsheet");
// Delete a column in the sheet.
excelObj.deleteEntireColumn(2, 3);
</script>

{% endhighlight %}

{% highlight html %}
<script>
// Delete a column in the sheet.
$("#Spreadsheet").ejSpreadsheet("deleteEntireColumn",2,3);
</script> 

{% endhighlight %}

### deleteEntireRow(startRow, endRow)
{:#methods:deleteentirerow}

This method is used to delete the entire row which is selected.

<table class="params">
<thead>
<tr>
<th>Name</th>
<th>Type</th>
<th>Description</th>
</tr>
</thead>
<tbody>
<tr>
<td class="name">startRow</td>
<td class="type"><span class="param-type">number</span></td>
<td class="description">Pass the start row index.</td>
</tr>
<tr>
<td class="name">endRow</td>
<td class="type"><span class="param-type">number</span></td>
<td class="description">Pass the end row index.</td>
</tr>
</tbody>
</table>

#### Example

{% highlight html %}
<script>
// Initialize the Spreadsheet object.
var excelObj = $("#Spreadsheet").data("ejSpreadsheet");
// Delete a row in the sheet.
excelObj.deleteEntireRow(2,3);
</script>

{% endhighlight %}

{% highlight html %}
<script>
// Delete a row in the sheet.
$("#Spreadsheet").ejSpreadsheet("deleteEntireRow", 2, 3);
</script> 

{% endhighlight %}

### deleteSheet(idx)
{:#methods:deletesheet}

This method is used to delete a particular sheet in the Spreadsheet.

<table class="params">
<thead>
<tr>
<th>Name</th>
<th>Type</th>
<th>Description</th>
</tr>
</thead>
<tbody>
<tr>
<td class="name">idx</td>
<td class="type"><span class="param-type">number</span></td>
<td class="description">Pass the sheet index to perform delete action.</td>
</tr>
</tbody>
</table>

#### Example

{% highlight html %}
<script>
// Initialize the Spreadsheet object.
var excelObj = $("#Spreadsheet").data("ejSpreadsheet");
excelObj.deleteSheet(3); // Sends a sheet delete request to the Spreadsheet
</script>

{% endhighlight %}

{% highlight html %}
<script>
// Sends a sheet delete request to the Spreadsheet
$("#Spreadsheet").ejSpreadsheet("deleteSheet", 3);        
</script>

{% endhighlight %}


### deleteShiftLeft(startCell, endCell)
{:#methods:deleteshiftleft}

This method is used to delete the selected cells and shift the remaining cells to left.
<table class="params">
<thead>
<tr>
<th>Name</th>
<th>Type</th>
<th>Description</th>
</tr>
</thead>
<tbody>
<tr>
<td class="name">startCell</td>
<td class="type"><ts ref="CellIndex"/><span class="param-type">Object</span></td>
<td class="description">Pass the Object "CellIndex"
<table class="params">
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
<td class="type"><span class="param-type">number</span></td>
<td class="description">Pass the row index of the starting cell</td>
</tr>
<tr>
<td class="name">colIndex</td>
<td class="type"><span class="param-type">number</span></td>
<td class="description">Pass the column index of the starting cell</td>
</tr>
</tbody>
</table>
</td></tr>
<tr>
<td class="name">endCell</td>
<td class="type"><ts ref="CellIndex"/><span class="param-type">Object</span></td>
<td class="description">Pass the Object "CellIndex"
<table class="params">
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
<td class="type"><span class="param-type">number</span></td>
<td class="description">Pass the row index of the ending cell</td>
</tr>
<tr>
<td class="name">colIndex</td>
<td class="type"><span class="param-type">number</span></td>
<td class="description">Pass the column index of the ending cell</td>
</tr>
</tbody>
</table>
</td></tr>
</tbody>
</table>

#### Example

{% highlight html %}
<script>
var startCell= {rowIndex: 1, colIndex: 2}, endCell= {rowIndex: 1, colIndex: 2};
// Initialize the Spreadsheet object
var excelObj = $("#Spreadsheet").data("ejSpreadsheet");
//Delete a cell and shift cells left in the sheet.
excelObj.deleteShiftLeft(startCell, endCell);
</script>

{% endhighlight %}

{% highlight html %}
<script>
var startCell= {rowIdx: 1, colIdx: 2}, endCell= {rowIdx: 1, colIdx: 2};
// Delete a cell and shift cells left in the sheet.
$("#Spreadsheet").ejSpreadsheet("deleteShiftLeft", startCell, endCell);
</script> 

{% endhighlight %}

### deleteShiftUp(startCell, endCell)
{:#methods:deleteshiftup}

This method is used to delete the selected cells and shift the remaining cells up.
<table class="params">
<thead>
<tr>
<th>Name</th>
<th>Type</th>
<th>Description</th>
</tr>
</thead>
<tbody>
<tr>
<td class="name">startCell</td>
<td class="type"><ts ref="CellIndex"/><span class="param-type">Object</span></td>
<td class="description">Pass the Object "CellIndex"
<table class="params">
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
<td class="type"><span class="param-type">number</span></td>
<td class="description">Pass the row index of the start cell</td>
</tr>
<tr>
<td class="name">colIndex</td>
<td class="type"><span class="param-type">number</span></td>
<td class="description">Pass the column index of the start cell</td>
</tr>
</tbody>
</table>
</td></tr>
<tr>
<td class="name">endCell</td>
<td class="type"><ts ref="CellIndex"/><span class="param-type">Object</span></td>
<td class="description">Pass the Object "CellIndex"
<table class="params">
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
<td class="type"><span class="param-type">number</span></td>
<td class="description">Pass the row index of the end cell</td>
</tr>
<tr>
<td class="name">colIndex</td>
<td class="type"><span class="param-type">number</span></td>
<td class="description">Pass the column index of the end cell</td>
</tr>
</tbody>
</table>
</td></tr>
</tbody>
</table>

#### Example

{% highlight html %}
<script>
var startCell= {rowIndex: 1, colIndex: 2}, endCell= {rowIndex: 1, colIndex: 2};
// Initialize the Spreadsheet object
var excelObj = $("#Spreadsheet").data("ejSpreadsheet");
// Delete a cell and shift cells up in the sheet.
excelObj.deleteShiftUp(startCell, endCell);
</script>

{% endhighlight %}

{% highlight html %}
<script>
var startCell= {rowIdx: 1, colIdx: 2}, endCell= {rowIdx: 1, colIdx: 2};
// Delete a cell and shift cells up in the sheet.
$("#Spreadsheet").ejSpreadsheet("deleteShiftUp", startCell, endCell);
</script> 

{% endhighlight %}

### editRange(rangeName, fn)
{:#methods:editrange}

This method is used to edit data in the specified range of cells based on its corresponding rangeSettings.

<table class="params">
<thead>
<tr>
<th>Name</th>
<th>Type</th>
<th>Description</th>
</tr>
</thead>
<tbody>
<tr>
<td class="name">rangeName</td>
<td class="type"><span class="param-type">string</span></td>
<td class="description">Pass the defined rangeSettings property name.</td>
</tr>
<tr>
<td class="name">fn</td>
<td class="type"><span class="param-type">function</span></td>
<td class="description">Pass the function that you want to perform range edit.</td>
</tr>
</tbody>
</table>

#### Example

{% highlight html %}
<script>
// Initialize the Spreadsheet object.
var excelObj = $("#Spreadsheet").data("ejSpreadsheet");
var updateFn = function(cell, cellIdx) {
if (cellIdx % 2 == 0)
return "SpreadSheet";
else
return "Grid";
};
var rangeSettings = {
range: "B1:C2",
name: "updateTable",
cssClass: "readOnly1",
readOnly: true,
contextTab: {},
contextMenuSettings: {
dataSource: [{
id: 1,
text: "Copy",
parentId: null,
sprite: "e-icon e-copy"
}, {
id: 2,
text: "Refresh",
parentId: null,
}]
},
showPanel: true
};
//Update new rangeSettings property before invoking edit range
excelObj.model.sheets[1].rangeSettings["updateTable"] = rangeSettings;
//Sends a edit range request to the Spreadsheet
excelObj.editRange("updateTable", updateFn); 
</script>

{% endhighlight %}

{% highlight html %}
<script>
//Sends a edit range request to the Spreadsheet after updating new rangeSettings.
$("#Spreadsheet").ejSpreadsheet("editRange", "updateTable", updateFn);        
</script>

{% endhighlight %}

### getActivationPanel()
{:#methods:getactivationpanel}

This method is used to get the activation panel in the Spreadsheet.

#### Returns:
Element

#### Example
{% highlight html %}
<div id="Spreadsheet"></div> 
<script>
// Initialize Spreadsheet object.
var excelObj = $("#Spreadsheet").data("ejSpreadsheet");
excelObj.getActivationPanel(); // Gets sheet  ActivationPanel element in Spreadsheet.
</script>
{% endhighlight %}

{% highlight html %}
<script>
// Gets sheet ActivationPanel element in Spreadsheet.
$("#Spreadsheet").ejSpreadsheet("getActivationPanel");        
</script>

{% endhighlight %}


### getActiveCell(\[sheetIdx\])
{:#methods:getactivecell}

This method is used to get the active cell object in Spreadsheet. It will returns object which contains rowIndex and colIndex of the active cell.
<table class="params">
<thead>
<tr>
<th>Name</th>
<th>Type</th>
<th>Description</th>
</tr>
</thead>
<tbody>
<tr>
<td class="name">sheetIdx</td>
<td class="type"><span class="param-type">number</span></td>
<td class="description"><span class="optional">Optional.</span> If sheetIdx is specified, it will return the active cell object in specified sheet index else it will use the current sheet index</td>
</tr>
</tbody>
</table>

#### Returns:
Object

#### Example

{% highlight html %}
<div id="Spreadsheet"></div> 
<script>
// Initialize Spreadsheet object.
var excelObj = $("#Spreadsheet").data("ejSpreadsheet");
excelObj.getActiveCell(1); // Gets the activeCell  object in specified sheet index.
</script>

{% endhighlight %}

{% highlight html %}
<script>
// Gets the activeCell element in specified sheetindex
$("#Spreadsheet").ejSpreadsheet("getActiveCell", 1);        
</script>

{% endhighlight %}

### getActiveCellElem(\[sheetIdx\])
{:#methods:getactivecellelem}

This method is used to get the active cell element based on the given sheet index in the Spreadsheet.
<table class="params">
<thead>
<tr>
<th>Name</th>
<th>Type</th>
<th>Description</th>
</tr>
</thead>
<tbody>
<tr>
<td class="name">sheetIdx</td>
<td class="type"><span class="param-type">number</span></td>
<td class="description"><span class="optional">Optional.</span> If sheetIndex is specified, it will return the active cell element in specified <br/>sheet index else it will use the current active sheet index.</td>
</tr>
</tbody>
</table>

#### Returns:
Element

#### Example

{% highlight html %}
<div id="Spreadsheet"></div> 
<script>
// Initialize Spreadsheet object.
var excelObj = $("#Spreadsheet").data("ejSpreadsheet");
excelObj.getActiveCellElem(1); // Gets activeCell element in Spreadsheet.
</script>

{% endhighlight %}

{% highlight html %}
<script>
// Gets activeCell element in Spreadsheet.
$("#Spreadsheet").ejSpreadsheet("getActiveCellElem", 1);        
</script>

{% endhighlight %}

### getActiveSheetIndex()
{:#methods:getactivesheetindex}

This method is used to get the current active sheet index in Spreadsheet.

#### Returns:
number
 
#### Example

{% highlight html %}
<div id="Spreadsheet"></div> 
<script>
// Initialize Spreadsheet object.
var excelObj = $("#Spreadsheet").data("ejSpreadsheet");
excelObj.getActiveSheetIndex(); // Gets activeSheet index in Spreadsheet.
</script>

{% endhighlight %}

{% highlight html %}
<script>
// Gets activeSheet index in Spreadsheet
$("#Spreadsheet").ejSpreadsheet("getActiveSheetIndex");        
</script>

{% endhighlight %}

### getAutoFillElem()
{:#methods:getautofillelem}

This method is used to get the auto fill element in Spreadsheet.

#### Returns:
Element

#### Example

{% highlight html %}
<div id="Spreadsheet"></div> 
<script>
// Initialize Spreadsheet object.
var excelObj = $("#Spreadsheet").data("ejSpreadsheet");
excelObj.getAutoFillElem(); // Gets autofill element in Spreadsheet.
</script>

{% endhighlight %}

{% highlight html %}
<script>
// Gets autofill element in Spreadsheet.
$("#Spreadsheet").ejSpreadsheet("getAutoFillElem");        
</script>

{% endhighlight %}

### getAlphaRange(sRIndex, sCIndex, eRIndex, eCIndex)
{:#methods:getalpharange}

This method is used to get the alpha range of the given index in Spreadsheet.

<table class="params">
<thead>
<tr>
<th>Name</th>
<th>Type</th>
<th>Description</th>
</tr>
</thead>
<tbody>
<tr>
<td class="name">sRIndex</td>
<td class="type"><span class="param-type">number</span></td>
<td class="description">Pass the start row index.</td>
</tr>
<tr>
<td class="name">sCIndex</td>
<td class="type"><span class="param-type">number</span></td>
<td class="description">Pass the start column index.</td>
</tr>
<tr>
<td class="name">eRIndex</td>
<td class="type"><span class="param-type">number</span></td>
<td class="description">Pass the end row index.</td>
</tr>
<tr>
<td class="name">eCIndex</td>
<td class="type"><span class="param-type">number</span></td>
<td class="description">Pass the end column index.</td>
</tr>
</tbody>
</table>

#### Returns:
String

#### Example

{% highlight html %}
<div id="Spreadsheet"></div> 
<script>
// Initialize Spreadsheet object.
var excelObj = $("#Spreadsheet").data("ejSpreadsheet");
excelObj.getAlphaRange(2,3,4,5); // Get the alpha range for the given index
</script>

{% endhighlight %}

### getCell(rowIdx, colIdx, \[sheetIdx\])
{:#methods:getcell}

This method is used to get the cell element based on specified row and column index in the Spreadsheet.

<table class="params">
<thead>
<tr>
<th>Name</th>
<th>Type</th>
<th>Description</th>
</tr>
</thead>
<tbody>
<tr>
<td class="name">rowIdx</td>
<td class="type"><span class="param-type">number</span></td>
<td class="description">Pass the row index.</td>
</tr>
<tr>
<td class="name">colIdx</td>
<td class="type"><span class="param-type">number</span></td>
<td class="description">Pass the column index.</td>
</tr>
<tr>
<td class="name">sheetIdx</td>
<td class="type"><span class="param-type">number</span></td>
<td class="description"><span class="optional">Optional.</span> Pass the sheet index that you want to get cell.</td>
</tr>
</tbody>
</table>

#### Returns:
Element

#### Example

{% highlight html %}
<div id="Spreadsheet"></div> 
<script>
// Initialize Spreadsheet object.
var excelObj = $("#Spreadsheet").data("ejSpreadsheet");
excelObj.getCell(2, 3, 1); // Get the cell based on rowIndex and colIndex.
</script>

{% endhighlight %}

{% highlight html %}
<script>
// Get the cell based on row and column index
$("#Spreadsheet").ejSpreadsheet("getCell", 2, 3, 1);        
</script>

{% endhighlight %}

### getDataSettings(sheetIdx)
{:#methods:getdatasettings}

This method is used to get the data settings in the Spreadsheet.
<table class="params">
<thead>
<tr>
<th>Name</th>
<th>Type</th>
<th>Description</th>
</tr>
</thead>
<tbody>
<tr>
<td class="name">sheetIdx</td>
<td class="type"><span class="param-type">number</span></td>
<td class="description">Pass the sheet index.</td>
</tr>
</tbody>
</table>

#### Returns:
number

#### Example

{% highlight html %}
<div id="Spreadsheet"></div>
<script>
// Initialize Spreadsheet object.
var excelObj = $("#Spreadsheet").data("ejSpreadsheet");
excelObj.getDataSettings(1); // Gets the data settings in Spreadsheet
</script>

{% endhighlight %}

{% highlight html %}
<script>
// Gets the data settings in Spreadsheet
$("#Spreadsheet").ejSpreadsheet("getDataSettings", 1);        
</script>

{% endhighlight %}

### getFrozenColumns(sheetIdx)
{:#methods:getfrozencolumns}

This method is used to get the frozen columns index in the Spreadsheet.
<table class="params">
<thead>
<tr>
<th>Name</th>
<th>Type</th>
<th>Description</th>
</tr>
</thead>
<tbody>
<tr>
<td class="name">sheetIdx</td>
<td class="type"><span class="param-type">number</span></td>
<td class="description">Pass the sheet index.</td>
</tr>
</tbody>
</table>

#### Returns:
number

#### Example

{% highlight html %}
<div id="Spreadsheet"></div>
<script>
// Initialize Spreadsheet object.
var excelObj = $("#Spreadsheet").data("ejSpreadsheet");
excelObj.getFrozenColumns(1); // Gets the frozen column index in Spreadsheet
</script>

{% endhighlight %}

{% highlight html %}
<script>
// Gets the frozen column index in Spreadsheet
$("#Spreadsheet").ejSpreadsheet("getFrozenColumns", 1);        
</script>

{% endhighlight %}

### getFrozenRows(sheetIdx)
{:#methods:getfrozenrows}

This method is used to get the frozen row index in Spreadsheet.
<table class="params">
<thead>
<tr>
<th>Name</th>
<th>Type</th>
<th>Description</th>
</tr>
</thead>
<tbody>
<tr>
<td class="name">sheetIdx</td>
<td class="type"><span class="param-type">number</span></td>
<td class="description">Pass the sheet index.</td>
</tr>
</tbody>
</table>

#### Returns:
number

#### Example

{% highlight html %}
<div id="Spreadsheet"></div>
<script>
// Initialize Spreadsheet object.
var excelObj = $("#Spreadsheet").data("ejSpreadsheet");
excelObj.getFrozenRows(1); // Gets the frozen row index in Spreadsheet.
</script>

{% endhighlight %}

{% highlight html %}
<script>
// Gets the frozen row index in Spreadsheet
$("#Spreadsheet").ejSpreadsheet("getFrozenRows", 1);        
</script>

{% endhighlight %}

### getHyperlink(cell)
{:#methods:gethyperlink}

This method is used to get the hyperlink data as object from the specified cell in Spreadsheet.
<table class="params">
<thead>
<tr>
<th>Name</th>
<th>Type</th>
<th>Description</th>
</tr>
</thead>
<tbody>
<tr>
<td class="name">cell</td>
<td class="type"><span class="param-type">Element</span></td>
<td class="description">Pass the DOM element to get hyperlink</td>
</tr>
</tbody>
</table>

#### Returns:
Object

#### Example

{% highlight html %}
<script>
// Initialize Spreadsheet object.
var excelObj = $("#Spreadsheet").data("ejSpreadsheet");
excelObj.getHyperlink(excelObj.getCell(1, 1)); // To get the hyperlink data of specified cell.
</script>

{% endhighlight %}

{% highlight html %}
<script>
// To get the hyperlink data of specified cell.
$("#Spreadsheet").ejSpreadsheet("getHyperlink", excelObj.getCell(1, 1, 1));        
</script>

{% endhighlight %}

### getObjectKeys(obj)
{:#methods:getobjectkeys}

This method is used to get the keys from the given object in Spreadsheet.
<table class="params">
<thead>
<tr>
<th>Name</th>
<th>Type</th>
<th>Description</th>
</tr>
</thead>
<tbody>
<tr>
<td class="name">obj</td>
<td class="type"><span class="param-type">Object</span></td>
<td class="description">Pass the Object</td>
</tr>
</tbody>
</table>

#### Returns:
Array

#### Example

{% highlight html %}
<script>
// Initialize Spreadsheet object.
var excelObj = $("#Spreadsheet").data("ejSpreadsheet");
excelObj.getObjectKeys({"font-family": "Arial Black", "font-weight": "normal", "font-style": "Italic", "font-size": "9pt", "text-decoration": "line-through",color:"#FFFF00"}); // To get the keys from the given object.
</script>

{% endhighlight %}

### getRange(range, sheetIdx, \[skipHiddenRow\])
{:#methods:getrange}

This method is used to get all cell elements in the specified range.
<table class="params">
<thead>
<tr>
<th>Name</th>
<th>Type</th>
<th>Description</th>
</tr>
</thead>
<tbody>
<tr>
<td class="name">range</td>
<td class="type"><span class="param-type">string</span></td>
<td class="description">Pass the range that you want to get the cells.</td>
</tr>
<tr>
<td class="name">sheetIdx</td>
<td class="type"><span class="param-type">number</span></td>
<td class="description">Pass the index of the sheet.</td>
</tr>
<tr>
<td class="name">skipHiddenRow</td>
<td class="type"><span class="param-type">boolean</span></td>
<td class="description"><span class="optional">Optional.</span> Pass {{'`true`' | markdownify}}, if you want to skip the hidden rows.</td>
</tr>
</tbody>
</table>

#### Returns:
Element

#### Example

{% highlight html %}
<div id="Spreadsheet"></div> 
<script>
// Initialize Spreadsheet object.
var excelObj = $("#Spreadsheet").data("ejSpreadsheet");
excelObj.getRange("A2:A5", 1, false); // Get the cells based on the given range
</script>

{% endhighlight %}

{% highlight html %}
<script>
// Get the cells based on the given range
$("#Spreadsheet").ejSpreadsheet("getRange", "A2:A5", 1, false);        
</script>

{% endhighlight %}

### getRangeData(\[options\])
{:#methods:getrangedata}

This method is used to get the data in specified range in Spreadsheet.
<table class="params">
<thead>
<tr>
<th>Name</th>
<th>Type</th>
<th>Description</th>
</tr>
</thead>
<tbody>
<tr>
<td class="name">options</td>
<td class="type"><span class="param-type">Object</span></td>
<td class="description"><span class="optional">Optional.</span> Pass the range, property, sheetIdx, valueOnly in options
</td></tr>
</tbody>
</table>

#### Returns:
Array

#### Example

{% highlight html %}
<div id="Spreadsheet"></div> 
<script>
// Initialize Spreadsheet object.
var excelObj = $("#Spreadsheet").data("ejSpreadsheet");
excelObj.getRangeData({range: [2, 6, 2, 6], property: ["value", "value2", "format"], sheetIdx: 1}); // To get the cells data of specified range
</script>

{% endhighlight %}

{% highlight html %}
<script>
// To get the cells data of specified range
$("#Spreadsheet").ejSpreadsheet("getRangeData", {range: [2, 6, 2, 6], property: ["value", "value2", "format"], sheetIdx: 1});        
</script>

{% endhighlight %}

### getRangeDataAsObject(startcell, endcell, \[skipHiddenRow\])
{:#methods:getrangedataasobject}

This method is used to get the data as object in the specified range.
<table class="params">
<thead>
<tr>
<th>Name</th>
<th>Type</th>
<th>Description</th>
</tr>
</thead>
<tbody>
<tr>
<td class="name">startcell</td>
<td class="type"><ts ref="CellIndex"/><span class="param-type">object</span></td>
<td class="description">Pass the Object "CellIndex"
<table class="params">
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
<td class="type"><span class="param-type">number</span></td>
<td class="description">Pass the row index to get the data as object</td>
</tr>
<tr>
<td class="name">colIndex</td>
<td class="type"><span class="param-type">number</span></td>
<td class="description">Pass the column index to get the data as object</td>
</tr>
</tbody>
</table>
</td></tr>
<tr>
<td class="name">endcell</td>
<td class="type"><ts ref="CellIndex"/><span class="param-type">object</span></td>
<td class="description">Pass the Object "CellIndex"
<table class="params">
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
<td class="type"><span class="param-type">number</span></td>
<td class="description">Pass the row index to get the data as object</td>
</tr>
<tr>
<td class="name">colIndex</td>
<td class="type"><span class="param-type">number</span></td>
<td class="description">Pass the column index to get the data as object</td>
</tr>
</tbody>
</table>
</td></tr>
<tr>
<td class="name">skipHiddenRow</td>
<td class="type"><span class="param-type">boolean</span></td>
<td class="description"><span class="optional">Optional.</span> Pass {{'`true`' | markdownify}}, if you want to skip the hidden rows.</td>
</tr>
</tbody>
</table>

#### Returns:
Object

#### Example

{% highlight html %}
<div id="Spreadsheet"></div> 
<script>
// Initialize Spreadsheet object.
var excelObj = $("#Spreadsheet").data("ejSpreadsheet");
excelObj.getRangeDataAsObject({ rowIndex:2,colIndex:2 },{ rowIndex:4,colIndex:4 }, true, 1); // To get the data as object from the given cell
</script>

{% endhighlight %}

### getRangeIndices(range)
{:#methods:getrangeindices}

This method is used to get the range indices array based on the specified alpha range in Spreadsheet.

<table class="params">
<thead>
<tr>
<th>Name</th>
<th>Type</th>
<th>Description</th>
</tr>
</thead>
<tbody>
<tr>
<td class="name">range</td>
<td class="type"><span class="param-type">string</span></td>
<td class="description">Pass the alpha range that you want to get range indices.</td>
</tr>
</tbody>
</table>

#### Returns:
Array
 
#### Example

{% highlight html %}
<div id="Spreadsheet"></div> 
<script>
// Initialize Spreadsheet object.
var excelObj = $("#Spreadsheet").data("ejSpreadsheet");
excelObj.getRangeIndices("A1:A9"); // Get range indices based on specified alpha range.
</script>

{% endhighlight %}

{% highlight html %}
<script>
// Get cells based on specified range indices
$("#Spreadsheet").ejSpreadsheet("getRangeIndices", "A1:A9");        
</script>
{% endhighlight %}

### getSheet(sheetIdx)
{:#methods:getsheet}

This method is used to get the sheet details based on the given sheet index in Spreadsheet.

<table class="params">
<thead>
<tr>
<th>Name</th>
<th>Type</th>
<th>Description</th>
</tr>
</thead>
<tbody>
<tr>
<td class="name">sheetIdx</td>
<td class="type"><span class="param-type">number</span></td>
<td class="description">Pass the sheet index to get the sheet object.</td>
</tr>
</tbody>
</table>

#### Returns:
Object

#### Example

{% highlight html %}
<div id="Spreadsheet"></div>
<script>
// Initialize the Spreadsheet object.
var excelObj = $("#Spreadsheet").data("ejSpreadsheet");
excelObj.getSheet(1); // Gets sheet details of Spreadsheet.
</script>

{% endhighlight %}

{% highlight html %}
<script>
// Gets sheet details of Spreadsheet
$("#Spreadsheet").ejSpreadsheet("getSheet", 1);        
</script>

{% endhighlight %}

### getSheetElement(sheetIdx)
{:#methods:getsheetelement}

This method is used to get the sheet content div element of Spreadsheet.

<table class="params">
<thead>
<tr>
<th>Name</th>
<th>Type</th>
<th>Description</th>
</tr>
</thead>
<tbody>
<tr>
<td class="name">sheetIdx</td>
<td class="type"><span class="param-type">number</span></td>
<td class="description">Pass the sheet index to get the sheet content.</td>
</tr>
</tbody>
</table>

#### Returns:
Element

#### Example

{% highlight html %}
<div id="Spreadsheet"></div>
<script>
// Initialize the Spreadsheet object.
var excelObj = $("#Spreadsheet").data("ejSpreadsheet");
excelObj.getSheetElement(1); // Gets sheet content of Spreadsheet.
</script>

{% endhighlight %}

{% highlight html %}
<script>
// Gets sheet content of Spreadsheet.
$("#Spreadsheet").ejSpreadsheet("getSheetElement", 1);        
</script>

{% endhighlight %}

### getSheets()
{:#methods:getsheets}

This method is used to get all the sheets in workbook.

#### Returns:
Array

#### Example

{% highlight html %}
<div id="Spreadsheet"></div>
<script>
// Initialize the Spreadsheet object.
var excelObj = $("#Spreadsheet").data("ejSpreadsheet");
excelObj.getSheets(); // Gets sheets details of Spreadsheet.
</script>

{% endhighlight %}

{% highlight html %}
<script>
// Gets sheets details of Spreadsheet
$("#Spreadsheet").ejSpreadsheet("getSheets");        
</script>

{% endhighlight %}

### gotoPage(sheetIdx, newSheet)
{:#methods:gotopage}

This method is used to send a paging request to the specified sheet Index in the Spreadsheet.

<table class="params">
<thead>
<tr>
<th>Name</th>
<th>Type</th>
<th>Description</th>
</tr>
</thead>
<tbody>
<tr>
<td class="name">sheetIdx</td>
<td class="type"><span class="param-type">number</span></td>
<td class="description">Pass the sheet index to perform paging at specified sheet index</td>
</tr>
<tr>
<td class="name">newSheet</td>
<td class="type"><span class="param-type">boolean</span></td>
<td class="description">Pass {{'`true`' | markdownify}} to create a new sheet. If the specified sheet index is already exist,<br/> it navigate to that sheet else it create a new sheet.</td>
</tr>
</tbody>
</table>

#### Example

{% highlight html %}
<div id="Spreadsheet"></div>
<script>
// Initialize the Spreadsheet object.
var excelObj = $("#Spreadsheet").data("ejSpreadsheet");
excelObj.gotoPage(1, false); // Sends a paging request to the Spreadsheet with specified sheet index
</script>

{% endhighlight %}

{% highlight html %}
<script>
// Sends a paging request to the Spreadsheet with specified sheet index.
$("#Spreadsheet").ejSpreadsheet("gotoPage", 3, true);        
</script>

{% endhighlight %}

### getVisibleCellDetails()
{:#methods:getvisiblecelldetails}

This method is used to get the visible cell details in Spreadsheet.

#### Example

{% highlight html %}
<script>
//initialize the Spreadsheet object
var excelObj = $("#Spreadsheet").data("ejSpreadsheet"),
cellDetails = excelObj.getVisibleCellDetails(),  //To get the visible cell details in Spreadsheet.
topLeftCell = cellDetails.topLeftCell,  // To get the visible topLeftCell.
rowCount = cellDetails.rowCount,  // To get the visible rowcount.
colCount = cellDetails.colCount;  // To get the visible colCount.
</script>

{% endhighlight %}

### hideActivationPanel()
{:#methods:hideactivationpanel}

This method is used to hide the pivot table activationPanel in the Spreadsheet.

#### Example

{% highlight html %}
<script>
// Initialize Spreadsheet object.
var excelObj = $("#Spreadsheet").data("ejSpreadsheet");
excelObj.hideActivationPanel(); // To hide the pivot table activationPanel in the Spreadsheet.
</script>

{% endhighlight %}

{% highlight html %}
<script>
// To hide the pivot table activationPanel in the Spreadsheet.
$("#Spreadsheet").ejSpreadsheet("hideActivationPanel");        
</script>

{% endhighlight %}

### hideColumn(startCol, endCol)
{:#methods:hidecolumn}

This method is used to hide the entire columns from the specified range (startCol, endCol) in Spreadsheet.

<table class="params">
<thead>
<tr>
<th>Name</th>
<th>Type</th>
<th>Description</th>
</tr>
</thead>
<tbody>
<tr>
<td class="name">startCol</td>
<td class="type"><span class="param-type">number</span></td>
<td class="description">Index of the start column.</td>
</tr>
<tr>
<td class="name">endCol</td>
<td class="type"><span class="param-type">number</span></td>
<td class="description">Optional. Index of the end column.</td>
</tr>
</tbody>
</table>

#### Example

{% highlight html %}
<div id="Spreadsheet"></div>
<script>
// Initialize the Spreadsheet object
var excelObj = $("#Spreadsheet").data("ejSpreadsheet");
// Hide the column by passing column index in the active sheet.
excelObj.hideColumn(1);
// Hide the columns from startCol to endCol in the active sheet.
excelObj.hideColumn(1, 4);
</script>

{% endhighlight %}

{% highlight html %}
<script>
// Hide the column by passing column index in the active sheet.
$("#Spreadsheet").ejSpreadsheet("hideColumn", 1);
// Hide the columns from startCol to endCol in the active sheet.
$("#Spreadsheet").ejSpreadsheet("hideColumn", 1, 4);
</script>

{% endhighlight %}

### hideFormulaBar()
{:#methods:hideformulabar}

This method is used to hide the formula bar in Spreadsheet.

#### Example

{% highlight html %}
<script>
// Initialize the Spreadsheet object.
var excelObj = $("#Spreadsheet").data("ejSpreadsheet");
//To hide formula bar in Spreadsheet.
excelObj.hideFormulaBar();
</script>

{% endhighlight %}

### hideRow(startRow, endRow)
{:#methods:hiderow}

This method is used to hide the rows, based on the specified row index in Spreadsheet.

<table class="params">
<thead>
<tr>
<th>Name</th>
<th>Type</th>
<th>Description</th>
</tr>
</thead>
<tbody>
<tr>
<td class="name">startRow</td>
<td class="type"><span class="param-type">number</span></td>
<td class="description">Index of the start row.</td>
</tr>
<tr>
<td class="name">endRow</td>
<td class="type"><span class="param-type">number</span></td>
<td class="description"> Optional. Index of the end row.</td>
</tr>
</tbody>
</table>

#### Example

{% highlight html %}
<div id="Spreadsheet"></div>
<script>
// Initialize the Spreadsheet object
var excelObj = $("#Spreadsheet").data("ejSpreadsheet");
// Hide the row by passing row index in the active sheet.
excelObj.hideRow(1);
// Hide a rows from startRow to endRow in the active sheet.
excelObj.hideRow(1, 4);
</script>


{% endhighlight %}

{% highlight html %}
<script>
// Hide the row by passing row index in the active sheet.
$("#Spreadsheet").ejSpreadsheet("hideRow", 1);
// Hide a rows from startRow to endRow in the active sheet.
$("#Spreadsheet").ejSpreadsheet("hideRow", 1, 4);
</script>

{% endhighlight %}

### hideSheet(sheetIdx)
{:#methods:hidesheet}

This method is used to hide the sheet based on the specified sheetIndex or sheet name in the Spreadsheet.

<table class="params">
<thead>
<tr>
<th>Name</th>
<th>Type</th>
<th>Description</th>
</tr>
</thead>
<tbody>
<tr>
<td class="name">sheetIdx</td>
<td class="type"><span class="param-type">string|number</span></td>
<td class="description">Pass the sheet name or index that you want to hide.</td>
</tr>
</tbody>
</table>

#### Example

{% highlight html %}
<div id="Spreadsheet"></div>
<script>
// Initialize the Spreadsheet object.
var excelObj = $("#Spreadsheet").data("ejSpreadsheet");
//Sends a hide sheet request to the Spreadsheet.
excelObj.hideSheet("Sheet2");
</script>

{% endhighlight %}

{% highlight html %}
<script>
//Sends a hide sheet request to the Spreadsheet.
$("#Spreadsheet").ejSpreadsheet("hideSheet", 2);
</script>

{% endhighlight %}

### hideWaitingPopUp()
{:#methods:hidewaitingpopup}

This method is used to hide the displayed waiting pop-up in Spreadsheet.

#### Example

{% highlight html %}
<div id="Spreadsheet"></div>
<script>
// Initialize the Spreadsheet object.
var excelObj = $("#Spreadsheet").data("ejSpreadsheet");
// hide waiting popup in the Spreadsheet.
excelObj.hideWaitingPopUp();
</script>

{% endhighlight %}

{% highlight html %}
<script>
// hide waiting popup in the Spreadsheet.
$("#Spreadsheet").ejSpreadsheet("hideWaitingPopUp");
</script>

{% endhighlight %}

### insertEntireColumn(startCol, endCol)
{:#methods:insertentirecolumn}

This method is used to insert a column before the active cell's column in the Spreadsheet.

<table class="params">
<thead>
<tr>
<th>Name</th>
<th>Type</th>
<th>Description</th>
</tr>
</thead>
<tbody>
<tr>
<td class="name">startCol</td>
<td class="type"><span class="param-type">number</span></td>
<td class="description">Pass start column.</td>
</tr>
<tr>
<td class="name">endCol</td>
<td class="type"><span class="param-type">number</span></td>
<td class="description">Pass end column.</td>
</tr>
</tbody>
</table>

#### Example

{% highlight html %}
<div id="Spreadsheet"></div>
<script>
//initialize the Spreadsheet object.
var excelObj = $("#Spreadsheet").data("ejSpreadsheet");
// Insert a column in the sheet.
excelObj.insertEntireColumn(1, 2);
</script>

{% endhighlight %}

{% highlight html %}
<script>
// Insert a column in the sheet.
$("#Spreadsheet").ejSpreadsheet("insertEntireColumn", 1, 2);
</script>

{% endhighlight %}

### insertEntireRow(startRow, endRow)
{:#methods:insertentirerow}

This method is used to insert a row before the active cell's row in the Spreadsheet.

<table class="params">
<thead>
<tr>
<th>Name</th>
<th>Type</th>
<th>Description</th>
</tr>
</thead>
<tbody>
<tr>
<td class="name">startRow</td>
<td class="type"><span class="param-type">number</span></td>
<td class="description">Pass start row.</td>
</tr>
<tr>
<td class="name">endRow</td>
<td class="type"><span class="param-type">number</span></td>
<td class="description">Pass end row.</td>
</tr>
</tbody>
</table>

#### Example

{% highlight html %}
<div id="Spreadsheet"></div>
<script>
//initialize the Spreadsheet object
var excelObj = $("#Spreadsheet").data("ejSpreadsheet");
// Insert a row in the sheet.
excelObj.insertEntireRow(1, 2);
</script>

{% endhighlight %}

{% highlight html %}
<script>
// Insert a row in the sheet.
$("#Spreadsheet").ejSpreadsheet("insertEntireRow", 1, 2);
</script>

{% endhighlight %}

### insertSheet()
{:#methods:insertsheet}

This method is used to insert a new sheet to the left of the current active sheet.

#### Example

{% highlight html %}
<div id="Spreadsheet"></div>
<script>
// Initialize the Spreadsheet object.
var excelObj = $("#Spreadsheet").data("ejSpreadsheet");
excelObj.insertSheet(); // Sends a insert new sheet request to the Spreadsheet.
</script>

{% endhighlight %}

{% highlight html %}
<script>
// Sends an insert new sheet request to the Spreadsheet.
$("#Spreadsheet").ejSpreadsheet("insertSheet");        
</script>

{% endhighlight %}

### insertShiftBottom(startCell, endCell)
{:#methods:insertshiftbottom}

This method is used to insert cells in the selected or specified range and shift remaining cells to bottom.

<table class="params">
<thead>
<tr>
<th>Name</th>
<th>Type</th>
<th>Description</th>
</tr>
</thead>
<tbody>
<tr>
<td class="name">startCell</td>
<td class="type"><ts ref="CellIndex"/><span class="param-type">Object</span></td>
<td class="description">Pass the Object "CellIndex"
<table class="params">
<thead><tr>
<th>Name</th>
<th>Type</th>
<th>Description</th>
</tr>
</thead>
<tbody>
<tr>
<td class="name">rowIndex</td>
<td class="type"><span class="param-type">number</span></td>
<td class="description">Pass the row index of start cell</td>
</tr>
<tr>
<td class="name">colIndex</td>
<td class="type"><span class="param-type">number</span></td>
<td class="description">Pass the column index of start cell</td>
</tr>
</tbody>
</table>
</td></tr>
<tr>
<td class="name">endCell</td>
<td class="type"><ts ref="CellIndex"/><span class="param-type">Object</span></td>
<td class="description">Pass the Object "CellIndex"
<table class="params">
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
<td class="type"><span class="param-type">number</span></td>
<td class="description">Pass the row index of end cell</td>
</tr>
<tr>
<td class="name">colIndex</td>
<td class="type"><span class="param-type">number</span></td>
<td class="description">Pass the column index of end cell</td>
</tr>
</tbody>
</table>
</td></tr>
</tbody>
</table>

#### Example

{% highlight html %}
<div id="Spreadsheet"></div>
<script>
var startCell= {rowIndex: 1, colIndex: 2}, endCell= {rowIndex: 1, colIndex: 2};
//initialize the Spreadsheet object
var excelObj = $("#Spreadsheet").data("ejSpreadsheet");
// Insert a cells and shift cells bottom in the sheet.
excelObj.insertShiftBottom(startCell, endCell);
</script>

{% endhighlight %}

{% highlight html %}
<script>
var startCell= {rowIndex: 1, colIndex: 2}, endCell= {rowIndex: 1, colIndex: 2};
// Insert a cell and shift cells bottom in the sheet.
$("#Spreadsheet").ejSpreadsheet("insertShiftBottom", startCell, endCell);
</script>

{% endhighlight %}

### insertShiftRight(startCell, endCell)
{:#methods:insertshiftright}

This method is used to insert cells in the selected or specified range and shift remaining cells to right.

<table class="params">
<thead>
<tr>
<th>Name</th>
<th>Type</th>
<th>Description</th>
</tr>
</thead>
<tbody>
<tr>
<td class="name">startCell</td>
<td class="type"><ts ref="CellIndex"/><span class="param-type">Object</span></td>
<td class="description">Pass the Object "CellIndex"
<table class="params">
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
<td class="type"><span class="param-type">number</span></td>
<td class="description">Pass the row index of start cell</td>
</tr>
<tr>
<td class="name">colIndex</td>
<td class="type"><span class="param-type">number</span></td>
<td class="description">Pass the column index of start cell</td>
</tr>
</tbody>
</table>
</td></tr>
<tr>
<td class="name">endCell</td>
<td class="type"><ts ref="CellIndex"/><span class="param-type">Object</span></td>
<td class="description">Pass the Object "CellIndex"
<table class="params">
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
<td class="type"><span class="param-type">number</span></td>
<td class="description">Pass the row index of end cell</td>
</tr>
<tr>
<td class="name">colIndex</td>
<td class="type"><span class="param-type">number</span></td>
<td class="description">Pass the column index of end cell</td>
</tr>
</tbody>
</table>
</td></tr>
</tbody>
</table>

#### Example

{% highlight html %}
<div id="Spreadsheet"></div>
<script>
var startCell= {rowIndex: 1, colIndex: 2}, endCell= {rowIndex: 1, colIndex: 2};
//initialize the Spreadsheet object.
var excelObj = $("#Spreadsheet").data("ejSpreadsheet");
// Insert a cells and shift cells right in the sheet.
excelObj.insertShiftRight(startCell, endCell);
</script>

{% endhighlight %}

{% highlight html %}
<script>
var startCell= {rowIndex: 1, colIndex: 2}, endCell= {rowIndex: 1, colIndex: 2};
// Insert a cell and shift cells right in the sheet.
$("#Spreadsheet").ejSpreadsheet("insertShiftRight", startCell, endCell);
</script> 

{% endhighlight %}

### import(importRequest)
{:#methods:import}

This method is used to import excel file manually by using form data.

<table class="params">
<thead>
<tr>
<th>Name</th>
<th>Type</th>
<th>Description</th>
</tr>
</thead>
<tbody>
<tr>
<td class="name">importRequest</td>
<td class="type"><ts ref="ImportingOptions"/><span class="param-type">Object</span></td>
<td class="description">Pass the form data object to import files manually.
<table class="params">Pass the Object "ImportingOptions"
<thead>
<tr>
<th>Name</th>
<th>Type</th>
<th>Description</th>
</tr>
</thead>
<tbody>
<tr>
<td class="name">file</td>
<td class="type"><span class="param-type">string</span></td>
<td class="description">Pass the file to import manually</td>
</tr>
<tr>
<td class="name">password</td>
<td class="type"><span class="param-type">string</span></td>
<td class="description">Pass the password to import manually</td>
</tr>
<tr>
<td class="name">Url</td>
<td class="type"><span class="param-type">string</span></td>
<td class="description">Pass the url to import manually</td>
</tr>
<tr>
<td class="name">fileStream</td>
<td class="type"><span class="param-type">string</span></td>
<td class="description">Pass the file stream to import manually</td>
</tr>
<tr>
<td class="name">fileType</td>
<td class="type"><span class="param-type">string</span></td>
<td class="description">Pass the filetype to import manually</td>
</tr>
</tbody>
</table>
</td></tr>
</tbody>
</table>

The Objects are File, Password, URL, FileStream, FileType. 

#### Example

{% highlight html %}

<div id="Spreadsheet"></div> 
<script>
var excelObj = $("#Spreadsheet").data("ejSpreadsheet"); // Initialize the Spreadsheet object.
var importRequest = { Url:"http://staging.syncfusion.com:7777/ejSpreadsheet/Spreadsheet.xlsx" };
excelObj.import(importRequest); 
</script>

{% endhighlight %}

### loadFromJSON(response)
{:#methods:loadfromjson}

This method is used to load JSON data in Spreadsheet.

<table class="params">
<thead>
<tr>
<th>Name</th>
<th>Type</th>
<th>Description</th>
</tr>
</thead>
<tbody>
<tr>
<td class="name">response</td>
<td class="type"><span class="param-type">Element</span></td>
<td class="description">Pass the response that you want to load.</td>
</tr>
</tbody>
</table>

#### Example

{% highlight html %}
 
<script>
// Initialize the Spreadsheet object.
var excelObj = $("#Spreadsheet").data("ejSpreadsheet"), response;
response = excelObj.saveAsJSON();
excelObj.loadFromJSON(response); // To load JSON data in the Spreadsheet.
</script>

{% endhighlight %}

### lockCells(range, \[isLocked\])
{:#methods:lockcells}

This method is used to lock/unlock the range of cells in active sheet. Lock cells are activated only after the sheet is protected. Once the sheet is protected it is unable to lock/unlock cells.

<table class="params">
<thead>
<tr>
<th>Name</th>
<th>Type</th>
<th>Description</th>
</tr>
</thead>
<tbody>
<tr>
<td class="name">range</td>
<td class="type"><span class="param-type">string|Array</span></td>
<td class="description">Pass the alpha range cells or array range of cells.</td>
</tr>
<tr>
<td class="name">isLocked</td>
<td class="type"><span class="param-type">string</span></td>
<td class="description"><span class="optional">Optional.</span> By default is {{'`true`' | markdownify}}. If it is {{'`false`' | markdownify}} locked cells are unlocked.</td>
</tr>
</tbody>
</table>

#### Example

{% highlight html %}
<div id="Spreadsheet"></div> 
<script>
// Initialize the Spreadsheet object.
var excelObj = $("#Spreadsheet").data("ejSpreadsheet");
excelObj.lockCells("A3:B5", true); // To lock cells in the Spreadsheet.
</script>

{% endhighlight %}

{% highlight html %}
<script>
// To lock cells in the Spreadsheet.
$("#Spreadsheet").ejSpreadsheet("lockCells","A3:B5", true);        
</script>

{% endhighlight %}

### mergeAcrossCells(\[range\], \[alertStatus\])
{:#methods:mergeacrosscells}

This method is used to merge cells by across in the Spreadsheet.

<table class="params">
<thead>
<tr>
<th>Name</th>
<th>Type</th>
<th>Description</th>
</tr>
</thead>
<tbody>
<tr>
<td class="name">range</td>
<td class="type"><span class="param-type">string</span></td>
<td class="description"><span class="optional">Optional.</span> To pass the cell range or selected cells are process.</td>
</tr>
<tr>
<td class="name">alertStatus</td>
<td class="type"><span class="param-type">boolean</span></td>
<td class="description"><span class="optional">Optional.</span> If pass {{'`true`' | markdownify}} it does not show alert.</td>
</tr>
</tbody>
</table>

#### Example

{% highlight html %}
<script>
// Create Spreadsheet object.
var excelObj = $("#Spreadsheet").data("ejSpreadsheet");
excelObj.mergeAcrossCells("A3:B5", true); // To merge cells across in the Spreadsheet.
</script>

{% endhighlight %}

{% highlight html %}
<script>
// To merge cells across in the Spreadsheet.
$("#Spreadsheet").ejSpreadsheet("mergeAcrossCells","A3:B5");        
</script>

{% endhighlight %}

### mergeCells(\[range\], \[alertStatus\])
{:#methods:mergecells}

This method is used to merge the selected cells in the Spreadsheet.

<table class="params">
<thead>
<tr>
<th>Name</th>
<th>Type</th>
<th>Description</th>
</tr>
</thead>
<tbody>
<tr>
<td class="name">range</td>
<td class="type"><span class="param-type">string|Array</span></td>
<td class="description"><span class="optional">Optional.</span> To pass the cell range or selected cells are process.</td>
</tr>
<tr>
<td class="name">alertStatus</td>
<td class="type"><span class="param-type">boolean</span></td>
<td class="description"><span class="optional">Optional.</span> If pass {{'`true`' | markdownify}} it does not show alert.</td>
</tr>
</tbody>
</table>

#### Example

{% highlight html %}
<script>
// Initialize Spreadsheet object.
var excelObj = $("#Spreadsheet").data("ejSpreadsheet");
excelObj.mergeCells("A3:B5", true); // To merge the selected cell in Spreadsheet.
</script>

{% endhighlight %}

{% highlight html %}
<script>
// To merge the selected cell in Spreadsheet
$("#Spreadsheet").ejSpreadsheet("mergeCells","A3:B5");        
</script>

{% endhighlight %}

### performSelection(startCell, endCell)
{:#methods:performselection}

This method is used to select a cell or range in the Spreadsheet.

<table class="params">
<thead>
<tr>
<th>Name</th>
<th>Type</th>
<th>Description</th>
</tr>
</thead>
<tbody>
<tr>
<td class="name">startCell</td>
<td class="type"><ts ref="CellIndex"/><span class="param-type">Object</span></td>
<td class="description">Pass the Object "CellIndex"
<table class="params">
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
<td class="type"><span class="param-type">number</span></td>
<td class="description">Pass the row index of start cell</td>
</tr>
<tr>
<td class="name">colIndex</td>
<td class="type"><span class="param-type">number</span></td>
<td class="description">Pass the column index of start cell</td>
</tr>
</tbody>
</table>
</td></tr>
<tr>
<td class="name">endCell</td>
<td class="type"><ts ref="CellIndex"/><span class="param-type">Object</span></td>
<td class="description">Pass the Object "CellIndex"
<table class="params">
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
<td class="type"><span class="param-type">number</span></td>
<td class="description">Pass the row index of end cell</td>
</tr>
<tr>
<td class="name">colIndex</td>
<td class="type"><span class="param-type">number</span></td>
<td class="description">Pass the row index of end cell</td>
</tr>
</tbody>
</table>
</td></tr>
</tbody>
</table>

{% highlight html %}
<div id="Spreadsheet"></div>
<script>
// Initialize the Spreadsheet object.
var excelObj = $("#Spreadsheet").data("ejSpreadsheet");
// To perform selection for the specified range.
excelObj.performSelection({ rowIndex: 1, colIndex: 1 }, { rowIndex: 2, colIndex: 2 }); 
// Range as string
excelObj.performSelection("B1:C3");
</script>

{% endhighlight %}

{% highlight html %}
<script>
// To perform selection for the specified range.
$("#Spreadsheet").ejSpreadsheet("performSelection", { rowIndex: 1, colIndex: 1 }, { rowIndex: 2, colIndex: 2 });
// Range as string
$("#Spreadsheet").ejSpreadsheet("performSelection", "B1:C3");
</script>

{% endhighlight %}

### protectSheet(\[isProtected\])
{:#methods:protectsheet}

This method is used to protect or unprotect active sheet.

<table class="params">
<tr>
<th>Name</th>
<th>Type</th>
<th>Description</th>
</tr>
<tr>
<td class="name">isProtected</td>
<td class="type"><span class="param-type">boolean</span></td>
<td class="description"><span class="optional">Optional.</span> By default is {{'`true`' | markdownify}}. If it is {{'`false`' | markdownify}} active sheet is unprotected.</td>
</tr>
</table>

#### Example

{% highlight html %}
<script>
//initialize the Spreadsheet object.
var excelObj = $("#Spreadsheet").data("ejSpreadsheet");
// To protect sheet in Spreadsheet.
excelObj.protectSheet(false);
</script>
{% endhighlight %}

{% highlight html %}
<script>
// To defined refresh selection in Spreadsheet.
$("#Spreadsheet").ejSpreadsheet("protectSheet", false);
</script>

{% endhighlight %}

### redo()
{:#methods:redo}

This method is used to perform the redo action in Spreadsheet.

#### Example

{% highlight html %}
<script>
// Initialize the Spreadsheet object.
var excelObj = $("#Spreadsheet").data("ejSpreadsheet");
// To perform redo action in Spreadsheet
excelObj.redo();
</script>

{% endhighlight %}

### refreshContent(sheetIdx)
{:#methods:refreshcontent}
This method is used to refresh the Spreadsheet based on the sheet model values.
<table class="params">
<thead>
<tr>
<th>Name</th>
<th>Type</th>
<th>Description</th>
</tr>
</thead>
<tbody>
<tr>
<td class="name">sheetIdx</td>
<td class="type"><span class="param-type">number</span></td>
<td class="description">Pass the index of the sheet.</td>
</tr>
</tbody>
</table>

#### Example
{% highlight html %}
<script>
//initialize the Spreadsheet object.
var excelObj = $("#Spreadsheet").data("ejSpreadsheet"), sheet = excelObj.getSheet(); 
    sheet.rowCount = 30; 
    sheet.colCount = 20; 
    excelObj.refreshContent(1); // refresh the spreadsheet based on the row count and column count in normal mode
</script>
{% endhighlight %}

{% highlight html %}
<script>
$("#Spreadsheet").ejSpreadsheet("refreshContent",1);
</script>
{% endhighlight %}


### refreshSpreadsheet()
{:#methods:refreshspreadsheet}
This method is used to refresh the Spreadsheet element based on the page layout.

#### Example
{% highlight html %}
<script>
//initialize the Spreadsheet object
var excelObj = $("#Spreadsheet").data("ejSpreadsheet");
excelObj.refreshSpreadsheet();
</script>
{% endhighlight %}

{% highlight html %}
<script>
$("#Spreadsheet").ejSpreadsheet("refreshSpreadsheet");
</script>
{% endhighlight %}

### refresh()
{:#methods:refresh}
This method destroys and re-creates the entire Spreadsheet control.

#### Example
{% highlight html %}
<script>
//initialize the Spreadsheet object
var excelObj = $("#Spreadsheet").data("ejSpreadsheet");
excelObj.refresh();
</script>
{% endhighlight %}

{% highlight html %}
<script>
$("#Spreadsheet").ejSpreadsheet("refresh");
</script>
{% endhighlight %}

### removeCustomFormula(formulaName, functionName)
{:#methods:removecustomformula}

This method is used to remove custom formulae in Spreadsheet.
<table class="params">
<thead>
<tr>
<th>Name</th>
<th>Type</th>
<th>Description</th>
</tr>
</thead>
<tbody>
<tr>
<td class="name">formulaName</td>
<td class="type"><span class="param-type">string</span></td>
<td class="description">Pass the name of the formula.</td>
</tr>
<tr>
<td class="name">functionName</td>
<td class="type"><span class="param-type">string</span></td>
<td class="description">Pass the name of the function.</td>
</tr>
</tbody>
</table>

{% highlight html %}
<script>
// Initialize the Spreadsheet object.
var excelObj = $("#Spreadsheet").data("ejSpreadsheet");
excelObj.removeCustomFormula("CUSTOMTOTAL","customTotal"); // Sends a remove custom formula request to the Spreadsheet.
function customTotal(args){}//args-It uses the value given by the user while using custom formula in Spreadsheet.
</script>
{% endhighlight %}

{% highlight html %}
<script>
// Sends a remove custom formula request to the Spreadsheet.
$("#Spreadsheet").ejSpreadsheet("removeCustomFormula","CUSTOMTOTAL","customTotal" ); 
function customTotal(args){}//args-It uses the value given by the user while using custom formula in Spreadsheet .      
</script>
{% endhighlight %}

### removeHyperlink(range, \[isClearHLink\], \[status\], \[cells\], \[skipHiddenRow\])
{:#methods:removehyperlink}

This method is used to remove the hyperlink from selected cells of current sheet.

<table class="params">
<thead>
<tr>
<th>Name</th>
<th>Type</th>
<th>Description</th>
</tr>
</thead>
<tbody>
<tr>
<td class="name">range</td>
<td class="type"><span class="param-type">string</span></td>
<td class="description">Hyperlink remove from the specified range.</td>
</tr>
<tr>
<td class="name">isClearHLink</td>
<td class="type"><span class="param-type">boolean</span></td>
<td class="description"><span class="optional">Optional.</span> If it is {{'`true`' | markdownify}}, It will clear link only not format.</td>
</tr>
<tr>
<td class="name">status</td>
<td class="type"><span class="param-type">boolean</span></td>
<td class="description"><span class="optional">Optional.</span> Pass the status to perform undo and redo operations.</td>
</tr>
<tr>
<td class="name">cells</td>
<td class="type"><span class="param-type">String|Array</span></td>
<td class="description"><span class="optional">Optional.</span> Pass the cells that you want to remove hyperlink.</td>
</tr>
<tr>
<td class="name">skipHiddenRow</td>
<td class="type"><span class="param-type">boolean</span></td>
<td class="description"><span class="optional">Optional.</span> Pass {{'`true`' | markdownify}}, if you want to skip the hidden rows.</td>
</tr>
</tbody>
</table>

#### Example

{% highlight html %}
<script>
// Initialize Spreadsheet object.
var excelObj = $("#Spreadsheet").data("ejSpreadsheet");
excelObj.removeHyperlink("A2:A3", false); // To remove the hyperlink  of specified range
</script>
{% endhighlight %}

{% highlight html %}
<script>
// To remove the hyperlink  of specified range
$("#Spreadsheet").ejSpreadsheet("removeHyperlink", "A2:A3", false);        
</script>

{% endhighlight %}

### removeRange(rangeName)
{:#methods:removerange}

This method is used to remove the range data and its defined rangeSettings property based on the specified range name.

<table class="params">
<thead>
<tr>
<th>Name</th>
<th>Type</th>
<th>Description</th>
</tr>
</thead>
<tbody>
<tr>
<td class="name">rangeName</td>
<td class="type"><span class="param-type">string</span></td>
<td class="description">Pass the defined rangeSetting property name.</td>
</tr>
</tbody>
</table>

#### Example

{% highlight html %}
<script>
// Initialize Spreadsheet object.
var excelObj = $("#Spreadsheet").data("ejSpreadsheet");
// Sends a remove range request to the Spreadsheet.
excelObj.removeRange("updateTable"); 
</script>

{% endhighlight %}

{% highlight html %}
<script>
// Sends a remove range request to the Spreadsheet.
$("#Spreadsheet").ejSpreadsheet("removeRange", "updateTable");
</script>

{% endhighlight %}

### removeReadOnly([range])
{:#methods:removereadonly}

This method is used to remove the readonly option for the specified range.

<table class="params">
<thead>
<tr>
<th>Name</th>
<th>Type</th>
<th>Description</th>
</tr>
</thead>
<tbody>
<tr>
<td class="name">range</td>
<td class="type"><span class="param-type">string|Array</span></td>
<td class="description">Pass the range.</td>
</tr>
</tbody>
</table>

#### Example

{% highlight html %}
<div id="Spreadsheet"></div>
<script>
// Initialize Spreadsheet object.
var excelObj = $("#Spreadsheet").data("ejSpreadsheet");
// Removes readonly option for the range.
excelObj.removeReadOnly("B3"); 
</script>

{% endhighlight %}

{% highlight html %}
<script>
// Removes readonly option for the range.
$("#Spreadsheet").ejSpreadsheet("removeReadOnly", "B3");
</script>

{% endhighlight %}

### saveAsJSON()
{:#methods:saveasjson}

This method is used to save JSON data in Spreadsheet.

#### Returns:
Object

#### Example

{% highlight html %}
<script>
//initialize the Spreadsheet object
var excelObj = $("#Spreadsheet").data("ejSpreadsheet");
excelObj.saveAsJSON();
</script>
{% endhighlight %}

{% highlight html %}
<script>
$("#Spreadsheet").ejSpreadsheet("saveAsJSON");
</script>

{% endhighlight %}

### saveBatchChanges(sheetIdx)
{:#methods:savebatchchanges}

This method is used to save batch changes in Spreadsheet.

<table class="params">
<thead>
<tr>
<th>Name</th>
<th>Type</th>
<th>Description</th>
</tr>
</thead>
<tbody>
<tr>
<td class="name">sheetIdx</td>
<td class="type"><span class="param-type">number</span></td>
<td class="description">Pass the sheet index for Spreadsheet.</td>
</tr>
</tbody>
</table>

#### Example

{% highlight html %}
<script>
//initialize the Spreadsheet object
var excelObj = $("#Spreadsheet").data("ejSpreadsheet");
//Set sheet index for Spreadsheet. 
excelObj.saveBatchChanges(1);
</script>

{% endhighlight %}

{% highlight html %}
<script>
//Set sheet index for Spreadsheet.
$("#Spreadsheet").ejSpreadsheet("saveBatchChanges", 1);
</script>

{% endhighlight %}

### setActiveCell(rowIdx, colIdx, sheetIdx)
{:#methods:setactivecell}

This method is used to set the active cell in the Spreadsheet.

<table class="params">
<thead>
<tr>
<th>Name</th>
<th>Type</th>
<th>Description</th>
</tr>
</thead>
<tbody>
<tr>
<td class="name">rowIdx</td>
<td class="type"><span class="param-type">number</span></td>
<td class="description">Pass the row index.</td>
</tr>
<tr>
<td class="name">colIdx</td>
<td class="type"><span class="param-type">number</span></td>
<td class="description">Pass the column index.</td>
</tr>
<tr>
<td class="name">sheetIdx</td>
<td class="type"><span class="param-type">number</span></td>
<td class="description">Pass the index of the sheet.</td>
</tr>
</tbody>
</table>

#### Example

{% highlight html %}
<script>
// Initialize Spreadsheet object.
var excelObj = $("#Spreadsheet").data("ejSpreadsheet");
excelObj.setActiveCell(1, 0, 1); // Sets activeCell in Spreadsheet.
</script>

{% endhighlight %}

{% highlight html %}
<script>
// Sets activeCell in Spreadsheet.
$("#Spreadsheet").ejSpreadsheet("setActiveCell", 1, 0, 1);
</script>

{% endhighlight %}

### setActiveSheetIndex(sheetIdx)
{:#methods:setactivesheetindex}

This method is used to set active sheet index for the Spreadsheet.

<table class="params">
<thead>
<tr>
<th>Name</th>
<th>Type</th>
<th>Description</th>
</tr>
</thead>
<tbody>
<tr>
<td class="name">sheetIdx</td>
<td class="type"><span class="param-type">number</span></td>
<td class="description">Pass the active sheet index for Spreadsheet.</td>
</tr>
</tbody>
</table>

#### Example

{% highlight html %}
<script>
var sheetIndex= 1;
//initialize the Spreadsheet object
var excelObj = $("#Spreadsheet").data("ejSpreadsheet");
//Set active sheet index for Spreadsheet. 
excelObj.setActiveSheetIndex(sheetIndex);
</script>

{% endhighlight %}

{% highlight html %}
<script>
//Set active sheet index for Spreadsheet.
$("#Spreadsheet").ejSpreadsheet("setActiveSheetIndex", sheetIndex);
</script>

{% endhighlight %}

### setBorder(property, \[range\])
{:#methods:setborder}

This method is used to set border for the specified range of cells in the Spreadsheet.

<table class="params">
<thead>
<tr>
<th>Name</th>
<th>Type</th>
<th>Description</th>
</tr>
</thead>
<tbody>
<tr>
<td class="name">property</td>
<td class="type"><ts ref="BorderOptions"/><span class="param-type">Object</span></td>
<td class="description">Pass the Object "BorderOptions".
<table class="params">
<thead>
<tr>
<th>Name</th>
<th>Type</th>
<th>Description</th>
</tr>
</thead>
<tbody>
<tr>
<td class="name">style</td>
<td class="type"><span class="param-type">string</span></td>
<td class="description">Pass the style to set border of the cell</td>
</tr>
<tr>
<td class="name">type</td>
<td class="type"><span class="param-type">string</span></td>
<td class="description">Pass the type to set border of the cell</td>
</tr>
<tr>
<td class="name">color</td>
<td class="type"><span class="param-type">string</span></td>
<td class="description">Pass the color to set border of the cell</td>
</tr>
</tbody>
</table>
</td></tr>
<tr>
<td class="name">range</td>
<td class="type"><span class="param-type">string</span></td>
<td class="description"><span class="optional">Optional.</span> If range is specified, it will set border for the specified range else it will use the selected range.</td>
</tr>
</tbody>
</table>

#### Example

{% highlight html %}
<script>
// Initialize Spreadsheet object.
var excelObj = $("#Spreadsheet").data("ejSpreadsheet");
excelObj.setBorder({ style: "solid", type: "outside", color: "#000000"}, "B2:B6"); // To set borders in Spreadsheet
</script>

{% endhighlight %}

{% highlight html %}
<script>
// To set borders in Spreadsheet.
$("#Spreadsheet").ejSpreadsheet("setBorder", { style: "solid", type: "outside", color: "#000000"}, "B2:B6");        
</script>

{% endhighlight %}

### setHeightToRows(heightColl)
{:#methods:setheighttorows}

This method is used to set the height for the rows in the Spreadsheet.

<table class="params">
<thead>
<tr>
<th>Name</th>
<th>Type</th>
<th>Description</th>
</tr>
</thead>
<tbody>
<tr>
<td class="name">heightColl</td>
<td class="type"><span class="param-type">Array|Object</span></td>
<td class="description">Pass the row index and height of the rows.</td></tr>
</tbody>
</table>

#### Example

{% highlight html %}
<div id="Spreadsheet"></div>
<script>
var heightRowObj= [{rowIndex: 2, height: 40}, {rowIndex: 3, height: 50}], heightRowArr = [50, 40];
//Initialize the Spreadsheet object
var excelObj = $("#Spreadsheet").data("ejSpreadsheet");
// Set height for specified rows in active sheet.
excelObj.setHeightToRows(heightRowObj);
// Set height for rows starting from the '0'th index in active sheet.
excelObj.setHeightToRows(heightRowArr);
</script>

{% endhighlight %}

{% highlight html %}
<script>
var heightRowObj= [{rowIndex: 2, height: 40}, {rowIndex: 3, height: 50}], heightRowArr = [50, 40];
// Set height for specified rows in active sheet.
$("#Spreadsheet").ejSpreadsheet("setHeightToRows", heightRowObj);
// Set height for rows starting from the '0'th index in active sheet.
$("#Spreadsheet").ejSpreadsheet("setHeightToRows", heightRowArr);

</script>

{% endhighlight %}

### setHyperlink(range, link, sheetIdx)
{:#methods:sethyperlink}

This method is used to set the hyperlink in selected cells of the current sheet.
<table class="params">
<thead>
<tr>
<th>Name</th>
<th>Type</th>
<th>Description</th>
</tr>
</thead>
<tbody>
<tr>
<td class="name">range</td>
<td class="type"><span class="param-type">string|Array</span></td>
<td class="description">If range is specified, it will set the hyperlink in range of the cells.</td>
</tr>
<tr>
<td class="name">link</td>
<td class="type"><ts ref="LinkOptions"/><span class="param-type">Object</span></td>
<td class="description">Pass the Object "LinkOptions"
<table class="params">
<thead>
<tr>
<th>Name</th>
<th>Type</th>
<th>Description</th>
</tr>
</thead>
<tbody>
<tr>
<td class="name">cellAddress</td>
<td class="type"><span class="param-type">string</span></td>
<td class="description">Pass the cell address in the cell</td>
</tr>
<tr>
<td class="name">text</td>
<td class="type"><span class="param-type">string</span></td>
<td class="description">Pass the text address in the cell</td>
</tr>
<tr>
<td class="name">webAddress</td>
<td class="type"><span class="param-type">string</span></td>
<td class="description">Pass the web address in the cell</td>
</tr>
</tbody>
</table>
</td></tr>
<tr>
<td class="name">sheetIdx</td>
<td class="type"><span class="param-type">number</span></td>
<td class="description">If we pass cellAddress then which sheet to be navigate in the applied link.</td>
</tr>
</tbody>
</table>

#### Example

{% highlight html %}

<script>
// Initialize Spreadsheet object.
var excelObj = $("#Spreadsheet").data("ejSpreadsheet");
excelObj.setHyperlink("A2:A3",{"cellAddr":"A2:A8"}, 3); // To set the hyperlink  of specified range.
</script>

{% endhighlight %}

{% highlight html %}
<script>
// To set the hyperlink  of specified range
$("#Spreadsheet").ejSpreadsheet("setHyperlink", "A2:A3",{"cellAddr":"A2:A8"},3);        
</script>

{% endhighlight %}

### setReadOnly([range])
{:#methods:setreadonly}

This method is used to set the readonly option for the specified range.

<table class="params">
<thead>
<tr>
<th>Name</th>
<th>Type</th>
<th>Description</th>
</tr>
</thead>
<tbody>
<tr>
<td class="name">range</td>
<td class="type"><span class="param-type">string|Array</span></td>
<td class="description">Pass the range.</td>
</tr>
</tbody>
</table>

#### Example

{% highlight html %}
<div id="Spreadsheet"></div>
<script>
// Initialize Spreadsheet object.
var excelObj = $("#Spreadsheet").data("ejSpreadsheet");
// Sets readonly option for the range.
excelObj.setReadOnly("B3"); 
</script>

{% endhighlight %}

{% highlight html %}
<script>
// Sets readonly option for the range.
$("#Spreadsheet").ejSpreadsheet("setReadOnly", "B3");
</script>

{% endhighlight %}

### setSheetFocus()
{:#methods:setsheetfocus}

This method is used to set the focus to the Spreadsheet.

#### Example

{% highlight html %}
<script>
//initialize the Spreadsheet object.
var excelObj = $("#Spreadsheet").data("ejSpreadsheet");
// Set focus on Spreadsheet.
excelObj.setSheetFocus();
</script>

{% endhighlight %}

{% highlight html %}
<script>
// Set focus on Spreadsheet.
$("#Spreadsheet").ejSpreadsheet("setSheetFocus");
</script>

{% endhighlight %}

### setWidthToColumns(widthColl, \[sheetIndex\])
{:#methods:setwidthtocolumns}

This method is used to set the width for the columns in the Spreadsheet.
<table class="params">
<thead>
<tr>
<th>Name</th>
<th>Type</th>
<th>Description</th>
</tr>
</thead>
<tbody>
<tr>
<td class="name">widthColl</td>
<td class="type"><span class="param-type">Array|Object</span></td>
<td class="description">Pass the column index and width of the columns.</td>
</tr>
<tr>
<td class="name">sheetIndex</td>
<td  class="type"><span class="param-type">Number</span></td>
<td  class="description">Optional. If sheetIdx is specified, it will set the width for columns to the specified sheet else it will use active sheet.</td>
</tr>
</tbody>
</table>

#### Example

{% highlight html %}
<script>
var widthCollObj= [{colIndex: 2, width: 40}, {colIndex: 3, width: 50}], widthCollArr = [80, 90];
//initialize the Spreadsheet object
var excelObj = $("#Spreadsheet").data("ejSpreadsheet");
// Set width for specified columns in active sheet
excelObj.setWidthToColumns(widthCollObj);
// Set width for columns starting from the '0'th index in second sheet.
excelObj.setWidthToColumns(widthCollArr, 2);
</script>

{% endhighlight %}

{% highlight html %}
<script>
// Set width for specified columns in active sheet.
$("#Spreadsheet").ejSpreadsheet("setWidthToColumns", widthCollObj);
// Set width for columns starting from the '0'th index in second sheet.
$("#Spreadsheet").ejSpreadsheet("setWidthToColumns", widthCollArr, 2);

</script>

{% endhighlight %}

### sheetRename(sheetName)
{:#methods:sheetrename}

This method is used to rename the active sheet.
<table class="params">
<thead>
<tr>
<th>Name</th>
<th>Type</th>
<th>Description</th>
</tr>
</thead>
<tbody>
<tr>
<td class="name">sheetName</td>
<td class="type"><span class="param-type">string</span></td>
<td class="description">Pass the sheet name that you want to change the current active sheet name.</td>
</tr>
</tbody>
</table>

#### Example

{% highlight html %}
<script>
// Initialize Spreadsheet object.
var excelObj = $("#Spreadsheet").data("ejSpreadsheet");
excelObj.sheetRename("Sep-Billing"); // Sends a sheet rename request to the Spreadsheet
</script>

{% endhighlight %}

{% highlight html %}
<script>
// To rename a sheet in Spreadsheet
$("#Spreadsheet").ejSpreadsheet("sheetRename", "Sep-Billing");        
</script>

{% endhighlight %}

### showActivationPanel(rangeName)
{:#methods:showactivationpanel}

This method is used to display the activationPanel for the specified range name.
<table class="params">
<thead>
<tr>
<th>Name</th>
<th>Type</th>
<th>Description</th>
</tr>
</thead>
<tbody>
<tr>
<td class="name">rangeName</td>
<td class="type"><span class="param-type">string</span></td>
<td class="description">Pass the range name that you want to display the activation panel.</td>
</tr>
</tbody>
</table>

#### Example

{% highlight html %}
<script>
// Initialize Spreadsheet object.
var excelObj = $("#Spreadsheet").data("ejSpreadsheet");
excelObj.showActivationPanel("upTable"); // To display the activationPanel in Spreadsheet
</script>

{% endhighlight %}

{% highlight html %}
<script>
// To display the activationPanel in Spreadsheet
$("#Spreadsheet").ejSpreadsheet("showActivationPanel", "upTable");        
</script>

{% endhighlight %}

### showColumn(startCol, endCol)
{:#methods:showcolumn}

This method is used to show the hidden columns within the specified range in the Spreadsheet.
<table class="params">
<thead>
<tr>
<th>Name</th>
<th>Type</th>
<th>Description</th>
</tr>
</thead>
<tbody>
<tr>
<td class="name">startColIdx</td>
<td class="type"><span class="param-type">number</span></td>
<td class="description">Index of the start column.</td>
</tr>
<tr>
<td class="name">endColIdx</td>
<td class="type"><span class="param-type">number</span></td>
<td class="description">Optional. Index of the end column.</td>
</tr>
</tbody>
</table>

#### Example

{% highlight html %}
<script>
//initialize the Spreadsheet object
var excelObj = $("#Spreadsheet").data("ejSpreadsheet");
// show the hidden column by passing column index in the active sheet.
excelObj.showColumn(1);
// show the hidden columns from startColIdx to startColIdx in the active sheet.
excelObj.showColumn(3, 6);

</script>

{% endhighlight %}

{% highlight html %}
<script>
// show the hidden column by passing column index in the active sheet.
$("#Spreadsheet").ejSpreadsheet("showColumn", 1);
// show the hidden columns from startColIdx to startColIdx in the active sheet.
$("#Spreadsheet").ejSpreadsheet("showColumn", 3, 6);
</script>

{% endhighlight %}

### showFormulaBar()
{:#methods:showformulabar}

This method is used to show the formula bar in Spreadsheet.

#### Example

{% highlight html %}
<script>
//initialize the Spreadsheet object
var excelObj = $("#Spreadsheet").data("ejSpreadsheet");
//To show the formula bar in Spreadsheet
excelObj.showFormulaBar();
</script>

{% endhighlight %}

{% highlight html %}
<script>
// To show the formula bar in Spreadsheet.
$("#Spreadsheet").ejSpreadsheet("showFormulaBar ");
</script>

{% endhighlight %}

### showGridlines(status)
{:#methods:showgridlines}

This method is used to show/hide gridlines in active sheet in the Spreadsheet.
<table class="params">
<thead>
<tr>
<th>Name</th>
<th>Type</th>
<th>Description</th>
</tr>
</thead>
<tbody>
<tr>
<td class="name">status</td>
<td class="type"><span class="param-type">boolean</span></td>
<td class="description">Pass {{'`true`' | markdownify}} to show the gridlines</td>
</tr>
</tbody>
</table>

#### Example

{% highlight html %}
<script>
// Initialize the Spreadsheet object.
var excelObj = $("#Spreadsheet").data("ejSpreadsheet");
// To hide the gridlines in the sheet.
excelObj.showGridlines(false);
</script>

{% endhighlight %}

{% highlight html %}
<script>
// hide the gridlines in the sheet.
$("#Spreadsheet").ejSpreadsheet("showGridlines", false);
</script>

{% endhighlight %}

### showHeadings(status)
{:#methods:showheadings}

This method is used to show/hide the headers in active sheet in the Spreadsheet.
<table class="params">
<thead>
<tr>
<th>Name</th>
<th>Type</th>
<th>Description</th>
</tr>
</thead>
<tbody>
<tr>
<td class="name">startRow</td>
<td class="type"><span class="param-type">boolean</span></td>
<td class="description">Pass {{'`true`' | markdownify}} to show the sheet headers.</td>
</tr>
</tbody>
</table>

#### Example

{% highlight html %}
<script>
// Initialize the Spreadsheet object.
var excelObj = $("#Spreadsheet").data("ejSpreadsheet");
// To hide the headers in the sheet.
excelObj.showHeadings(false);
</script>
{% endhighlight %}

{% highlight html %}
<script>
// To hide the headers in the sheet.
$("#Spreadsheet").ejSpreadsheet("showHeadings", false);
</script>

{% endhighlight %}

### showPager(status)
{:#methods:showpager}

This method is used to show/hide pager in the Spreadsheet.

<table class="params">
<thead>
<tr>
<th>Name</th>
<th>Type</th>
<th>Description</th>
</tr>
</thead>
<tbody>
<tr>
<td class="name">status</td>
<td class="type"><span class="param-type">boolean</span></td>
<td class="description">Pass {{'`true`' | markdownify}} to show pager.</td>
</tr>
</tbody>
</table>

{% highlight html %}
<div id="Spreadsheet"></div>
<script>
// Initialize the Spreadsheet object.
var excelObj = $("#Spreadsheet").data("ejSpreadsheet");
excelObj.showPager(false); // Gets or sets the value to show/hide pager.
</script>

{% endhighlight %}

{% highlight html %}
<script>
// Gets or sets the value to show/hide pager.
$("#Spreadsheet").ejSpreadsheet("showPager",false);
</script>

{% endhighlight %}

### showRow(startRow, endRow)
{:#methods:showrow}

This method is used to show the hidden rows in the specified range in the Spreadsheet. 
<table class="params">
<thead>
<tr>
<th>Name</th>
<th>Type</th>
<th>Description</th>
</tr>
</thead>
<tbody>
<tr>
<td class="name">startRow</td>
<td class="type"><span class="param-type">number</span></td>
<td class="description">Index of the start row.</td>
</tr>
<tr>
<td class="name">endRow</td>
<td class="type"><span class="param-type">number</span></td>
<td class="description">Optional. Index of the end row.</td>
</tr>
</tbody>
</table>

#### Example

{% highlight html %}
<script>
// Initialize the Spreadsheet object.
var excelObj = $("#Spreadsheet").data("ejSpreadsheet");
// show the hidden row by passing row index in the active sheet.
excelObj.showRow(1);
// To show the hidden rows for startRow to endRow in the active sheet.
excelObj.showRow(3, 6);
</script>

{% endhighlight %}

{% highlight html %}
<script>
// show the hidden row by passing row index in the active sheet.
$("#Spreadsheet").ejSpreadsheet("showRow", 1);
// To show the hidden rows for startRow to endRow in the active sheet.
$("#Spreadsheet").ejSpreadsheet("showRow", 3, 6);
</script>

{% endhighlight %}

### showWaitingPopUp()
{:#methods:showwaitingpopup}

This method is used to show waiting pop-up in Spreadsheet.

#### Example

{% highlight html %}
<script>
//initialize the Spreadsheet object
var excelObj = $("#Spreadsheet").data("ejSpreadsheet");
// To show waiting popup in Spreadsheet
excelObj.showWaitingPopUp();
</script>

{% endhighlight %}

{% highlight html %}
<script>
// show waiting popup in the Spreadsheet
$("#Spreadsheet").ejSpreadsheet("showWaitingPopUp");
</script>

{% endhighlight %}

### undo()
{:#methods:undo}

This method is used to perform the undo action in Spreadsheet.

#### Example

{% highlight html %}
<script>
// Initialize the Spreadsheet object.
var excelObj = $("#Spreadsheet").data("ejSpreadsheet");
// To perform undo action in Spreadsheet
excelObj.undo();
</script>

{% endhighlight %}

### unhideSheet(sheetInfo)
{:#methods:unhidesheet}

This method is used to unhide the sheet based on specified sheet name or sheet index.
<table class="params">
<thead>
<tr>
<th>Name</th>
<th>Type</th>
<th>Description</th>
</tr>
</thead>
<tbody>
<tr>
<td class="name">sheetInfo</td>
<td class="type"><span class="param-type">string|number</span></td>
<td class="description">Pass the sheet name or index that you want to unhide.</td>
</tr>
</tbody>
</table>

#### Example

{% highlight html %}
<script>
//Initialize Spreadsheet object.
var excelObj = $("#Spreadsheet").data("ejSpreadsheet");
//To unhide a sheet in Spreadsheet.
excelObj.unhideSheet("Sheet2");
</script>

{% endhighlight %}

{% highlight html %}
<script>
//To unhide a sheet in Spreadsheet.
$("#Spreadsheet").ejSpreadsheet("unhideSheet", "Sheet2");
</script>

{% endhighlight %}

### unmergeCells(\[range\])
{:#methods:unmergecells}

This method is used to unmerge the selected range of cells in the Spreadsheet.
<table class="params">
<thead>
<tr>
<th>Name</th>
<th>Type</th>
<th>Description</th>
</tr>
</thead>
<tbody>
<tr>
<td class="name">range</td>
<td class="type"><span class="param-type">string</span></td>
<td class="description"><span class="optional">Optional.</span> If the range is specified, then it will un merge the specified range else it will use the current selected range.</td>
</tr>
</tbody>
</table>

#### Example

{% highlight html %}
<script>
// Initialize Spreadsheet object.
var excelObj = $("#Spreadsheet").data("ejSpreadsheet");
// To unmerge the selected cells in Spreadsheet.
excelObj.unmergeCells("A3:B5"); 
</script>

{% endhighlight %}

{% highlight html %}
<script>
// To unmerge the selected cells in Spreadsheet.
$("#Spreadsheet").ejSpreadsheet("unmergeCells","A3:B5");        
</script>

{% endhighlight %}

### unWrapText(\[range\])
{:#methods:unwraptext}

This method is used to unwrap the selected range of cells in the Spreadsheet.
<table class="params">
<thead>
<tr>
<th>Name</th>
<th>Type</th>
<th>Description</th>
</tr>
</thead>
<tbody>
<tr>
<td class="name">range</td>
<td class="type"><span class="param-type">Array|string</span></td>
<td class="description"><span class="optional">Optional.</span> If the range is specified, then it will update unwrap in the specified <br/>range else it will use the current selected range.</td>
</tr>
</tbody>
</table>

#### Example

{% highlight html %}
<script>
//Initialize the Spreadsheet object.
var excelObj = $("#Spreadsheet").data("ejSpreadsheet");
// To unwrap the cell text.
excelObj.unWrapText("A1:B3");
</script>

{% endhighlight %}

{% highlight html %}
<script>
// To unwrap the cell text.
$("#Spreadsheet").ejSpreadsheet("unWrapText","A1:B3")
</script>

{% endhighlight %}

### updateData(data, \[range\])
{:#methods:updatedata}

This method is used to update the data for the specified range of cells in the Spreadsheet.
<table class="params">
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
<td class="type"><ts ref="DataOptions"/><span class="param-type">Object</span></td>
<td class="description">Pass the Object "DataOptions"
<table class="params">
<thead>
<tr>
<th>Name</th>
<th>Type</th>
<th>Description</th>
</tr>
</thead>
<tbody>
<tr>
<td class="name">value</td>
<td class="type"><span class="param-type">number</span></td>
<td class="description">Pass the value to update</td>
</tr>
<tr>
<td class="name">value2</td>
<td class="type"><span class="param-type">number</span></td>
<td class="description">Pass the value2 to update</td>
</tr>
<tr>
<td class="name">type</td>
<td class="type"><span class="param-type">string</span></td>
<td class="description">Pass the type to update</td>
</tr>
</tbody>
</table>
</td></tr>
<tr>
<td class="name">range</td>
<td class="type"><span class="param-type">Array|string</span></td>
<td class="description"><span class="optional">Optional.</span> If range is specified, it will update data for the specified range <br/> else it will use the current selected range. </td>
</tr>
</tbody>
</table>

#### Example

{% highlight html %}
<script>
// Initialize Spreadsheet object.
var excelObj = $("#Spreadsheet").data("ejSpreadsheet");
// To update data in the specified range of the cells in Spreadsheet.
excelObj.updateData([{ value: 10, value2: 10, type: "general"}, { value: 25000, value2: 25000, type: "general"}], "A3"); 
</script>

{% endhighlight %}

{% highlight html %}
<script>
// To update a data in the specified range of cells in Spreadsheet.
$("#Spreadsheet").ejSpreadsheet("updateData", [{ value: 10, value2: 10, type: "general"}, { value: 25000, value2: 25000, type: "general"}], "A3");        
</script>

{% endhighlight %}

### updateFormulaBar()
{:#methods:updateformulabar}

This method is used to update the formula bar in the Spreadsheet.

#### Example

{% highlight html %}
<script>
//initialize the Spreadsheet object
var excelObj = $("#Spreadsheet").data("ejSpreadsheet");
//To update the formula bar in Spreadsheet
excelObj.updateFormulaBar();
</script>

{% endhighlight %}

### updateRange(sheetIdx, settings)
{:#methods:updaterange}

This method is used to update the range of cells based on the specified settings which we want to update in the Spreadsheet.
<table class="params">
<thead>
<tr>
<th>Name</th>
<th>Type</th>
<th>Description</th>
</tr>
</thead>
<tbody>
<tr>
<td class="name">sheetIdx</td>
<td class="type"><span class="param-type">number</span></td>
<td class="description">Pass the sheet index that you want to update.</td>
</tr>
<tr>
<td class="name">settings</td>
<td class="type"><ts ref="RangeOptions"/><span class="param-type">Object</span></td>
<td class="description">Pass the Object "RangeOptions"
<table class="params">
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
<td class="type"><span class="param-type">object</span></td>
<td class="description">Pass the datasource object values as settings</td>
</tr>
<tr>
<td class="name">showHeader</td>
<td class="type"><span class="param-type">boolean</span></td>
<td class="description">Pass the showheader condition as settings</td>
</tr>
<tr>
<td class="name">startCell</td>
<td class="type"><span class="param-type">string</span></td>
<td class="description">Pass the startcell values as settings</td>
</tr>
</tbody>
</table>
</td></tr>
</tbody>
</table>

#### Example

{% highlight html %}
<script>
// Initialize Spreadsheet object.
var excelObj = $("#Spreadsheet").data("ejSpreadsheet");
var settings = { dataSource: [{ Product: "XYZ", Price: "2000" }], showHeader: "true", startCell: "F1" };
// To update range of cells with the specified settings
excelObj.updateRange(1, settings); 
</script>

{% endhighlight %}

{% highlight html %}
<script>
var settings = { dataSource: [{ Product: "XYZ", Price: "2000" }], showHeader: "true", startCell: "F1" };
// To update cells range of cells with the specified settings
$("#Spreadsheet").ejSpreadsheet("updateRange", 1, settings);        
</script>

{% endhighlight %}

### updateUndoRedoCollection(details)
{:#methods:updateundoredocollection}

This method is used to update the details for custom undo and redo operations.

<table class="params">
<thead>
<tr>
<th>Name</th>
<th>Type</th>
<th>Description</th>
</tr>
</thead>
<tbody>
<tr>
<td class="name">details</td>
<td class="type"><ts ref="UndoRedoOptions"/><span class="param-type">Object</span></td>
<td class="description">Pass the Object "UndoRedoOptions"
<table class="params">
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
<td class="description">Pass the action to update undo and redo collection</td>
</tr>
<tr>
<td class="name">cell</td>
<td class="type"><span class="param-type">element</span></td>
<td class="description">Pass the cell to update undo and redo collection</td>
</tr>
<tr>
<td class="name">sheetIndex</td>
<td class="type"><span class="param-type">number</span></td>
<td class="description">Pass the sheet index to update undo and redo collection</td>
</tr>
</tbody>
</table>
</td></tr>
</tbody>
</table>

#### Example

{% highlight html %}
<div id="Spreadsheet"></div>
<script>
// Initialize Spreadsheet object.
var excelObj = $("#Spreadsheet").data("ejSpreadsheet"), details = { action: "custom", cell: excelObj.getActiveCell(), sheetIndex: 1 };
// To update undo and redo collections.
excelObj.updateUndoRedoCollection(details); 
</script>

{% endhighlight %}

{% highlight html %}
<script>
var excelObj = $("#Spreadsheet").data("ejSpreadsheet"), details = { action: "custom", cell: excelObj.getActiveCell() };
// To update undo and redo collections.
$("#Spreadsheet").ejSpreadsheet("updateUndoRedoCollection", details);        
</script>

{% endhighlight %}

### updateUniqueData(data, \[range\], \[skipCell\])
{:#methods:updateuniquedata}

This method is used to update the unique data for the specified range of cells in Spreadsheet.
<table class="params">
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
<td class="type"><ts ref="DataOptions"/><span class="param-type">Object</span></td>
<td class="description"><span>Pass the Object "DataOptions"</span>
<table class="params">
<thead>
<tr>
<th>Name</th>
<th>Type</th>
<th>Description</th>
</tr>
</thead>
<tbody>
<tr>
<td class="name">value</td>
<td class="type"><span class="param-type">number<</span></td>
<td class="description">Pass the value to update in particular range</td>
</tr>
<tr>
<td class="name">value2</td>
<td class="type"><span class="param-type">number</span></td>
<td class="description">Pass the value2 to update in particular range</td>
</tr>
<tr>
<td class="name">type</td>
<td class="type"><span class="param-type">string</span></td>
<td class="description">Pass the type to update in particular range</td>
</tr>
</tbody>
</table>
</td></tr>
<tr>
<td class="name">range</td>
<td class="type"><span class="param-type">Array|string</span></td>
<td class="description"><span class="optional">Optional.</span> If range is specified, it will update data for the specified range else it will use the current selected range.</td>
</tr>
<tr>
<td class="name">skipCell</td>
<td class="type"><span class="param-type">boolean</span></td>
<td class="description"><span class="optional">Optional.</span> It specifies whether to skip element processing or not.
</td></tr>
</tbody>
</table>

#### Example

{% highlight html %}
<script>
// Initialize Spreadsheet object.
var excelObj = $("#Spreadsheet").data("ejSpreadsheet");
// To update unique data in Spreadsheet.
excelObj.updateUniqueData({ value: 10, value2: 10, type: "general"}, [1, 0, 5, 0]); 
</script>

{% endhighlight %}

{% highlight html %}
<script>
// To update unique data in Spreadsheet.
$("#Spreadsheet").ejSpreadsheet("updateUniqueData", [{ value: 10, value2: 10, type: "general"}], [1, 0, 5, 0]);        
</script>

{% endhighlight %}

### wrapText(\[range\])
{:#methods:wraptext}

This method is used to wrap the selected range of cells in the Spreadsheet.
<table class="params">
<thead>
<tr>
<th>Name</th>
<th>Type</th>
<th>Description</th>
</tr>
</thead>
<tbody>
<tr>
<td class="name">range</td>
<td class="type"><span class="param-type">Array|string</span></td>
<td class="description"><span class="optional">Optional.</span> If the range is specified, then it will update wrap in the specified <br/> range else it will use the current selected range.</td>
</tr>
</tbody>
</table>

#### Example

{% highlight html %}
<script>
//Initialize the Spreadsheet object.
var excelObj = $("#Spreadsheet").data("ejSpreadsheet");
// To wrap the cell Text.
excelObj.wrapText("A1:B3");
</script>

{% endhighlight %}

{% highlight html %}
<script>
// To wrap the cell Text.
$("#Spreadsheet").ejSpreadsheet("wrapText","A1:B3")
</script>

{% endhighlight %}

### XLCellType
{:#methods:xlcelltype}

### XLCellType.addCellTypes(range, settings, \[sheetIdx\])
{:#methods:xlcelltype-addcelltypes}

This method is used to set a cell type from the specified range of cells in the spreadsheet.
<table class="params">
<thead>
<tr>
<th>Name</th>
<th>Type</th>
<th>Description</th>
</tr>
</thead>
<tbody>
<tr>
<td class="name">range</td>
<td class="type"><span class="param-type">string</span></td>
<td class="description">Pass the range where you want apply cell type.</td>
</tr>
<tr>
<td class="name">settings</td>
<td class="type"><ts ref="CellTypeSettings"/><span class="param-type">object</span></td>
<td class="description">Pass the Object "CellTypeSettings"
<table class="params">
<thead>
<tr>
<th>Name</th>
<th>Type</th>
<th>Description</th>
</tr>
</thead>
<tbody>
<tr>
<td class="name">type</td>
<td class="type"><ts name="ej.Spreadsheet.CustomCellType"/><span class="param-type">enum</span></td>
<td class="description">Specifies the button type of Custom Cell type.</td>
</tr>
<tr>
<td class="name">text</td>
<td class="type"><span class="param-type">string</span></td>
<td class="description">Specifies the button text of Custom Cell type.</td>
</tr>
<tr>
<td class="name">backgroundColor</td>
<td class="type"><span class="param-type">string</span></td>
<td class="description">Specifies the button background color of Custom Cell type.</td>
</tr>
<tr>
<td class="name">dataSourceRange</td>
<td class="type"><span class="param-type">string</span></td>
<td class="description">Specifies the dropdown list data source range of Custom Cell type.</td>
</tr>
<tr>
<td class="name">dataSourceSheetIndex</td>
<td class="type"><span class="param-type">number</span></td>
<td class="description">Specifies the dropdown list data source sheet index of Custom Cell type.</td>
</tr>
<tr>
<td class="name">field</td>
<td class="type"><span class="param-type">object</span></td>
<td class="description">Specifies the text and value of field in dropdown list.</td>
</tr>
<tr>
<td class="name">isChecked</td>
<td class="type"><span class="param-type">boolean</span></td>
<td class="description">Specifies the checkbox is set true or false of Custom Cell type.</td>
</tr>
<tr>
<td class="name">value</td>
<td class="type"><span class="param-type">string</span></td>
<td class="description">Specifies the datepicker of Custom Cell type.</td>
</tr>
</tbody>
</table>
</td></tr>
<tr>
<td class="name">sheetIdx</td>
<td class="type"><span class="param-type">number</span></td>
<td class="description">Optional. Pass sheet index.</td>
</tr>
</tbody>
</table>

#### Example

{% highlight html %}
<script>
// Initialize the Spreadsheet object.
var excelObj = $("#Spreadsheet").data("ejSpreadsheet");
 var customList = [{ id: "1", text: "ALFKI" }, { id: "2", text: "ANATR" }, { id: "3", text: "ANTON" }, { id: "4", text: "AROUT" }, { id: "5", text: "BERGS" }, { id: "6", text: "BLAUS" }];
// To add button cell type in Spreadsheet.
excelObj.XLCellType.addCellTypes("A1:B3", {"type" : ej.Spreadsheet.CustomCellType.Button, "text" : "Button1", "background-color" : "green" },  1);
// To add dropdownlist cell type in spreadsheet.
excelObj.XLCellType.addCellTypes("A1:B3", { 'type': ej.Spreadsheet.CustomCellType.DropDownList, 'dataSourceRange': 'A2:A23', 'dataSourceSheetIndex': 1 }, 2);
// To add the dropdownlist with custom datasource in Spreadsheet.
 this.XLCellType.addCellTypes("A1:B3", { 'type': ej.Spreadsheet.CustomCellType.DropDownList, 'dataSource': customList, 'field': "text" });
//To add checkbox cell type in spreadsheet.
excelObj.XLCellType.addCellTypes("A1:B3", { 'type': ej.Spreadsheet.CustomCellType.CheckBox, isChecked:true});
//To add date picker cell type in spreadsheet.
xlObj.XLCellType.addCellTypes("B1", { 'type': ej.Spreadsheet.CustomCellType.DatePicker, 'value': '2/12/2016'});
</script>

{% endhighlight %}

#### CustomCellType

Specifies the cell type in the Spreadsheet,

<table class="props">
<thead>
<tr>
<th>Name</th>
<th>Description</th>
</tr>
</thead>
<tbody>
<tr>
<td>Button</td>
<td>To insert the Button in cell.</td>
</tr>
<tr>
<td>CheckBox</td>
<td>To insert the Checkbox in cell.</td>
</tr>
<tr>
<td>DatePicker</td>
<td>To insert the Datepicker in cell.</td>
</tr>
<tr>
<td>DropDownList</td>
<td>To insert the Dropdownlist in cell.</td>
</tr>
</tbody>
</table>


### XLCellType.removeCellTypes(range, \[sheetIdx\])
{:#methods:xlcelltype-removecelltypes}

This method is used to remove cell type from the specified range of cells in the Spreadsheet.
<table class="params">
<thead>
<tr>
<th>Name</th>
<th>Type</th>
<th>Description</th>
</tr>
</thead>
<tbody>
<tr>
<td class="name">range</td>
<td class="type"><span class="param-type">string|Array</span></td>
<td class="description">Pass the range where you want remove cell type.</td>
</tr>
<tr>
<td class="name">sheetIdx</td>
<td class="type"><span class="param-type">number</span></td>
<td class="description"><span class="optional">Optional.</span> Pass sheet index.</td>
</tr>
</tbody>
</table>

#### Example

{% highlight html %}
<script>
// Initialize the Spreadsheet object.
var excelObj = $("#Spreadsheet").data("ejSpreadsheet");
// To remove cell types in Spreadsheet.
excelObj.XLCellType.removeCellTypes("A1:B2", 1);
</script>

{% endhighlight %}

### XLCFormat
{:#methods:xlcformat}

### XLCFormat.clearCF(\[range\])
{:#methods:xlcformat-clearcf}

This method is used to clear the applied conditional formatting rules in the Spreadsheet.
<table class="params">
<thead>
<tr>
<th>Name</th>
<th>Type</th>
<th>Description</th>
</tr>
</thead>
<tbody>
<tr>
<td class="name">range</td>
<td class="type"><span class="param-type">Array|string</span></td>
<td class="description"><span class="optional">Optional.</span> If range is specified, it will clear rules for the specified range else it will use the current selected range.</td>
</tr>
</tbody>
</table>

#### Example

{% highlight html %}
<script>
// Initialize the Spreadsheet object.
var excelObj = $("#Spreadsheet").data("ejSpreadsheet");
// To clear conditional formatting rules in Spreadsheet.
excelObj.XLCFormat.clearCF([1, 0, 7, 0]);
</script>

{% endhighlight %}

### XLCFormat.getCFRule(rowIdx, colIdx)
{:#methods:xlcformat-getcfrule}

This method is used to get the applied conditional formatting rules as array of objects based on the specified row Index and column Index in the Spreadsheet.
<table class="params">
<thead>
<tr>
<th>Name</th>
<th>Type</th>
<th>Description</th>
</tr>
</thead>
<tbody>
<tr>
<td class="name">rowIdx</td>
<td class="type"><span class="param-type">number</span></td>
<td class="description">Pass the row index.</td>
</tr>
<tr>
<td class="name">colIdx</td>
<td class="type"><span class="param-type">number</span></td>
<td class="description">Pass the column index.</td>
</tr>
</tbody>
</table>

#### Returns:
Array

#### Example

{% highlight html %}
<div id="Spreadsheet"></div> 
<script>
// Initialize the Spreadsheet object.
var excelObj = $("#Spreadsheet").data("ejSpreadsheet");
// Gets the conditional formatting rules in Spreadsheet.
excelObj.XLCFormat.getCFRule(2, 0);
</script>

{% endhighlight %}

### XLCFormat.setCFRule(rule)
{:#methods:xlcformat-setcfrule}

This method is used to set the conditional formatting rule in the Spreadsheet.

<table class="params">
<thead>
<tr>
<th>Name</th>
<th>Type</th>
<th>Description</th>
</tr>
</thead>
<tbody>
<tr>
<td class="name">rule</td>
<td class="type"><ts ref="CFormatOptions"/><span class="param-type">Object</span></td>
<td class="description">Pass the Object "CFormatOptions"
<table class="params">
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
<td class="description">Pass the condition to set the conditional formatting</td>
</tr>
<tr>
<td class="name">color</td>
<td class="type"><span class="param-type">string</span></td>
<td class="description">Pass the color to set the conditional formatting</td>
</tr>
<tr>
<td class="name">inputs</td>
<td class="type"><span class="param-type">array|string</span></td>
<td class="description">Pass the inputs to set the conditional formatting</td>
</tr>
<tr>
<td class="name">bgColor</td>
<td class="type"><span class="param-type">string</span></td>
<td class="description">Pass the bgColor to set the conditional formatting</td>
</tr>
<tr>
<td class="name">range</td>
<td class="type"><span class="param-type">string</span></td>
<td class="description">Pass the range to set the conditional formatting</td>
</tr>
</tbody>
</table>
</td></tr>
</tbody>
</table>

#### Example

{% highlight html %}
<script>
//initialize the Spreadsheet object
var excelObj = $("#Spreadsheet").data("ejSpreadsheet");
// Sets the conditional formatting rules in Spreadsheet
excelObj.XLCFormat.setCFRule({ action: "lessthan", inputs: ["30"], color: "yellowft", range: "H3:H7" });
</script>

{% endhighlight %}

### XLChart
{:#methods:xlchart}

### XLChart.changeTheme(chartId, theme)
{:#methods:xlchart-changetheme}

This method is used to change the theme of the chart in the Spreadsheet.

<table>
<tr>
<th>Name</th>
<th>Type</th>
<th>Description</th></tr>
<tr>
<td class="name">chartId</td>
<td class="type"><span class="param-type">string</span></td>
<td class="description">Pass the chart id.</td></tr>
<tr>
<td class="name">theme</td>
<td class="type"><ts ref="ej.datavisualization.Chart.Theme"/>enum</td>
<td class="description">Pass the chart theme which want to update.</td>
</tr>
</table>

#### Example

{% highlight html %}

<div id="Spreadsheet"></div> 
<script>
// Initialize Spreadsheet object.
var excelObj = $("#Spreadsheet").data("ejSpreadsheet"), chartId = "Spreadsheet_chart1"
var theme = ej.datavisualization.Chart.Theme.Azuredark;
excelObj.XLChart.changeTheme(chartId, theme); // To update chart theme.
</script>

{% endhighlight %}

N> You can use the supported [chart themes](https://help.syncfusion.com/api/js/ejchart#members:theme).

### XLChart.changeType(chartId, option)
{:#methods:xlchart-changetype}

This method is used to change the type of the chart in the Spreadsheet.

<table>
<tr>
<th>Name</th>
<th>Type</th>
<th>Description</th></tr>
<tr>
<td class="name">chartId</td>
<td class="type"><span class="param-type">string</span></td>
<td class="description">Pass the chart id.</td></tr>
<tr>
<td class="name">option</td>
<td class="type"><ts ref="ChartOptions"/><span class="param-type">Object</span></td>
<td class="description">Pass Object ChartOptions.
<table class="params">
<thead>
<tr>
<th>Name</th>
<th>Type</th>
<th>Description</th>
</tr>
</thead>
<tbody>
<tr>
<td class="name">type</td>
<td class="type"><span class="param-type">string</span></td>
<td class="description">Pass the chart type</td>
</tr>
<tr>
<td class="name">enable3D</td>
<td class="type"><span class="param-type">boolean</span></td>
<td class="description">Pass the enable3D condition</td>
</tr>
<tr>
<td class="name">marker</td>
<td class="type"><span class="param-type">object</span></td>
<td class="description">Pass the marker object to change type</td>
</tr>
</tbody>
</table>
</td></tr>
</table>

#### Example

{% highlight html %}

<div id="Spreadsheet"></div> 
<script>
// Initialize Spreadsheet object.
var excelObj = $("#Spreadsheet").data("ejSpreadsheet"), chartId = "Spreadsheet_chart1"
excelObj.XLChart.changeType(chartId,{type: "radar", enable3D: false, marker: {visible: false}} ); // To change chart type.
</script>

{% endhighlight %}

### XLChart.changeDataRange(chartId, xRange, yRange, lRange)
{:#methods:xlchart-changedatarange}

This method is used to change the data range of the chart in the Spreadsheet.

<table>
<tr>
<th>
Name</th><th>
Type</th><th>
Description</th></tr>
<tr>
<td>
chartId</td><td>
string</td><td>
Pass the chart id.</td></tr>
<tr>
<td>
xRange</td><td>
string</td><td>
X axis range of chart data.</td></tr>
<tr>
<td>
yRange</td><td>
string</td><td>
Y axis range of chart data.</td></tr>
<tr>
<td>
lRange</td><td>
string</td><td>
Legend range of chart data.</td></tr>
</table>

#### Example

{% highlight html %}

<div id="Spreadsheet"></div> 
<script>
// Initialize Spreadsheet object.
var excelObj = $("#Spreadsheet").data("ejSpreadsheet"), chartId = "Spreadsheet_chart1";
excelObj.XLChart.changeDataRange(chartId, "A2:A7", "A2:B5", "A1:B1"); // To change the data range of the chart.
</script>

{% endhighlight %}


### XLChart.createChart(\[range\], \[options\])
{:#methods:xlchart-createchart}

This method is used to create a chart for specified range in Spreadsheet.
<table class="params">
<thead>
<tr>
<th>Name</th>
<th>Type</th>
<th>Description</th>
</tr>
</thead>
<tbody>
<tr>
<td class="name">range</td>
<td class="type"><span class="param-type">string|Array</span></td>
<td class="description"><span class="optional">Optional.</span> If range is specified, it will create chart for the specified range else it will use the current selected range.</td>
</tr>
<tr>
<td class="name">options</td>
<td class="type"><ts ref="ChartOptions"/><span class="param-type">Object</span></td>
<td class="description"><span class="optional">Optional.</span>Pass Object ChartOptions.
<table class="params">
<thead>
<tr>
<th>Name</th>
<th>Type</th>
<th>Description</th>
</tr>
</thead>
<tbody>
<tr>
<td class="name">type</td>
<td class="type"><span class="param-type">string</span></td>
<td class="description">Pass the chart type</td>
</tr>
<tr>
<td class="name">enable3D</td>
<td class="type"><span class="param-type">boolean</span></td>
<td class="description">Pass the enable3D condition</td>
</tr>
<tr>
<td class="name">marker</td>
<td class="type"><span class="param-type">object</span></td>
<td class="description">Pass the marker object to create chart</td>
</tr>
</tbody>
</table>
</td></tr>
</tbody>
</table>

#### Example

{% highlight html %}
<script>
// Initialize the Spreadsheet object.
var excelObj = $("#Spreadsheet").data("ejSpreadsheet");
excelObj.XLChart.createChart("A3:A7",{"type":"stackingcolumn100","enable3D":"true","marker":{"visible":false}}); // To create chart in Spreadsheet.
</script>

{% endhighlight %}

### XLChart.refreshChart(id, options)
{:#methods:xlchart-refreshchart}

This method is used to refresh the chart in the Spreadsheet.
<table class="params">
<thead>
<tr>
<th>Name</th>
<th>Type</th>
<th>Description</th>
</tr>
</thead>
<tbody>
<tr>
<td class="name">id</td>
<td class="type"><span class="param-type">string</span></td>
<td class="description">To pass the chart Id.</td>
</tr>
<tr>
<td class="name">options</td>
<td class="type"><ts ref="ChartOptions"/><span class="param-type">Object</span></td>
<td class="description">
<table class="params">
<thead>
<tr>
<th>Name</th>
<th>Type</th>
<th>Description</th>
</tr>
</thead>
<tbody>
<tr>
<td class="name">type</td>
<td class="type"><span class="param-type">string</span></td>
<td class="description">Pass the chart type</td>
</tr>
<tr>
<td class="name">enable3D</td>
<td class="type"><span class="param-type">boolean</span></td>
<td class="description">Pass the enable3D condition</td>
</tr>
<tr>
<td class="name">marker</td>
<td class="type"><span class="param-type">object</span></td>
<td class="description">Pass the marker object</td>
</tr>
</tbody>
</table>
</td></tr>
</tbody>
</table>

#### Example 

{% highlight html %}
<script>
// Create Spreadsheet object.
var excelObj = $("#Spreadsheet").data("ejSpreadsheet");
excelObj.XLChart.refreshChart(id,{"type":"stackingcolumn100","enable3D":"true","marker":{"visible":false}}); // To refresh the chart in Spreadsheet
</script>
{% endhighlight %}

### XLChart.resizeChart(id, height, width)
{:#methods:xlchart-resizechart}

This method is used to resize the chart of specified id in the Spreadsheet.
<table class="params">
<thead>
<tr>
<th>Name</th>
<th>Type</th>
<th>Description</th>
</tr>
</thead>
<tbody>
<tr>
<td class="name">id</td>
<td class="type"><span class="param-type">string</span></td>
<td class="description">To pass the chart id.</td>
</tr>
<tr>
<td class="name">height</td>
<td class="type"><span class="param-type">number</span></td>
<td class="description">To pass height value.</td>
</tr>
<tr>
<td class="name">width</td>
<td class="type"><span class="param-type">number</span></td>
<td class="description">To pass the width value.</td>
</tr>
</tbody>
</table>

#### Example

{% highlight html %}
<script>
// Create Spreadsheet object.
var excelObj = $("#Spreadsheet").data("ejSpreadsheet");
excelObj.XLChart.resizeChart("Spreadsheet_chart1", 200, 300); // It is used to resize the chart in Spreadsheet.
</script>

{% endhighlight %}

### XLChart.updateChartElement(chartId, value)
{:#methods:xlchart-updatechartelement}

This method is used to update the chart element, such as axes, titles, data labels, grid lines and legends in the Spreadsheet.

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
<td class="name">chartId</td>
<td class="type"><span class="param-type">string</span></td>
<td class="description">Pass the chart id.</td></tr>
<tr>
<td class="name">value</td>
<td class="type"><ts name="ej.Spreadsheet.ChartProperties"/><span class="param-type">enum</span></td>
<td class="description">Pass chart element value which you want to update.</td>
</tr>
</tbody>
</table>


#### Example

{% highlight html %}

<div id="Spreadsheet"></div> 
<script>
// Initialize Spreadsheet object.
var excelObj = $("#Spreadsheet").data("ejSpreadsheet"), chartId = "Spreadsheet_chart1", value = ej.Spreadsheet.ChartProperties.PrimaryHorizontal; 
excelObj.XLChart.updateChartElement(chartId, value); // To update chart property.
</script>

{% endhighlight %}

#### ChartProperties

Specifies the chart element value in the Spreadsheet,

<table class="props">
<thead>
<tr>
<th>Name</th>
<th>Description</th>
</tr>
</thead>
<tbody>
<tr>
<td>DataLabelCenter</td>
<td>Specifies to make the data label center of the chart.</td>
</tr>
<tr>
<td>DataLabelInsideBase</td>
<td>Specifies to make the data label inside base of the chart.</td>
</tr>
<tr>
<td>DataLabelInsideEnd</td>
<td>Specifies to make the data label inside end of the chart.</td>
</tr>
<tr>
<td>DataLabelNone</td>
<td>Specifies to make the data label none of the chart.</td>
</tr>
<tr>
<td>DataLabelOutsideEnd</td>
<td>Specifies to make the data label outside end of the chart.</td>
</tr>
<tr>
<td>LegendsBottom</td>
<td>Specifies to make the legends to bottom of the chart.</td>
</tr>
<tr>
<td>LegendsLeft</td>
<td>Specifies to make the legends to left of the chart.</td>
</tr>
<tr>
<td>LegendsNone</td>
<td>Specifies to make the legends to none of the chart.</td>
</tr>
<tr>
<td>LegendsRight</td>
<td>Specifies to make the legends to right of the chart.</td>
</tr>
<tr>
<td>LegendsTop</td>
<td>Specifies to make the legends to top of the chart.</td>
</tr>
<tr>
<td>PrimaryHorizontal</td>
<td>To set the primary horizontal of the chart.</td>
</tr>
<tr>
<td>PrimaryHorizontalAxisTitle</td>
<td>To set the primary horizontal axis title of the chart.</td>
</tr>
<tr>
<td>PrimaryMajorHorizontal</td>
<td>To set the primary major horizontal of the chart.</td>
</tr>
<tr>
<td>PrimaryMajorVertical</td>
<td>To set the primary major vertical of the chart.</td>
</tr>
<tr>
<td>PrimaryMinorHorizontal</td>
<td>To set the primary minor horizontal of the chart.</td>
</tr>
<tr>
<td>PrimaryMinorVertical</td>
<td>To set the primary minor vertical of the chart.</td>
</tr>
<tr>
<td>PrimaryVertical</td>
<td>To set the primary vertical of the chart.</td>
</tr>
<tr>
<td>PrimaryVerticalAxisTitle</td>
<td>To set the primary vertical axis title of the chart.</td>
</tr>
<tr>
<td>TitleCenter</td>
<td>Specifies to make the title to center of the chart.</td>
</tr>
<tr>
<td>TitleFar</td>
<td>Specifies to make the title to far of the chart.</td>
</tr>
<tr>
<td>TitleNear</td>
<td>Specifies to make the title to near of the chart.</td>
</tr>
<tr>
<td>TitleNone</td>
<td>Specifies to make the title to none of the chart.</td>
</tr>
</tbody>
</table>

### XLChart.switchRowColumn(chartId)
{:#methods:xlchart-switchrowcolumn}

This method is used switch row to columns and vice versa for chart in the Spreadsheet. So that the data is displayed in the chart the way you want.

<table>
<tr>
<th>
Name</th><th>
Type</th><th>
Description</th></tr>
<tr>
<td>
chartId</td><td>
string</td><td>
Pass the chart id.</td></tr>
</table>

#### Example

{% highlight html %}

<div id="Spreadsheet"></div> 
<script>
// Initialize Spreadsheet object.
var excelObj = $("#Spreadsheet").data("ejSpreadsheet"), chartId = "Spreadsheet_chart1";
excelObj.XLChart.switchRowColumn(chartId);
</script>

{% endhighlight %}

### XLClipboard
{:#methods:xlclipboard}

### XLClipboard.copy()
{:#methods:xlclipboard-copy}

This method is used to copy the selected cells in the Spreadsheet.

#### Example
{% highlight html %}
<script>
// Initialize the Spreadsheet object.
var excelObj = $("#Spreadsheet").data("ejSpreadsheet");
// To copy cells in a Spreadsheet.
excelObj.XLClipboard.copy();
</script>

{% endhighlight %}

### XLClipboard.cut()
{:#methods:xlclipboard-cut}

This method is used to cut the selected cells in the Spreadsheet.

#### Example

{% highlight html %}
<script>
// Initialize the Spreadsheet object.
var excelObj = $("#Spreadsheet").data("ejSpreadsheet");
// To cut cells in a Spreadsheet
excelObj.XLClipboard.cut();
</script>

{% endhighlight %}

### XLClipboard.paste()
{:#methods:xlclipboard-paste}

This method is used to paste the cut or copied cells data in the Spreadsheet.

#### Example

{% highlight html %}
<script>
//initialize the Spreadsheet object
var excelObj = $("#Spreadsheet").data("ejSpreadsheet");
// To paste data in Spreadsheet
excelObj.XLClipboard.paste();
</script>

{% endhighlight %}

### XLComment
{:#methods:xlcomment}

### XLComment.deleteComment(\[range\], \[sheetIdx\], \[skipHiddenRow\])
{:#methods:xlcomment-deletecomment}

This method is used to delete the comment in the specified range in Spreadsheet.
<table class="params">
<thead>
<tr>
<th>Name</th>
<th>Type</th>
<th>Description</th>
</tr>
</thead>
<tbody>
<tr>
<td class="name">range</td>
<td class="type"><span class="param-type">Array|string</span></td>
<td class="description"><span class="optional">Optional.</span> If range is specified, it will delete comments for the specified range else it will use the current selected range. </td>
</tr>
<tr>
<td class="name">sheetIdx</td>
<td class="type"><span class="param-type">number</span></td>
<td class="description"><span class="optional">Optional.</span> If sheetIdx is specified, it will delete comment in specified sheet else it will use active sheet.</td>
</tr>
<tr>
<td class="name">skipHiddenRow</td>
<td class="type"><span class="param-type">boolean</span></td>
<td class="description"><span class="optional">Optional.</span> Pass {{'`true`' | markdownify}}, if you want to skip the hidden rows data.</td>
</tr>
</tbody>
</table>

#### Example

{% highlight html %}
<script>
// Initialize the Spreadsheet object.
var excelObj = $("#Spreadsheet").data("ejSpreadsheet");
//Sends a delete comment request to the Spreadsheet.
excelObj.XLComment.deleteComment("A1:D3", 1, true);
</script>

{% endhighlight %}

### XLComment.editComment(\[targetCell\])
{:#methods:xlcomment-editcomment}

This method is used to edit the comment in the target Cell in Spreadsheet.
<table class="params">
<thead>
<tr>
<th>Name</th>
<th>Type</th>
<th>Description</th>
</tr>
</thead>
<tbody>
<tr>
<td class="name">targetCell</td>
<td class="type"><ts ref="CellIndex"/><span class="param-type">Object</span></td>
<td class="description"><span class="optional">Optional.</span> Pass Object CellIndex.
<table class="params">
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
<td class="type"><span class="param-type">number</span></td>
<td class="description">Pass the row index of the cell which contains comment</td>
</tr>
<tr>
<td class="name">colIndex</td>
<td class="type"><span class="param-type">number</span></td>
<td class="description">Pass the col index of the cell which contains comment</td>
</tr>
</tbody>
</table>
</td></tr>
</tbody>
</table>

#### Example

{% highlight html %}
<script>
// Initialize the Spreadsheet object.
var excelObj = $("#Spreadsheet").data("ejSpreadsheet");
//Sends an edit comment request to the Spreadsheet.
excelObj.XLComment.editComment({rowIndex: 1, colIndex: 1});
</script>

{% endhighlight %}

### XLComment.findNextComment()
{:#methods:xlcomment-findnextcomment}

This method is used to find the next comment from the active cell in Spreadsheet.

#### Returns:
boolean

#### Example

{% highlight html %}
<div id="Spreadsheet"></div> 
<script>
// Initialize the Spreadsheet object.
var excelObj = $("#Spreadsheet").data("ejSpreadsheet");
//Sends a find next comment request to the Spreadsheet.
excelObj.XLComment.findNextComment();
</script>

{% endhighlight %}

### XLComment.findPrevComment()
{:#methods:xlcomment-findprevcomment}

This method is used to find the previous comment from the active cell in Spreadsheet.

#### Returns:
boolean

#### Example

{% highlight html %}
<div id="Spreadsheet"></div> 
<script>
// Initialize the Spreadsheet object.
var excelObj = $("#Spreadsheet").data("ejSpreadsheet");
//Sends a find previous comment request to the Spreadsheet.
excelObj.XLComment.findPrevComment();
</script>

{% endhighlight %}

### XLComment.getComment(cell)
{:#methods:xlcomment-getcomment}

This method is used to get comment data for the specified cell.
<table class="params">
<thead>
<tr>
<th>Name</th>
<th>Type</th>
<th>Description</th>
</tr>
</thead>
<tbody>
<tr>
<td class="name">cell</td>
<td class="type"><span class="param-type">Element</span></td>
<td class="description">Pass the DOM element to get comment data as object.</td>
</tr>
</tbody>
</table>

#### Returns:
Object

#### Example

{% highlight html %}
<div id="Spreadsheet"></div> 
<script>
// Create Spreadsheet object.
var excelObj = $("#Spreadsheet").data("ejSpreadsheet");
excelObj.getComment(excelObj.getCell(1, 5)); // Get the specified cell comment data.
</script>

{% endhighlight %}

{% highlight html %}
<script>
// Get the specified cell comment data
$("#Spreadsheet").ejSpreadsheet("getComment", excelObj.getCell(1, 5));        
</script>

{% endhighlight %}

### XLComment.setComment(\[range\], \[data\], \[showEditPanel\], \[showUserName\])
{:#methods:xlcomment-setcomment}

This method is used to set new comment in Spreadsheet.
<table class="params">
<thead>
<tr>
<th>Name</th>
<th>Type</th>
<th>Description</th>
</tr>
</thead>
<tbody>
<tr>
<td class="name">range</td>
<td class="type"><span class="param-type">string|Array</span> </td>
<td class="description"><span class="optional">Optional.</span> If we pass the range comment will set in the range otherwise it will set with selected cells. </td>
</tr>
<tr>
<td class="name">data</td>
<td class="type"><span class="param-type">string</span></td>
<td class="description"><span class="optional">Optional.</span> Pass the comment data.</td>
</tr>
<tr>
<td class="name">showEditPanel</td>
<td class="type"><span class="param-type">boolean</span></td>
<td class="description"><span class="optional">Optional.</span> Pass {{'`true`' | markdownify}} to show comment in edit mode </td>
</tr>
<tr>
<td class="name">showUserName</td>
<td class="type"><span class="param-type">boolean</span></td>
<td class="description"><span class="optional">Optional.</span> Pass {{'`true`' | markdownify}} to show the user name </td>
</tr>
</tbody>
</table>

#### Example

{% highlight html %}
<script>
// Initialize Spreadsheet object.
var excelObj = $("#Spreadsheet").data("ejSpreadsheet");
//To set comment in Spreadsheet.
excelObj.XLComment.setComment("A2", "Spreadsheet Comment!");
</script>

{% endhighlight %}

### XLComment.showAllComments()
{:#methods:xlcomment-showallcomments}

This method is used to show all the comments in the Spreadsheet.

#### Example

{% highlight html %}
<script>
// Initialize Spreadsheet object.
var excelObj = $("#Spreadsheet").data("ejSpreadsheet");
//Sends a show all comment request to the Spreadsheet.
excelObj.XLComment.showAllComments();
</script>

{% endhighlight %}

### XLComment.showHideComment(\[targetCell\])
{:#methods:xlcomment-showhidecomment}

This method is used to show or hide the specific comment in the Spreadsheet.
<table class="params">
<thead>
<tr>
<th>Name</th>
<th>Type</th>
<th>Description</th>
</tr>
</thead>
<tbody>
<tr>
<td class="name">targetCell</td>
<td class="type"><span class="param-type">Element</span></td>
<td class="description"><span class="optional">Optional.</span> Pass the cell DOM element to show or hide its comment. If pass empty argument active cell will processed.</td>
</tr>
</tbody>
</table>

#### Example

{% highlight html %}
<script>
// Initialize Spreadsheet object.
var excelObj = $("#Spreadsheet").data("ejSpreadsheet");
//To show/hide comment request in Spreadsheet.
excelObj.XLComment.showHideComment(excelObj.getCell(1, 5));
</script>

{% endhighlight %}

### XLCMenu
{:#methods:xlcmenu}

### XLCMenu.addItem(target, itemColl, operation, itemIdx)
{:#methods:xlcmenu-additem}

This method is used to dynamically add items in the context menu.
<table class="params">
<thead>
<tr>
<th>Name</th>
<th>Type</th>
<th>Description</th>
</tr>
</thead>
<tbody>
<tr>
<td class="name">target</td>
<td class="type"><ts name="ej.Spreadsheet.ContextMenuType"/><span class="param-type">enum</span></td>
<td class="description">Specifies the context menu type in which the item to be inserted.</td>
</tr>
<tr>
<td class="name">itemColl</td>
<td class="type"><span class="param-type">Array</span></td>
<td class="description">Pass the items to be inserted</td>
</tr>
<tr>
<td class="name">operation</td>
<td class="type"><span class="param-type">string</span></td>
<td class="description">Specifies the type of operation to be performed</td>
</tr>
<tr>
<td class="name">itemIdx</td>
<td class="type"><span class="param-type">Number</span></td>
<td class="description">Specifies the item index</td>
</tr>
</tbody>
</table>

#### Example

{% highlight html %}
<script>
// Create Spreadsheet object.
var excelObj = $("#Spreadsheet").data("ejSpreadsheet");
// To add an item in the context menu at last position.
excelObj.XLCMenu.addItem(ej.Spreadsheet.ContextMenu.Cell, [{"text":"Added item 1!!!", "url":"#", "id": "Added item1", "spriteCssClass": "e-icon e-ss-cut" }], 'insert'); 
// To add an item in the context menu before the particular item index.
excelObj.XLCMenu.addItem(ej.Spreadsheet.ContextMenu.Cell, [{"text":"Added item 2!!!", "url":"#", "id": "Added item2", "spriteCssClass": "e-icon e-ss-copy" }], 'insertbefore', 2);
// To add an item in the context menu after the particular item index.
excelObj.XLCMenu.addItem(ej.Spreadsheet.ContextMenu.Cell, [{"text":"Added item 3!!!", "url":"#", "id": "Added item3", "spriteCssClass": "e-icon e-ss-paste" }], 'insertafter', 2);
</script>

{% endhighlight %}

#### ContextMenuType

Specifies the Context Menu type in the Spreadsheet,

<table class="props">
<thead>
<tr>
<th>Name</th>
<th>Description</th>
</tr>
</thead>
<tbody>
<tr>
<td>Cell</td>
<td>To specify cell Context Menu.</td>
</tr>
<tr>
<td>RowHeader</td>
<td>To specify row header Context Menu.</td>
</tr>
<tr>
<td>ColumnHeader</td>
<td>To specify column header Context Menu.</td>
</tr>
<tr>
<td>Footer</td>
<td>To specify footer Context Menu.</td>
</tr>
</tbody>
</table>

### XLCMenu.changeDataSource(target, data)
{:#methods:xlcmenu-changedatasource}

This method is used to change data source in the context menu.
<table class="params">
<thead>
<tr>
<th>Name</th>
<th>Type</th>
<th>Description</th>
</tr>
</thead>
<tbody>
<tr>
<td class="name">target</td>
<td class="type"><span class="param-type">string</span></td>
<td class="description">Specifies the context menu type to bind the data source.</td>
</tr>
<tr>
<td class="name">data</td>
<td class="type"><span class="param-type">Array</span></td>
<td class="description">Pass the data source to be binded</td>
</tr>
</tbody>
</table>

#### Example

{% highlight html %}
<script>
// Create Spreadsheet object.
var excelObj = $("#Spreadsheet").data("ejSpreadsheet");
excelObj.XLCMenu.changeDataSource(ej.Spreadsheet.ContextMenu.Cell,[{ id: "Comment", text: 'cmnt', parentId: null, spriteCssClass: "e-icon e-ss-newcmnt" }]); // To change the data source in the context menu.
</script>

{% endhighlight %}

### XLCMenu.disableItem(target, idxColl)
{:#methods:xlcmenu-disableitem}

This method is used to disable the items in the context menu.
<table class="params">
<thead>
<tr>
<th>Name</th>
<th>Type</th>
<th>Description</th>
</tr>
</thead>
<tbody>
<tr>
<td class="name">target</td>
<td class="type"><span class="param-type">string</span></td>
<td class="description">Specifies the context menu type in which the item to be disabled.</td>
</tr>
<tr>
<td class="name">idxColl</td>
<td class="type"><span class="param-type">Array</span></td>
<td class="description">Specifies the Menu Item id collection to be disabled</td>
</tr>
</tbody>
</table>

#### Example

{% highlight html %}
<script>
// Create Spreadsheet object.
var excelObj = $("#Spreadsheet").data("ejSpreadsheet");
excelObj.XLCMenu.disableItem(ej.Spreadsheet.ContextMenu.Cell, ["Cut", "Insert", "Copy"]); // To disable the item in the context menu.
</script>

{% endhighlight %}

### XLCMenu.enableItem(target, idxColl)
{:#methods:xlcmenu-enableitem}

This method is used to enable the items in the context menu.
<table class="params">
<thead>
<tr>
<th>Name</th>
<th>Type</th>
<th>Description</th>
</tr>
</thead>
<tbody>
<tr>
<td class="name">target</td>
<td class="type"><span class="param-type">string</span></td>
<td class="description">Specifies the context menu type in which the item to be enabled.</td>
</tr>
<tr>
<td class="name">idxColl</td>
<td class="type"><span class="param-type">Array</span></td>
<td class="description">Specifies the Menu Item id collection to be enabled</td>
</tr>
</tbody>
</table>

#### Example

{% highlight html %}
<script>
// Create Spreadsheet object.
var excelObj = $("#Spreadsheet").data("ejSpreadsheet");
excelObj.XLCMenu.enableItem(ej.Spreadsheet.ContextMenu.Cell, ["Cut", "Insert", "Copy"]); // To enable the item in the context menu.
</script>

{% endhighlight %}

### XLCMenu.hideItem(cMenuType, idxColl)
{:#methods:xlcmenu-hideitem}

This method is used to hide the items in the context menu.
<table class="params">
<thead>
<tr>
<th>Name</th>
<th>Type</th>
<th>Description</th>
</tr>
</thead>
<tbody>
<tr>
<td class="name">cMenuType</td>
<td class="type"><span class="param-type">string</span></td>
<td class="description">Specifies the context menu type in which the item to be hides.</td>
</tr>
<tr>
<td class="name">idxColl</td>
<td class="type"><span class="param-type">Array</span></td>
<td class="description">Specifies the Menu Item id collection to be hides</td>
</tr>
</tbody>
</table>

#### Example

{% highlight html %}
<script>
// Create Spreadsheet object.
var excelObj = $("#Spreadsheet").data("ejSpreadsheet");
excelObj.XLCMenu.hideItem(ej.Spreadsheet.ContextMenu.Cell, ["Cut", "Insert", "Copy"]); // To hide the item in the context menu.
</script>

{% endhighlight %}

### XLCMenu.removeItem(target, idxColl)
{:#methods:xlcmenu-removeitem}

This method is used to remove the items in the context menu.
<table class="params">
<thead>
<tr>
<th>Name</th>
<th>Type</th>
<th>Description</th>
</tr>
</thead>
<tbody>
<tr>
<td class="name">target</td>
<td class="type"><span class="param-type">string</span></td>
<td class="description">Specifies the context menu type in which the item to be removed.</td>
</tr>
<tr>
<td class="name">idxColl</td>
<td class="type"><span class="param-type">Array</span></td>
<td class="description">Specifies the Menu Item id collection to be removed</td>
</tr>
</tbody>
</table>

#### Example

{% highlight html %}
<script>
// Create Spreadsheet object.
var excelObj = $("#Spreadsheet").data("ejSpreadsheet");
excelObj.XLCMenu.removeItem(ej.Spreadsheet.ContextMenu.Cell, ["Cut", "Insert", "Copy"]); // To remove the item in the context menu.
</script>

{% endhighlight %}

### XLCMenu.showItem(cMenuType, idxColl)
{:#methods:xlcmenu-showitem}

This method is used to show the items in the context menu.
<table class="params">
<thead>
<tr>
<th>Name</th>
<th>Type</th>
<th>Description</th>
</tr>
</thead>
<tbody>
<tr>
<td class="name">cMenuType</td>
<td class="type"><span class="param-type">string</span></td>
<td class="description">Specifies the context menu type in which the item to be shown.</td>
</tr>
<tr>
<td class="name">idxColl</td>
<td class="type"><span class="param-type">Array</span></td>
<td class="description">Specifies the Menu Item id collection to be shown</td>
</tr>
</tbody>
</table>

#### Example

{% highlight html %}
<script>
// Create Spreadsheet object.
var excelObj = $("#Spreadsheet").data("ejSpreadsheet");
excelObj.XLCMenu.showItem(ej.Spreadsheet.ContextMenu.Cell, ["Cut", "Insert", "Copy"]); // To show the item in the context menu.
</script>

{% endhighlight %}

### XLDragDrop
{:#methods:xldragdrop}

### XLDragDrop.moveRangeTo(sourceRange, destinationRange)
{:#methods:xldragdrop-moverangeto}

This method is used to drag and drop the selected range of cells to destination range in the Spreadsheet.
<table class="params">
<thead>
<tr>
<th>Name</th>
<th>Type</th>
<th>Description</th>
</tr>
</thead>
<tbody>
<tr>
<td class="name">sourceRange</td>
<td class="type"><span class="param-type">Object|Array</span></td>
<td class="description">Pass the source range to perform drag and drop.</td>
</tr>
<tr>
<td class="name">destinationRange</td>
<td class="type"><span class="param-type">Object|Array</span></td>
<td class="description">Pass the destination range to drop the dragged cells.</td>
</tr>
</tbody>
</table>

#### Example

{% highlight html %}
<script>
// Create Spreadsheet object.
var excelObj = $("#Spreadsheet").data("ejSpreadsheet");
var options = {sourcerange: [1,2,1,2], destinationrange: [1,3,1,6]}
excelObj.XLDragDrop.moveRangeTo(options.sourcerange, options.destinationrange); // To perform drag and drop in Spreadsheet.
</script>

{% endhighlight %}

### XLDragFill
{:#methods:xldragfill}

### XLDragFill.autoFill(options)
{:#methods:xldragfill-autofill}

This method is used to perform auto fill in Spreadsheet.
<table class="params">
<thead>
<tr>
<th>Name</th>
<th>Type</th>
<th>Description</th>
</tr>
</thead>
<tbody>
<tr>
<td class="name">options</td>
<td class="type"><ts ref="AutoFillObject"/><span class="param-type">Object</span></td>
<td class="description">Pass Object AutoFillObject.
<table class="params">
<thead>
<tr>
<th>Name</th>
<th>Type</th>
<th>Description</th>
</tr>
</thead>
<tbody>
<tr>
<td class="name">dataRange</td>
<td class="type"><span class="param-type">string</span></td>
<td class="description">Pass the data range to autofill</td>
</tr>
<tr>
<td class="name">direction</td>
<td class="type"><span class="param-type">string</span></td>
<td class="description">Pass the direction to autofill </td>
</tr>
<tr>
<td class="name">fillRange</td>
<td class="type"><span class="param-type">string</span></td>
<td class="description">Pass the fill range to autofill</td>
</tr>
<tr>
<td class="name">fillType</td>
<td class="type"><span class="param-type">string</span></td>
<td class="description">Pass the fill type to perform autofill in spreadsheet</td>
</tr>
</tbody>
</table>
</td></tr>
</tbody>
</table>

#### Example

{% highlight html %}
<script>
// Initialize the Spreadsheet object.
var excelObj = $("#Spreadsheet").data("ejSpreadsheet");
var options = {dataRange: "A1:B1", direction: "right", fillRange:"A1:B2"}
excelObj.XLDragFill.autoFill(options); // To perform autofill in Spreadsheet.
</script>

{% endhighlight %}

### XLDragFill.hideAutoFillElement()
{:#methods:xldragfill-hideautofillelement}

This method is used to hide the auto fill element in the Spreadsheet.

#### Example

{% highlight html %}
<div id="Spreadsheet"></div>
<script>
// Initialize the Spreadsheet object
var excelObj = $("#Spreadsheet").data("ejSpreadsheet");
// To hide auto fill element in Spreadsheet
excelObj.XLDragFill.hideAutoFillElement();
</script>

{% endhighlight %}

### XLDragFill.hideAutoFillOptions()
{:#methods:xldragfill-hideautofilloptions}

This method is used to hide the auto fill options in the Spreadsheet.

#### Example

{% highlight html %}
<div id="Spreadsheet"></div>
<script>
// Initialize the Spreadsheet object
var excelObj = $("#Spreadsheet").data("ejSpreadsheet");
// To hide auto fill element in Spreadsheet
excelObj.XLDragFill.hideAutoFillOptions();
</script>

{% endhighlight %}


### XLDragFill.positionAutoFillElement(isDragFill)
{:#methods:xldragfill-positionautofillelement}

This method is used to set position of the auto fill element in the Spreadsheet.
<table class="params">
<thead>
<tr>
<th>Name</th>
<th>Type</th>
<th>Description</th>
</tr>
</thead>
<tbody>
<tr>
<td class="name">isDragFill</td>
<td class="type"><span class="param-type">boolean</span></td>
<td class="description">Pass the isDragFill option as {{'`boolean`' | markdownify}} value to show auto fill options in Spreadsheet.</td>
</tr>
</tbody>
</table>

#### Example

{% highlight html %}
<script>
// Create Spreadsheet object.
var excelObj = $("#Spreadsheet").data("ejSpreadsheet");
excelObj.XLDragFill.positionAutoFillElement(false); // set position of the autofill element in Spreadsheet.
</script>

{% endhighlight %}

### XLEdit
{:#methods:xledit}

### XLEdit.calcNow(\[sheetIdx\])
{:#methods:xledit-calcnow}

This method is used to calculate formulas in the specified sheet.
<table class="params">
<thead>
<tr>
<th>Name</th>
<th>Type</th>
<th>Description</th>
</tr>
</thead>
<tbody>
<tr>
<td class="name">sheetIdx</td>
<td class="type"><span class="param-type">number</span></td>
<td class="description"><span class="optional">Optional.</span> If sheet index is specified, then it will calculate formulas in the specified sheet only else it will calculate formulas in all sheets.</td>
</tr>
</tbody>
</table>

#### Example

{% highlight html %}
<script>
// Initialize the Spreadsheet object.
var excelObj = $("#Spreadsheet").data("ejSpreadsheet");
excelObj.XLEdit.calcNow(1); // To calculate formulas in specified sheet in Spreadsheet.
</script>

{% endhighlight %}

### XLEdit.editCell(rowIdx, colIdx, oldData)
{:#methods:xledit-editcell}

This method is used to edit a particular cell based on the row index and column index in the Spreadsheet.
<table class="params">
<thead>
<tr>
<th>Name</th>
<th>Type</th>
<th>Description</th>
</tr>
</thead>
<tbody>
<tr>
<td class="name">rowIdx</td>
<td class="type"><span class="param-type">number</span></td>
<td class="description">Pass the row index to edit particular cell.</td>
</tr>
<tr>
<td class="name">colIdx</td>
<td class="type"><span class="param-type">number</span></td>
<td class="description">Pass the column index to edit particular cell.</td>
</tr>
<tr>
<td class="name">oldData</td>
<td class="type"><span class="param-type">boolean</span></td>
<td class="description">Pass {{'`true`' | markdownify}}, if you want to maintain previous cell value.</td>
</tr>
</tbody>
</table>

#### Example

{% highlight html %}
<script>
//initialize the Spreadsheet object.
var spreadsheetObj = $("#Spreadsheet").data("ejSpreadsheet");
// Edit particular cell based on row index and column index.
spreadsheetObj.XLEdit.editCell(1, 1, true);
</script>

{% endhighlight %}

{% highlight html %}
<script>
// Edit particular cell based on row index and column index.
$("#Spreadsheet").ejSpreadsheet("XLEdit").editCell(1, 1, true);
</script> 

{% endhighlight %}

### XLEdit.getColumnIndexByField(field)
{:#methods:xledit-getcolumnindexbyfield}

This method is used to get the column index with specified field value in Spreadsheet.
<table class="params">
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
<td class="type"><span class="param-type">string</span></td>
<td class="description">Pass the column field value</td>
</tr>
</tbody>
</table>

#### Example

{% highlight html %}
<script>
//initialize the Spreadsheet object.
var excelObj = $("#Spreadsheet").data("ejSpreadsheet");
// To get the column index
excelObj.XLEdit.getColumnIndexByField("D");
</script>

{% endhighlight %}

### XLEdit.getPropertyValue(rowIdx, colIdx, \[prop\], \[sheetIdx\])
{:#methods:xledit-getpropertyvalue}

This method is used to get the property value of particular cell, based on the row and column index in the Spreadsheet.
<table class="params">
<thead>
<tr>
<th>Name</th>
<th>Type</th>
<th>Description</th>
</tr>
</thead>
<tbody>
<tr>
<td class="name">rowIdx</td>
<td class="type"><span class="param-type">number</span></td>
<td class="description">Pass the row index to get the property value.</td>
</tr>
<tr>
<td class="name">colIdx</td>
<td class="type"><span class="param-type">number</span></td>
<td class="description">Pass the column index to get the property value.</td>
</tr>
<tr>
<td class="name">prop</td>
<td class="type"><span class="param-type">string</span></td>
<td class="description"><p><span class="optional">Optional.</span> Pass the property name that you want("value", "value2", "type",<br/> "cFormatRule", "range", "thousandSeparator", "rule", "format", "border",<br/> "picture", "chart", "calcValue", "align", "hyperlink", "formats", "borders",<br/> "tformats", "tborders", "isFilterHeader",  "filterState", "tableName",<br/> "comment", "formatStr", "decimalPlaces", "cellType").</p></td>
</tr>
<tr>
<td class="name">sheetIdx</td>
<td class="type"><span class="param-type">number</span></td>
<td class="description"><span class="optional">Optional.</span> Pass the index of the sheet.</td>
</tr>
</tbody>
</table>

#### Returns:
Object|string|Array

#### Example

{% highlight html %}
<div id="Spreadsheet"></div>
<script>
// Initialize the Spreadsheet object.
var ssObj = $("#Spreadsheet").data("ejSpreadsheet");
// Get the cell property value.
excelObj.XLEdit.getPropertyValue(1, 1, "value", 1);
</script>

{% endhighlight %}

### XLEdit.getPropertyValueByElem(elem, property, sheetIdx)
{:#methods:xledit-getpropertyvaluebyelem}

This method is used to get the property value in specified cell in Spreadsheet.

<table class="params">
<thead>
<tr>
<th>Name</th>
<th>Type</th>
<th>Description</th>
</tr>
</thead>
<tbody>
<tr>
<td class="name">elem</td>
<td class="type"><span class="param-type">Element</span></td>
<td class="description">Pass the cell element to get property value.</td>
</tr>
<tr>
<td class="name">property</td>
<td class="type"><span class="param-type">string</span></td>
<td class="description"><p>Pass the property name that you want ("value", "value2", "type",<br/> "cFormatRule", "range", "thousandSeparator", "rule", "format", "border",<br/> "picture", "chart", "calcValue", "align", "hyperlink", "formats", "borders",<br/> "tformats", "tborders", "isFilterHeader", "filterState", "tableName", <br/>"comment", "formatStr", "decimalPlaces", "cellType").</p></td>
</tr>
<tr>
<td class="name">sheetIdx</td>
<td class="type"><span class="param-type">number</span></td>
<td class="description">Pass the index of sheet.</td>
</tr>
</tbody>
</table>

#### Returns:
Object|string|Array

#### Example

{% highlight html %}
<div id="Spreadsheet"></div>
<script>
// Initialize the Spreadsheet object.
var excelObj = $("#Spreadsheet").data("ejSpreadsheet");
// Get the cell property value based on tag element.
excelObj.XLEdit.getPropertyValueByElem(excelObj.getCell(1, 1), "value", 1);
</script>

{% endhighlight %}

### XLEdit.saveCell()
{:#methods:xledit-savecell}

This method is used to save the edited cell value in the Spreadsheet.

#### Example

{% highlight html %}
<script>
// Initialize the Spreadsheet object
var excelObj = $("#Spreadsheet").data("ejSpreadsheet");
// Save the edited cell value
excelObj.XLEdit.saveCell();
</script>

{% endhighlight %}

### XLEdit.updateCell(cell, value)
{:#methods:xledit-updatecell}

This method is used to update a particular cell value in the Spreadsheet.
<table class="params">
<thead>
<tr>
<th>Name</th>
<th>Type</th>
<th>Description</th>
</tr>
</thead>
<tbody>
<tr>
<td class="name">cell</td>
<td class="type"><ts ref="CellIndex"/><span class="param-type">Object</span></td>
<td class="description">Pass Object CellIndex.
<table class="params">
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
<td class="type"><span class="param-type">number</span></td>
<td class="description">Pass the row index</td>
</tr>
<tr>
<td class="name">colIndex</td>
<td class="type"><span class="param-type">number</span></td>
<td class="description">Pass the Column index</td>
</tr>
</tbody>
</table>
</td></tr>
<tr>
<td class="name">value</td>
<td class="type"><span class="param-type">string|number</span></td>
<td class="description">Pass the cell value.</td>
</tr>
</tbody>
</table>

#### Example

{% highlight html %}
<script>
// Initialize the Spreadsheet object
var excelObj = $("#Spreadsheet").data("ejSpreadsheet");
// Update the specified values to a particular cell.
excelObj.XLEdit.updateCell({rowIndex: 1, colIndex: 1}, "product");
</script>

{% endhighlight %}

### XLEdit.updateCellValue(cellIdx, val, formatClass, sheetIdx)
{:#methods:xledit-updatecellvalue}

This method is used to update a particular cell value and its format in the Spreadsheet.
<table class="params">
<thead>
<tr>
<th>Name</th>
<th>Type</th>
<th>Description</th>
</tr>
</thead>
<tbody>
<tr>
<td class="name">cellIdx</td>
<td class="type"><ts ref="CellIndex"/><span class="param-type">Object</span></td>
<td class="description">Pass Object CellIndex.
<table class="params">
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
<td class="type"><span class="param-type">number</span></td>
<td class="description">Pass the row index</td>
</tr>
<tr>
<td class="name">colIndex</td>
<td class="type"><span class="param-type">number</span></td>
<td class="description">Pass the column index</td>
</tr>
</tbody>
</table>
</td></tr>
<tr>
<td class="name">val</td>
<td class="type"><span class="param-type">string|number</span></td>
<td class="description">Pass the cell value.</td>
</tr>
<tr>
<td class="name">formatClass</td>
<td class="type"><span class="param-type">string</span></td>
<td class="description">Pass the class name to update format. </td>
</tr>
<tr>
<td class="name">sheetIdx</td>
<td class="type"><span class="param-type">number</span></td>
<td class="description">Pass sheet index.</td>
</tr>
</tbody>
</table>

#### Example

{% highlight html %}
<script>
// Initialize the Spreadsheet object
var excelObj = $("#Spreadsheet").data("ejSpreadsheet"), className;
className = excelObj.XLFormat.getFormatHashCode({ color: "#FF0000" });
// To update the specified values in a particular cell.
excelObj.XLEdit.updateCellValue({rowIndex: 1, colIndex: 1}, "product", className, 1);
</script>

{% endhighlight %}

### XLEdit.updateValue(aRange, val, formatClass, sheetIdx)
{:#methods:xledit-updatevalue}

This method is used to update a particular cell value and its format in the Spreadsheet.
<table class="params">
<thead>
<tr>
<th>Name</th>
<th>Type</th>
<th>Description</th>
</tr>
</thead>
<tbody>
<tr>
<td class="name">aRange</td>
<td class="type"><span class="param-type">string</span></td>
<td class="description">Pass the range.</td>
</tr>
<tr>
<td class="name">val</td>
<td class="type"><span class="param-type">string|number</span></td>
<td class="description">Pass the cell value.</td>
</tr>
<tr>
<td class="name">formatClass</td>
<td class="type"><span class="param-type">string</span></td>
<td class="description">Pass the class name to update format. </td>
</tr>
<tr>
<td class="name">sheetIdx</td>
<td class="type"><span class="param-type">number</span></td>
<td class="description">Pass sheet index.</td>
</tr>
</tbody>
</table>

#### Example

{% highlight html %}
<script>
// Initialize the Spreadsheet object
var excelObj = $("#Spreadsheet").data("ejSpreadsheet"), className;
className = excelObj.XLFormat.getFormatHashCode({ color: "#FF0000" });
// To update the specified values in a particular cell.
excelObj.XLEdit.updateValue("A1", "product", className, 1);
</script>

{% endhighlight %}

### XLExport
{:#methods:xlexport}

### XLExport.export(type, fileName)
{:#methods:xlexport-export}

This method is used to save the sheet data as Excel ,CSV or PDF document (.xls, .xlsx .csv, .pdf) in Spreadsheet.

N> To use export, user must provide the [`excelUrl`](https://help.syncfusion.com/js/api/ejspreadsheet#members:exportsettings-excelurl "excelUrl"), [`csvUrl`](https://help.syncfusion.com/js/api/ejspreadsheet#members:exportsettings-csvurl "csvUrl"), and [`pdfUrl`](https://help.syncfusion.com/js/api/ejspreadsheet#members:exportsettings-pdfurl "pdfUrl") property in [`exportSettings`](https://help.syncfusion.com/js/api/ejspreadsheet#members:exportsettings "exportSettings").

<table class="params">
<thead>
<tr>
<th>Name</th>
<th>Type</th>
<th>Description</th>
</tr>
</thead>
<tbody>
<tr>
<td class="name">type</td>
<td class="type"><span class="param-type">string</span></td>
<td class="description">Pass the export type that you want. </td>
</tr>
<tr>
<td class="name">fileName</td>
<td class="type"><ts name="ej.Spreadsheet.ExportType"/><span class="param-type">enum</span></td>
<td class="description">Pass the export filename that you want. </td>
</tr>
</tbody>
</table>

#### Example

{% highlight html %}
<script>
// Initialize the Spreadsheet object.
var excelObj = $("#Spreadsheet").data("ejSpreadsheet");
// To save the worksheet on Excel format.
excelObj.XLExport.export("Excel", "sample");
</script>

{% endhighlight %}

#### ExportType

Specifies the export type in the Spreadsheet,

<table class="props">
<thead>
<tr>
<th>Name</th>
<th>Description</th>
</tr>
</thead>
<tbody>
<tr>
<td>Excel</td>
<td>Specifies to export the file in Excel format.</td>
</tr>
<tr>
<td>Csv</td>
<td>Specifies to export the file in Csv format.</td>
</tr>
<tr>
<td>Pdf</td>
<td>Specifies to export the file in Pdf format.</td>
</tr>
</tbody>
</table>

### XLExport.getExportProps()
{:#methods:xlexport-getexportprops}

This method is used to get the export properties in the Spreadsheet.

#### Returns:
Object

#### Example
{% highlight html %}
<script>
// Initialize the Spreadsheet object.
var excelObj = $("#Spreadsheet").data("ejSpreadsheet");
excelObj.XLExport.getExportProps(); // Gets export properties in Spreadsheet.
</script>
{% endhighlight %}

{% highlight html %}
<script>
// Gets export properties in Spreadsheet.
$("#Spreadsheet").ejSpreadsheet("getExportProps");        
</script>

{% endhighlight %}

### XLFilter
{:#methods:xlfilter}

### XLFilter.clearFilter()
{:#methods:xlfilter-clearfilter}

This method is used to clear the filter in filtered columns in the Spreadsheet.

#### Example

{% highlight html %}
<script>
// Initialize the Spreadsheet object.
var excelObj = $("#Spreadsheet").data("ejSpreadsheet");
// Clear filter for columns in the sheet.
excelObj.XLFilter.clearFilter();
</script>

{% endhighlight %}

### XLFilter.filter(range)
{:#methods:xlfilter-filter}

This method is used to apply filter for the selected range of cells in the Spreadsheet.
<table class="params">
<thead>
<tr>
<th>Name</th>
<th>Type</th>
<th>Description</th>
</tr>
</thead>
<tbody>
<tr>
<td class="name">range</td>
<td class="type"><span class="param-type">string|Array</span></td>
<td class="description">Pass the range of the selected cells.</td>
</tr>
</tbody>
</table>

#### Example

{% highlight html %}
<div id="Spreadsheet"></div> 
<script>
// Initialize the Spreadsheet object.
var excelObj = $("#Spreadsheet").data("ejSpreadsheet");
// To apply filter for specified range of cells.
excelObj.XLFilter.filter("A3:C8");
</script>

{% endhighlight %}

### XLFilter.filterByActiveCell()
{:#methods:xlfilter-filterbyactivecell}

This method is used to apply filter for the column by active cell's value in the Spreadsheet.

#### Example

{% highlight html %}
<div id="Spreadsheet"></div> 
<script>
// Initialize the Spreadsheet object.
var excelObj = $("#Spreadsheet").data("ejSpreadsheet");
// Apply filter for columns with active cell in the sheet.
excelObj.XLFilter.filterByActiveCell();
</script>

{% endhighlight %}

### XLFormat
{:#methods:xlformat}

### XLFormat.addCustomFormatSpecifier(name, formatSpecifier, type)
{:#methods:xlformat-addcustomformatspecifier}

This method is used to add the custom Date & Time format and recognize it as a preferred pattern in spreadsheet. 

<table class="params">
<thead>
<tr>
<th>Name</th>
<th>Type</th>
<th>Description</th>
</tr>
</thead>
<tbody>
<tr>
<td class="name">name</td>
<td class="type"><span class="param-type">string</span></td>
<td class="description">Pass the name for custom format.</td>
</tr>
<tr>
<td class="name">formatSpecifier</td>
<td class="type"><span class="param-type">string</span></td>
<td class="description">Pass the custom format string.</td>
</tr>
<tr>
<td class="name">type</td>
<td class="type"><span class="param-type">string</span></td>
<td class="description">Pass the type for custom format.</td>
</tr>
</tbody>
</table>

#### Example

{% highlight html %}
<div id="Spreadsheet"></div>
<script>
// Initialize the Spreadsheet object.
var excelObj = $("#Spreadsheet").data("ejSpreadsheet");
excelObj.XLFormat.addCustomFormatSpecifier("formatStr","dd/MM/yyyy", ej.Spreadsheet.CellType.Date) // To add the custom date format in spreadsheet
</script>

{% endhighlight %}

### XLFormat.addFontFamily(fontName)
{:#methods:xlformat-addfontfamily}

This method is used to add the font to the Ribbon font family dropdown.  

<table class="params">
<thead>
<tr>
<th>Name</th>
<th>Type</th>
<th>Description</th>
</tr>
</thead>
<tbody>
<tr>
<td class="name">fontName</td>
<td class="type"><span class="param-type">string</span></td>
<td class="description">Font name which needs to add into the font family option.</td>
</tr>
</tbody>
</table>

#### Example

{% highlight html %}
<div id="Spreadsheet"></div>
<script>
// Initialize the Spreadsheet object.
var excelObj = $("#Spreadsheet").data("ejSpreadsheet");
excelObj.XLFormat.addFontFamily("Gisha"); // To add the font name into font family option.
</script>

{% endhighlight %}

### XLFormat.addNewCustomStyle(styleName, options)
{:#methods:xlformat-addnewcustomstyle}

This method is used to add the new custom cell style in spreadsheet.

<table class="params">
<thead>
<tr>
<th>Name</th>
<th>Type</th>
<th>Description</th>
</tr>
</thead>
<tbody>
<tr>
<td class="name">styleName</td>
<td class="type"><span class="param-type">string</span></td>
<td class="description">Pass the style name.</td>
</tr>
<tr>
<td class="name">options</td>
<td class="type"><ts ref="NumberFormatOptions"/><span class="param-type">Object</span></td>
<td class="description">Pass Object NumberFormatOptions.
<table class="params">
<thead>
<tr>
<th>Name</th>
<th>Type</th>
<th>Description</th>
</tr>
</thead>
<tbody>
<tr>
<td class="name">NumFormat</td>
<td class="type"><span class="param-type">object</span></td>
<td class="description">Pass the number format object</td>
</tr>
<tr>
<td class="name">style</td>
<td class="type"><span class="param-type">object</span></td>
<td class="description">Pass the style object</td>
</tr>
</tbody>
</table>
</td></tr>
</tbody>
</table>

#### Example

{% highlight html %}
<div id="Spreadsheet"></div>
<script>
// Initialize the Spreadsheet object.
var excelObj = $("#Spreadsheet").data("ejSpreadsheet");
// To add the new custom cell style
excelObj.XLFormat.addNewCustomStyle("StyleName",{NumFormat:{type: "currency", decimalPlaces: 4, thousandSeparator: false, formatStr: "{0:C4}"},style:{"background-color": "#cccbcb", color: "#f16667", "font-family": "Arial", "font-size": "16pt", "font-style": "normal", "font-weight": "Bold","text-decoration": "line-through"}})
</script>

{% endhighlight %}

### XLFormat.applyCustomCellStyle(styleName, range)
{:#methods:xlformat-applycustomcellstyle}

This method is used to apply the custom cell style in the specified range.

<table class="params">
<thead>
<tr>
<th>Name</th>
<th>Type</th>
<th>Description</th>
</tr>
</thead>
<tbody>
<tr>
<td class="name">styleName</td>
<td class="type"><span class="param-type">string</span></td>
<td class="description">Pass the style name.</td>
</tr>
<tr>
<td class="name">range</td>
<td class="type"><span class="param-type">String</span></td>
<td class="description">Pass the range to applied.</td>
</tr>
</tbody>
</table>

#### Example

{% highlight html %}
<div id="Spreadsheet"></div>
<script>
// Initialize the Spreadsheet object.
var excelObj = $("#Spreadsheet").data("ejSpreadsheet");
// To apply the custom cell style to specified range
excelObj.XLFormat.applyCustomCellStyle("StyleName","A1:B4");
</script>

{% endhighlight %}

### XLFormat.convertToRange(options)
{:#methods:xlformat-converttorange}

This method is used to convert table range to normal range.

<table class="params">
<thead>
<tr>
<th>Name</th>
<th>Type</th>
<th>Description</th>
</tr>
</thead>
<tbody>
<tr>
<td class="name">options</td>
<td class="type"><ts ref="TableIDOptions"/><span class="param-type">Object</span></td>
<td class="description">Pass Object TableIDOptions.
<table class="params">
<thead>
<tr>
<th>Name</th>
<th>Type</th>
<th>Description</th>
</tr>
</thead>
<tbody>
<tr>
<td class="name">sheetIdx</td>
<td class="type"><span class="param-type">number</span></td>
<td class="description">Pass the sheet index</td>
</tr>
<tr>
<td class="name">tableId</td>
<td class="type"><span class="param-type">number</span></td>
<td class="description">Pass the table id</td>
</tr>
</tbody>
</table>
</td></tr>
</tbody>
</table>

#### Example

{% highlight html %}
<div id="Spreadsheet"></div>
<script>
// Initialize the Spreadsheet object.
var excelObj = $("#Spreadsheet").data("ejSpreadsheet");
excelObj.XLFormat.convertToRange({sheetIdx: 1, tableId: 1}); // To convert table range to normal range.
</script>

{% endhighlight %}

### XLFormat.createTable( tableObject, \[range\])
{:#methods:xlformat-createtable}

This method is used to create a table for the selected range of cells in the Spreadsheet.
<table class="params">
<thead>
<tr>
<th>Name</th>
<th>Type</th>
<th>Description</th>
</tr>
</thead>
<tbody>
<tr>
<td class="name">tableObject</td>
<td class="type"><ts ref="TableOptions"/><span class="param-type">Object</span></td>
<td class="description">Pass Object TableOptions.
<table class="params">
<thead>
<tr>
<th>Name</th>
<th>Type</th>
<th>Description</th>
</tr>
</thead>
<tbody>
<tr>
<td class="name">header</td>
<td class="type"><span class="param-type">boolean</span></td>
<td class="description">Pass the header boolean condition of table</td>
</tr>
<tr>
<td class="name">name</td>
<td class="type"><span class="param-type">string</span></td>
<td class="description">Pass the name of the table</td>
</tr>
<tr>
<td class="name">formatName</td>
<td class="type"><span class="param-type">string</span></td>
<td class="description">Pass the format name of table</td>
</tr>
</tbody>
</table>
</td></tr>
<tr>
<td class="name">range</td>
<td class="type"><span class="param-type">string|Array</span></td>
<td class="description"><span class="optional">Optional.</span> If the range is specified, then it will create table in the specified range else it will use the current selected range. </td>
</tr>
</tbody>
</table>

#### Returns:
string

#### Example

{% highlight html %}
<script>
// Initialize the Spreadsheet object
var excelObj = $("#Spreadsheet").data("ejSpreadsheet"), tableObj;
tableObj = { header: true, name: "Table1", formatName: "TableStyleLight1"};
// Sends a create table request to the Spreadsheet
excelObj.XLFormat.createTable(tableObj, "A1:C6");
</script>

{% endhighlight %}

### XLFormat.deleteCustomStyle(styleName)
{:#methods:xlformat-deletecustomstyle}

This method is used to delete the added custom cell style in spreadsheet.

<table class="params">
<thead>
<tr>
<th>Name</th>
<th>Type</th>
<th>Description</th>
</tr>
</thead>
<tbody>
<tr>
<td class="name">styleName</td>
<td class="type"><span class="param-type">String</span></td>
<td class="description">Pass the cell style name</td>
</tr>
</tbody>
</table>

#### Example

{% highlight html %}
<div id="Spreadsheet"></div>
<script>
// Initialize the Spreadsheet object.
var excelObj = $("#Spreadsheet").data("ejSpreadsheet");
excelObj.XLFormat.deleteCustomStyle("StyleName") // To delete the custom cell style.
</script>

{% endhighlight %}

### XLFormat.format(formatObj, range)
{:#methods:xlformat-format}

This method is used to set format style and values in a cell or range of cells.
<table class="params">
<thead>
<tr>
<th>Name</th>
<th>Type</th>
<th>Description</th>
</tr>
</thead>
<tbody>
<tr>
<td class="name">formatObj</td>
<td class="type"><ts ref="FormatObjectOptions"/><span class="param-type">Object</span></td>
<td class="description">Pass Object FormatObjectOptions.
<table class="params">
<thead>
<tr>
<th>Name</th>
<th>Type</th>
<th>Description</th>
</tr>
</thead>
<tbody>
<tr>
<td class="name">style</td>
<td class="type"><span class="param-type">object</span></td>
<td class="description">Pass the style object in a cell</td>
</tr>
<tr>
<td class="name">type</td>
<td class="type"><span class="param-type">string</span></td>
<td class="description">Pass the type of cell</td>
</tr>
<tr>
<td class="name">thousandSeparator</td>
<td class="type"><span class="param-type">string</span></td>
<td class="description">Pass the thousand separator in cell</td>
</tr>
<tr>
<td class="name">decimalPlaces</td>
<td class="type"><span class="param-type">string</span></td>
<td class="description">Pass the decimal places in cell</td>
</tr>
<tr>
<td class="name">formatStr</td>
<td class="type"><span class="param-type">string</span></td>
<td class="description">Pass the format str in cell</td>
</tr>
</tbody>
</table>
</td></tr>
<tr>
<td class="name">range</td>
<td class="type"><span class="param-type">string</span></td>
<td class="description">Pass the range to format cells.</td>
</tr>
</tbody>
</table>

#### Example

{% highlight html %}
<div id="Spreadsheet"></div> 
<script>
// Initialize the Spreadsheet object.
var excelObj = $("#Spreadsheet").data("ejSpreadsheet");
// Sends a format request to the Spreadsheet.
excelObj.XLFormat.format({style:{ "background-color": "#C0C0C0"}}, "A1:C10");
//Default Number format - decimal places is 2.
excelObj.XLFormat.format({ "type": "number" }, "B1");
//Number format with 3 decimal places by default thousandseparator as true.
excelObj.XLFormat.format({ "type": "number", "decimalPlaces": 3, "thousandSeparator": false }, "B3");
//Currency format with formatStr property.
excelObj.XLFormat.format({ "type": "currency", "formatStr":"{0:C3}" }, "B1");
//Accounting format with formatStr property.
excelObj.XLFormat.format({ "type": "accounting", "formatStr":"{0:C2}" }, "A1");
//Percentage format with formatStr property.
excelObj.XLFormat.format({ "type": "percentage", "formatStr":"{0:P2}" }, "B1");
//Short date format with formatStr property.
excelObj.XLFormat.format({ "type": "shortdate", "formatStr":"{0:MM/dd/yyyy}" }, "C1");
excelObj.XLFormat.format({ "type": "longdate" }, "D1");
//Time format with formatStr property.
excelObj.XLFormat.format({ "type": "time", "formatStr":"{0:hh:mm:ss tt}" }, "E1");
excelObj.XLFormat.format({ "type": "scientific" }, "F1");
excelObj.XLFormat.format({ "type": "fraction" }, "G1");
</script>

{% endhighlight %}

### XLFormat.getBorderFromHashCode(code, isComplete)
{:#methods:xlformat-getborderfromhashcode}

This method is used to get the border from hashcode in the Spreadsheet.
<table class="params">
<thead>
<tr>
<th>Name</th>
<th>Type</th>
<th>Description</th>
</tr>
</thead>
<tbody>
<tr>
<td class="name">code</td>
<td class="type"><span class="param-type">String</span></td>
<td class="description">Pass the border hashcode.</td>
</tr>
<tr>
<td class="name">isComplete</td>
<td class="type"><span class="param-type">boolean</span></td>
<td class="description"><span class="optional">Optional.</span> pass `true` to get the complete border object </td>
</tr>
</tbody>
</table>

#### Returns:
Object

#### Example

{% highlight html %}
<script>
// Initialize the Spreadsheet object
var excelObj = $("#Spreadsheet").data("ejSpreadsheet");
// To get the border object from the Spreadsheet
excelObj.XLFormat.getBorderFromHashCode("e-border1N1N6N1N1N6N210000001N1N6N",true);
</script>

{% endhighlight %}

### XLFormat.getFormatClass(classname, isborder)
{:#methods:xlformat-getformatclass}

This method is used to get the format class in spreadsheet.  

<table class="params">
<thead>
<tr>
<th>Name</th>
<th>Type</th>
<th>Description</th>
</tr>
</thead>
<tbody>
<tr>
<td class="name">classname</td>
<td class="type"><span class="param-type">string</span></td>
<td class="description">Pass the style name.</td>
</tr>
<tr>
<td class="name">isborder</td>
<td class="type"><span class="param-type">boolean</span></td>
<td class="description"><span class="optional">Optional.</span> Pass true to get the border class.</td>
</tr>
</tbody>
</table>

#### Example

{% highlight html %}
<div id="Spreadsheet"></div>
<script>
// Initialize the Spreadsheet object.
var excelObj = $("#Spreadsheet").data("ejSpreadsheet");
excelObj.XLFormat.getFormatClass(excelObj.getCell(1,1)[0].className);// to get the format class
</script>

{% endhighlight %}

### XLFormat.getFormatFromHashCode(hashCode)
{:#methods:xlformat-getformatfromhashcode}

This method is used to get the format from the given hashcode in spreadsheet.  

<table class="params">
<thead>
<tr>
<th>Name</th>
<th>Type</th>
<th>Description</th>
</tr>
</thead>
<tbody>
<tr>
<td class="name">hashCode</td>
<td class="type"><span class="param-type">String</span></td>
<td class="description">Pass the hashcode.</td>
</tr>
</tbody>
</table>

#### Example

{% highlight html %}
<div id="Spreadsheet"></div>
<script>
// Initialize the Spreadsheet object.
var excelObj = $("#Spreadsheet").data("ejSpreadsheet");
excelObj.XLFormat.getFormatFromHashCode(excelObj.XLFormat.getFormatClass(excelObj.getCell(1,1)[0].className)); // To get the format from the given hashcode
</script>

{% endhighlight %}

### XLFormat.getFormatHashCode(style)
{:#methods:xlformat-getformathashcode}

This method is used to get the hashcode from the given style object in spreadsheet.  

<table class="params">
<thead>
<tr>
<th>Name</th>
<th>Type</th>
<th>Description</th>
</tr>
</thead>
<tbody>
<tr>
<td class="name">style</td>
<td class="type"><ts ref="FontOptions"/><span class="param-type">Object</span></td>
<td class="description">Pass Object FontOptions.
<table class="params">
<thead>
<tr>
<th>Name</th>
<th>Type</th>
<th>Description</th>
</tr>
</thead>
<tbody>
<tr>
<td class="name">fontFamily</td>
<td class="type"><span class="param-type">object</span></td>
<td class="description">Pass the font family </td>
</tr>
<tr>
<td class="name">fontWeight</td>
<td class="type"><span class="param-type">string</span></td>
<td class="description">Pass the font weight</td>
</tr>
<tr>
<td class="name">fontStyle</td>
<td class="type"><span class="param-type">string</span></td>
<td class="description">Pass the font style</td>
</tr>
<tr>
<td class="name">fontSize</td>
<td class="type"><span class="param-type">string</span></td>
<td class="description">Pass the font size</td>
</tr>
<tr>
<td class="name">color</td>
<td class="type"><span class="param-type">string</span></td>
<td class="description">Pass the color</td>
</tr>
<tr>
<td class="name">textDecoration</td>
<td class="type"><span class="param-type">string</span></td>
<td class="description">Pass the text decoration</td>
</tr>
</tbody>
</table>
</td></tr>
</tbody>
</table>

#### Example

{% highlight html %}
<div id="Spreadsheet"></div>
<script>
// Initialize the Spreadsheet object.
var excelObj = $("#Spreadsheet").data("ejSpreadsheet");
excelObj.XLFormat.getFormatHashCode({"font-family": "Arial Black", "font-weight": "normal", "font-style": "Italic", "font-size": "9pt", "text-decoration": "line-through",color:"#FFFF00"}); // To get the hashcode from the given style object
</script>

{% endhighlight %}

### XLFormat.getHashCodeClassAsArray(range)
{:#methods:xlformat-gethashcodeclassasarray}

This method is used to get the format as array from the given specified range in spreadsheet.  

<table class="params">
<thead>
<tr>
<th>Name</th>
<th>Type</th>
<th>Description</th>
</tr>
</thead>
<tbody>
<tr>
<td class="name">range</td>
<td class="type"><span class="param-type">String</span></td>
<td class="description">Pass the range.</td>
</tr>
</tbody>
</table>

#### Example

{% highlight html %}
<div id="Spreadsheet"></div>
<script>
// Initialize the Spreadsheet object.
var excelObj = $("#Spreadsheet").data("ejSpreadsheet");
excelObj.XLFormat.getHashCodeClassAsArray("A1:B4"); // To get the format as an array from the given range.
</script>

{% endhighlight %}

### XLFormat.modifyCustomStyle(oldStyleName, options, newStyleName)
{:#methods:xlformat-modifycustomstyle}

This method is used to modify the added custom cell style in spreadsheet. 

<table class="params">
<thead>
<tr>
<th>Name</th>
<th>Type</th>
<th>Description</th>
</tr>
</thead>
<tbody>
<tr>
<td class="name">oldStyleName</td>
<td class="type"><span class="param-type">string</span></td>
<td class="description">pass the old style name</td>
</tr>
<tr>
<td class="name">options</td>
<td class="type"><ts ref="CustomStyleOptions"/><span class="param-type">Object</span></td>
<td class="description">Pass Object CustomStyleOptions.
<table class="params">
<thead>
<tr>
<th>Name</th>
<th>Type</th>
<th>Description</th>
</tr>
</thead>
<tbody>
<tr>
<td class="name">style</td>
<td class="type"><span class="param-type">object</span></td>
<td class="description">Pass the style object</td>
</tr>
<tr>
<td class="name">NumFormat</td>
<td class="type"><span class="param-type">object</span></td>
<td class="description">Pass the number format object</td>
</tr>
</tbody>
</table>
</td></tr>
<tr>
<td class="name">newStyleName</td>
<td class="type"><span class="param-type">string</span></td>
<td class="description">pass the new style name</td>
</tr>
</tbody>
</table>

#### Example

{% highlight html %}
<div id="Spreadsheet"></div>
<script>
// Initialize the Spreadsheet object.
var excelObj = $("#Spreadsheet").data("ejSpreadsheet");
excelObj.XLFormat.modifyCustomStyle("NewStyle",{ NumFormat: {type: "currency", decimalPlaces: 4, thousandSeparator: false, formatStr: "{0:C4}"},style:{color: "#f16667", "font-family": "Arial", "font-size": "16pt", "font-weight": "Bold"}},"StyleName")); // To modify the custom cell style.
</script>

{% endhighlight %}

### XLFormat.removeFontFamily(fontName)
{:#methods:xlformat-removefontfamily}

This method is used to remove the font from the Ribbon font family dropdown.  

<table class="params">
<thead>
<tr>
<th>Name</th>
<th>Type</th>
<th>Description</th>
</tr>
</thead>
<tbody>
<tr>
<td class="name">fontName</td>
<td class="type"><span class="param-type">string</span></td>
<td class="description">Font name which needs to remove from the font family drop down.</td>
</tr>
</tbody>
</table>

#### Example

{% highlight html %}
<div id="Spreadsheet"></div>
<script>
// Initialize the Spreadsheet object.
var excelObj = $("#Spreadsheet").data("ejSpreadsheet");
excelObj.XLFormat.removeFontFamily("Gisha"); // To remove the name from the font family drop down.
</script>

{% endhighlight %}

### XLFormat.removeStyle(range,options)
{:#methods:xlformat-removestyle}

This method is used to remove the style in the specified range.

<table class="params">
<thead>
<tr>
<th>Name</th>
<th>Type</th>
<th>Description</th>
</tr>
</thead>
<tbody>
<tr>
<td class="name">range</td>
<td class="type"><span class="param-type">Array|string</span></td>
<td class="description">Pass the cell range .</td>
</tr>
<tr>
<td class="name">options</td>
<td class="type"><ts ref="FormatOptions"/><span class="param-type">Object</span></td>
<td class="description"><span class="optional">Optional.</span> Pass Object FormatOptions.
<table class="params">
<thead>
<tr>
<th>Name</th>
<th>Type</th>
<th>Description</th>
</tr>
</thead>
<tbody>
<tr>
<td class="name">cellStyle</td>
<td class="type"><span class="param-type">boolean</span></td>
<td class="description">Pass the cell style to be removed</td>
</tr>
<tr>
<td class="name">tableStyle</td>
<td class="type"><span class="param-type">boolean</span></td>
<td class="description">Pass the table style to be removed</td>
</tr>
<tr>
<td class="name">format</td>
<td class="type"><span class="param-type">boolean</span></td>
<td class="description">Pass the format</td>
</tr>
<tr>
<td class="name">border</td>
<td class="type"><span class="param-type">boolean</span></td>
<td class="description">Pass the border condition</td>
</tr>
</tbody>
</table>
</td></tr>
</tbody>
</table>

#### Example

{% highlight html %}
<script>
// Initialize Spreadsheet object.
var excelObj = $("#Spreadsheet").data("ejSpreadsheet");
// Sends a remove style request to the Spreadsheet.
excelObj.XLFormat.removeStyle("E4:F13",{ cellStyle: true, tableStyle: true, format: true, border: true }); 
</script>

{% endhighlight %}

### XLFormat.removeTable(tableId)
{:#methods:xlformat-removetable}

This method is used to remove table with specified tableId in the Spreadsheet.

<table class="params">
<thead>
<tr>
<th>Name</th>
<th>Type</th>
<th>Description</th>
</tr>
</thead>
<tbody>
<tr>
<td class="name">tableId</td>
<td class="type"><span class="param-type">number</span></td>
<td class="description">Pass the tableId that you want to remove.</td>
</tr>
</tbody>
</table>

#### Example

{% highlight html %}
<script>
// Initialize the Spreadsheet object.
var excelObj = $("#Spreadsheet").data("ejSpreadsheet");
// Sends a remove table request to the Spreadsheet.
excelObj.XLFormat.removeTable(1);
</script>

{% endhighlight %}

### XLFormat.updateDecimalPlaces(type, range)
{:#methods:xlformat-updatedecimalplaces}

This method is used to update the decimal places for numeric value for the selected range of cells in the Spreadsheet.

<table class="params">
<thead>
<tr>
<th>Name</th>
<th>Type</th>
<th>Description</th>
</tr>
</thead>
<tbody>
<tr>
<td class="name">type</td>
<td class="type"><span class="param-type">string</span></td>
<td class="description">Pass the decimal places type in IncreaseDecimal/DecreaseDecimal.</td>
</tr>
<tr>
<td class="name">range</td>
<td class="type"><span class="param-type">string|Array</span></td>
<td class="description">Pass the range.</td>
</tr>
</tbody>
</table>

#### Example

{% highlight html %}
<script>
// Initialize the Spreadsheet object.
var excelObj = $("#Spreadsheet").data("ejSpreadsheet");
// To update decimal place value in the range of cells in the Spreadsheet.
excelObj.XLFormat.updateDecimalPlaces("IncreaseDecimal", "A1:C3");
</script>

{% endhighlight %}

### XLFormat.updateFormat(formatObj, \[range\])
{:#methods:xlformat-updateformat}

This method is used to update the format for the selected range of cells in the Spreadsheet.
<table class="params">
<thead>
<tr>
<th>Name</th>
<th>Type</th>
<th>Description</th>
</tr>
</thead>
<tbody>
<tr>
<td class="name">formatObj</td>
<td class="type"><ts ref="BorderOptions"/><span class="param-type">Object</span></td>
<td class="description">Pass Object BorderOptions.
<table class="params">
<thead>
<tr>
<th>Name</th>
<th>Type</th>
<th>Description</th>
</tr>
</thead>
<tbody>
<tr>
<td class="name">format</td>
<td class="type"><span class="param-type">Object</span></td>
<td class="description">Pass the format object of selected range of cells</td>
</tr>
<tr>
<td class="name">leftBorder</td>
<td class="type"><span class="param-type">string</span></td>
<td class="description">Pass the left border</td>
</tr>
<tr>
<td class="name">topBorder</td>
<td class="type"><span class="param-type">string</span></td>
<td class="description">Pass the top border</td>
</tr>
</tbody>
</table>
</td></tr>
<tr>
<td class="name">range</td>
<td class="type"><span class="param-type">Array</span></td>
<td class="description"><span class="optional">Optional.</span> If the range is specified, then it will update format in the specified range else it will use the current selected range. </td>
</tr>
</tbody>
</table>

#### Example

{% highlight html %}
<script>
// Initialize the Spreadsheet object
var excelObj = $("#Spreadsheet").data("ejSpreadsheet"), formatObj;
formatObj = { format: ["e-formatFFFF006N2N2N1N1N1N1N2N1N", "", "e-formatFFFF006N2N2N1N1N1N1N2N1N"], leftborder: ["","",""], topborder: ["e-border1N1N6N1N1N6NS1N1N6N11000000"]};
// To update a format in the specified range of cells.
excelObj.XLFormat.updateFormat(formatObj, [1, 0, 3, 0]);
</script>

{% endhighlight %}

### XLFormat.updateUniqueFormat(formatClass, \[range\])
{:#methods:xlformat-updateuniqueformat}

This method is used to update the unique format for selected range of cells in the Spreadsheet.
<table class="params">
<thead>
<tr>
<th>Name</th>
<th>Type</th>
<th>Description</th>
</tr>
</thead>
<tbody>
<tr>
<td class="name">formatClass</td>
<td class="type"><span class="param-type">string</span></td>
<td class="description">Pass the unique format class.</td>
</tr>
<tr>
<td class="name">range</td>
<td class="type"><span class="param-type">Array</span></td>
<td class="description"><span class="optional">Optional.</span> If the range is specified, then it will update format in the specified range else it will use the current selected range.</td>
</tr>
</tbody>
</table>

#### Example

{% highlight html %}
<script>
// Initialize the Spreadsheet object.
var excelObj = $("#Spreadsheet").data("ejSpreadsheet");
// To update the unique format.
excelObj.XLFormat.updateUniqueFormat("e-formatFFFF006N2N2N251N1N2N", [1, 0, 4, 0]);
</script>

{% endhighlight %}

### XLFreeze
{:#methods:xlfreeze}

### XLFreeze.freezeColumns(colIdx)
{:#methods:xlfreeze-freezecolumns}

This method is used to freeze columns upto the specified column index in the Spreadsheet.

<table class="params">
<thead>
<tr>
<th>Name</th>
<th>Type</th>
<th>Description</th>
</tr>
</thead>
<tbody>
<tr>
<td class="name">colIdx</td>
<td class="type"><span class="param-type">number</span></td>
<td class="description">Index of the column to be freeze.</td>
</tr>
</tbody>
</table>

#### Example

{% highlight html %}
<div id="Spreadsheet"></div> 
<script>
//Initialize the Spreadsheet object
var excelObj = $("#Spreadsheet").data("ejSpreadsheet");
// Freeze a column in the sheet.
excelObj.XLFreeze.freezeColumns(2);
</script>

{% endhighlight %}

### XLFreeze.freezeLeftColumn()
{:#methods:xlfreeze-freezeleftcolumn}

This method is used to freeze the first column in the Spreadsheet.

#### Example

{% highlight html %}
<div id="Spreadsheet"></div> 
<script>
// Initialize the Spreadsheet object.
var excelObj = $("#Spreadsheet").data("ejSpreadsheet");
// Freeze the first column in the sheet.
excelObj.XLFreeze.freezeLeftColumn();
</script>

{% endhighlight %}

### XLFreeze.freezePanes(rowIdx, colIdx)
{:#methods:xlfreeze-freezepanes}

This method is used to freeze rows and columns before the specified cell in the Spreadsheet.

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
<td class="name">rowIdx</td>
<td class="type"><span class="param-type">number</span></td>
<td class="description">Index of the row to be freeze.</td>
</tr>
<tr>
<td class="name">colIdx</td>
<td class="type"><span class="param-type">number</span></td>
<td class="description">Index of the column to be freeze.</td>
</tr>
</tbody>
</table>

#### Example

{% highlight html %}
<div id="Spreadsheet"></div> 
<script>
// Initialize the Spreadsheet object
var excelObj = $("#Spreadsheet").data("ejSpreadsheet");
// Freeze some rows and columns in the sheet.
excelObj.XLFreeze.freezePanes(2, 3);
</script>

{% endhighlight %}

### XLFreeze.freezeRows(rowIdx)
{:#methods:xlfreeze-freezerows}

This method is used to freeze rows upto the specified row index in the Spreadsheet.
<table class="params">
<thead>
<tr>
<th>Name</th>
<th>Type</th>
<th>Description</th>
</tr>
</thead>
<tbody>
<tr>
<td class="name">rowIdx</td>
<td class="type"><span class="param-type">number</span></td>
<td class="description">Index of the row to be freeze.</td>
</tr>
</tbody>
</table>

#### Example

{% highlight html %}
<script>
//initialize the Spreadsheet object.
var excelObj = $("#Spreadsheet").data("ejSpreadsheet");
// Freeze a row in the sheet.
excelObj.XLFreeze.freezeRows(2);
</script>

{% endhighlight %}

### XLFreeze.freezeTopRow()
{:#methods:xlfreeze-freezetoprow}

This method is used to freeze the top row in the Spreadsheet.

#### Example

{% highlight html %}
<div id="Spreadsheet"></div> 
<script>
//Initialize the Spreadsheet object
var excelObj = $("#Spreadsheet").data("ejSpreadsheet");
// Freeze the top row in the sheet.
excelObj.XLFreeze.freezeTopRow();
</script>

{% endhighlight %}

### XLFreeze.unfreezePanes()
{:#methods:xlfreeze-unfreezepanes}

This method is used to unfreeze the frozen rows and columns in the Spreadsheet.

#### Example

{% highlight html %}
<script>
//Initialize the Spreadsheet object.
var excelObj = $("#Spreadsheet").data("ejSpreadsheet");
// To unfreeze the frozen rows and columns in the sheet.
excelObj.XLFreeze.unfreezePanes();
</script>

{% endhighlight %}


### XLPivot
{:#methods:xlpivot}

### XLPivot.clearPivotFieldList(pivotName)
{:#methods:xlpivot-clearpivotfieldlist}

This property is used to clear the pivot table list in Spreadsheet.

<table class="params">
<thead>
<tr>
<th>Name</th>
<th>Type</th>
<th>Description</th>
</tr>
</thead>
<tbody>
<tr>
<td class="name">pivotName</td>
<td class="type"><span class="param-type">string</span></td>
<td class="description">Pass the name of the pivot table. </td>
</tr>
</tbody>
</table>

#### Example

{% highlight html %}
<script>
// Create Spreadsheet object.
var excelObj = $("#Spreadsheet").data("ejSpreadsheet");
excelObj.XLPivot.clearPivotFieldList("name"); // Sends a clear pivot field list request to the Spreadsheet.
</script>

{% endhighlight %}


### XLPivot.createPivotTable(range,location,name,settings,pvt)
{:#methods:xlpivot-createpivottable}

This method is used to create pivot table.

<table class="params">
<thead>
<tr>
<th>Name</th>
<th>Type</th>
<th>Description</th>
</tr>
</thead>
<tbody>
<tr>
<td class="name">range</td>
<td class="type"><span class="param-type">string</span></td>
<td class="description">It specifies the range for which the pivot table is created.</td>
</tr>
<tr>
<td class="name">location</td>
<td class="type"><span class="param-type">string</span></td>
<td class="description">It specifies the location in which the pivot table is created.</td>
</tr>
<tr>
<td class="name">name</td>
<td class="type"><span class="param-type">string</span></td>
<td class="description">It specifies the name of the pivot table.</td>
</tr>
<tr>
<td class="name">settings</td>
<td class="type"><ts ref="PivotOptions"/><span class="param-type">Object</span></td>
<td class="description">Pass Object PivotOptions.
<table class="params">
<thead>
<tr>
<th>Name</th>
<th>Type</th>
<th>Description</th>
</tr>
</thead>
<tbody>
<tr>
<td class="name">rows</td>
<td class="type"><span class="param-type">object</span></td>
<td class="description">Pass the rows object to create pivot table</td>
</tr>
<tr>
<td class="name">columns</td>
<td class="type"><span class="param-type">object</span></td>
<td class="description">Pass the column object to create pivot table</td>
</tr>
<tr>
<td class="name">values</td>
<td class="type"><span class="param-type">object</span></td>
<td class="description">Pass the values to create pivot table</td>
</tr>
<tr>
<td class="name">filter</td>
<td class="type"><span class="param-type">object</span></td>
<td class="description">Pass the filter object to create pivot table</td>
</tr>
</tbody>
</table>
</td></tr>
<tr>
<td class="name">pvt</td>
<td class="type"><span class="param-type">Object</span></td>
<td class="description">Pass the pivot range, sheet index, address and data source .</td>
</tr>
</tbody>
</table>

#### Returns:
string

#### Example

{% highlight html %}
<script>
// Initialize the Spreadsheet object.
var excelObj = $("#Spreadsheet").data("ejSpreadsheet");
// create a pivot table in the sheet.
var settings = {
                 rows: [ {fieldName: "Country",},{fieldName: "State",}],
                 columns: [{fieldName: "Product",}],
                 values: [{fieldName: "Amount", },{fieldName: "Quantity", } ],
                 filters: [ {fieldName: "Date", }] };
excelObj.XLPivot.createPivotTable("Sheet1!$A$1:$F$25","Sheet1!$A$1", null, settings);
</script>

{% endhighlight %}

### XLPivot.deletePivotTable(pivotName)
{:#methods:xlpivot-deletepivottable}

This method is used to delete the pivot table which is selected.

<table class="params">
<thead>
<tr>
<th>Name</th>
<th>Type</th>
<th>Description</th>
</tr>
</thead>
<tbody>
<tr>
<td class="name">pivotName</td>
<td class="type"><span class="param-type">string</span></td>
<td class="description">Pass the name of the pivot table.</td>
</tr>
</tbody>
</table>

#### Example

{% highlight html %}
<script>
// Initialize the Spreadsheet object.
var excelObj = $("#Spreadsheet").data("ejSpreadsheet");
// Delete pivot table in the sheet.
excelObj.XLPivot.deletePivotTable("name");
</script>

{% endhighlight %}

### XLPivot.refreshDataSource(name, sheetIdx)
{:#methods:xlpivot-refreshdatasource}

This method is used to refresh data in pivot table.
<table class="params">
<thead>
<tr>
<th>Name</th>
<th>Type</th>
<th>Description</th>
</tr>
</thead>
<tbody>
<tr>
<td class="name">name</td>
<td class="type"><span class="param-type">string</span></td>
<td class="description"><span class="optional">Optional.</span> Pass the name of the pivot table.</td>
</tr>
<tr>
<td class="name">sheetIdx</td>
<td class="type"><span class="param-type">number</span></td>
<td class="description"><span class="optional">Optional.</span> Pass the index of the sheet.</td>
</tr>
</tbody>
</table>

#### Example

{% highlight html %}
<script>
// Initialize the Spreadsheet object.
var excelObj = $("#Spreadsheet").data("ejSpreadsheet");
excelObj.XLPivot.refreshDataSource(); // Sends a refresh data source request to the Spreadsheet.
</script>

{% endhighlight %}

### XLPrint
{:#methods:xlprint}

### XLPrint.printSelection()
{:#methods:xlprint-printselection}

This method is used to print the selected contents in the Spreadsheet.

#### Example

{% highlight html %}
<script>
var excelObj = $("#Spreadsheet").data("ejSpreadsheet");
// Print the selected area in the sheet.
excelObj.XLPrint.printSelection();
</script>

{% endhighlight %}

### XLPrint.printSheet()
{:#methods:xlprint-printsheet}

This method is used to print the entire contents in the active sheet.

#### Example

{% highlight html %}
<script>
var excelObj = $("#Spreadsheet").data("ejSpreadsheet");
//Sends a print entire sheet request to the Spreadsheet.
excelObj.XLPrint.printSheet();
</script>

{% endhighlight %}

### XLResize
{:#methods:xlresize}

### XLResize.fitHeight(\[rowIndexes\])
{:#methods:xlresize-fitheight}

This method is used to fit the height of rows in the Spreadsheet.
<table class="params">
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
<td class="type"><span class="param-type">Array</span></td>
<td class="description"><span class="optional">Optional.</span> Pass row index collection that you want to fit its height.</td>
</tr>
</tbody>
</table>

#### Example

{% highlight html %}
<script>
//initialize the Spreadsheet object
var excelObj = $("#Spreadsheet").data("ejSpreadsheet");
// To fit the height of the rows in Spreadsheet.
excelObj.XLResize.fitHeight([2,3,4,5])
</script>

{% endhighlight %}

### XLResize.fitWidth(\[colIndexes\])
{:#methods:xlresize-fitwidth}

This method is used to fit the width of columns in the Spreadsheet.
<table class="params">
<thead>
<tr>
<th>Name</th>
<th>Type</th>
<th>Description</th>
</tr>
</thead>
<tbody>
<tr>
<td class="name">colIndexes</td>
<td class="type"><span class="param-type">Array</span></td>
<td class="description"><span class="optional">Optional.</span> Pass column index collection that you want to fit its width.</td>
</tr>
</tbody>
</table>

#### Example

{% highlight html %}
<script>
//initialize the Spreadsheet object
var excelObj = $("#Spreadsheet").data("ejSpreadsheet");
// To fit the width of the columns in Spreadsheet.
excelObj.XLResize.fitWidth([2,3,4,5])
</script>

{% endhighlight %}

### XLResize.getColWidth(colIdx)
{:#methods:xlresize-getcolwidth}

This method is used to get the column width of the specified column index in the Spreadsheet.
<table class="params">
<thead>
<tr>
<th>Name</th>
<th>Type</th>
<th>Description</th>
</tr>
</thead>
<tbody>
<tr>
<td class="name">colIdx</td>
<td class="type"><span class="param-type">number</span></td>
<td class="description">Pass the column index.</td>
</tr>
</tbody>
</table>

#### Returns:
number

#### Example

{% highlight html %}
<div id="Spreadsheet"></div> 
<script>
//initialize the Spreadsheet object
var excelObj = $("#Spreadsheet").data("ejSpreadsheet");
// Gets the particular column width in Spreadsheet.
excelObj.XLResize.getColWidth(2);
</script>

{% endhighlight %}

### XLResize.getRowHeight(rowIdx)
{:#methods:xlresize-getrowheight}

This method is used to get the row height of the specified row index in the Spreadsheet.
<table class="params">
<thead>
<tr>
<th>Name</th>
<th>Type</th>
<th>Description</th>
</tr>
</thead>
<tbody>
<tr>
<td class="name">rowIdx</td>
<td class="type"><span class="param-type">number</span></td>
<td class="description">Pass the row index which you want to find its height.</td>
</tr>
</tbody>
</table>

#### Returns:
number

#### Example

{% highlight html %}
<div id="Spreadsheet"></div> 
<script>
// Initialize the Spreadsheet object.
var excelObj = $("#Spreadsheet").data("ejSpreadsheet");
// Gets the particular row height in Spreadsheet.
excelObj.XLResize.getRowHeight(2);
</script>

{% endhighlight %}

{% highlight html %}
<script>
// Gets the particular row height in Spreadsheet.
$("#Spreadsheet").ejSpreadsheet("XLResize.getRowHeight",2);
</script>

{% endhighlight %}

### XLResize.setColWidth(colIdx, size)
{:#methods:xlresize-setcolwidth}

This method is used to set the column width of the specified column index in the Spreadsheet.
<table class="params">
<thead>
<tr>
<th>Name</th>
<th>Type</th>
<th>Description</th>
</tr>
</thead>
<tbody>
<tr>
<td class="name">colIdx</td>
<td class="type"><span class="param-type">number</span></td>
<td class="description">Pass the column index.</td>
</tr>
<tr>
<td class="name">size</td>
<td class="type"><span class="param-type">number</span></td>
<td class="description">Pass the width value that you want to set.</td>
</tr>
</tbody>
</table>

#### Example

{% highlight html %}
<script>
// Initialize the Spreadsheet object
var excelObj = $("#Spreadsheet").data("ejSpreadsheet");
// Sets the column width in the Spreadsheet.
excelObj.XLResize.setColWidth(2, 100);
</script>

{% endhighlight %}

### XLResize.setRowHeight(rowIdx, size)
{:#methods:xlresize-setrowheight}

This method is used to set the row height of the specified row index in the Spreadsheet.
<table class="params">
<thead>
<tr>
<th>Name</th>
<th>Type</th>
<th>Description</th>
</tr>
</thead>
<tbody>
<tr>
<td class="name">rowIdx</td>
<td class="type"><span class="param-type">number</span></td>
<td class="description">Pass the row index.</td>
</tr>
<tr>
<td class="name">size</td>
<td class="type"><span class="param-type">number</span></td>
<td class="description">Pass the height value that you want to set.</td>
</tr>
</tbody>
</table>

#### Example

{% highlight html %}
<script>
//initialize the Spreadsheet object
var excelObj = $("#Spreadsheet").data("ejSpreadsheet");
// Sets the row height in Spreadsheet.
excelObj.XLResize.setRowHeight(2, 100);
</script>

{% endhighlight %}

### XLRibbon
{:#methods:xlribbon}

### XLRibbon.addBackStageItem(pageItem, index)
{:#methods:xlribbon-addbackstageitem}

This method is used to add a new item in the backstage.
<table class="params">
<thead>
<tr>
<th>Name</th>
<th>Type</th>
<th>Description</th>
</tr>
</thead>
<tbody>
<tr>
<td class="name">pageItem</td>
<td class="type"><ts ref="BackstageOptions"/><span class="param-type">Object</span></td>
<td class="description">Pass Object BackstageOptions.
<table class="params">
<thead>
<tr>
<th>Name</th>
<th>Type</th>
<th>Description</th>
</tr>
</thead>
<tbody>
<tr>
<td class="name">id</td>
<td class="type"><span class="param-type">string</span></td>
<td class="description">Pass the id to added in backstage</td>
</tr>
<tr>
<td class="name">text</td>
<td class="type"><span class="param-type">string</span></td>
<td class="description">Pass the text to added in backstage</td>
</tr>
<tr>
<td class="name">itemType</td>
<td class="type"><span class="param-type">element</span></td>
<td class="description">Pass the item type to added in backstage</td>
</tr>
</tbody>
</table>
</td></tr>
<tr>
<td class="name">index</td>
<td class="type"><span class="param-type">number</span></td>
<td class="description">pass the index of the item to be added in the backstage.</td>
</tr>
</tbody>
</table>

#### Example

{% highlight html %}
<script>
//initialize the Spreadsheet object
var excelObj = $("#Spreadsheet").data("ejSpreadsheet");
var addBackStage = {   id: "File", text: "File", itemType: ej.Ribbon.ItemType.Tab};
excelObj.XLRibbon.addBackStageItem(addBackStage, 1); // To add a item in the backstage.
</script>

{% endhighlight %}

### XLRibbon.addContextualTabs(contextualTabSet, index)
{:#methods:xlribbon-addcontextualtabs}

This method is used to dynamically add the contextual tabs in the ribbon.
<table class="params">
<thead>
<tr>
<th>Name</th>
<th>Type</th>
<th>Description</th>
</tr>
</thead>
<tbody>
<tr>
<td class="name">contextualTabSet</td>
<td class="type"><ts ref="ContextualTabOptions"/><span class="param-type">Object</span></td>
<td class="description">Pass Object ContextualTabOptions.
<table class="params">
<thead>
<tr>
<th>Name</th>
<th>Type</th>
<th>Description</th>
</tr>
</thead>
<tbody>
<tr>
<td class="name">backgroundColor</td>
<td class="type"><span class="param-type">string</span></td>
<td class="description">Pass the background color</td>
</tr>
<tr>
<td class="name">borderColor</td>
<td class="type"><span class="param-type">string</span></td>
<td class="description">Pass the border color</td>
</tr>
<tr>
<td class="name">tabs</td>
<td class="type"><span class="param-type">object</span></td>
<td class="description">Pass the tabs object to add in ribbon</td>
</tr>
</tbody>
</table>
</td></tr>
<tr>
<td class="name">index</td>
<td class="type"><span class="param-type">number</span></td>
<td class="description">pass the index of the contextual tab.</td>
</tr>
</tbody>
</table>

#### Example

{% highlight html %}
<script>
//initialize the Spreadsheet object
var excelObj = $("#Spreadsheet").data("ejSpreadsheet");
var cTab = { backgroundColor: "#FCFBEB", borderColor: "#F2CC1C", tabs: [{id: "Design", text: "DESIGN",groups: [{ text: "Table Style",type: "custom", contentID: "design" }]}] };
excelObj.XLRibbon.addContextualTabs(cTab, 7); // To add a contextual tab in the ribbon.
</script>

{% endhighlight %}

### XLRibbon.addMenuItem(item, index)
{:#methods:xlribbon-addmenuitem}

This method is used to dynamically add the menu item in the file menu.
<table class="params">
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
<td class="type"><span class="param-type">Array</span></td>
<td class="description">Specifies the item to be added</td>
</tr>
<tr>
<td class="name">index</td>
<td class="type"><span class="param-type">number</span></td>
<td class="description">pass the index of the menu item.</td>
</tr>
</tbody>
</table>

#### Example

{% highlight html %}
<script>
//initialize the Spreadsheet object
var excelObj = $("#Spreadsheet").data("ejSpreadsheet");
excelObj.XLRibbon.addMenuItem([{ id: "SignIn1", text: "AddMenuItem", parentId: "FILE", spriteCssClass: "e-icon e-ssr-cut" }], 2); // To add the menu item in the ribbon.
</script>

{% endhighlight %}

### XLRibbon.addNamedRange(name, refersTo, \[comment\], \[sheetIdx\], \[scope\])
{:#methods:xlribbon-addnamedrange}

This method is used to add a new name in the Spreadsheet name manager.
<table class="params">
<thead>
<tr>
<th>Name</th>
<th>Type</th>
<th>Description</th>
</tr>
</thead>
<tbody>
<tr>
<td class="name">name</td>
<td class="type"><span class="param-type">string</span></td>
<td class="description">Pass the name that you want to define in name manager.</td>
</tr>
<tr>
<td class="name">refersTo</td>
<td class="type"><span class="param-type">string</span></td>
<td class="description">Pass the cell reference.</td>
</tr>
<tr>
<td class="name">comment</td>
<td class="type"><span class="param-type">string</span></td>
<td class="description"><span class="optional">Optional.</span> Pass comment, if you want.</td>
</tr>
<tr>
<td class="name">sheetIdx</td>
<td class="type"><span class="param-type">number</span></td>
<td class="description"><span class="optional">Optional.</span> Pass the sheet index.</td>
</tr>
<tr>
<td class="name">scope</td>
<td class="type"><span class="param-type">string</span></td>
<td class="description"><span class="optional">Optional.</span> Pass the scope of the name manager.</td>
</tr>
</tbody>
</table>

#### Example

{% highlight html %}
<script>
// Initialize the Spreadsheet object.
var excelObj = $("#Spreadsheet").data("ejSpreadsheet");
// To define new name in the Spreadsheet.
excelObj.XLRibbon.addNamedRange("PRICE_LIST", "=Sheet1!$A$2:$A$7", "Month_Wise", 1, "Sheet1");
</script>

{% endhighlight %}

### XLRibbon.addTab(tabText, ribbonGroups, index)
{:#methods:xlribbon-addtab}

This method is used to dynamically add the tab in the ribbon.
<table class="params">
<thead>
<tr>
<th>Name</th>
<th>Type</th>
<th>Description</th>
</tr>
</thead>
<tbody>
<tr>
<td class="name">tabText</td>
<td class="type"><span class="param-type">string</span></td>
<td class="description">Specifies the text to be displayed in the tab.</td>
</tr>
<tr>
<td class="name">ribbonGroups</td>
<td class="type"><span class="param-type">Array</span></td>
<td class="description">pass the groups to be displayed in the ribbon tab.</td>
</tr>
<tr>
<td class="name">index</td>
<td class="type"><span class="param-type">number</span></td>
<td class="description">pass the index of the tab.</td>
</tr>
</tbody>
</table>

#### Example

{% highlight html %}
<script>
//initialize the Spreadsheet object
var excelObj = $("#Spreadsheet").data("ejSpreadsheet");
var tabGroup = [{ alignType: ej.Ribbon.AlignType.Rows, content: [{ groups: [{ id: "new", text: "New", toolTip: "New", 
                     buttonSettings: {
                                    contentType: ej.ContentType.ImageOnly,
                                    imagePosition: ej.ImagePosition.ImageTop,
                                    prefixIcon: "e-icon e-ssr-cut",
                                    click: "executeAction"
                                }}], defaults: { type: ej.Ribbon.Type.Button, width: 60, height: 70} }] }];
excelObj.XLRibbon.addTab("Tab2", tabGroup, 2); // To add the tab in the ribbon.
</script>

{% endhighlight %}

### XLRibbon.addTabGroup(tabIndex, tabGroup, groupIndex)
{:#methods:xlribbon-addtabgroup}

This method is used to dynamically add the tab group in the ribbon.
<table class="params">
<thead>
<tr>
<th>Name</th>
<th>Type</th>
<th>Description</th>
</tr>
</thead>
<tbody>
<tr>
<td class="name">tabIndex</td>
<td class="type"><span class="param-type">number</span></td>
<td class="description">Specifies the ribbon tab index.</td>
</tr>
<tr>
<td class="name">tabGroup</td>
<td class="type"><ts ref="TabOptions"/><span class="param-type">Object</span></td>
<td class="description">Pass Object TabOptions.
<table class="params">
<thead>
<tr>
<th>Name</th>
<th>Type</th>
<th>Description</th>
</tr>
</thead>
<tbody>
<tr>
<td class="name">text</td>
<td class="type"><span class="param-type">string</span></td>
<td class="description">Pass the text to displayed in ribbon tab</td>
</tr>
<tr>
<td class="name">alignType</td>
<td class="type"><span class="param-type">element</span></td>
<td class="description">Pass the align type</td>
</tr>
<tr>
<td class="name">contents</td>
<td class="type"><span class="param-type">object</span></td>
<td class="description">Pass the content object to be displayed in ribbon tab</td>
</tr>
<tr>
<td class="name">defaults</td>
<td class="type"><span class="param-type">object</span></td>
<td class="description">Pass the defaults object to be displayed in ribbon tab</td>
</tr>
</tbody>
</table>
</td></tr>
<tr>
<td class="name">groupIndex</td>
<td class="type"><span class="param-type">number</span></td>
<td class="description">pass the index of the ribbon group.</td>
</tr>
</tbody>
</table>

#### Example

{% highlight html %}
<script>
//initialize the Spreadsheet object
var excelObj = $("#Spreadsheet").data("ejSpreadsheet");
var ribbonGrp = { text: "Cut", alignType: ej.Ribbon.AlignType.Rows, content: [{ groups: [{  id: "new",  text: "CUT",buttonSettings: {
                                    contentType: ej.ContentType.TextAndImage,
                                    imagePosition: ej.ImagePosition.ImageTop,
                                    prefixIcon: "e-icon e-ssr-cut",
                                    click: "executeAction"
                                } }], defaults: { type: ej.Ribbon.Type.Button,  width: 60, height: 70 } }] };
excelObj.XLRibbon.addTabGroup(1, ribbonGrp, 0); // To add the tab group in the ribbon.
</script>

{% endhighlight %}

### XLRibbon.autoSum(type, range)
{:#methods:xlribbon-autosum}

This method is used to insert the few type (SUM, MAX, MIN, AVG, COUNT) of formulas in the selected range of cells in the Spreadsheet.
<table class="params">
<thead>
<tr>
<th>Name</th>
<th>Type</th>
<th>Description</th>
</tr>
</thead>
<tbody>
<tr>
<td class="name">type</td>
<td class="type"><span class="param-type">string</span></td>
<td class="description">To pass the type("SUM","MAX","MIN","AVG","COUNT").</td>
</tr>
<tr>
<td class="name">range</td>
<td class="type"><span class="param-type">string|Array</span></td>
<td class="description">If range is specified, it will apply auto sum for the specified range else it will use the current selected range.</td>
</tr>
</tbody>
</table>

#### Example

{% highlight html %}
<script>
// Initialize the Spreadsheet object.
var excelObj = $("#Spreadsheet").data("ejSpreadsheet");
excelObj.XLRibbon.autoSum("SUM", "A2:A6"); // To insert the formula after selected range of cells in Spreadsheet.
</script>

{% endhighlight %}

## XLRibbon.changeDimension(options)
{:#methods:xlribbon-changedimension}

This method is used to change the dimensions for chart/picture.

<table class="params">
<thead>
<tr>
<th>Name</th>
<th>Type</th>
<th>Description</th>
</tr>
</thead>
<tbody>
<tr>
<td class="name">options</td>
<td class="type"><ts ref="ShapeOptions"/><span class="param-type">Object</span></td>
<td class="description">Pass Object ShapeOptions.
<table class="params">
<thead>
<tr>
<th>Name</th>
<th>Type</th>
<th>Description</th>
</tr>
</thead>
<tbody>
<tr>
<td class="name">id</td>
<td class="type"><span class="param-type">string</span></td>
<td class="description">Pass the id to change the dimension</td>
</tr>
<tr>
<td class="name">width</td>
<td class="type"><span class="param-type">number</span></td>
<td class="description">Pass the width to change the dimension</td>
</tr>
<tr>
<td class="name">height</td>
<td class="type"><span class="param-type">number</span></td>
<td class="description">Pass the height to change the dimension</td>
</tr>
<tr>
<td class="name">shapeType</td>
<td class="type"><span class="param-type">string</span></td>
<td class="description">Pass the shape type to change the dimension</td>
</tr>
</tbody>
</table>
</td></tr>
</tbody>
</table>

#### Example

{% highlight html %}
<div id="Spreadsheet"></div>
<script>
// Initialize the Spreadsheet object.
var excelObj = $("#Spreadsheet").data("ejSpreadsheet");
// To change chart/picture dimensions.
excelObj.XLRibbon.changeDimension({id:"Spreadsheet_chart1" , width: 330, height: 500, shapeType: "chart"}); 
</script>

{% endhighlight %}

## XLRibbon.disableRibbonItems([idCollection])
{:#methods:xlribbon-disableribbonitems}

This method is used to disable ribbon items in the Spreadsheet.

<table class="params">
<thead>
<tr>
<th>Name</th>
<th>Type</th>
<th>Description</th>
</tr>
</thead>
<tbody>
<tr>
<td class="name">idCollection</td>
<td class="type"><span class="param-type">Array</span></td>
<td class="description">Pass the id's of the ribbon items.</td>
</tr>
</tbody>
</table>

#### Example

{% highlight html %}
<div id="Spreadsheet"></div>
<script>
// Initialize the Spreadsheet object.
var excelObj = $("#Spreadsheet").data("ejSpreadsheet");
excelObj.XLRibbon.disableRibbonItems(["Spreadsheet_Ribbon_Insert_Illustrations_Pictures"]); // To disable ribbon items.
</script>

{% endhighlight %}

## XLRibbon.enableRibbonItems([idCollection])
{:#methods:xlribbon-enableribbonitems}

This method is used to enable ribbon items in the Spreadsheet.

<table class="params">
<thead>
<tr>
<th>Name</th>
<th>Type</th>
<th>Description</th>
</tr>
</thead>
<tbody>
<tr>
<td class="name">idCollection</td>
<td class="type"><span class="param-type">Array</span></td>
<td class="description">Pass the id's of the ribbon items.</td>
</tr>
</tbody>
</table>

#### Example

{% highlight html %}
<div id="Spreadsheet"></div>
<script>
// Initialize the Spreadsheet object.
var excelObj = $("#Spreadsheet").data("ejSpreadsheet");
excelObj.XLRibbon.enableRibbonItems(["Spreadsheet_Ribbon_Insert_Illustrations_Pictures"]); // To enable ribbon items.
</script>

{% endhighlight %}

### XLRibbon.hideMenu()
{:#methods:xlribbon-hidemenu}

This method is used to hide the file menu in the ribbon tab.

#### Example

{% highlight html %}
<script>
//initialize the Spreadsheet object
var excelObj = $("#Spreadsheet").data("ejSpreadsheet");
excelObj.XLRibbon.hideMenu(); // To hide the file menu option in the Spreadsheet.
</script>

{% endhighlight %}

### XLRibbon.removeBackStageItem(index)
{:#methods:xlribbon-removebackstageitem}

This method is used to remove the item from the backstage in the spreadsheet.
<table class="params">
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
<td class="type"><span class="param-type">number</span></td>
<td class="description">Specifies the index of the item to be removed from backstage.</td>
</tr>
</tbody>
</table>

#### Example

{% highlight html %}
<script>
//initialize the Spreadsheet object
var excelObj = $("#Spreadsheet").data("ejSpreadsheet");
excelObj.XLRibbon.removeBackStageItem(2); // To remove the item in the backstage.
</script>

{% endhighlight %}

### XLRibbon.removeMenuItem(index)
{:#methods:xlribbon-removemenuitem}

This method is used to remove the menu item form file menu in spreadsheet.
<table class="params">
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
<td class="type"><span class="param-type">number</span></td>
<td class="description">Specifies the index of the item to be removed from the file menu.</td>
</tr>
</tbody>
</table>

#### Example

{% highlight html %}
<script>
//initialize the Spreadsheet object
var excelObj = $("#Spreadsheet").data("ejSpreadsheet");
excelObj.XLRibbon.removeMenuItem(2); // To remove the item in the file menu.
</script>

{% endhighlight %}

### XLRibbon.removeNamedRange(name, \[scope\])
{:#methods:xlribbon-removenamedrange}

This method is used to delete the defined name in the Spreadsheet name manager.
<table class="params">
<thead>
<tr>
<th>Name</th>
<th>Type</th>
<th>Description</th>
</tr>
</thead>
<tbody>
<tr>
<td class="name">name</td>
<td class="type"><span class="param-type">string</span></td>
<td class="description">Pass the defined name that you want to remove from name manager.</td>
</tr>
<tr>
<td class="name">scope</td>
<td class="type"><span class="param-type">string</span></td>
<td class="description"><span class="optional">Optional.</span> Pass the scope of the name manager.</td>
</tr>
</tbody>
</table>

#### Example

{% highlight html %}
<script>
//initialize the Spreadsheet object
var excelObj = $("#Spreadsheet").data("ejSpreadsheet");
// To remove the define name in Spreadsheet name manager.
excelObj.XLRibbon.removeNamedRange("PRICE_LIST","Sheet1");
</script>

{% endhighlight %}

### XLRibbon.removeTab(index, isRemoveMenu)
{:#methods:xlribbon-removetab}

This method is used to remove the tab form ribbon in the spreadsheet.
<table class="params">
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
<td class="type"><span class="param-type">number</span></td>
<td class="description">Specifies the index of the tab to be removed from the ribbon.</td>
</tr>
<tr>
<td class="name">isRemoveMenu</td>
<td class="type"><span class="param-type">boolean</span></td>
<td class="description">pass the boolean value to remove the tab from ribbon</td>
</tr>
</tbody>
</table>

#### Example

{% highlight html %}
<script>
//initialize the Spreadsheet object
var excelObj = $("#Spreadsheet").data("ejSpreadsheet");
excelObj.XLRibbon.removeTab(2, true) // To remove the tab from the ribbon.
</script>

{% endhighlight %}

### XLRibbon.removeTabGroup(tabIndex, groupText)
{:#methods:xlribbon-removetabgroup}

This method is used to remove the tab group form ribbon in the spreadsheet.
<table class="params">
<thead>
<tr>
<th>Name</th>
<th>Type</th>
<th>Description</th>
</tr>
</thead>
<tbody>
<tr>
<td class="name">tabIndex</td>
<td class="type"><span class="param-type">number</span></td>
<td class="description">Specifies the index of the tab group to be removed from the ribbon.</td>
</tr>
<tr>
<td class="name">groupText</td>
<td class="type"><span class="param-type">string</span></td>
<td class="description">Specifies the text to be displayed in the tab group</td>
</tr>
</tbody>
</table>

#### Example

{% highlight html %}
<script>
//initialize the Spreadsheet object
var excelObj = $("#Spreadsheet").data("ejSpreadsheet");
excelObj.XLRibbon.removeTabGroup(1,"Clipboard"); // To remove the tab group from the ribbon.
</script>

{% endhighlight %}

### XLRibbon.showMenu()
{:#methods:xlribbon-showmenu}

This method is used to show the file menu in the ribbon tab.

#### Example

{% highlight html %}
<script>
//initialize the Spreadsheet object
var excelObj = $("#Spreadsheet").data("ejSpreadsheet");
excelObj.XLRibbon.showMenu(); // To show the file menu option in the Spreadsheet.
</script>

{% endhighlight %}

### XLRibbon.updateMenuItem(item, index)
{:#methods:xlribbon-updatemenuitem}

This method is used to update the menu item in the file menu.
<table class="params">
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
<td class="type"><ts ref="MenuItemOptions"/><span class="param-type">Object</span></td>
<td class="description">Pass Object MenuItemOptions.
<table class="params">
<thead>
<tr>
<th>Name</th>
<th>Type</th>
<th>Description</th>
</tr>
</thead>
<tbody>
<tr>
<td class="name">id</td>
<td class="type"><span class="param-type">string</span></td>
<td class="description">Pass the id to update the menu item</td>
</tr>
<tr>
<td class="name">text</td>
<td class="type"><span class="param-type">string</span></td>
<td class="description">Pass the text to update the menu item</td>
</tr>
<tr>
<td class="name">parentId</td>
<td class="type"><span class="param-type">string</span></td>
<td class="description">Pass the parent id to update the menu item</td>
</tr>
<tr>
<td class="name">spriteCssClass</td>
<td class="type"><span class="param-type">string</span></td>
<td class="description">Pass the sprite css class to update the menu item</td>
</tr>
</tbody>
</table>
</td></tr>
<tr>
<td class="name">index</td>
<td class="type"><span class="param-type">number</span></td>
<td class="description">pass the index of the item to be updated</td>
</tr>
</tbody>
</table>

#### Example

{% highlight html %}
<script>
//initialize the Spreadsheet object
var excelObj = $("#Spreadsheet").data("ejSpreadsheet");
excelObj.XLRibbon.updateMenuItem([{ id: "SignIn1", text: "AddMenuItem", parentId: "FILE", spriteCssClass: "e-icon e-ssr-cut"}], 3); // To update the menu item in the file menu
</script>

{% endhighlight %}

### XLRibbon.updateRibbonIcons()
{:#methods:xlribbon-updateribbonicons}

This method is used to update the ribbon icons in the Spreadsheet.

#### Example

{% highlight html %}
<script>
//initialize the Spreadsheet object
var excelObj = $("#Spreadsheet").data("ejSpreadsheet");
// To update the ribbon icons in the spreadsheet based on the active sheet index.
excelObj.XLRibbon.updateRibbonIcons();
</script>

{% endhighlight %}

### XLScroll
{:#methods:xlscroll}

### XLScroll.scrollToCell(cellAddr)
{:#methods:xlscroll-scrolltocell}

This method is used to scroll the sheet content to the specified cell address in the Spreadsheet.

<table class="params">
<thead>
<tr>
<th>Name</th>
<th>Type</th>
<th>Description</th>
</tr>
</thead>
<tbody>
<tr>
<td class="name">range</td>
<td class="type"><span class="param-type">string</span></td>
<td class="description">Pass the cell address that you want to scroll to it.</td>
</tr>
</tbody>
</table>

#### Example

{% highlight html %}
<script>
// Initialize the Spreadsheet object.
var excelObj = $("#Spreadsheet").data("ejSpreadsheet");
// To scroll the sheet to the specified cell address.
excelObj.XLScroll.scrollToCell("A30");
</script>

{% endhighlight %}

### XLSearch
{:#methods:xlsearch}

## XLSearch.findNext(value, options, sIndex)
{:#methods:xlsearch-findnext}

This method is used to find the next occurrence of given value in the sheet/workbook.  

<table class="params">
<thead>
<tr>
<th>Name</th>
<th>Type</th>
<th>Description</th>
</tr>
</thead>
<tbody>
<tr>
<td class="name">value</td>
<td class="type"><span class="param-type">string</span></td>
<td class="description">Pass the value to search.</td>
</tr>
<tr>
<td class="name">options</td>
<td class="type"><ts ref="SearchOptions"/><span class="param-type">Object</span></td>
<td class="description">Pass Object SearchOptions.
<table class="params">
<thead>
<tr>
<th>Name</th>
<th>Type</th>
<th>Description</th>
</tr>
</thead>
<tbody>
<tr>
<td class="name">isCSen</td>
<td class="type"><span class="param-type">boolean</span></td>
<td class="description">Pass the condition to find previous</td>
</tr>
<tr>
<td class="name">isEMatch</td>
<td class="type"><span class="param-type">boolean</span></td>
<td class="description">Pass the condition to find previous</td>
</tr>
<tr>
<td class="name">type</td>
<td class="type"><span class="param-type">string</span></td>
<td class="description">Pass the type to find previous</td>
</tr>
<tr>
<td class="name">mode</td>
<td class="type"><span class="param-type">string</span></td>
<td class="description">Pass the mode to find previous</td>
</tr>
<tr>
<td class="name">searchBy</td>
<td class="type"><span class="param-type">string</span></td>
<td class="description">Pass the search by to find previous</td>
</tr>
</tbody>
</table>
</td></tr>
<tr>
<td class="name">sIndex</td>
<td class="type"><span class="param-type">number</span></td>
<td class="description">Pass the sheet index.</td>
</tr>
</tbody>
</table>

#### Example

{% highlight html %}
<div id="Spreadsheet"></div>
<script>
// Initialize the Spreadsheet object.
var excelObj = $("#Spreadsheet").data("ejSpreadsheet");
// To find the next occurrence of given value.
excelObj.XLSearch.findNext("g", {isCSen: false, isEMatch: false, type: "value", mode: "sheet", searchBy: "rows"}, 1); 
</script>

{% endhighlight %}

## XLSearch.findPrevious(value, options, sIndex)
{:#methods:xlsearch-findprevious}

This method is used to find the previous occurrence of given value in the sheet/workbook.  

<table class="params">
<thead>
<tr>
<th>Name</th>
<th>Type</th>
<th>Description</th>
</tr>
</thead>
<tbody>
<tr>
<td class="name">value</td>
<td class="type"><span class="param-type">string</span></td>
<td class="description">Pass the value to search.</td>
</tr>
<tr>
<td class="name">options</td>
<td class="type"><ts ref="SearchOptions"/><span class="param-type">Object</span></td>
<td class="description">Pass Object SearchOptions.
<table class="params">
<thead>
<tr>
<th>Name</th>
<th>Type</th>
<th>Description</th>
</tr>
</thead>
<tbody>
<tr>
<td class="name">isCSen</td>
<td class="type"><span class="param-type">boolean</span></td>
<td class="description">Pass the condition to find previous</td>
</tr>
<tr>
<td class="name">isEMatch</td>
<td class="type"><span class="param-type">boolean</span></td>
<td class="description">Pass the condition to find previous</td>
</tr>
<tr>
<td class="name">type</td>
<td class="type"><span class="param-type">string</span></td>
<td class="description">Pass the type to find previous</td>
</tr>
<tr>
<td class="name">mode</td>
<td class="type"><span class="param-type">string</span></td>
<td class="description">Pass the mode to find previous</td>
</tr>
<tr>
<td class="name">searchBy</td>
<td class="type"><span class="param-type">string</span></td>
<td class="description">Pass the search by to find previous</td>
</tr>
</tbody>
</table>
</td></tr>
<tr>
<td class="name">sIndex</td>
<td class="type"><span class="param-type">number</span></td>
<td class="description">Pass the sheet index.</td>
</tr>
</tbody>
</table>

#### Example

{% highlight html %}
<div id="Spreadsheet"></div>
<script>
// Initialize the Spreadsheet object.
var excelObj = $("#Spreadsheet").data("ejSpreadsheet");
 // To find the previous occurrence of given value.
excelObj.XLSearch.findPrevious("g", {isCSen: true, isEMatch: false, type: "value", mode: "sheet", searchBy: "columns"}, 1);
</script>

{% endhighlight %}

## XLSearch.goTo(range)
{:#methods:xlsearch-goto}

This method is used to perform goto operation in the Spreadsheet.  

<table class="params">
<thead>
<tr>
<th>Name</th>
<th>Type</th>
<th>Description</th>
</tr>
</thead>
<tbody>
<tr>
<td class="name">range</td>
<td class="type"><span class="param-type">string</span></td>
<td class="description">Pass the range to perform goto operation.</td>
</tr>
</tbody>
</table>

#### Example

{% highlight html %}
<div id="Spreadsheet"></div>
<script>
// Initialize the Spreadsheet object.
var excelObj = $("#Spreadsheet").data("ejSpreadsheet");
excelObj.XLSearch.goTo("L4"); // To perform goto operation.
</script>

{% endhighlight %}

## XLSearch.goToSpecial(type, options)
{:#methods:xlsearch-gotospecial}

This method is used to perform goto special operation in the Spreadsheet.

<table class="params">
<thead>
<tr>
<th>Name</th>
<th>Type</th>
<th>Description</th>
</tr>
</thead>
<tbody>
<tr>
<td class="name">type</td>
<td class="type"><span class="param-type">string</span></td>
<td class="description">Pass the type of the cell.</td>
</tr>
<tr>
<td class="name">options</td>
<td class="type"><ts ref="GotoOptions"/><span class="param-type">Object</span></td>
<td class="description">Pass Object GotoOptions.
<table class="params">
<thead>
<tr>
<th>Name</th>
<th>Type</th>
<th>Description</th>
</tr>
</thead>
<tbody>
<tr>
<td class="name">isNumber</td>
<td class="type"><span class="param-type">boolean</span></td>
<td class="description">Pass the isNumber condition to perform goto special</td>
</tr>
<tr>
<td class="name">isText</td>
<td class="type"><span class="param-type">boolean</span></td>
<td class="description">Pass the isText condition to perform goto special</td>
</tr>
<tr>
<td class="name">isLogical</td>
<td class="type"><span class="param-type">boolean</span></td>
<td class="description">Pass the isLogical condition to perform goto special</td>
</tr>
<tr>
<td class="name">isError</td>
<td class="type"><span class="param-type">boolean</span></td>
<td class="description">Pass the isError condition to perform goto special</td>
</tr>
</tbody>
</table>
</td></tr>
</tbody>
</table>

#### Example

{% highlight html %}
<div id="Spreadsheet"></div>
<script>
// Initialize the Spreadsheet object.
var excelObj = $("#Spreadsheet").data("ejSpreadsheet");
// To perform goto special operation.
excelObj.XLSearch.goToSpecial("comments",{isNumber:true, isText:true, isLogical:true, isError: true}); 
</script>

{% endhighlight %}

### XLSearch.replaceAllByBook(findData, replaceData, isCSen, isEMatch)
{:#methods:xlsearch-replaceallbybook}

This method is used to find and replace all data by workbook in the Spreadsheet.
<table class="params">
<thead>
<tr>
<th>Name</th>
<th>Type</th>
<th>Description</th>
</tr>
</thead>
<tbody>
<tr>
<td class="name">findData</td>
<td class="type"><span class="param-type">string</span></td>
<td class="description">Pass the search data.</td>
</tr>
<tr>
<td class="name">replaceData</td>
<td class="type"><span class="param-type">string</span></td>
<td class="description">Pass the replace data.</td>
</tr>
<tr>
<td class="name">isCSen</td>
<td class="type"><span class="param-type">boolean</span></td>
<td class="description">Pass {{'`true`' | markdownify}}, if you want to match with case-sensitive.</td>
</tr>
<tr>
<td class="name">isEMatch</td>
<td class="type"><span class="param-type">boolean</span></td>
<td class="description">Pass {{'`true`' | markdownify}}, if you want to match with entire cell contents.</td>
</tr>
</tbody>
</table>

#### Example

{% highlight html %}
<script>
// initialize Spreadsheet object.
var excelObj = $("#Spreadsheet").data("ejSpreadsheet");
excelObj.XLSearch.replaceAllByBook("Sheet", "Spreadsheet", true, false); // Sends a replace all by workbook request to the Spreadsheet.
</script>

{% endhighlight %}

### XLSearch.replaceAllBySheet(findData, replaceData, isCSen, isEMatch)
{:#methods:xlsearch-replaceallbysheet}

This method is used to find and replace all data by sheet in Spreadsheet.
<table class="params">
<thead>
<tr>
<th>Name</th>
<th>Type</th>
<th>Description</th>
</tr>
</thead>
<tbody>
<tr>
<td class="name">findData</td>
<td class="type"><span class="param-type">string</span></td>
<td class="description">Pass the search data.</td>
</tr>
<tr>
<td class="name">replaceData</td>
<td class="type"><span class="param-type">string</span></td>
<td class="description">Pass the replace data.</td>
</tr>
<tr>
<td class="name">isCSen</td>
<td class="type"><span class="param-type">boolean</span></td>
<td class="description">Pass {{'`true`' | markdownify}}, if you want to match with case-sensitive.</td>
</tr>
<tr>
<td class="name">isEMatch</td>
<td class="type"><span class="param-type">boolean</span></td>
<td class="description">Pass {{'`true`' | markdownify}}, if you want to match with entire cell contents.</td>
</tr>
</tbody>
</table>

#### Example

{% highlight html %}
<script>
// initialize Spreadsheet object.
var excelObj = $("#Spreadsheet").data("ejSpreadsheet");
excelObj.XLSearch.replaceAllBySheet("Sheet", "Spreadsheet", true, false); // Sends a replace all by sheet request to Spreadsheet
</script>

{% endhighlight %}

### XLSelection
{:#methods:xlselection}

### XLSelection.clearAll()
{:#methods:xlselection-clearall}

This method is used to clear the selection of the active sheet in the Spreadsheet.

#### Example

{% highlight html %}

<div id="Spreadsheet"></div> 
<script>
// Initialize Spreadsheet object.
var excelObj = $("#Spreadsheet").data("ejSpreadsheet");
excelObj.XLSelection.clearAll(); // To clear selection.
</script>

{% endhighlight %}

### XLSelection.getSelectedCells(sheetIdx)
{:#methods:xlselection-getselectedcells}

This method is used to get the selected cells element based on specified sheet index in the Spreadsheet.
<table class="params">
<thead>
<tr>
<th>Name</th>
<th>Type</th>
<th>Description</th>
</tr>
</thead>
<tbody>
<tr>
<td class="name">sheetIdx</td>
<td class="type"><span class="param-type">number</span></td>
<td class="description">Pass the sheet index to get the cells element.</td>
</tr>
</tbody>
</table>

#### Returns:
Element

#### Example

{% highlight html %}
<div id="Spreadsheet"></div>
<script>
// Initialize the Spreadsheet object.
var excelObj = $("#Spreadsheet").data("ejSpreadsheet");
excelObj.XLSelection.getSelectedCells(1); //Gets the selected cells element.
</script>

{% endhighlight %}

### XLSelection.refreshSelection(\[range\])
{:#methods:xlselection-refreshselection}

This method is used to refresh the selection in the Spreadsheet.
<table class="params">
<thead>
<tr>
<th>Name</th>
<th>Type</th>
<th>Description</th>
</tr>
</thead>
<tbody>
<tr>
<td class="name">range</td>
<td class="type"><span class="param-type">Array|string</span></td>
<td class="description"><span class="optional">Optional.</span> Pass range to refresh selection.</td>
</tr>
</tbody>
</table>

#### Example

{% highlight html %}
<script>
//initialize the Spreadsheet object.
var excelObj = $("#Spreadsheet").data("ejSpreadsheet");
// To defined refresh selection in Spreadsheet.
excelObj.XLSelection.refreshSelection("A1:D3");
</script>

{% endhighlight %}

### XLSelection.selectColumn(colIdx)
{:#methods:xlselection-selectcolumn}

This method is used to select a single column in the Spreadsheet.
<table class="params">
<thead>
<tr>
<th>Name</th>
<th>Type</th>
<th>Description</th>
</tr>
</thead>
<tbody>
<tr>
<td class="name">colIdx</td>
<td class="type"><span class="param-type">number</span></td>
<td class="description">Pass the column index value.</td>
</tr>
</tbody>
</table>

#### Example

{% highlight html %}
<script>
// initialize Spreadsheet object.
var excelObj = $("#Spreadsheet").data("ejSpreadsheet");
excelObj.XLSelection.selectColumn(1); //To select a single column in the active sheet.
</script>

{% endhighlight %}

### XLSelection.selectColumns(startIdx, endIdx)
{:#methods:xlselection-selectcolumns}

This method is used to select entire columns in a specified range (start index and end index) in the Spreadsheet.
<table class="params">
<thead>
<tr>
<th>Name</th>
<th>Type</th>
<th>Description</th>
</tr>
</thead>
<tbody>
<tr>
<td class="name">startIdx</td>
<td class="type"><span class="param-type">number</span></td>
<td class="description">Pass the column start index.</td>
</tr>
<tr>
<td class="name">endIdx</td>
<td class="type"><span class="param-type">number</span></td>
<td class="description">Pass the column end index.</td>
</tr>
</tbody>
</table>

#### Example

{% highlight html %}
<script>
// initialize Spreadsheet object.
var excelObj = $("#Spreadsheet").data("ejSpreadsheet");
excelObj.XLSelection.selectColumns(2, 4); //To select entire columns in the specified range.
</script>

{% endhighlight %}

### XLSelection.selectRange(range)
{:#methods:xlselection-selectrange}

This method is used to select the specified range of cells in the Spreadsheet.
<table class="params">
<thead>
<tr>
<th>Name</th>
<th>Type</th>
<th>Description</th>
</tr>
</thead>
<tbody>
<tr>
<td class="name">range</td>
<td class="type"><span class="param-type">string</span></td>
<td class="description">Pass range which want to select.</td>
</tr>
</tbody>
</table>

#### Example

{% highlight html %}
<script>
// initialize Spreadsheet object.
var excelObj = $("#Spreadsheet").data("ejSpreadsheet");
excelObj.XLSelection.selectRange("A1:B2"); //To select range of cells in Spreadsheet.
</script>
{% endhighlight %}

### XLSelection.selectRow(rowIdx)
{:#methods:xlselection-selectrow}

This method is used to select a single row in the Spreadsheet.
<table class="params">
<thead>
<tr>
<th>Name</th>
<th>Type</th>
<th>Description</th>
</tr>
</thead>
<tbody>
<tr>
<td class="name">rowIdx</td>
<td class="type"><span class="param-type">number</span></td>
<td class="description">Pass the row index value.</td>
</tr>
</tbody>
</table>

#### Example

{% highlight html %}
<script>
// initialize Spreadsheet object.
var excelObj = $("#Spreadsheet").data("ejSpreadsheet");
excelObj.XLSelection.selectRow(1); //To select a single row in the specified sheet index in Spreadsheet.
</script>

{% endhighlight %}

### XLSelection.selectRows(startIdx, endIdx)
{:#methods:xlselection-selectrows}

This method is used to select entire rows in a specified range (start index and end index) in the Spreadsheet.
<table class="params">
<thead>
<tr>
<th>Name</th>
<th>Type</th>
<th>Description</th>
</tr>
</thead>
<tbody>
<tr>
<td class="name">startIdx</td>
<td class="type"><span class="param-type">number</span></td>
<td class="description">Pass the start row index.</td>
</tr>
<tr>
<td class="name">endIdx</td>
<td class="type"><span class="param-type">number</span></td>
<td class="description">Pass the end row index.</td>
</tr>
</tbody>
</table>

#### Example

{% highlight html %}
<script>
// Initialize Spreadsheet object.
var excelObj = $("#Spreadsheet").data("ejSpreadsheet");
excelObj.XLSelection.selectRows(2, 4); //To select entire rows in the specified range.
</script>

{% endhighlight %}

### XLSelection.selectSheet()
{:#methods:xlselection-selectsheet}

This method is used to select all cells in active sheet.

#### Example

{% highlight html %}
<script>
// Initialize Spreadsheet object.
var excelObj = $("#Spreadsheet").data("ejSpreadsheet");
excelObj.XLSelection.selectSheet(); //To select all cells in a sheet
</script>

{% endhighlight %}

### XLShape
{:#methods:xlshape}

## XLShape.changePicture(pictureId, url)
{:#methods:xlshape-changepicture}

This method is used to change the picture.

<table class="params">
<thead>
<tr>
<th>Name</th>
<th>Type</th>
<th>Description</th>
</tr>
</thead>
<tbody>
<tr>
<td class="name">pictureId</td>
<td class="type"><span class="param-type">string</span></td>
<td class="description">Pass the id of the picture.</td>
</tr>
<tr>
<td class="name">url</td>
<td class="type"><span class="param-type">string</span></td>
<td class="description">Pass the relative path of the picture.</td>
</tr>
</tbody>
</table>

#### Example

{% highlight html %}
<div id="Spreadsheet"></div>
<script>
// Initialize the Spreadsheet object.
var excelObj = $("#Spreadsheet").data("ejSpreadsheet");
excelObj.XLShape.changePicture('Spreadsheet_picture1', "img.png"); // To change the picture.
</script>

{% endhighlight %}

## XLShape.changePictureBorder(pictureId, width, style, color)
{:#methods:xlshape-changepictureborder}

This method is used to change the border of the picture.  

<table class="params">
<thead>
<tr>
<th>Name</th>
<th>Type</th>
<th>Description</th>
</tr>
</thead>
<tbody>
<tr>
<td class="name">pictureId</td>
<td class="type"><span class="param-type">string</span></td>
<td class="description">Pass the id of the picture.</td>
</tr>
<tr>
<td class="name">width</td>
<td class="type"><span class="param-type">string</span></td>
<td class="description">Pass the width of the border.</td>
</tr>
<tr>
<td class="name">style</td>
<td class="type"><span class="param-type">string</span></td>
<td class="description">Pass the style of the border.</td>
</tr>
<tr>
<td class="name">color</td>
<td class="type"><span class="param-type">string</span></td>
<td class="description">Pass the color of the border.</td>
</tr>
</tbody>
</table>

#### Example

{% highlight html %}
<div id="Spreadsheet"></div>
<script>
// Initialize the Spreadsheet object.
var excelObj = $("#Spreadsheet").data("ejSpreadsheet");
// To change the border of the picture.
excelObj.XLShape.changePictureBorder("Spreadsheet_picture1", "1px", "solid", "#89c987"); 
</script>

{% endhighlight %}

## XLShape.resetPicture(pictureId, action)
{:#methods:xlshape-resetpicture}

This method is used to reset the picture.

<table class="params">
<thead>
<tr>
<th>Name</th>
<th>Type</th>
<th>Description</th>
</tr>
</thead>
<tbody>
<tr>
<td class="name">pictureId</td>
<td class="type"><span class="param-type">string</span></td>
<td class="description">Pass the id of the picture.</td>
</tr>
<tr>
<td class="name">action</td>
<td class="type"><span class="param-type">string</span></td>
<td class="description">Pass the type of action.</td>
</tr>
</tbody>
</table>

#### Example

{% highlight html %}
<div id="Spreadsheet"></div>
<script>
// Initialize the Spreadsheet object.
var excelObj = $("#Spreadsheet").data("ejSpreadsheet"), pictureId = "Spreadsheet_picture1";
excelObj.XLShape.resetPicture(pictureId, "resetSize"); // To reset the picture.
</script>

{% endhighlight %}

### XLShape.setPicture(range, url, width, height, top, left)
{:#methods:xlshape-setpicture}

This method is used to set a picture in the Spreadsheet.

<table class="params">
<thead>
<tr>
<th>Name</th>
<th>Type</th>
<th>Description</th>
</tr>
</thead>
<tbody>
<tr>
<td class="name">range</td>
<td class="type"><span class="param-type">string</span></td>
<td class="description">Pass the range of the cell.</td>
</tr>
<tr>
<td class="name">url</td>
<td class="type"><span class="param-type">string</span></td>
<td class="description">Pass the path of the specified image.</td>
</tr>
<tr>
<td class="name">width</td>
<td class="type"><span class="param-type">number</span></td>
<td class="description"><span class="optional">Optional.</span> Pass the width of the image that you want to set.</td>
</tr>
<tr>
<td class="name">height</td>
<td class="type"><span class="param-type">number</span></td>
<td class="description"><span class="optional">Optional.</span> Pass the height of the image that you want to set.</td>
</tr>
<tr>
<td class="name">top</td>
<td class="type"><span class="param-type">number</span></td>
<td class="description"><span class="optional">Optional.</span> Pass the top of the image that you want to set.</td>
</tr>
<tr>
<td class="name">left</td>
<td class="type"><span class="param-type">number</span></td>
<td class="description"><span class="optional">Optional.</span> Pass the left of the image that you want to set.</td>
</tr>
</tbody>
</table>

#### Returns:
string

#### Example

{% highlight html %}
<script>
// Initialize Spreadsheet object.
var excelObj = $("#Spreadsheet").data("ejSpreadsheet");
//To set the picture in the Spreadsheet.
excelObj.XLShape.setPicture('D4', "../images/spreadsheet/ladybug.png", 538, 319);
</script>
 
{% endhighlight %}

### XLSort
{:#methods:xlsort}

### XLSort.sortByColor(operation, color, range)
{:#methods:xlsort-sortbycolor}

This method is used to sort a particular range of cells based on its cell or font color in the Spreadsheet.

<table class="params">
<thead>
<tr>
<th>Name</th>
<th>Type</th>
<th>Description</th>
</tr>
</thead>
<tbody>
<tr>
<td class="name">operation</td>
<td class="type"><span class="param-type">string</span></td>
<td class="description">Pass {{'`PutCellColor`' | markdownify}} to sort by cell color or {{'`PutFontColor`' | markdownify}} for sort by font color.</td>
</tr>
<tr>
<td class="name">color</td>
<td class="type"><ts ref="ColorOptions"/><span class="param-type">Object</span></td>
<td class="description">Pass Object ColorOptions.
<table class="params">
<thead>
<tr>
<th>Name</th>
<th>Type</th>
<th>Description</th>
</tr>
</thead>
<tbody>
<tr>
<td class="name">backgroundColor</td>
<td class="type"><span class="param-type">string</span></td>
<td class="description">Pass the background color to sort the cell</td>
</tr>
<tr>
<td class="name">color</td>
<td class="type"><span class="param-type">string</span></td>
<td class="description">Pass the color to sort the cell</td>
</tr>
</tbody>
</table>
</td></tr>
<tr>
<td class="name">range</td>
<td class="type"><span class="param-type">string</span></td>
<td class="description">Pass the range</td>
</tr>
</tbody>
</table>

#### Example

{% highlight html %}
<script>
// Initialize Spreadsheet object.
var excelObj = $("#Spreadsheet").data("ejSpreadsheet");
//To sort range based on cell color in the Spreadsheet.
excelObj.XLSort.sortByColor("PutCellColor", {"background-color" : "#EC2024", color:  "#6N2N2N"}, "D2:D8"); </script>

{% endhighlight %}

### XLSort.sortByRange(range, columnName, direction)
{:#methods:xlsort-sortbyrange}

This method is used to sort a particular range of cells based on its values in the Spreadsheet.
<table class="params">
<thead>
<tr>
<th>Name</th>
<th>Type</th>
<th>Description</th>
</tr>
</thead>
<tbody>
<tr>
<td class="name">range</td>
<td class="type"><span class="param-type">Array|string</span></td>
<td class="description">Pass the range to sort.</td>
</tr>
<tr>
<td class="name">columnName</td>
<td class="type"><span class="param-type">string</span></td>
<td class="description">Pass the column name.</td>
</tr>
<tr>
<td class="name">direction</td>
<td class="type"><span class="param-type">string</span></td>
<td class="description">Pass the direction to sort</td>
</tr>
</tbody>
</table>

#### Returns:
boolean

#### Example

{% highlight html %}
<script>
// Initialize Spreadsheet object.
var excelObj = $("#Spreadsheet").data("ejSpreadsheet");
//To sort the cell value in a specified range in the Spreadsheet.
excelObj.XLSort.sortByRange("A1:D3", "B",  "ascending"); 
</script>

{% endhighlight %}

### XLSparkline
{:#methods:xlsparkline}

### XLSparkline.createSparkline(dataRange, locationRange, type, options, \[sheetIndex\])
{:#methods:xlsparkline-createsparkline}

This method used for creating the sparkline chart for specified range in spreadsheet.

<table class="params">
<thead>
<tr>
<th>Name</th>
<th>Type</th>
<th>Description</th>
</tr>
</thead>
<tbody>
<tr>
<td class="name">dataRange</td>
<td class="type"><span class="param-type">String</span></td>
<td class="description">Pass the data range</td>
</tr>
<tr>
<td class="name">locationRange</td>
<td class="type"><span class="param-type">String</span></td>
<td class="description">Pass the location range</td>
</tr>
<tr>
<td class="name">type</td>
<td class="type"><span class="param-type">String</span></td>
<td class="description">Pass the sparkline chart type</td>
</tr>
<tr>
<td class="name">options</td>
<td class="type"><ts ref="SparklineOptions"/><span class="param-type">Object</span></td>
<td class="description">Pass Object SparklineOptions.
<table class="params">
<thead>
<tr>
<th>Name</th>
<th>Type</th>
<th>Description</th>
</tr>
</thead>
<tbody>
<tr>
<td class="name">markerSettings</td>
<td class="type"><span class="param-type">object</span></td>
<td class="description">Pass the marker settings object to create sparkline</td>
</tr>
<tr>
<td class="name">highPointColor</td>
<td class="type"><span class="param-type">string</span></td>
<td class="description">Pass the high point color to create sparkline</td>
</tr>
<tr>
<td class="name">negativePointColor</td>
<td class="type"><span class="param-type">string</span></td>
<td class="description">Pass the negative point color to create sparkline</td>
</tr>
<tr>
<td class="name">startPointColor</td>
<td class="type"><span class="param-type">string</span></td>
<td class="description">Pass the start point color to create sparkline</td>
</tr>
</tbody>
</table>
</td></tr>
<tr>
<td class="name">sheetIndex</td>
<td class="type"><span class="param-type">Number</span></td>
<td class="description">Pass the sheetIndex</td>
</tr>
</tbody>
</table>

#### Example

{% highlight html %}
<script>

// Initialize the Spreadsheet object.
var excelObj = $("#Spreadsheet").data("ejSpreadsheet");
// To create the sparkline chart
excelObj.XLSparkline.createSparkline("C3:C5", "F10",  "Line", {markerSettings:{visible:true},highPointColor: "red", negativePointColor: "black", startPointColor: "green"} ); // To create sparkline in Spreadsheet.

</script>

{% endhighlight %}

### XLSparkline.changePointColor(sparklineId, option, \[sheetIdx\])
{:#methods:xlsparkline-changepointcolor}

This method used to change the sparkline color and marker point color in the spreadsheet.

<table class="params">
<thead>
<tr>
<th>Name</th>
<th>Type</th>
<th>Description</th>
</tr>
</thead>
<tbody>
<tr>
<td class="name">sparklineId</td>
<td class="type"><span class="param-type">String</span></td>
<td class="description">Pass the sparkline ID</td>
</tr>
<tr>
<td class="name">option</td>
<td class="type"><span class="param-type">Object</span></td>
<td class="description"> pass the high point color as object.</td>
</tr>
<tr>
<td class="name">sheetIdx</td>
<td class="type"><span class="param-type">Number</span></td>
<td class="description"><span class="optional">Optional.</span> Pass the sheet index</td>
</tr>
</tbody>
</table>

#### Example

{% highlight html %}

<script>
// Initialize the Spreadsheet object.
var excelObj = $("#Spreadsheet").data("ejSpreadsheet");
// To change the sparkline color and marker color 
excelObj.XLSparkline.changePointColor("Spreadsheet_S1_Column_2_6", {highPointColor: "red"});
</script>

{% endhighlight %}

### XLSparkline.changeType(sparklineId, type, \[sheetIdx\])
{:#methods:xlsparkline-changetype}

This method used to change the sparkline type in the spreadsheet.

<table class="params">
<thead>
<tr>
<th>Name</th>
<th>Type</th>
<th>Description</th>
</tr>
</thead>
<tbody>
<tr>
<td class="name">sparklineId</td>
<td class="type"><span class="param-type">String</span></td>
<td class="description">Pass the sparkline ID</td>
</tr>
<tr>
<td class="name">type</td>
<td class="type"><span class="param-type">string</span></td>
<td class="description">Pass the sparkline type</td>
</tr>
<tr>
<td class="name">sheetIdx</td>
<td class="type"><span class="param-type">Number</span></td>
<td class="description"><span class="optional">Optional.</span> Pass the sheet index</td>
</tr>
</tbody>
</table>

#### Example

{% highlight html %}

<script>
// Initialize the Spreadsheet object.
var excelObj = $("#Spreadsheet").data("ejSpreadsheet");
// To change the sparkline chart type
excelObj.XLSparkline.changeType("Spreadsheet_S1_Column_2_6", "Line");
</script>
{% endhighlight %}

### XLValidate
{:#methods:xlvalidate}

### XLValidate.applyDVRules(range, values, type, required, showErrorAlert)
{:#methods:xlvalidate-applydvrules}

This method is used to apply data validation rules in a selected range of cells based on the defined condition in the Spreadsheet.

<table class="params">
<thead>
<tr>
<th>Name</th>
<th>Type</th>
<th>Description</th>
</tr>
</thead>
<tbody>
<tr>
<td class="name">range</td>
<td class="type"><span class="param-type">string|Array</span></td>
<td class="description">If range is specified, it will apply rules for the specified range else it will use the current selected range. </td>
</tr>
<tr>
<td class="name">values</td>
<td class="type"><span class="param-type">Array</span></td>
<td class="description">Pass the validation condition, value1 and value2.</td>
</tr>
<tr>
<td class="name">type</td>
<td class="type"><span class="param-type">string</span></td>
<td class="description">Pass the data type.</td>
</tr>
<tr>
<td class="name">required</td>
<td class="type"><span class="param-type">boolean</span></td>
<td class="description">Pass {{'`true`' | markdownify}} if you ignore blank values.</td>
</tr>
<tr>
<td class="name">showErrorAlert</td>
<td class="type"><span class="param-type">boolean</span></td>
<td class="description">Pass {{'`true`' | markdownify}} if you want to show an error alert.</td>
</tr>
</tbody>
</table>

#### Example

{% highlight html %}
<script>
//Initialize the Spreadsheet object.
var excelObj = $("#Spreadsheet").data("ejSpreadsheet");
// To apply validation rule to allow whole number between 15 and 20.
excelObj.XLValidate.applyDVRules("A1:D3", ["Between", "15", "20"], "number" ,true, true);
</script>

{% endhighlight %}

### XLValidate.clearDV(\[range\])
{:#methods:xlvalidate-cleardv}

This method is used to clear the applied validation rules in a specified range of cells in the Spreadsheet.

<table class="params">
<thead>
<tr>
<th>Name</th>
<th>Type</th>
<th>Description</th>
</tr>
</thead>
<tbody>
<tr>
<td class="name">range</td>
<td class="type"><span class="param-type">string|Array</span></td>
<td class="description"><span class="optional">Optional.</span> If range is specified, it will clear rules for the specified range else it will use the current selected range. </td>
</tr>
</tbody>
</table>

#### Example

{% highlight html %}
<script>
// Initialize the Spreadsheet object.
var spreadsheetObj = $("#Spreadsheet").data("ejSpreadsheet");
// To clear validation rules in selected cells.
spreadsheetObj.XLValidate.clearDV("A2:A7");
</script>

{% endhighlight %}

## XLValidate.clearHighlightedValData(range)
{:#methods:xlvalidate-clearhighlightedvaldata}

This method is used to clear invalid data highlights in the given range.  

<table class="params">
<thead>
<tr>
<th>Name</th>
<th>Type</th>
<th>Description</th>
</tr>
</thead>
<tbody>
<tr>
<td class="name">range</td>
<td class="type"><span class="param-type">string</span></td>
<td class="description">Pass the range to clear highlights.</td>
</tr>
</tbody>
</table>

#### Example

{% highlight html %}
<div id="Spreadsheet"></div>
<script>
// Initialize the Spreadsheet object.
var excelObj = $("#Spreadsheet").data("ejSpreadsheet");
excelObj.XLValidate.clearHighlightedValData("A1:K15"); // To clear highlighted data.
</script>

{% endhighlight %}

### XLValidate.highlightInvalidData(\[range\])
{:#methods:xlvalidate-highlightinvaliddata}

This method is used to highlight invalid data in a specified range of cells in the Spreadsheet.
<table class="params">
<thead>
<tr>
<th>Name</th>
<th>Type</th>
<th>Description</th>
</tr>
</thead>
<tbody>
<tr>
<td class="name">range</td>
<td class="type"><span class="param-type">string|Array</span></td>
<td class="description"><span class="optional">Optional.</span> If range is specified, it will clear rules for the specified range else it will use the current selected range.</td>
</tr>
</tbody>
</table>

#### Example

{% highlight html %}
<div id="Spreadsheet"></div>
<script>
//initialize the Spreadsheet object
var spreadsheetObj = $("#Spreadsheet").data("ejSpreadsheet");
// To highlight invalid cell data
spreadsheetObj.XLValidate.highlightInvalidData("A2:A7");
</script>

{% endhighlight %}

## Events

### actionBegin
{:#events:actionbegin}

Triggered for every action before its starts.

<table class="params">
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
<td class="description">Arguments when actionBegin event is triggered. 
<table class="params">
<thead>
<tr>
<th>Name</th>
<th>Type</th>
<th>Description</th>
</tr>
</thead>
<tbody>
<tr>
<td class="name">afterFormat</td>
<td class="type"><span class="param-type">Object</span></td>
<td class="description">Returns the applied style format object.</td>
</tr>
<tr>
<td class="name">beforeFormat</td>
<td class="type"><span class="param-type">Object</span></td>
<td class="description">Returns the applied style format object.</td>
</tr>
<tr>
<td class="name">sheetIdx</td>
<td class="type"><span class="param-type">number</span></td>
<td class="description">Returns the sheet index.</td>
</tr>
<tr>
<td class="name">range</td>
<td class="type"><span class="param-type">Array</span></td>
<td class="description">Returns the cell range.</td>
</tr>
<tr>
<td class="name">reqType</td>
<td class="type"><span class="param-type">string</span></td>
<td class="description">Returns the action format.</td>
</tr>
<tr>
<td class="name">gotoIdx</td>
<td class="type"><span class="param-type">number</span></td>
<td class="description">Returns goto index while paging.</td>
</tr>
<tr>
<td class="name">newSheet</td>
<td class="type"><span class="param-type">boolean</span></td>
<td class="description">Returns boolean value. If create new sheet it returns true.</td>
</tr>
<tr>
<td class="name">columnName</td>
<td class="type"><span class="param-type">string</span></td>
<td class="description">Return column name while sorting.</td>
</tr>
<tr>
<td class="name">colSelected</td>
<td class="type"><span class="param-type">number</span></td>
<td class="description">Returns selected columns while sorting or filtering begins.</td>
</tr>
<tr>
<td class="name">sortDirection</td>
<td class="type"><span class="param-type">string</span></td>
<td class="description">Returns sort direction while sort action begins.</td>
</tr>
</tbody>
</table>
</td></tr>
</tbody>
</table>

#### Example

{% highlight html %}
<div id="Spreadsheet"></div>
<script>
//actionBegin event for Spreadsheet
$("#Spreadsheet").ejSpreadsheet({
    actionBegin: function (args){}
});
</script>

{% endhighlight %}

### actionComplete
{:#events:actioncomplete}

Triggered for every action complete.
<table class="params">
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
<td class="description">Arguments when actionComplete event is triggered. 
<table class="params">
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
<td class="type"><ts ref="ej.Spreadsheet.Model"/><span class="param-type">Object</span></td>
<td class="description">Returns Spreadsheet model.</td>
</tr>
<tr>
<td class="name">selectedCell</td>
<td class="type"><span class="param-type">Array|Object</span></td>
<td class="description">Returns the applied cell format object.</td>
</tr>
<tr>
<td class="name">sheetIdx</td>
<td class="type"><span class="param-type">number</span></td>
<td class="description">Returns the sheet index.</td>
</tr>
<tr>
<td class="name">reqType</td>
<td class="type"><span class="param-type">string</span></td>
<td class="description">Returns the request type.</td>
</tr>
<tr>
<td class="name">cancel</td>
<td class="type"><span class="param-type">boolean</span></td>
<td class="description">Returns the cancel option value.</td>
</tr>
<tr>
<td class="name">type</td>
<td class="type"><span class="param-type">string</span></td>
<td class="description">Returns the name of the event.</td>
</tr>
</tbody>
</table>
</td></tr>
</tbody>
</table>

#### Example

{% highlight html %}
<div id="Spreadsheet"></div>
<script>
//actionComplete event for Spreadsheet
$("#Spreadsheet").ejSpreadsheet({
    actionComplete: function (args){}
});
</script>

{% endhighlight %}

### autoFillBegin
{:#events:autofillbegin}

Triggered when the auto fill operation begins.

<table class="params">
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
<td class="description">Arguments when autoFillBegin event is triggered. 
<table class="params">
<thead>
<tr>
<th>Name</th>
<th>Type</th>
<th>Description</th>
</tr>
</thead>
<tbody>
<tr>
<td class="name">dataRange</td>
<td class="type"><span class="param-type">Array</span></td>
<td class="description">Returns auto fill begin cell range.</td>
</tr>
<tr>
<td class="name">direction</td>
<td class="type"><span class="param-type">string</span></td>
<td class="description">Returns which direction drag the auto fill.</td>
</tr>
<tr>
<td class="name">fillRange</td>
<td class="type"><span class="param-type">Array</span></td>
<td class="description">Returns fill cells range.</td>
</tr>
<tr>
<td class="name">fillType</td>
<td class="type"><span class="param-type">string</span></td>
<td class="description">Returns the auto fill type.</td>
</tr>
<tr>
<td class="name">sheetIdx</td>
<td class="type"><span class="param-type">number</span></td>
<td class="description">Returns the sheet index.</td>
</tr>
<tr>
<td class="name">model</td>
<td class="type"><ts ref="ej.Spreadsheet.Model"/><span class="param-type">Object</span></td>
<td class="description">Returns the Spreadsheet model.</td>
</tr>
<tr>
<td class="name">type</td>
<td class="type"><span class="param-type">string</span></td>
<td class="description">Returns the name of the event.</td>
</tr><tr>
<td class="name">cancel</td>
<td class="type"><span class="param-type">boolean</span></td>
<td class="description">Returns the cancel option value.</td>
</tr>
</tbody>
</table>
</td></tr>
</tbody>
</table>

#### Example

{% highlight html %}
<div id="Spreadsheet"></div>
<script>
//autoFillBegin event for Spreadsheet
$("#Spreadsheet").ejSpreadsheet({
    autoFillBegin: function (args){}
});
</script>

{% endhighlight %}

### autoFillComplete
{:#events:autofillcomplete}

Triggered when the auto fill operation completes.

<table class="params">
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
<td class="description">Arguments when autoFillComplete event is triggered. 
<table class="params">
<thead>
<tr>
<th>Name</th>
<th>Type</th>
<th>Description</th>
</tr>
</thead>
<tbody>
<tr>
<td class="name">dataRange</td>
<td class="type"><span class="param-type">Array</span></td>
<td class="description">Returns auto fill begin cell range.</td>
</tr>
<tr>
<td class="name">direction</td>
<td class="type"><span class="param-type">string</span></td>
<td class="description">Returns which direction to drag the auto fill.</td>
</tr>
<tr>
<td class="name">fillRange</td>
<td class="type"><span class="param-type">Array</span></td>
<td class="description">Returns fill cells range.</td>
</tr>
<tr>
<td class="name">fillType</td>
<td class="type"><span class="param-type">string</span></td>
<td class="description">Returns the auto fill type.</td>
</tr>
<tr>
<td class="name">sheetIdx</td>
<td class="type"><span class="param-type">number</span></td>
<td class="description">Returns the sheet index.</td>
</tr>
<tr>
<td class="name">model</td>
<td class="type"><ts ref="ej.Spreadsheet.Model"/><span class="param-type">Object</span></td>
<td class="description">Returns the Spreadsheet model.</td>
</tr>
<tr>
<td class="name">type</td>
<td class="type"><span class="param-type">string</span></td>
<td class="description">Returns the name of the event.</td>
</tr>
<tr>
<td class="name">cancel</td>
<td class="type"><span class="param-type">boolean</span></td>
<td class="description">Returns the cancel option value.</td>
</tr>
</tbody>
</table>
</td></tr>
</tbody>
</table>

#### Example

{% highlight html %}
<div id="Spreadsheet"></div>
<script>
//autoFillComplete event for Spreadsheet
$("#Spreadsheet").ejSpreadsheet({
    autoFillComplete: function (args){}
});
</script>

{% endhighlight %}

### beforeBatchSave
{:#events:beforebatchsave}

Triggered before the batch save.

<table class="params">
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
<td class="description">Arguments when beforeBatchSave event is triggered. 
<table class="params">
<thead>
<tr>
<th>Name</th>
<th>Type</th>
<th>Description</th>
</tr>
</thead>
<tbody>
<tr>
<td class="name">sheetIdx</td>
<td class="type"><span class="param-type">number</span></td>
<td class="description">Returns the sheet index.</td>
</tr><tr>
<td class="name">dataSetting</td>
<td class="type"><span class="param-type">Object</span></td>
<td class="description">Returns the query, primary key,batch changes for the data Source.</td>
</tr>
<tr>
<td class="name">batchChanges</td>
<td class="type"><span class="param-type">Object</span></td>
<td class="description">Returns the changed record object.</td>
</tr>
</tbody>
</table>
</td></tr>
</tbody>
</table>

#### Example

{% highlight html %}
<div id="Spreadsheet"></div>
<script>
//beforeBatchSave event for Spreadsheet
$("#Spreadsheet").ejSpreadsheet({
    beforeBatchSave: function (args){}
});
</script>

{% endhighlight %}

### beforeCellFormat
{:#events:beforecellformat}

Triggered before the cells to be formatted.

<table class="params">
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
<td class="description">Arguments when beforeCellFormat event is triggered. 
<table class="params">
<thead>
<tr>
<th>Name</th>
<th>Type</th>
<th>Description</th>
</tr>
</thead>
<tbody>
<tr>
<td class="name">sheetIdx</td>
<td class="type"><span class="param-type">number</span></td>
<td class="description">Returns the sheet index.</td>
</tr><tr>
<td class="name">format</td>
<td class="type"><span class="param-type">Object</span></td>
<td class="description">Returns the applied style format object.</td>
</tr>
<tr>
<td class="name">cells</td>
<td class="type"><span class="param-type">Array|Object</span></td>
<td class="description">Returns the selected cells.</td>
</tr>
<tr>
<td class="name">model</td>
<td class="type"><ts ref="ej.Spreadsheet.Model"/><span class="param-type">Object</span></td>
<td class="description">Returns the Spreadsheet model.</td>
</tr>
<tr>
<td class="name">cancel</td>
<td class="type"><span class="param-type">boolean</span></td>
<td class="description">Returns the cancel option value.</td>
</tr>
<tr>
<td class="name">type</td>
<td class="type"><span class="param-type">string</span></td>
<td class="description">Returns the name of the event.</td>
</tr>
</tbody>
</table>
</td></tr>
</tbody>
</table>

#### Example

{% highlight html %}
<div id="Spreadsheet"></div>
<script>
//beforeCellFormat event for Spreadsheet
$("#Spreadsheet").ejSpreadsheet({
    beforeCellFormat: function (args){}
});
</script>

{% endhighlight %}


### beforeCellSelect
{:#events:beforecellselect}

Triggered before the cell selection.

<table class="params">
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
<td class="description">Arguments when beforeCellSelect event is triggered. 
<table class="params">
<thead>
<tr>
<th>Name</th>
<th>Type</th>
<th>Description</th>
</tr>
</thead>
<tbody>
<tr>
<td class="name">prevRange</td>
<td class="type"><span class="param-type">Array</span></td>
<td class="description">Returns the previous cell range.</td>
</tr>
<tr>
<td class="name">currRange</td>
<td class="type"><span class="param-type">Array</span></td>
<td class="description">Returns the current cell range.</td>
</tr>
<tr>
<td class="name">model</td>
<td class="type"><ts ref="ej.Spreadsheet.Model"/><span class="param-type">Object</span></td>
<td class="description">Returns the Spreadsheet model.</td>
</tr>
<tr>
<td class="name">type</td>
<td class="type"><span class="param-type">string</span></td>
<td class="description">Returns the name of the event.</td>
</tr>
<tr>
<td class="name">cancel</td>
<td class="type"><span class="param-type">boolean</span></td>
<td class="description">Returns the cancel option value.</td>
</tr>
</tbody>
</table>
</td></tr>
</tbody>
</table>

#### Example

{% highlight html %}
<div id="Spreadsheet"></div> 
<script>
// beforeCellSelect event for Spreadsheet
$('#Spreadsheet').ejSpreadsheet({   
    beforeCellSelect: function (args){}
});
</script>

{% endhighlight %}

### beforeDrop
{:#events:beforedrop}

Triggered before the selected cells are dropped.

<table class="params">
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
<td class="description">Arguments when beforeDrop event is triggered. 
<table class="params">
<thead>
<tr>
<th>Name</th>
<th>Type</th>
<th>Description</th>
</tr>
</thead>
<tbody>
<tr>
<td class="name">sheetIdx</td>
<td class="type"><span class="param-type">number</span></td>
<td class="description">Returns the sheet index.</td>
</tr>
<tr>
<td class="name">currentCell</td>
<td class="type"><span class="param-type">Object</span></td>
<td class="description">Returns the current cell row and column index.</td>
</tr>
<tr>
<td class="name">dragAndDropRange</td>
<td class="type"><span class="param-type">Object</span></td>
<td class="description">Returns the drag cells range object.</td>
</tr>
<tr>
<td class="name">preventAlert</td>
<td class="type"><span class="param-type">boolean</span></td>
<td class="description">Returns the cell Overwriting alert option value.</td>
</tr>
<tr>
<td class="name">model</td>
<td class="type"><ts ref="ej.Spreadsheet.Model"/><span class="param-type">Object</span></td>
<td class="description">Returns the Spreadsheet model.</td>
</tr>
<tr>
<td class="name">target</td>
<td class="type"><span class="param-type">Element</span></td>
<td class="description">Returns the target item.</td>
</tr>
<tr>
<td class="name">type</td>
<td class="type"><span class="param-type">string</span></td>
<td class="description">Returns the name of the event.</td>
</tr>
<tr>
<td class="name">cancel</td>
<td class="type"><span class="param-type">boolean</span></td>
<td class="description">Returns the cancel option value.</td>
</tr>
</tbody>
</table>
</td></tr>
</tbody>
</table>

#### Example

{% highlight html %}
<div id="Spreadsheet"></div>
<script>
//beforeDrop event for Spreadsheet.
$("#Spreadsheet").ejSpreadsheet({
    beforeDrop: function (args){}
});
</script>

{% endhighlight %}

### beforeEditComment
{:#events:beforeeditcomment}

Triggered while start to edit the comment.

<table class="params">
<tr>
<th>Name</th>
<th>Type</th>
<th>Description</th>
</tr>
<tr>
<td class="name">argument</td>
<td class="type"><span class="param-type">Object</span></td>
<td class="description">Arguments when beforeEditComment event is triggered.
<table>
<tr>
<th>Name</th>
<th>Type</th>
<th>Description</th></tr>
<tr>
<td class="name">sheetIdx</td>
<td class="type"><span class="param-type">number</span></td>
<td class="description">Returns the sheet index.</td>
</tr>
<tr>
<td class="name">cellIndex</td>
<td class="type"><span class="param-type">Object</span></td>
<td class="description">Returns the comment cell index.</td></tr>
<tr>
<td class="name">disable</td>
<td class="type"><span class="param-type">boolean</span></td>
<td class="description">Returns the disable option value.</td></tr>
<tr>
<td class="name">model</td>
<td class="type"><span class="param-type">Object</span></td>
<td class="description">Returns the Spreadsheet model.</td>
</tr>
<tr>
<td class="name">value</td>
<td class="type"><span class="param-type">string</span></td>
<td class="description">Returns the value of the comment</td>
</tr>
<tr>
<td class="name">type</td>
<td class="type"><span class="param-type">string</span></td>
<td class="description">Returns the name of the event.</td>
</tr>
<tr>
<td class="name">cancel</td>
<td class="type"><span class="param-type">boolean</span></td>
<td class="description">Returns the cancel option value.</td>
</tr>
</table>
</td></tr>
</table>

#### Example

{% highlight html %}
<div id="Spreadsheet"></div> 
<script>
// beforeEditComment event for Spreadsheet
$('#Spreadsheet').ejSpreadsheet({   
    beforeEditComment: function (args){}
});
</script>

{% endhighlight %}

### beforeOpen
{:#events:beforeopen}

Triggered before the contextmenu is open.

<table class="params">
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
<td class="description">Arguments when beforeOpen event is triggered. 
<table class="params">
<thead>
<tr>
<th>Name</th>
<th>Type</th>
<th>Description</th>
</tr>
</thead>
<tbody>
<tr>
<td class="name">target</td>
<td class="type"><span class="param-type">Element</span></td>
<td class="description">Returns the target element.</td>
</tr>
<tr>
<td class="name">type</td>
<td class="type"><span class="param-type">string</span></td>
<td class="description">Returns the name of the event.</td>
</tr>
<tr>
<td class="name">model</td>
<td class="type"><ts ref="ej.Spreadsheet.Model"/><span class="param-type">Object</span></td>
<td class="description">Returns the Spreadsheet model.</td>
</tr>
<tr>
<td class="name">cancel</td>
<td class="type"><span class="param-type">boolean</span></td>
<td class="description">Returns the cancel option value.</td>
</tr>
</tbody>
</table>
</td></tr>
</tbody>
</table>

#### Example

{% highlight html %}
<div id="Spreadsheet"></div> 
<script>
//beforeOpen event for Spreadsheet
$('#Spreadsheet').ejSpreadsheet({ 
    beforeOpen: function (args){}
});
</script>

{% endhighlight %}

### beforePanelOpen
{:#events:beforepanelopen}

Triggered before the activation panel is open.

<table class="params">
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
<td class="description">Arguments when beforePanelOpen event is triggered. 
<table class="params">
<thead>
<tr>
<th>Name</th>
<th>Type</th>
<th>Description</th>
</tr>
</thead>
<tbody>
<tr>
<td class="name">sheetIdx</td>
<td class="type"><span class="param-type">number</span></td>
<td class="description">Returns the sheet index.</td>
</tr>
<tr>
<td class="name">activationPanel</td>
<td class="type"><span class="param-type">Object</span></td>
<td class="description">Returns the activation panel element.</td>
</tr>
<tr>
<td class="name">range</td>
<td class="type"><span class="param-type">Object</span></td>
<td class="description">Returns the range option value.</td>
</tr>
<tr>
<td class="name">model</td>
<td class="type"><ts ref="ej.Spreadsheet.Model"/><span class="param-type">Object</span></td>
<td class="description">Returns the Spreadsheet model.</td>
</tr>
<tr>
<td class="name">type</td>
<td class="type"><span class="param-type">string</span></td>
<td class="description">Returns the name of the event.</td>
</tr>
<tr>
<td class="name">cancel</td>
<td class="type"><span class="param-type">boolean</span></td>
<td class="description">Returns the cancel option value.</td>
</tr>
</tbody>
</table>
</td></tr>
</tbody>
</table>

#### Example

{% highlight html %}
<div id="Spreadsheet"></div> 
<script>
// beforePanelOpen event for Spreadsheet
$('#Spreadsheet').ejSpreadsheet({ 
    beforePanelOpen: function (args){}
});
</script>

{% endhighlight %}

### cellClick
{:#events:cellclick}

Triggered when click on sheet cell.

<table class="params">
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
<td class="description">Arguments when cellClick event is triggered. 
<table class="params">
<thead>
<tr>
<th>Name</th>
<th>Type</th>
<th>Description</th>
</tr>
</thead>
<tbody>
<tr>
<td class="name">cell</td>
<td class="type"><span class="param-type">Element</span></td>
<td class="description">Returns the click cell element.</td>
</tr>
<tr>
<td class="name">columnIndex</td>
<td class="type"><span class="param-type">number</span></td>
<td class="description">Returns the column index of clicked cell.</td>
</tr>
<tr>
<td class="name">rowIndex</td>
<td class="type"><span class="param-type">number</span></td>
<td class="description">Returns the row index of clicked cell.</td>
</tr>
<tr>
<td class="name">columnName</td>
<td class="type"><span class="param-type">string</span></td>
<td class="description">Returns the column name of clicked cell.</td>
</tr>
<tr>
<td class="name">columnObject</td>
<td class="type"><span class="param-type">Object</span></td>
<td class="description">Returns the column information.</td>
</tr>
<tr>
<td class="name">model</td>
<td class="type"><ts ref="ej.Spreadsheet.Model"/><span class="param-type">Object</span></td>
<td class="description">Returns the Spreadsheet model.</td>
</tr>
<tr>
<td class="name">type</td>
<td class="type"><span class="param-type">string</span></td>
<td class="description">Returns the name of the event.</td>
</tr>
<tr>
<td class="name">target</td>
<td class="type"><span class="param-type">Element</span></td>
<td class="description">Returns the target element.</td>
</tr>
<tr>
<td class="name">value</td>
<td class="type"><span class="param-type">string</span></td>
<td class="description">Returns the value of the cell.</td>
</tr>
<tr>
<td class="name">cancel</td>
<td class="type"><span class="param-type">boolean</span></td>
<td class="description">Returns the cancel option value.</td>
</tr>
</tbody>
</table>
</td></tr>
</tbody>
</table>

#### Example

{% highlight html %}
<div id="Spreadsheet"></div> 
<script>
//cellClick event for Spreadsheet
$('#Spreadsheet').ejSpreadsheet({ 
    cellClick: function (args){}
});
</script>

{% endhighlight %}

### cellEdit
{:#events:celledit}

Triggered when the cell is edited.

<table class="params">
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
<td class="description">Arguments when cellEdit event is triggered. 
<table class="params">
<thead>
<tr>
<th>Name</th>
<th>Type</th>
<th>Description</th>
</tr>
</thead>
<tbody>
<tr>
<td class="name">cell</td>
<td class="type"><span class="param-type">Element</span></td>
<td class="description">Returns the click cell element.</td>
</tr>
<tr>
<td class="name">columnName</td>
<td class="type"><span class="param-type">string</span></td>
<td class="description">Returns the columnName of clicked cell.</td>
</tr>
<tr>
<td class="name">columnObject</td>
<td class="type"><span class="param-type">Object</span></td>
<td class="description">Returns the column field information.</td>
</tr>
<tr>
<td class="name">model</td>
<td class="type"><ts ref="ej.Spreadsheet.Model"/><span class="param-type">Object</span></td>
<td class="description">Returns the Spreadsheet model.</td>
</tr>
<tr>
<td class="name">type</td>
<td class="type"><span class="param-type">string</span></td>
<td class="description">Returns the name of the event.</td>
</tr>
<tr>
<td class="name">target</td>
<td class="type"><span class="param-type">Element</span></td>
<td class="description">Returns the target element.</td>
</tr>
<tr>
<td class="name">cancel</td>
<td class="type"><span class="param-type">boolean</span></td>
<td class="description">Returns the cancel option value.</td>
</tr>
</tbody>
</table>
</td></tr>
</tbody>
</table>

#### Example

{% highlight html %}
<div id="Spreadsheet"></div> 
<script>
//cellEdit event for Spreadsheet
$('#Spreadsheet').ejSpreadsheet({ 
    cellEdit: function (args){}
});
</script>

{% endhighlight %}

### cellFormatting
{:#events:cellformatting}

Triggered while cell is formatting.

<table class="params">
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
<td class="description">Arguments when cellFormatting event is triggered. 
<table class="params">
<thead>
<tr>
<th>Name</th>
<th>Type</th>
<th>Description</th>
</tr>
</thead>
<tbody>
<tr>
<td class="name">SheetIdx</td>
<td class="type"><span class="param-type">number</span></td>
<td class="description">Returns the sheet index</td>
</tr>
<tr>
<td class="name">Format</td>
<td class="type"><span class="param-type">Object</span></td>
<td class="description">Returns the applied style format object</td>
</tr>
<tr>
<td class="name">Cell</td>
<td class="type"><span class="param-type">number</span></td>
<td class="description">Returns the cell index.</td>
</tr>
<tr>
<td class="name">cssClass</td>
<td class="type"><span class="param-type">string</span></td>
<td class="description">Returns the name of the CSS theme.</td>
</tr>
<tr>
<td class="name">type</td>
<td class="type"><span class="param-type">string</span></td>
<td class="description">Returns the name of the event.</td>
</tr>
<tr>
<td class="name">target</td>
<td class="type"><span class="param-type">Element</span></td>
<td class="description">Returns the target element.</td>
</tr>
<tr>
<td class="name">model</td>
<td class="type"><ts ref="ej.Spreadsheet.Model"/><span class="param-type">Object</span></td>
<td class="description">Returns the Spreadsheet model.</td>
</tr>
</tbody>
</table>
</td></tr>
</tbody>
</table>

#### Example

{% highlight html %}
<div id="Spreadsheet"></div> 
<script>
//cellFormatting event for Spreadsheet
$('#Spreadsheet').ejSpreadsheet({ 
    cellFormatting: function (args){}
});
</script>

{% endhighlight %}

### cellHover
{:#events:cellhover}

Triggered when mouse hover on cell in sheets.

<table class="params">
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
<td class="description">Arguments when cellHover event is triggered. 
<table class="params">
<thead>
<tr>
<th>Name</th>
<th>Type</th>
<th>Description</th>
</tr>
</thead>
<tbody>
<tr>
<td class="name">target</td>
<td class="type"><span class="param-type">Element</span></td>
<td class="description">Returns the target element.</td>
</tr>
<tr>
<td class="name">type</td>
<td class="type"><span class="param-type">string</span></td>
<td class="description">Returns the name of the event.</td>
</tr>
<tr>
<td class="name">model</td>
<td class="type"><ts ref="ej.Spreadsheet.Model"/><span class="param-type">Object</span></td>
<td class="description">Returns the Spreadsheet model.</td>
</tr>
<tr>
<td class="name">cancel</td>
<td class="type"><span class="param-type">boolean</span></td>
<td class="description">Returns the cancel option value.</td>
</tr>
</tbody>
</table>
</td></tr>
</tbody>
</table>

#### Example

{% highlight html %}
<div id="Spreadsheet"></div> 
<script>
// cellHover event for Spreadsheet
$('#Spreadsheet').ejSpreadsheet({ 
    cellHover: function (args){}
});
</script>

{% endhighlight %}

### cellSave
{:#events:cellsave}

Triggered when save the edited cell.

<table class="params">
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
<td class="description">Arguments when cellSave event is triggered. 
<table class="params">
<thead>
<tr>
<th>Name</th>
<th>Type</th>
<th>Description</th>
</tr>
</thead>
<tbody>
<tr>
<td class="name">cell</td>
<td class="type"><span class="param-type">Element</span></td>
<td class="description">Returns the save cell element.</td>
</tr>
<tr>
<td class="name">columnName</td>
<td class="type"><span class="param-type">string</span></td>
<td class="description">Returns the columnName of clicked cell.</td>
</tr>
<tr>
<td class="name">columnObject</td>
<td class="type"><span class="param-type">Object</span></td>
<td class="description">Returns the column field information.</td>
</tr>
<tr>
<td class="name">rowIndex</td>
<td class="type"><span class="param-type">number</span></td>
<td class="description">Returns the index of the row.</td>
</tr>
<tr>
<td class="name">colIndex</td>
<td class="type"><span class="param-type">number</span></td>
<td class="description">Returns the index of the column.</td>
</tr>
<tr>
<td class="name">model</td>
<td class="type"><ts ref="ej.Spreadsheet.Model"/><span class="param-type">Object</span></td>
<td class="description">Returns the Spreadsheet model.</td>
</tr>
<tr>
<td class="name">prevValue</td>
<td class="type"><span class="param-type">string</span></td>
<td class="description">Returns the cell previous value.</td>
</tr>
<tr>
<td class="name">type</td>
<td class="type"><span class="param-type">string</span></td>
<td class="description">Returns the name of the event.</td>
</tr>
<tr>
<td class="name">cancel</td>
<td class="type"><span class="param-type">boolean</span></td>
<td class="description">Returns the cancel option value.</td>
</tr>
<tr>
<td class="name">target</td>
<td class="type"><span class="param-type">Element</span></td>
<td class="description">Returns the target element.</td>
</tr>
<tr>
<td class="name">value</td>
<td class="type"><span class="param-type">string</span></td>
<td class="description">Returns the cell value.</td>
</tr>
</tbody>
</table>
</td></tr>
</tbody>
</table>

#### Example

{% highlight html %}
<div id="Spreadsheet"></div> 
<script>
//cellSave event for Spreadsheet
$('#Spreadsheet').ejSpreadsheet({ 
    cellSave: function (args){}
});
</script>

{% endhighlight %}

### cellSelected
{:#events:cellselected}

Triggered when the cell is selected.

<table class="params">
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
<td class="name">sheetIdx</td>
<td class="type"><span class="param-type">number</span></td>
<td class="description">Returns the active sheet index.</td>
</tr>
<tr>
<td class="name">selectedRange</td>
<td class="type"><span class="param-type">Array</span></td>
<td class="description">Returns the selected range.</td>
</tr>
<tr>
<td class="name">target</td>
<td class="type"><span class="param-type">Element</span></td>
<td class="description">Returns the target element.</td>
</tr>
<tr>
<td class="name">model</td>
<td class="type"><ts ref="ej.Spreadsheet.Model"/><span class="param-type">Object</span></td>
<td class="description">Returns Spreadsheet model.</td>
</tr>
<tr>
<td class="name">type</td>
<td class="type"><span class="param-type">string</span></td>
<td class="description">Returns the name of the event.</td>
</tr>
<tr>
<td class="name">target</td>
<td class="type"><span class="param-type">Element</span></td>
<td class="description">Returns the target element.</td>
</tr>
<tr>
<td class="name">cancel</td>
<td class="type"><span class="param-type">boolean</span></td>
<td class="description">Returns the cancel option value.</td>
</tr>
</tbody>
</table>
</td></tr>
</tbody>
</table>

#### Example

{% highlight html %}

<div id="Spreadsheet"></div> 
<script>
//cellSelected event for Spreadsheet
$('#Spreadsheet').ejSpreadsheet({ 
    cellSelected: function (args){}
 });
 </script>
 
{% endhighlight %}

### contextMenuClick
{:#events:contextmenuclick}

Triggered when click the contextmenu items.
<table class="params">
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
<td class="description">Arguments when contextMenuClick event is triggered. 
<table class="params">
<thead>
<tr>
<th>Name</th>
<th>Type</th>
<th>Description</th>
</tr>
</thead>
<tbody>
<tr>
<td class="name">Id</td>
<td class="type"><span class="param-type">string</span></td>
<td class="description">Returns target element Id.</td>
</tr>
<tr>
<td class="name">element</td>
<td class="type"><span class="param-type">Element</span></td>
<td class="description">Returns the target element.</td>
</tr>
<tr>
<td class="name">event</td>
<td class="type"><span class="param-type">Object</span></td>
<td class="description">Returns event information.</td>
</tr>
<tr>
<td class="name">events</td>
<td class="type"><span class="param-type">Object</span></td>
<td class="description">Returns target element and event information.</td>
</tr>
<tr>
<td class="name">model</td>
<td class="type"><ts ref="ej.Spreadsheet.Model"/><span class="param-type">Object</span></td>
<td class="description">Returns the Spreadsheet model.</td>
</tr>
<tr>
<td class="name">parentId</td>
<td class="type"><span class="param-type">string</span></td>
<td class="description">Returns target element parent Id.</td>
</tr>
<tr>
<td class="name">parentText</td>
<td class="type"><span class="param-type">string</span></td>
<td class="description">Returns target element parent text.</td>
</tr>
<tr>
<td class="name">text</td>
<td class="type"><span class="param-type">string</span></td>
<td class="description">Returns target element text.</td>
</tr>
<tr>
<td class="name">type</td>
<td class="type"><span class="param-type">string</span></td>
<td class="description">Returns the name of the event.</td>
</tr>
<tr>
<td class="name">cancel</td>
<td class="type"><span class="param-type">boolean</span></td>
<td class="description">Returns the cancel option value.</td>
</tr>
</tbody>
</table>
</td></tr>
</tbody>
</table>

#### Example

{% highlight html %}
<div id="Spreadsheet"></div> 
<script>
// contextMenuClick event for Spreadsheet.
$('#Spreadsheet').ejSpreadsheet({ 
    contextMenuClick: function (args){}
});
</script>

{% endhighlight %}

### drag
{:#events:drag}

Triggered when the selected cells are being dragged.

<table class="params">
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
<td class="description">Arguments when drag event is triggered. 
<table class="params">
<thead>
<tr>
<th>Name</th>
<th>Type</th>
<th>Description</th>
</tr>
</thead>
<tbody>
<tr>
<td class="name">sheetIdx</td>
<td class="type"><span class="param-type">number</span></td>
<td class="description">Returns the sheet index.</td>
</tr>
<tr>
<td class="name">currentCell</td>
<td class="type"><span class="param-type">Object</span></td>
<td class="description">Returns the current cell row and column index.</td>
</tr>
<tr>
<td class="name">dragAndDropRange</td>
<td class="type"><span class="param-type">Object</span></td>
<td class="description">Returns the drag cells range object.</td>
</tr>
<tr>
<td class="name">model</td>
<td class="type"><ts ref="ej.Spreadsheet.Model"/><span class="param-type">Object</span></td>
<td class="description">Returns the Spreadsheet model.</td>
</tr>
<tr>
<td class="name">target</td>
<td class="type"><span class="param-type">Element</span></td>
<td class="description">Returns the target item.</td>
</tr>
<tr>
<td class="name">type</td>
<td class="type"><span class="param-type">string</span></td>
<td class="description">Returns the name of the event.</td>
</tr>
<tr>
<td class="name">cancel</td>
<td class="type"><span class="param-type">boolean</span></td>
<td class="description">Returns the cancel option value.</td>
</tr>
</tbody>
</table>
</td></tr>
</tbody>
</table>

#### Example

{% highlight html %}
<div id="Spreadsheet"></div>
<script>
//drag event for Spreadsheet
$("#Spreadsheet").ejSpreadsheet({
    drag: function (args){}
});
</script>

{% endhighlight %}

### dragShape
{:#events:dragshape}

Triggered when you start to drag the picture or chart.

<table class="params">
<tr>
<th>Name</th>
<th>Type</th>
<th>Description</th>
</tr>
<tr>
<td class="name">argument</td>
<td class="type"><span class="param-type">Object</span></td>
<td class="description">Arguments when dragShape event is triggered.
<table>
<tr>
<th>Name</th>
<th>Type</th>
<th>Description</th>
</tr>
<tr>
<td class="name">model</td>
<td class="type"><span class="param-type">Object</span></td>
<td class="description">Returns the Spreadsheet model.</td>
</tr>
<tr>
<td class="name">type</td>
<td class="type"><span class="param-type">string</span></td>
<td class="description">Returns the name of the event.</td>
</tr>
<tr>
<td class="name">target</td>
<td class="type"><span class="param-type">element</span></td>
<td class="description">Returns the target element.</td>
</tr>
<tr>
<td class="name">cancel</td>
<td class="type"><span class="param-type">boolean</span></td>
<td class="description">Returns the cancel option value.</td>
</tr>
</table>
</td></tr>
</table>

#### Example

{% highlight html %}
<div id="Spreadsheet"></div> 
<script>
// dragShape event for Spreadsheet
$('#Spreadsheet').ejSpreadsheet({   
    dragShape: function (args){}
});
</script>

{% endhighlight %}

### dragStart
{:#events:dragstart}

Triggered when the selected cells are initiated to drag.
<table class="params">
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
<td class="description">Arguments when dragStart event is triggered. 
<table class="params">
<thead>
<tr>
<th>Name</th>
<th>Type</th>
<th>Description</th>
</tr>
</thead>
<tbody>
<tr>
<td class="name">sheetIdx</td>
<td class="type"><span class="param-type">number</span></td>
<td class="description">Returns the sheet index.</td>
</tr>
<tr>
<td class="name">currentCell</td>
<td class="type"><span class="param-type">Object</span></td>
<td class="description">Returns the current cell row and column index.</td>
</tr>
<tr>
<td class="name">dragAndDropRange</td>
<td class="type"><span class="param-type">Object</span></td>
<td class="description">Returns the drag cells range object.</td>
</tr>
<tr>
<td class="name">model</td>
<td class="type"><ts ref="ej.Spreadsheet.Model"/><span class="param-type">Object</span></td>
<td class="description">Returns the Spreadsheet model.</td>
</tr>
<tr>
<td class="name">target</td>
<td class="type"><span class="param-type">Element</span></td>
<td class="description">Returns the target item.</td>
</tr>
<tr>
<td class="name">type</td>
<td class="type"><span class="param-type">string</span></td>
<td class="description">Returns the name of the event.</td>
</tr>
<tr>
<td class="name">cancel</td>
<td class="type"><span class="param-type">boolean</span></td>
<td class="description">Returns the cancel option value.</td>
</tr>
</tbody>
</table>
</td></tr>
</tbody>
</table>

#### Example

{% highlight html %}
<div id="Spreadsheet"></div>
<script>
//dragStart event for Spreadsheet
$("#Spreadsheet").ejSpreadsheet({
    dragStart: function (args){}
});
</script>

{% endhighlight %}

### drop
{:#events:drop}

Triggered when the selected cells are dropped.

<table class="params">
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
<td class="description">Arguments when drop event is triggered. 
<table class="params">
<thead>
<tr>
<th>Name</th>
<th>Type</th>
<th>Description</th>
</tr>
</thead>
<tbody>
<tr>
<td class="name">sheetIdx</td>
<td class="type"><span class="param-type">number</span></td>
<td class="description">Returns the sheet index.</td>
</tr>
<tr>
<td class="name">currentCell</td>
<td class="type"><span class="param-type">Object</span></td>
<td class="description">Returns the current cell row and column index.</td>
</tr>
<tr>
<td class="name">dragAndDropRange</td>
<td class="type"><span class="param-type">Object</span></td>
<td class="description">Returns the drag cells range object.</td>
</tr>
<tr>
<td class="name">model</td>
<td class="type"><ts ref="ej.Spreadsheet.Model"/><span class="param-type">Object</span></td>
<td class="description">Returns the Spreadsheet model.</td>
</tr>
<tr>
<td class="name">target</td>
<td class="type"><span class="param-type">Element</span></td>
<td class="description">Returns the target item.</td>
</tr>
<tr>
<td class="name">type</td>
<td class="type"><span class="param-type">string</span></td>
<td class="description">Returns the name of the event.</td>
</tr>
<tr>
<td class="name">cancel</td>
<td class="type"><span class="param-type">boolean</span></td>
<td class="description">Returns the cancel option value.</td>
</tr>
</tbody>
</table>
</td></tr>
</tbody>
</table>

#### Example

{% highlight html %}
<div id="Spreadsheet"></div>
<script>
//drop event for Spreadsheet
$("#Spreadsheet").ejSpreadsheet({
    drop: function (args){}
});
</script>

{% endhighlight %}

### editRangeBegin
{:#events:editrangebegin}

Triggered before the range editing starts.

<table class="params">
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
<td class="description">Arguments when editRangeBegin event is triggered. 
<table class="params">
<thead>
<tr>
<th>Name</th>
<th>Type</th>
<th>Description</th>
</tr>
</thead>
<tbody>
<tr>
<td class="name">sheetIdx</td>
<td class="type"><span class="param-type">number</span></td>
<td class="description">Returns the sheet index.</td>
</tr>
<tr>
<td class="name">model</td>
<td class="type"><ts ref="ej.Spreadsheet.Model"/><span class="param-type">Object</span></td>
<td class="description">Returns the Spreadsheet model.</td>
</tr>
<tr>
<td class="name">range</td>
<td class="type"><span class="param-type">Object</span></td>
<td class="description">Returns the range option value.</td>
</tr>
<tr>
<td class="name">type</td>
<td class="type"><span class="param-type">string</span></td>
<td class="description">Returns the name of the event.</td>
</tr>
<tr>
<td class="name">cancel</td>
<td class="type"><span class="param-type">boolean</span></td>
<td class="description">Returns the cancel option value.</td>
</tr>
</tbody>
</table>
</td></tr>
</tbody>
</table>

#### Example

{% highlight html %}
<div id="Spreadsheet"></div> 
<script>
// editRangeBegin event for Spreadsheet.
$('#Spreadsheet').ejSpreadsheet({ 
    editRangeBegin: function (args){}
});
</script>

{% endhighlight %}

### editRangeComplete
{:#events:editrangecomplete}

Triggered after range editing completes.

<table class="params">
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
<td class="description">Arguments when editRangeComplete event is triggered. 
<table class="params">
<thead>
<tr>
<th>Name</th>
<th>Type</th>
<th>Description</th>
</tr>
</thead>
<tbody>
<tr>
<td class="name">sheetIdx</td>
<td class="type"><span class="param-type">number</span></td>
<td class="description">Returns the sheet index.</td>
</tr>
<tr>
<td class="name">model</td>
<td class="type"><ts ref="ej.Spreadsheet.Model"/><span class="param-type">Object</span></td>
<td class="description">Returns the Spreadsheet model.</td>
</tr>
<tr>
<td class="name">range</td>
<td class="type"><span class="param-type">Object</span></td>
<td class="description">Returns the range option value.</td>
</tr>
<tr>
<td class="name">type</td>
<td class="type"><span class="param-type">string</span></td>
<td class="description">Returns the name of the event.</td>
</tr>
<tr>
<td class="name">cancel</td>
<td class="type"><span class="param-type">boolean</span></td>
<td class="description">Returns the cancel option value.</td>
</tr>
</tbody>
</table>
</td></tr>
</tbody>
</table>

#### Example

{% highlight html %}
<div id="Spreadsheet"></div> 
<script>
// editRangeComplete event for Spreadsheet
$('#Spreadsheet').ejSpreadsheet({ 
    editRangeComplete: function (args){}
});
</script>

{% endhighlight %}

### keyDown
{:#events:keydown}

Triggered when the key is pressed down.

<table class="params">
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
<td class="description">Arguments when keyDown event is triggered. 
<table class="params">
<thead>
<tr>
<th>Name</th>
<th>Type</th>
<th>Description</th>
</tr>
</thead>
<tbody>
<tr>
<td class="name">sheetIndex</td>
<td class="type"><span class="param-type">number</span></td>
<td class="description">Returns the sheet index.</td>
</tr>
<tr>
<td class="name">model</td>
<td class="type"><ts ref="ej.Spreadsheet.Model"/><span class="param-type">Object</span></td>
<td class="description">Returns the Spreadsheet model.</td>
</tr>
<tr>
<td class="name">isCommentEdit</td>
<td class="type"><span class="param-type">boolean</span></td>
<td class="description">Returns the boolean value.</td>
</tr>
<tr>
<td class="name">isEdit</td>
<td class="type"><span class="param-type">boolean</span></td>
<td class="description">Returns the boolean value.</td>
</tr>
<tr>
<td class="name">isSheetRename</td>
<td class="type"><span class="param-type">boolean</span></td>
<td class="description">Returns the boolean value.</td>
</tr>
<tr>
<td class="name">target</td>
<td class="type"><span class="param-type">Element</span></td>
<td class="description">Returns the target element.</td>
</tr>
<tr>
<td class="name">type</td>
<td class="type"><span class="param-type">string</span></td>
<td class="description">Returns the name of the event.</td>
</tr>
<tr>
<td class="name">cancel</td>
<td class="type"><span class="param-type">boolean</span></td>
<td class="description">Returns the cancel option value.</td>
</tr>
</tbody>
</table>
</td></tr>
</tbody>
</table>

#### Example

{% highlight html %}
<div id="Spreadsheet"></div> 
<script>
// keyDown event for Spreadsheet
$('#Spreadsheet').ejSpreadsheet({ 
    keyDown: function (args){}
});
</script>

{% endhighlight %}

### keyUp
{:#events:keyup}

Triggered when the key is released.

<table class="params">
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
<td class="description">Arguments when keyUp event is triggered. 
<table class="params">
<thead>
<tr>
<th>Name</th>
<th>Type</th>
<th>Description</th>
</tr>
</thead>
<tbody>
<tr>
<td class="name">sheetIndex</td>
<td class="type"><span class="param-type">number</span></td>
<td class="description">Returns the sheet index.</td>
</tr>
<tr>
<td class="name">model</td>
<td class="type"><ts ref="ej.Spreadsheet.Model"/><span class="param-type">Object</span></td>
<td class="description">Returns the Spreadsheet model.</td>
</tr>
<tr>
<td class="name">isCommentEdit</td>
<td class="type"><span class="param-type">boolean</span></td>
<td class="description">Returns the boolean value.</td>
</tr>
<tr>
<td class="name">isEdit</td>
<td class="type"><span class="param-type">boolean</span></td>
<td class="description">Returns the boolean value.</td>
</tr>
<tr>
<td class="name">isSheetRename</td>
<td class="type"><span class="param-type">boolean</span></td>
<td class="description">Returns the boolean value.</td>
</tr>
<tr>
<td class="name">target</td>
<td class="type"><span class="param-type">Element</span></td>
<td class="description">Returns the target element.</td>
</tr>
<tr>
<td class="name">type</td>
<td class="type"><span class="param-type">string</span></td>
<td class="description">Returns the name of the event.</td>
</tr>
<tr>
<td class="name">cancel</td>
<td class="type"><span class="param-type">boolean</span></td>
<td class="description">Returns the cancel option value.</td>
</tr>
</tbody>
</table>
</td></tr>
</tbody>
</table>

#### Example

{% highlight html %}
<div id="Spreadsheet"></div> 
<script>
// keyUp event for Spreadsheet
$('#Spreadsheet').ejSpreadsheet({ 
    keyUp: function (args){}
});
</script>

{% endhighlight %}

### load
{:#events:load}

Triggered before the sheet is loaded.

<table class="params">
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
<td class="name">type</td>
<td class="type"><span class="param-type">string</span></td>
<td class="description">Returns the name of the event.</td>
</tr>
<tr>
<td class="name">model</td>
<td class="type"><ts ref="ej.Spreadsheet.Model"/><span class="param-type">Object</span></td>
<td class="description">Returns the Spreadsheet model.</td>
</tr>
<tr>
<td class="name">cancel</td>
<td class="type"><span class="param-type">boolean</span></td>
<td class="description">Returns the cancel option value.</td>
</tr>
<tr>
<td class="name">sheetIndex</td>
<td class="type"><span class="param-type">number</span></td>
<td class="description">Returns the active sheet index.</td>
</tr>
</tbody>
</table>
</td></tr>
</tbody>
</table>

#### Example

{% highlight html %}
<div id="Spreadsheet"></div> 
<script>
//load event for Spreadsheet
$('#Spreadsheet').ejSpreadsheet({ 
    load: function (args){}
});
</script>

{% endhighlight %}

### loadComplete
{:#events:loadcomplete}

Triggered after the sheet is loaded.

<table class="params">
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
<td class="description">Arguments when loadComplete event is triggered. 
<table class="params">
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
<td class="type"><ts ref="ej.Spreadsheet.Model"/><span class="param-type">Object</span></td>
<td class="description">Returns the Spreadsheet model.</td>
</tr>
<tr>
<td class="name">type</td>
<td class="type"><span class="param-type">string</span></td>
<td class="description">Returns the name of the event.</td>
</tr>
<tr>
<td class="name">cancel</td>
<td class="type"><span class="param-type">boolean</span></td>
<td class="description">Returns the cancel option value.</td>
</tr>
</tbody>
</table>
</td></tr>
</tbody>
</table>

#### Example

{% highlight html %}
<div id="Spreadsheet"></div> 
<script>
// loadComplete event for Spreadsheet
$('#Spreadsheet').ejSpreadsheet({ 
    loadComplete: function (args){}
});
</script>

{% endhighlight %}

### menuClick
{:#events:menuclick}

Triggered every click of the menu item.

<table class="params">
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
<td class="description">Arguments when menuClick event is triggered. 
<table class="params">
<thead>
<tr>
<th>Name</th>
<th>Type</th>
<th>Description</th>
</tr>
</thead>
<tbody>
<tr>
<td class="name">element</td>
<td class="type"><span class="param-type">Element</span></td>
<td class="description">Returns menu click element.</td>
</tr>
<tr>
<td class="name">event</td>
<td class="type"><span class="param-type">Object</span></td>
<td class="description">Returns the event information.</td>
</tr>
<tr>
<td class="name">model</td>
<td class="type"><ts ref="ej.Spreadsheet.Model"/><span class="param-type">Object</span></td>
<td class="description">Returns the Spreadsheet model.</td>
</tr>
<tr>
<td class="name">parentId</td>
<td class="type"><span class="param-type">string</span></td>
<td class="description">Returns target element parent Id.</td>
</tr>
<tr>
<td class="name">parentText</td>
<td class="type"><span class="param-type">string</span></td>
<td class="description">Returns target element parent text.</td>
</tr>
<tr>
<td class="name">text</td>
<td class="type"><span class="param-type">string</span></td>
<td class="description">Returns target element text.</td>
</tr>
<tr>
<td class="name">type</td>
<td class="type"><span class="param-type">string</span></td>
<td class="description">Returns the name of the event.</td>
</tr>
<tr>
<td class="name">cancel</td>
<td class="type"><span class="param-type">boolean</span></td>
<td class="description">Returns the cancel option value.</td>
</tr>
</tbody>
</table>
</td>
</tr>
</tbody>
</table>

#### Example

{% highlight html %}
<div id="Spreadsheet"></div> 
<script>
// menuClick event for Spreadsheet.
$('#Spreadsheet').ejSpreadsheet({ 
    menuClick: function (args){}
});
</script>

{% endhighlight %}

### onImport
{:#events:onimport}

Triggered when a file is imported.

<table class="params">
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
<td class="description">Arguments when onImport event is triggered. 
<table class="params">
<thead>
<tr>
<th>Name</th>
<th>Type</th>
<th>Description</th>
</tr>
</thead>
<tbody>
<tr>
<td class="name">type</td>
<td class="type"><span class="param-type">string</span></td>
<td class="description">Returns the name of the event.</td>
</tr>
<tr>
<td class="name">model</td>
<td class="type"><ts ref="ej.Spreadsheet.Model"/><span class="param-type">Object</span></td>
<td class="description">Returns the Spreadsheet model.</td>
</tr>
<tr>
<td class="name">cancel</td>
<td class="type"><span class="param-type">boolean</span></td>
<td class="description">Returns the cancel option value.</td>
</tr>
<tr>
<td class="name">importData</td>
<td class="type"><span class="param-type">Object</span></td>
<td class="description">Returns the imported data.</td>
</tr>
</tbody>
</table>
</td></tr>
</tbody>
</table>

#### Example

{% highlight html %}

<div id="Spreadsheet"></div> 
<script>
//onImport event for Spreadsheet
$('#Spreadsheet').ejSpreadsheet({ 
    onImport: function (args){}
 });
 </script>

{% endhighlight %}

### openFailure
{:#events:openfailure}

Triggered when import sheet is failed to open.

<table class="params">
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
<td class="description">Arguments when openFailure event is triggered. 
<table class="params">
<thead>
<tr>
<th>Name</th>
<th>Type</th>
<th>Description</th>
</tr>
</thead>
<tbody>
<tr>
<td class="name">failureType</td>
<td class="type"><span class="param-type">string</span></td>
<td class="description">Returns the failure type.</td>
</tr>
<tr>
<td class="name">status</td>
<td class="type"><span class="param-type">number</span></td>
<td class="description">Returns the status index.</td>
</tr>
<tr>
<td class="name">statusText</td>
<td class="type"><span class="param-type">string</span></td>
<td class="description">Returns the status in text.</td>
</tr>
<tr>
<td class="name">model</td>
<td class="type"><ts ref="ej.Spreadsheet.Model"/><span class="param-type">Object</span></td>
<td class="description">Returns the Spreadsheet model.</td>
</tr>
<tr>
<td class="name">type</td>
<td class="type"><span class="param-type">string</span></td>
<td class="description">Returns the name of the event.</td>
</tr>
<tr>
<td class="name">cancel</td>
<td class="type"><span class="param-type">boolean</span></td>
<td class="description">Returns the cancel option value.</td>
</tr>
</tbody>
</table>
</td></tr>
</tbody>
</table>

#### Example

{% highlight html %}
<div id="Spreadsheet"></div>
<script>
//openFailure event for Spreadsheet
$("#Spreadsheet").ejSpreadsheet({
openFailure: function (args){}
});
</script>

{% endhighlight %}

### pagerClick
{:#events:pagerclick}

Triggered when pager item is clicked in the Spreadsheet.

<table class="params">
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
<td class="description">Arguments when pagerClick event is triggered. 
<table class="params">
<thead>
<tr>
<th>Name</th>
<th>Type</th>
<th>Description</th>
</tr>
</thead>
<tbody>
<tr>
<td class="name">activeSheet</td>
<td class="type"><span class="param-type">number</span></td>
<td class="description">Returns the active sheet index.</td>
</tr>
<tr>
<td class="name">gotoSheet</td>
<td class="type"><span class="param-type">number</span></td>
<td class="description">Returns the new sheet index.</td>
</tr>
<tr>
<td class="name">newSheet</td>
<td class="type"><span class="param-type">boolean</span></td>
<td class="description">Returns whether new sheet icon is clicked.</td>
</tr>
<tr>
<td class="name">model</td>
<td class="type"><ts ref="ej.Spreadsheet.Model"/><span class="param-type">Object</span></td>
<td class="description">Returns the Spreadsheet model.</td>
</tr>
<tr>
<td class="name">type</td>
<td class="type"><span class="param-type">string</span></td>
<td class="description">Returns the name of the event.</td>
</tr>
<tr>
<td class="name">target</td>
<td class="type"><span class="param-type">Element</span></td>
<td class="description">Returns the target element.</td>
</tr>
<tr>
<td class="name">cancel</td>
<td class="type"><span class="param-type">boolean</span></td>
<td class="description">Returns the cancel option value.</td>
</tr>
</tbody>
</table>
</td></tr>
</tbody>
</table>

#### Example

{% highlight html %}
<div id="Spreadsheet"></div> 
<script>
// pagerClick event for Spreadsheet
$('#Spreadsheet').ejSpreadsheet({ 
    pagerClick: function (args){}
});
</script>

{% endhighlight %}

### resizeStart
{:#events:resizestart}

Triggered when you start resizing the chart, picture, row and column.

<table class="params">
<tr>
<th>
Name</th><th>
Type</th><th>
Description</th></tr>
<tr>
<td class="name">argument</td>
<td class="type"><span class="param-type">Object</span></td>
<td class="description">Arguments when resizeStart event is triggered.
<table><tr>
<th>Name</th>
<th>Type</th>
<th>Description</th>
</tr>
<tr>
<td class="name">colIndex</td>
<td class="type"><span class="param-type">number</span></td>
<td class="description">Returns the column index which column you start to resize.</td>
</tr>
<tr>
<td class="name">rowIndex</td>
<td class="type"><span class="param-type">number</span></td>
<td class="description">Returns the row index which row you start to resize.</td>
</tr>
<tr>
<td class="name">model</td>
<td class="type"><span class="param-type">Object</span></td>
<td class="description">Returns the Spreadsheet model.</td>
</tr>
<tr>
<td class="name">reqType</td>
<td class="type"><span class="param-type">string</span></td>
<td class="description">Returns type of the request.</td>
</tr>
<tr>
<td class="name">type</td>
<td class="type"><span class="param-type">string</span></td>
<td class="description">Returns the name of the event.</td>
</tr>
<tr>
<td class="name">cancel</td>
<td class="type"><span class="param-type">boolean</span></td>
<td class="description">Returns the cancel option value.</td>
</tr>
</table>
</td></tr>
</table>

#### Example

{% highlight html %}
<div id="Spreadsheet"></div> 
<script>
// resizeStart event for Spreadsheet
$('#Spreadsheet').ejSpreadsheet({   
    resizeStart: function (args){}
});
</script>

{% endhighlight %}

### resizeEnd
{:#events:resizeend}

Triggered after end of resizing the chart, picture, row and column.

<table class="params">
<tr>
<th>
Name</th><th>
Type</th><th>
Description</th></tr>
<tr>
<td class="name">argument</td>
<td class="type"><span class="param-type"> Object</span></td>
<td class="description">Arguments when resizeEnd event is triggered.<table>
<tr>
<th>Name</th>
<th>Type</th>
<th>Description</th></tr>
<tr>
<td class="name">colIndex</td>
<td class="type"><span class="param-type">number</span></td>
<td class="description">Returns the column index which you resized.</td></tr>
<tr>
<td class="name">oldWidth</td>
<td class="type"><span class="param-type">number</span></td>
<td class="description">Returns old width of the column or shape.</td></tr>
<tr>
<td class="name">newWidth</td>
<td class="type"><span class="param-type">number</span></td>
<td class="description">Returns new width of the column or shape.</td></tr>
<tr>
<td class="name">rowIndex</td>
<td class="type"><span class="param-type">number</span></td>
<td class="description">Returns the row index which you resized.</td></tr>
<tr>
<td class="name">oldHeight</td>
<td class="type"><span class="param-type">number</span></td>
<td class="description">Returns old height of the row or shape.</td></tr>
<tr>
<td class="name">newHeight</td>
<td class="type"><span class="param-type">number</span></td>
<td class="description">Returns new height of the row or shape.</td></tr>
<tr>
<td class="name">model</td>
<td class="type"><span class="param-type">Object</span></td>
<td class="description">Returns the Spreadsheet model.</td></tr>
<tr>
<td class="name">reqType</td>
<td class="type"><span class="param-type">string</span></td>
<td class="description">Returns type of the request.</td></tr>
<tr>
<td class="name">type</td>
<td class="type"><span class="param-type">string</span></td>
<td class="description">Returns the name of the event.</td></tr>
<tr>
<td class="name">cancel</td>
<td class="type"><span class="param-type">boolean</span></td>
<td class="description">Returns the cancel option value.</td></tr>
</table>
</td>
</tr>
</table>

#### Example

{% highlight html %}
<div id="Spreadsheet"></div> 
<script>
// resizeEnd event for Spreadsheet
$('#Spreadsheet').ejSpreadsheet({   
    resizeEnd: function (args){}
});
</script>

{% endhighlight %}

### ribbonClick
{:#events:ribbonclick}

Triggered when click on the ribbon.

<table class="params">
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
<td class="description">Arguments when ribbonClick event is triggered. 
<table class="params">
<thead>
<tr>
<th>Name</th>
<th>Type</th>
<th>Description</th>
</tr>
</thead>
<tbody>
<tr>
<td class="name">Id</td>
<td class="type"><span class="param-type">string</span></td>
<td class="description">Returns element Id.</td>
</tr>
<tr>
<td class="name">prop</td>
<td class="type"><span class="param-type">Object</span></td>
<td class="description">Returns target information.</td>
</tr>
<tr>
<td class="name">model</td>
<td class="type"><ts ref="ej.Spreadsheet.Model"/><span class="param-type">Object</span></td>
<td class="description">Returns the Spreadsheet model.</td>
</tr>
<tr>
<td class="name">status</td>
<td class="type"><span class="param-type">boolean</span></td>
<td class="description">Returns status.</td>
</tr>
<tr>
<td class="name">isChecked</td>
<td class="type"><span class="param-type">boolean</span></td>
<td class="description">Returns isChecked in boolean.</td>
</tr>
<tr>
<td class="name">type</td>
<td class="type"><span class="param-type">string</span></td>
<td class="description">Returns the name of the event.</td>
</tr>
<tr>
<td class="name">target</td>
<td class="type"><span class="param-type">Element</span></td>
<td class="description">Returns the target element.</td>
</tr>
<tr>
<td class="name">cancel</td>
<td class="type"><span class="param-type">boolean</span></td>
<td class="description">Returns the cancel option value.</td>
</tr>
</tbody>
</table>
</td></tr>
</tbody>
</table>

#### Example

{% highlight html %}
<div id="Spreadsheet"></div> 
<script>
// ribbonClick event for Spreadsheet
$('#Spreadsheet').ejSpreadsheet({ 
    ribbonClick: function (args){}
});
</script>

{% endhighlight %}

### scrollStop
{:#events:scrollstop}

Triggered after end of vertical and horizontal scrolling.

<table class="params">
<tr>
<th>Name</th>
<th>Type</th>
<th>Description</th></tr>
<tr>
<td class="name">argument</td>
<td class="type"><span class="param-type">Object</span></td>
<td class="description">Arguments when scrollStop event is triggered. 
<table>
<tr>
<th>Name</th>
<th>Type</th>
<th>Description</th></tr>
<tr>
<td class="name">reqType</td>
<td class="type"><span class="param-type">string</span></td>
<td class="description">Returns the request type.</td></tr>
<tr>
<td class="name">position</td>
<td class="type"><span class="param-type">number</span></td>
<td class="description">Returns the scrolled position.</td></tr>
<tr>
<td class="name">type</td>
<td class="type"><span class="param-type">string</span></td>
<td class="description">Returns the name of the event.</td></tr>
<tr>
<td class="name">model</td>
<td class="type"><ts ref="ej.Spreadsheet.Model"/><span class="param-type">Object</span></td>
<td class="description">Returns the Spreadsheet model.</td></tr>
<tr>
<td class="name">scrollData</td>
<td class="type"><span class="param-type">Object</span></td>
<td class="description">Returns the scrolling data</td></tr>
<tr>
<td class="name">cancel</td>
<td class="type"><span class="param-type">boolean</span></td>
<td class="description">Returns the cancel option value.</td></tr>
</table>
</td></tr>
</table>

#### Example

{% highlight html %}
<div id="Spreadsheet"></div> 
<script>
// scrollStop event for Spreadsheet
$('#Spreadsheet').ejSpreadsheet({ 
    scrollStop: function (args){}
});
</script>

{% endhighlight %}

### tabClick
{:#events:tabclick}

Triggered when click the ribbon tab.

<table class="params">
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
<td class="description">Arguments when tabClick event is triggered. 
<table class="params">
<thead>
<tr>
<th>Name</th>
<th>Type</th>
<th>Description</th>
</tr>
</thead>
<tbody>
<tr>
<td class="name">activeIndex</td>
<td class="type"><span class="param-type">number</span></td>
<td class="description">Returns the active tab index.</td>
</tr>
<tr>
<td class="name">activeHeader</td>
<td class="type"><span class="param-type">Object</span></td>
<td class="description">Returns active tab header element.</td>
</tr>
<tr>
<td class="name">prevActiveHeader</td>
<td class="type"><span class="param-type">Object</span></td>
<td class="description">Returns previous active tab header element.</td>
</tr>
<tr>
<td class="name">prevActiveIndex</td>
<td class="type"><span class="param-type">number</span></td>
<td class="description">Returns previous active tab index.</td>
</tr>
<tr>
<td class="name">model</td>
<td class="type"><ts ref="ej.Spreadsheet.Model"/><span class="param-type">Object</span></td>
<td class="description">Returns the Spreadsheet model.</td>
</tr>
<tr>
<td class="name">type</td>
<td class="type"><span class="param-type">string</span></td>
<td class="description">Returns the name of the event.</td>
</tr>
<tr>
<td class="name">target</td>
<td class="type"><span class="param-type">Element</span></td>
<td class="description">Returns the target element.</td>
</tr>
<tr>
<td class="name">cancel</td>
<td class="type"><span class="param-type">boolean</span></td>
<td class="description">Returns the cancel option value.</td>
</tr>
</tbody>
</table>
</td></tr>
</tbody>
</table>

#### Example

{% highlight html %}
<div id="Spreadsheet"></div> 
<script>
// tabClick event for Spreadsheet.
$('#Spreadsheet').ejSpreadsheet({ 
    tabClick: function (args){}
});
</script>

{% endhighlight %}

### tabSelect
{:#events:tabselect}

Triggered when select the ribbon tab.

<table class="params">
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
<td class="description">Arguments when tabSelect event is triggered. 
<table class="params">
<thead>
<tr>
<th>Name</th>
<th>Type</th>
<th>Description</th>
</tr>
</thead>
<tbody>
<tr>
<td class="name">activeIndex</td>
<td class="type"><span class="param-type">number</span></td>
<td class="description">Returns the active tab index.</td>
</tr>
<tr>
<td class="name">activeHeader</td>
<td class="type"><span class="param-type">Object</span></td>
<td class="description">Returns active tab header element.</td>
</tr>
<tr>
<td class="name">prevActiveHeader</td>
<td class="type"><span class="param-type">Object</span></td>
<td class="description">Returns previous active tab header element.</td>
</tr>
<tr>
<td class="name">prevActiveIndex</td>
<td class="type"><span class="param-type">number</span></td>
<td class="description">Returns previous active tab index.</td>
</tr>
<tr>
<td class="name">model</td>
<td class="type"><ts ref="ej.Spreadsheet.Model"/><span class="param-type">Object</span></td>
<td class="description">Returns the Spreadsheet model.</td>
</tr>
<tr>
<td class="name">type</td>
<td class="type"><span class="param-type">string</span></td>
<td class="description">Returns the name of the event.</td>
</tr>
<tr>
<td class="name">target</td>
<td class="type"><span class="param-type">Element</span></td>
<td class="description">Returns the target element.</td>
</tr>
<tr>
<td class="name">cancel</td>
<td class="type"><span class="param-type">boolean</span></td>
<td class="description">Returns the cancel option value.</td>
</tr>
</tbody>
</table>
</td></tr>
</tbody>
</table>

#### Example

{% highlight html %}
<div id="Spreadsheet"></div> 
<script>
// tabSelect event for Spreadsheet.
$('#Spreadsheet').ejSpreadsheet({ 
    tabSelect: function (args){}
});
</script>

{% endhighlight %}