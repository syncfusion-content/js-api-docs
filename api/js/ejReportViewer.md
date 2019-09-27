---
layout: post
title: Properties, Methods and Events of ejReportViewer Widget | Syncfusion
documentation: UG
platform: js-api
metaname: 
metacontent: 
---


# ejReportViewer

The ReportViewer is a visualization control to view Microsoft SSRS RDL/RDLC files on a web page and it is powered by HTML5/JavaScript. It has support to bind DataSources/Parameters to the Reports and also supports exporting, paging, zooming and printing the report.

$(element).ejReportViewer<span class="signature">()</span>

#### Example

{% highlight html %}

<div id="reportviewer">ReportViewer</div> 
<script>
    // Create ReportViewer
    $('#reportviewer').ejReportViewer();    
</script>

{% endhighlight %}

#### Requires

* module:jQuery

* module:jquery.easing.1.3.js

* module:jquery.globalize.js

* module:jquery.easing.1.3.js

* module:jsrender.js

* module:ej.core.js

* module:ej.editor.js

* module:ej.dialog.js

* module:ej.treeview.js

* module:ej.dropdownlist.js

* module:ej.checkbox.js

* module:ej.waitingpopup.js

* module:ej.toolbar.js

* module:ej.radiobutton.js

* module:ej.splitter.js

* module:ej.button.js

* module:ej.chart.js

* module:ej.datepicker.js

* module:ej.map.js

* module:ej.touch.js

* module:ej.data.js

* module:ej.circulargauge.js

* module:ej.lineargauge.js

* module:ej.reportviewer.js


## Members

### dataSources `array`
{:#members:datasources}

Gets or sets the list of data sources for the RDLC report.

#### Default Value

* []

#### Example

{% highlight html %}
 
<div id="reportviewer"></div> 
<script>
    $("#reportviewer").ejReportViewer({ dataSources: [{name:"Menu Items",
    values:[{ OrderId: "21D60", FoodName: "Burger", Price: 20, Category: "Veg" },
            { OrderId: "21D61", FoodName: "Pizza", Price: 25, Category: "Non-Veg" },
            { OrderId: "21D63", FoodName: "Sandwiches", Price: 30, Category: "Non-Veg" },
            { OrderId: "21D65", FoodName: "Chicken Drum Sticks", Price: 23, Category: "Non-Veg" },
            { OrderId: "21D64", FoodName: "Fulka", Price: 15, Category: "Veg" }]}]
    });
</script>

{% endhighlight %}

### dataSources.name `string`
{:#members:datasources-name}

Gets or sets the name of the data source.

#### Default Value

* empty

#### Example

{% highlight html %}

<div id="reportviewer"></div> 
<script>
    $("#reportviewer").ejReportViewer({ dataSources: [name:"Menu Items",
    values:[{ OrderId: "21D60", FoodName: "Burger", Price: 20, Category: "Veg" },
            { OrderId: "21D61", FoodName: "Pizza", Price: 25, Category: "Non-Veg" },
            { OrderId: "21D63", FoodName: "Sandwiches", Price: 30, Category: "Non-Veg" },
            { OrderId: "21D65", FoodName: "Chicken Drum Sticks", Price: 23, Category: "Non-Veg" },
            { OrderId: "21D64", FoodName: "Fulka", Price: 15, Category: "Veg" }]]
    });
</script>

{% endhighlight %}

### dataSources.value `array`
{:#members:datasources-value}

Gets or sets the values of data source.

#### Default Value

* []

#### Example

{% highlight html %}

<div id="reportviewer"></div> 
<script>
    $("#reportviewer").ejReportViewer({ dataSources: [name:"Menu Items",
    value:[{ OrderId: "21D60", FoodName: "Burger", Price: 20, Category: "Veg" },
            { OrderId: "21D61", FoodName: "Pizza", Price: 25, Category: "Non-Veg" },
            { OrderId: "21D63", FoodName: "Sandwiches", Price: 30, Category: "Non-Veg" },
            { OrderId: "21D65", FoodName: "Chicken Drum Sticks", Price: 23, Category: "Non-Veg" },
            { OrderId: "21D64", FoodName: "Fulka", Price: 15, Category: "Veg" }]]
    });
</script>

{% endhighlight %}

### enablePageCache `boolean`
{:#members:enablepagecache}

Enables or disables the page cache of report.

#### Default Value

* false

#### Example

{% highlight html %}
 
<div id="reportviewer"></div> 
<script>        
    $("#reportviewer").ejReportViewer({ enablePageCache: false });            
</script>

{% endhighlight %}

### exportSettings `object`
{:#members:exportsettings}

Specifies the export settings.

### exportSettings.exportOptions `enum`
{:#members:exportsettings-exportoptions}

<ts name = "ej.ReportViewer.ExportOptions"/>

Specifies the export formats.

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
<td class="description">Specifies the All property in ExportOptions to get all available options.</td>
</tr>
<tr>
<td class="name">Pdf</td>
<td class="description">Specifies the Pdf property in ExportOptions to get Pdf option.</td>
</tr>
<tr>
<td class="name">Word</td>
<td class="description">Specifies the Word property in ExportOptions to get Word option.</td>
</tr>
<tr>
<td class="name">Excel</td>
<td class="description">Specifies the Excel property in ExportOptions to get Excel option.</td>
</tr>
<tr>
<td class="name">Html</td>
<td class="description">Specifies the Html property in ExportOptions to get Html option.</td>
</tr>
<tr>
<td class="name">PPT</td>
<td class="description">Specifies the PPT property in ExportOptions to get PPT option.</td>
</tr>
<tr>
<td class="name">CSV</td>
<td class="description">Specifies the CSV property in ExportOptions to get CSV option.</td>
</tr>
<tr>
<td class="name">CustomItems</td>
<td class="description">Specifies the customItems property in ExportOptions to get customItems option.</td>
</tr>
</tbody>
</table>

#### Default Value

* ej.ReportViewer.ExportOptions.All

#### Example

{% highlight html %}
 
<div id="reportviewer"></div> 
<script>        
    $("#reportviewer").ejReportViewer(
        {
            exportSettings:{ exportOptions: ej.ReportViewer.ExportOptions.Html | ej.ReportViewer.ExportOptions.Pdf }
        });            
</script>

{% endhighlight %}

### exportSettings.excelFormat `enum`
{:#members:exportsettings-excelformat}

<ts name = "ej.ReportViewer.ExcelFormats"/>

Specifies the excel export format.

<table class="params">
<thead>
<tr>
<th>Name</th>
<th>Description</th>
</tr>
</thead>
<tbody>
<tr>
<td class="name">Excel97to2003</td>
<td class="description">Specifies the Excel97to2003 property in ExcelFormats to get specified version of exported format.</td>
</tr>
<tr>
<td class="name">Excel2007</td>
<td class="description">Specifies the Excel2007 property in ExcelFormats to get specified version of exported format.</td>
</tr>
<tr>
<td class="name">Excel2010</td>
<td class="description">Specifies the Excel2010 property in ExcelFormats to get specified version of exported format.</td>
</tr>
<tr>
<td class="name">Excel2013</td>
<td class="description">Specifies the Excel2013 property in ExcelFormats to get specified version of exported format.</td>
</tr>
</tbody>
</table>

#### Default Value

* ej.ReportViewer.ExcelFormats.Excel97to2003

#### Example

{% highlight html %}
 
<div id="reportviewer"></div> 
<script>        
    $("#reportviewer").ejReportViewer(
        {
            exportSettings:{ excelFormat: ej.ReportViewer.ExcelFormats.Excel97to2003}
        });            
</script>

{% endhighlight %}

### exportSettings.wordFormat `enum`
{:#members:exportsettings-wordformat}

<ts name = "ej.ReportViewer.WordFormats"/>

Specifies the word export format.

<table class="params">
<thead>
<tr>
<th>Name</th>
<th>Description</th>
</tr>
</thead>
<tbody>
<tr>
<td class="name">Doc</td>
<td class="description">Specifies the Doc property in WordFormats to get specified version of exported format.</td>
</tr>
<tr>
<td class="name">Dot</td>
<td class="description">Specifies the Dot property in WordFormats to get specified version of exported format.</td>
</tr>
<tr>
<td class="name">DOCX</td>
<td class="description">Specifies the DOCX property in WordFormats to get specified version of exported format.</td>
</tr>
<tr>
<td class="name">Word2007</td>
<td class="description">Specifies the Word2007 property in WordFormats to get specified version of exported format.</td>
</tr>
<tr>
<td class="name">Word2010</td>
<td class="description">Specifies the Word2010 property in WordFormats to get specified version of exported format.</td>
</tr>
<tr>
<td class="name">Word2013</td>
<td class="description">Specifies the Word2013 property in WordFormats to get specified version of exported format.</td>
</tr>
<tr>
<td class="name">Word2007Dotx</td>
<td class="description">Specifies the Word2007Dotx property in WordFormats to get specified version of exported format.</td>
</tr>
<tr>
<td class="name">Word2010Dotx</td>
<td class="description">Specifies the Word2010Dotx property in WordFormats to get specified version of exported format.</td>
</tr>
<tr>
<td class="name">Word2013Dotx</td>
<td class="description">Specifies the Word2013Dotx property in WordFormats to get specified version of exported format.</td>
</tr>
<tr>
<td class="name">Word2007Docm</td>
<td class="description">Specifies the Word2007Docm property in WordFormats to get specified version of exported format.</td>
</tr>
<tr>
<td class="name">Word2010Docm</td>
<td class="description">Specifies the Word2010Docm property in WordFormats to get specified version of exported format.</td>
</tr>
<tr>
<td class="name">Word2013Docm</td>
<td class="description">Specifies the Word2013Docm property in WordFormats to get specified version of exported format.</td>
</tr>
<tr>
<td class="name">Word2007Dotm</td>
<td class="description">Specifies the Word2007Dotm property in WordFormats to get specified version of exported format.</td>
</tr>
<tr>
<td class="name">Word2010Dotm</td>
<td class="description">Specifies the Word2010Dotm property in WordFormats to get specified version of exported format.</td>
</tr>
<tr>
<td class="name">Word2013Dotm</td>
<td class="description">Specifies the Word2013Dotm property in WordFormats to get specified version of exported format.</td>
</tr>
<tr>
<td class="name">RTF</td>
<td class="description">Specifies the RTF property in WordFormats to get specified version of exported format.</td>
</tr>
<tr>
<td class="name">Txt</td>
<td class="description">Specifies the Txt property in WordFormats to get specified version of exported format.</td>
</tr>
<tr>
<td class="name">EPUB</td>
<td class="description">Specifies the EPUB property in WordFormats to get specified version of exported format.</td>
</tr>
<tr>
<td class="name">HTML</td>
<td class="description">Specifies the HTML property in WordFormats to get specified version of exported format.</td>
</tr>
<tr>
<td class="name">XML</td>
<td class="description">Specifies the XML property in WordFormats to get specified version of exported format.</td>
</tr>
<tr>
<td class="name">Automatic</td>
<td class="description">Specifies the Automatic property in WordFormats to get specified version of exported format.</td>
</tr>
</tbody>
</table>

#### Default Value

* ej.ReportViewer.WordFormats.Doc

#### Example

{% highlight html %}
 
<div id="reportviewer"></div> 
<script>        
    $("#reportviewer").ejReportViewer(
        {
            exportSettings:{ wordFormat: ej.ReportViewer.WordFormats.Doc}
        });            
</script>

{% endhighlight %}

### exportSettings.pptFormat `enum`
{:#members:exportsettings-pptformat}

<ts name = "ej.ReportViewer.PPTFormats"/>

Specifies the ppt export format.

<table class="params">
<thead>
<tr>
<th>Name</th>
<th>Description</th>
</tr>
</thead>
<tbody>
<tr>
<td class="name">PowerPoint97to2003</td>
<td class="description">Represents PowerPoint97to2003 version.</td>
</tr>
<tr>
<td class="name">PowerPoint2007</td>
<td class="description">Represents PowerPoint2007 version.</td>
</tr>
<tr>
<td class="name">PowerPoint2010</td>
<td class="description">Represents PowerPoint2010 version.</td>
</tr>
<tr>
<td class="name">PowerPoint2013</td>
<td class="description">Represents PowerPoint2013 version.</td>
</tr>
</tbody>
</table>

#### Default Value

* ej.ReportViewer.PPTFormats.PowerPoint97to2003

#### Example

{% highlight html %}

<div id="reportviewer"></div> 
<script>
    $("#reportviewer").ejReportViewer(
        {
            exportSettings:{ pptFormat: ej.ReportViewer.PPTFormats.PowerPoint2010}
        });
</script>

{% endhighlight %}

### exportSettings.customItems `array`
{:#members:exportsettings-customitems}

Add the custom icon item to the export options.

#### Default Value

* empty

#### Example

{% highlight html %}
 
<div id="reportviewer"></div> 
<script>          
    $("#reportviewer").ejReportViewer(
        {
            exportSettings: {
                        customItems: [{
                            index: 2,
                            cssClass: '',
                            value: 'exportCustom',
                        },
                        {
                            index: 4,
                            cssClass: '',
                            value: 'exportCustom3',
                        }]
                    },
        });         
</script>

{% endhighlight %}

### isResponsive `boolean`
{:#members:isresponsive}

When set to true, adapts the report layout to fit the screen size of devices on which it renders.

#### Default Value

* true

#### Example

{% highlight html %}
 
<div id="reportviewer"></div> 
<script>        
    $("#reportviewer").ejReportViewer({ isResponsive: true });            
</script>

{% endhighlight %}

### locale `string`
{:#members:locale}

Specifies the locale for report viewer.

#### Default Value

* "en-US"

#### Example

{% highlight html %}
 
<div id="reportviewer"></div> 
<script>          
    $("#reportviewer").ejReportViewer(
        {
            locale: "it-IT"
        });             
</script>

{% endhighlight %}

### pageSettings `object`
{:#members:pagesettings}

Specifies the page settings.

### pageSettings.orientation `enum`
{:#members:pagesettings-orientation}

<ts name = "ej.ReportViewer.Orientation"/>

Specifies the print layout orientation.

<table class="params">
<thead>
<tr>
<th>Name</th>
<th>Description</th>
</tr>
</thead>
<tbody>
<tr>
<td class="name">Landscape</td>
<td class="description">Specifies the Landscape property in pageSettings.orientation to get specified layout.</td>
</tr>
<tr>
<td class="name">portrait</td>
<td class="description">Specifies the portrait property in pageSettings.orientation to get specified layout.</td>
</tr>
</tbody>
</table>

#### Default Value

* null

#### Example

{% highlight html %}
 
<div id="reportviewer"></div> 
<script>        
    $("#reportviewer").ejReportViewer(
        {
            pageSettings:{ orientation: ej.ReportViewer.Orientation.Landscape }
        });
</script>

{% endhighlight %}

### pageSettings.paperSize `enum`
{:#members:pagesettings-papersize}

<ts name = "ej.ReportViewer.PaperSize"/>

Specifies the paper size of print layout.

<table class="params">
<thead>
<tr>
<th>Name</th>
<th>Description</th>
</tr>
</thead>
<tbody>
<tr>
<td class="name">A3</td>
<td class="description">Specifies the A3 as value in pageSettings.paperSize to get specified size.</td>
</tr>
<tr>
<td class="name">portrait</td>
<td class="description">Specifies the A4 as value in pageSettings.paperSize to get specified size.</td>
</tr>
<tr>
<td class="name">B4_JIS</td>
<td class="description">Specifies the B4(JIS) as value in pageSettings.paperSize to get specified size.</td>
</tr>
<tr>
<td class="name">B5_JIS</td>
<td class="description">Specifies the B5(JIS) as value in pageSettings.paperSize to get specified size.</td>
</tr>
<tr>
<td class="name">Envelope_10</td>
<td class="description">Specifies the Envelope #10 as value in pageSettings.paperSize to get specified size.</td>
</tr>
<tr>
<td class="name">Envelope_Monarch</td>
<td class="description">Specifies the Envelope as value in pageSettings.paperSize to get specified size.</td>
</tr>
<tr>
<td class="name">Executive</td>
<td class="description">Specifies the Executive as value in pageSettings.paperSize to get specified size.</td>
</tr>
<tr>
<td class="name">Legal</td>
<td class="description">Specifies the Legal as value in pageSettings.paperSize to get specified size.</td>
</tr>
<tr>
<td class="name">Letter</td>
<td class="description">Specifies the Letter as value in pageSettings.paperSize to get specified size.</td>
</tr>
<tr>
<td class="name">Tabloid</td>
<td class="description">Specifies the Tabloid as value in pageSettings.paperSize to get specified size.</td>
</tr>
<tr>
<td class="name">Custom</td>
<td class="description">Specifies the Custom as value in pageSettings.paperSize to get specified size.</td>
</tr>
</tbody>
</table>

#### Default Value

* null

#### Example

{% highlight html %}
 
<div id="reportviewer"></div> 
<script>        
    $("#reportviewer").ejReportViewer(
        {
            pageSettings:{ paperSize: ej.ReportViewer.PaperSize.A4 }
        });
</script>

{% endhighlight %}

### parameters `array`
{:#members:parameters}

Gets or sets the list of parameters associated with the report.

#### Default Value

* []

#### Example

{% highlight html %}
 
<div id="reportviewer"></div> 
<script>
    $("#reportviewer").ejReportViewer({ 
        parameters: [{
            name:"Vehicle",
            labels:["Motor Bikes"],
            prompt:"Please select the color",
            values:["Red","Green","Blue","Yellow","Black"],
            nullable:false
        }]       
    });
</script>

{% endhighlight %}

### parameters.labels `array`
{:#members:parameters-labels}

Gets or sets the parameter labels.

#### Default Value

* null

#### Example

{% highlight html %}

<div id="reportviewer"></div> 
<script>
    $("#reportviewer").ejReportViewer({ 
        parameters: [{
            name:"Vehicle",
            labels:["Motor Bikes"],
            prompt:"Please select the color",
            values:["Red","Green","Blue","Yellow","Black"],
            nullable:false
        }]
    });
</script>

{% endhighlight %}

### parameters.name `string`
{:#members:parameters-name}

Gets or sets the name of the parameter.

#### Default Value

* empty

#### Example

{% highlight html %}

<div id="reportviewer"></div> 
<script>
    $("#reportviewer").ejReportViewer({
        parameters: [{
            name:"Vehicle",
            labels:["Motor Bikes"],
            prompt:"Please select the color",
            values:["Red","Green","Blue","Yellow","Black"],
            nullable:false
        }]
    });
</script>

{% endhighlight %}

### parameters.nullable `boolean`
{:#members:parameters-nullable}

Gets or sets whether the parameter allows nullable value or not.

#### Default Value

* false

#### Example

{% highlight html %}

<div id="reportviewer"></div> 
<script>
    $("#reportviewer").ejReportViewer({
        parameters: [{
            name:"Vehicle",
            labels:["Motor Bikes"],
            prompt:"Please select the color",
            values:["Red","Green","Blue","Yellow","Black"],
            nullable:false
        }]
    });
</script>

{% endhighlight %}

### parameters.prompt `string`
{:#members:parameters-prompt}

Gets or sets the prompt message associated with the specified parameter.

#### Default Value

* empty

#### Example

{% highlight html %}

<div id="reportviewer"></div> 
<script>
    $("#reportviewer").ejReportViewer({ 
        parameters: [{
            name:"Vehicle",
            labels:["Motor Bikes"],
            prompt:"Please select the Color",
            values:["Red","Green","Blue","Yellow","Black"],
            nullable:false
        }]
    });
</script>

{% endhighlight %}

### parameters.values `array`
{:#members:parameters-values}

Gets or sets the parameter values.

#### Default Value

* []

#### Example

{% highlight html %}

<div id="reportviewer"></div> 
<script>
    $("#reportviewer").ejReportViewer({ 
        parameters: [{
            name:"Vehicle",
            labels:["Motor Bikes"],
            prompt:"Please select the color",
            values:["Red","Green","Blue","Yellow","Black"],
            nullable:false
        }]
    });
</script>

{% endhighlight %}

### parameterSettings `object`

{:#members:parametersettings}

Specifies the parameter settings.

### parameterSettings.delimiterChar `string`
{:#members:parametersettings-delimiterchar}

Sets the separator when the multiSelectMode with delimiter option or checkbox is enabled with the dropdown. When you enter the delimiter value, the texts after the delimiter are considered as a separate word or query. The delimiter string is a single character and must be a symbol. Mostly, the delimiter symbol is used as comma (,) or semi-colon (;) or any other special character.

#### Default Value

* ","

#### Example

{% highlight html %}

<div id="reportviewer"></div> 
<script>
    $("#reportviewer").ejReportViewer(
        {
            parameterSettings: { delimiterChar: "," }
        });
</script>

{% endhighlight %}

### parameterSettings.popupHeight `string`
{:#members:parametersettings-popupheight}

Specifies the height of the combobox parameter popup list. By default, the popup height value is "152px".

#### Default Value

* "152px"

#### Example

{% highlight html %}

<div id="reportviewer"></div> 
<script>
    $("#reportviewer").ejReportViewer(
        {
            parameterSettings: { popupHeight: "200px" }
        });
</script>

{% endhighlight %}

### parameterSettings.popupWidth `string`
{:#members:parametersettings-popupwidth}

Specifies the width of the combobox parameter popup list. By default, the popup width sets based on the width of the component.

#### Default Value

* "auto"

#### Example

{% highlight html %}

<div id="reportviewer"></div> 
<script>
    $("#reportviewer").ejReportViewer(
        {
            parameterSettings: { popupWidth: "150px" }
        });
</script>

{% endhighlight %}


### parameterSettings.itemWidth `string`
{:#members:parametersettings-itemwidth}

Specifies the width of the parameter item. By default, the item width value is set as "185px".

#### Default Value

* "185px"

#### Example

{% highlight html %}

<div id="reportviewer"></div> 
<script>
    $("#reportviewer").ejReportViewer(
        {
            parameterSettings: { itemWidth: "250px" }
        });
</script>

{% endhighlight %}

### parameterSettings.labelWidth `string`
{:#members:parametersettings-labelwidth}

Specifies the width of the parameter label. By default, the parameter label width value is set as "110px".

#### Default Value

* "110px"

#### Example

{% highlight html %}

<div id="reportviewer"></div> 
<script>
    $("#reportviewer").ejReportViewer(
        {
            parameterSettings: { labelWidth: "auto" }
        });
</script>

{% endhighlight %}

### printMode `boolean`
{:#members:printmode}

Enables and disables the print mode.

#### Default Value

* false

#### Example

{% highlight html %}
 
<div id="reportviewer"></div> 
<script>          
    $("#reportviewer").ejReportViewer(
        {
            printMode:true
        });             
</script>

{% endhighlight %}

### printOption `enum`
{:#members:printoption}

<ts name = "ej.ReportViewer.PrintOptions"/>

Specifies the print option of the report.

<table class="params">
<thead>
<tr>
<th>Name</th>
<th>Description</th>
</tr>
</thead>
<tbody>
<tr>
<td class="name">Default</td>
<td class="description">Specifies the Default property in printOptions.</td>
</tr>
<tr>
<td class="name">NewTab</td>
<td class="description">Specifies the NewTab property in printOptions.</td>
</tr>
<tr>
<td class="name">None</td>
<td class="description">Specifies the None property in printOptions.</td>
</tr>
</tbody>
</table>

#### Default Value

* ej.ReportViewer.PrintOptions.Default

#### Example

{% highlight html %}
 
<div id="reportviewer"></div> 
<script>        
    $("#reportviewer").ejReportViewer({ printOption: ej.ReportViewer.PrintOptions.Default });            
</script>

{% endhighlight %}

### processingMode `enum`
{:#members:processingmode}

<ts name = "ej.ReportViewer.ProcessingMode"/>

Specifies the processing mode of the report.

<table class="params">
<thead>
<tr>
<th>Name</th>
<th>Description</th>
</tr>
</thead>
<tbody>
<tr>
<td class="name">Remote</td>
<td class="description">Specifies the Remote property in processingMode.</td>
</tr>
<tr>
<td class="name">Local</td>
<td class="description">Specifies the Local property in processingMode.</td>
</tr>
</tbody>
</table>

#### Default Value

* ej.ReportViewer.ProcessingMode.Remote

#### Example

{% highlight html %}
 
<div id="reportviewer"></div> 
<script>        
    $("#reportviewer").ejReportViewer({ processingMode: ej.ReportViewer.ProcessingMode.Remote });            
</script>

{% endhighlight %}

### renderMode `enum`
{:#members:rendermode}

<ts name = "ej.ReportViewer.RenderMode"/>

Specifies the render layout.

<table class="params">
<thead>
<tr>
<th>Name</th>
<th>Description</th>
</tr>
</thead>
<tbody>
<tr>
<td class="name">Default</td>
<td class="description">Specifies the Default property in RenderMode to get default output.</td>
</tr>
<tr>
<td class="name">Mobile</td>
<td class="description">Specifies the Mobile property in RenderMode to get specified output.</td>
</tr>
<tr>
<td class="name">Desktop</td>
<td class="description">Specifies the Desktop property in RenderMode to get specified output.</td>
</tr>
</tbody>
</table>

#### Default Value

* ej.ReportViewer.RenderMode.Default

#### Example

{% highlight html %}
 
<div id="reportviewer"></div> 
<script>        
    $("#reportviewer").ejReportViewer({ renderMode: ej.ReportViewer.RenderMode.Default });            
</script>

{% endhighlight %}

### reportPath `string`
{:#members:reportpath}

Gets or sets the path of the report file.

#### Default Value

* empty

#### Example

{% highlight html %}

<div id="reportviewer"></div> 
<script>
    $("#reportviewer").ejReportViewer({ reportPath: "~/App_Data/Sample.rdl" });            
</script>

{% endhighlight %}

### reportServerUrl `string`
{:#members:reportserverurl}

Gets or sets the reports server URL.

#### Default Value

* empty

#### Example

{% highlight html %}
 
<div id="reportviewer"></div> 
<script>
    $("#reportviewer").ejReportViewer({ reportServerUrl: "http://mvc.syncfusion.com/reportserver" });            
</script>

{% endhighlight %}

### reportServiceUrl `string`
{:#members:reportserviceurl}

Specifies the report Web API service URL.

#### Default Value

* empty

#### Example

{% highlight html %}

<div id="reportviewer"></div> 
<script>
    $("#reportviewer").ejReportViewer({ reportServiceUrl: "../api/RDLReport" });            
</script>

{% endhighlight %}

### toolbarSettings `object`
{:#members:toolbarsettings}

Specifies the toolbar settings.

### toolbarSettings.click `string`
{:#members:toolbarsettings-click}

Fires when user click on toolbar item in the toolbar.

#### Default Value

* empty

#### Example

{% highlight html %}
 
<div id="reportviewer"></div> 
<script>          
    $("#reportviewer").ejReportViewer(
        {
            toolbarSettings:{click: "onToolbarClick"}
        });         
</script>

{% endhighlight %}

### toolbarSettings.items `enum`
{:#members:toolbarsettings-items}

<ts name = "ej.ReportViewer.ToolbarItems"/>

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
<td class="name">Print</td>
<td class="description">Specifies the Print as value in ToolbarItems to get specified item.</td>
</tr>
<tr>
<td class="name">Refresh</td>
<td class="description">Specifies the Refresh as value in ToolbarItems to get specified item.</td>
</tr>
<tr>
<td class="name">Zoom</td>
<td class="description">Specifies the Zoom as value in ToolbarItems to get specified item.</td>
</tr>
<tr>
<td class="name">FittoPage</td>
<td class="description">Specifies the FittoPage as value in ToolbarItems to get specified item.</td>
</tr>
<tr>
<td class="name">Export</td>
<td class="description">Specifies the Export as value in ToolbarItems to get specified item.</td>
</tr>
<tr>
<td class="name">PageNavigation</td>
<td class="description">Specifies the PageNavigation as value in ToolbarItems to get specified item.</td>
</tr>
<tr>
<td class="name">Parameters</td>
<td class="description">Specifies the Parameters as value in ToolbarItems to get specified item.</td>
</tr>
<tr>
<td class="name">PrintLayout</td>
<td class="description">Specifies the PrintLayout as value in ToolbarItems to get specified item.</td>
</tr>
<tr>
<td class="name">PageSetup</td>
<td class="description">Specifies the PageSetup as value in ToolbarItems to get specified item.</td>
</tr>
</tbody>
</table>

#### Default Value

* ej.ReportViewer.ToolbarItems.All

#### Example

{% highlight html %}
 
<div id="reportviewer"></div> 
<script>        
    $("#reportviewer").ejReportViewer(
        {
            toolbarSettings:{ items: ej.ReportViewer.ToolbarItems.All }
        });
</script>

{% endhighlight %}

### toolbarSettings.showToolbar `boolean`
{:#members:toolbarsettings-showtoolbar}

Shows or hides the toolbar.

#### Default Value

* true

#### Example

{% highlight html %}
 
<div id="reportviewer"></div> 
<script>          
    $("#reportviewer").ejReportViewer(
        {
            toolbarSettings:{ showToolbar: true }
        });         
</script>

{% endhighlight %}

### toolbarSettings.showTooltip `boolean`
{:#members:toolbarsettings-showtooltip}

Shows or hides the tooltip of toolbar items.

#### Default Value

* true

#### Example

{% highlight html %}
 
<div id="reportviewer"></div> 
<script>          
    $("#reportviewer").ejReportViewer(
        {
            toolbarSettings:{ showTooltip: true }
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
 
<div id="reportviewer"></div> 
<script>          
    $("#reportviewer").ejReportViewer(
        {
            toolbarSettings:{ templateId: "customtoolbarId" }
        });         
</script>

{% endhighlight %}

### toolbarSettings.customItems `array`
{:#members:toolbarsettings-customitems}

Add the custom icon item to the toolbar.

#### Default Value

* empty

#### Example

{% highlight html %}
 
<div id="reportviewer"></div> 
<script>          
    $("#reportviewer").ejReportViewer(
        {
            toolbarSettings:{
                 customItems: [{
                            groupIndex: 1,
                            index: 1,
                            itemType: 'Default',
                            cssClass: "e-icon e-mail e-reportviewer-icon CustomItem",
                            tooltip: { header: 'CustomItem', content: 'toolbaritems', value: 'CustomItem' },
                        }]
             }
        });         
</script>

{% endhighlight %}

### toolbarSettings.customGroups `array`
{:#members:toolbarsettings-customgroups}

Add the custom icon groups to the toolbar.

#### Default Value

* empty

#### Example

{% highlight html %}
 
<div id="reportviewer"></div> 
<script>          
    $("#reportviewer").ejReportViewer(
        {
            toolbarSettings:{
                 customGroups: [{
                            items: [{
                                itemType: 'Default',
                                cssClass: "e-icon e-mail e-reportviewer-icon CustomGroup",
                                tooltip: { header: 'CustomGroup', content: 'toolbargroups', value: 'CustomGroup' },
                            },
                            {
                                itemType: 'Default',
                                cssClass: "e-icon e-mail e-reportviewer-icon subCustomGroup",
                                tooltip: { header: 'subCustomGroup', content: 'subtoolbargroups', value: 'subCustomGroup' },
                            }],
                            groupIndex: 3
                        }],
             }
        });         
</script>

{% endhighlight %}

### zoomFactor `number`
{:#members:zoomfactor}

Gets or sets the zoom factor for report viewer.

#### Default Value

* 1

#### Example

{% highlight html %}
 
<div id="reportviewer"></div> 
<script>
    $("#reportviewer").ejReportViewer({ zoomFactor:  2 });
</script>

{% endhighlight %}

### serviceAuthorizationToken `string`
{:#members:serviceauthorizationtoken}

Specifies the token for authorizing reporting service url to process the reports.

#### Default Value

* empty

#### Example

{% highlight html %}

<div id="reportviewer"></div> 
<script>
      $(function () {
            var dataValue = "";
            var apiRequest = new Object();
            apiRequest.password = "demo";
            apiRequest.userid = "guest";
            $.ajax({
                type: "POST",
                url: "http://reportserver.syncfusion.com/api/get-user-key",
                data: apiRequest,
                success: function (data) {
                    dataValue = data.Token;
                    var token = JSON.parse(dataValue);
                    $("#reportviewer").ejReportViewer(
                        {
                            reportServiceUrl: "http://reportserver.syncfusion.com/ReportService/api/Viewer",
                            serviceAuthorizationToken: token["token_type"] + " " + token["access_token"],
                            reportPath: '/Sample Reports/Company Sales'
                        });
                }
            });
        });            
</script>

{% endhighlight %}

### enableParameterBlockScroller `boolean`
{:#members:enableparameterblockscroller}

Enables and disables the parameter block scroller.

#### Default Value

* true

#### Example

{% highlight html %}
 
<div id="reportviewer"></div> 
<script>
    $("#reportviewer").ejReportViewer(
        {
            enableParameterBlockScroller: false
        });
</script>

{% endhighlight %}

### enableDatasourceBlockScroller `boolean`
{:#members:enabledatasourceblockscroller}

Enables and disables the data source credential block scroller.

#### Default Value

* true

#### Example

{% highlight html %}
 
<div id="reportviewer"></div> 
<script>
    $("#reportviewer").ejReportViewer(
        {
            enableDatasourceBlockScroller: false
        });
</script>
{% endhighlight %}

### sizeToReportContent `boolean`
{:#members:sizeToReportContent}

Render the ReportViewer height based on the report content size.

#### Default Value

* false

#### Example

{% highlight html %}
 
<div id="reportviewer"></div> 
<script>
    $("#reportviewer").ejReportViewer(
        {
            sizeToReportContent: true
        });
</script>
{% endhighlight %}

### autoRender `boolean`
{:#members:autorender}

Enables and disables the rendering of Viewer when default values are specified for the parameters.

#### Default Value

* true

#### Example

{% highlight html %}
 
<div id="reportviewer"></div> 
<script>
    $("#reportviewer").ejReportViewer(
        {
            autoRender: false
        });
</script>
{% endhighlight %}

### enableNotificationBar `boolean`
{:#members:enablenotificationbar}

Enables and disables the Error Notification bar.

#### Default Value

* true

#### Example

{% highlight html %}
 
<div id="reportviewer"></div> 
<script>
    $("#reportviewer").ejReportViewer(
        {
            enableNotificationBar: false
        });
</script>
{% endhighlight %}

### enableDropDownSearch `boolean`
{:#members:enabledropdownsearch}

Enables and disables the drop-down parameter search.

#### Default Value

* false

#### Example

{% highlight html %}
 
<div id="reportviewer"></div> 
<script>
    $("#reportviewer").ejReportViewer(
        {
            enableDropDownSearch: true
        });
</script>
{% endhighlight %}

### enablePageVirtualization `boolean`
{:#members:enablepagevirtualization}

Enables and disables the PageVirtualization.

#### Default Value

* false

#### Example

{% highlight html %}
 
<div id="reportviewer"></div> 
<script>
    $("#reportviewer").ejReportViewer(
        {
            enablePageVirtualization: true
        });
</script>
{% endhighlight %}

### showExceptionsInDialog `boolean`
{:#members:showexceptionsindialog}

Gets or sets the showExceptionsInDialog for report viewer.

#### Default Value

* false

#### Example

{% highlight html %}

<div id="reportviewer"></div> 
<script>
    $("#reportviewer").ejReportViewer(
        {
            showExceptionsInDialog: true
        });
</script>
{% endhighlight %}

## Methods

### exportReport()
{:#methods:exportreport}

Export the report to the specified format.

#### Example

{% highlight html %}
 
<div id="reportviewer">ReportViewer</div> 
<script>
    var reportviewerObj = $("#reportviewer").data("ejReportViewer");
    reportviewerObj.exportReport("PDF"); //Exports the report into PDF format.
</script>

{% endhighlight %}

### fitToPage()
{:#methods:fittopage}

Fit the report page to the container.

#### Example

{% highlight html %}
 
<div id="reportviewer">ReportViewer</div> 
<script>
    var reportviewerObj = $("#reportviewer").data("ejReportViewer");
    reportviewerObj.fitToPage(); // To fit the report page.
</script>

{% endhighlight %}

### fitToPageHeight()
{:#methods:fittopageheight}

Fit the report page height to the container.

#### Example

{% highlight html %}
 
<div id="reportviewer">ReportViewer</div> 
<script>
    var reportviewerObj = $("#reportviewer").data("ejReportViewer");
    reportviewerObj.fitToPageHeight(); // To fit the report page height.
</script>

{% endhighlight %}

### fitToPageWidth()
{:#methods:fittopagewidth}

Fit the report page width to the container.

#### Example

{% highlight html %}
 
<div id="reportviewer">ReportViewer</div> 
<script>
    var reportviewerObj = $("#reportviewer").data("ejReportViewer");
    reportviewerObj.fitToPageWidth(); // To fit the report page width.
</script>

{% endhighlight %}

### getDataSetNames()
{:#methods:getdatasetnames}

Get the available datasets name of the rdlc report.

#### Example

{% highlight html %}
 
<div id="reportviewer">ReportViewer</div> 
<script>
    var reportviewerObj = $("#reportviewer").data("ejReportViewer");
    reportviewerObj.getDataSetNames(); // To get the dataset names.
</script>

{% endhighlight %}

### getParameters()
{:#methods:getparameters}

Get the available parameters of the report.

#### Example

{% highlight html %}
 
<div id="reportviewer">ReportViewer</div> 
<script>
    var reportviewerObj = $("#reportviewer").data("ejReportViewer"); 
    reportviewerObj.getParameters(); // To get the parameters.
</script>

{% endhighlight %}

### gotoFirstPage()
{:#methods:gotofirstpage}

Navigate to first page of report.

#### Example

{% highlight html %}

<div id="reportviewer">ReportViewer</div> 
<script>
    var reportviewerObj = $("#reportviewer").data("ejReportViewer");
    reportviewerObj.gotoFirstPage(); // To navigate to first page
</script>

{% endhighlight %}

### gotoLastPage()
{:#methods:gotolastpage}

Navigate to last page of the report.

#### Example

{% highlight html %}
 
<div id="reportviewer">ReportViewer</div> 
<script>
    var reportviewerObj = $("#reportviewer").data("ejReportViewer");
    reportviewerObj.gotoLastPage(); // Navigate to the last page
</script>

{% endhighlight %}

### gotoNextPage()
{:#methods:gotonextpage}

Navigate to next page from the current page.

#### Example

{% highlight html %}
 
<div id="reportviewer">ReportViewer</div> 
<script>
    var reportviewerObj = $("#reportviewer").data("ejReportViewer");
    reportviewerObj.gotoNextPage(); //To navigate to the next page
</script>

{% endhighlight %}

### gotoPageIndex()
{:#methods:gotopageindex}

Go to specific page index of the report.

#### Example

{% highlight html %}
 
<div id="reportviewer">ReportViewer</div> 
<script>
    var reportviewerObj = $("#reportviewer").data("ejReportViewer");
    reportviewerObj.gotoPageIndex(5); // To navigate the specific page
</script>

{% endhighlight %}

### gotoPreviousPage()
{:#methods:gotopreviouspage}

Navigate to previous page from the current page.

#### Example

{% highlight html %}
 
<div id="reportviewer">ReportViewer</div> 
<script>
    var reportviewerObj = $("#reportviewer").data("ejReportViewer");
    reportviewerObj.gotoPreviousPage(); // To navigate to the previous page
</script>

{% endhighlight %}

### print()
{:#methods:print}

Print the report.

#### Example

{% highlight html %}
 
<div id="reportviewer">ReportViewer</div> 
<script>
    var reportviewerObj = $("#reportviewer").data("ejReportViewer");
    reportviewerObj.print(); //To perform print operation.
</script>

{% endhighlight %}

### printLayout()
{:#methods:printlayout}

Apply print layout to the report.

#### Example

{% highlight html %}
 
<div id="reportviewer">ReportViewer</div> 
<script>
    var reportviewerObj = $("#reportviewer").data("ejReportViewer");
    reportviewerObj.printLayout(); //Changes between print layout and normal modes.
</script>

{% endhighlight %}

### refresh()
{:#methods:refresh}

Refresh the report.

#### Example

{% highlight html %}
 
<div id="reportviewer">ReportViewer</div> 
<script>
    var reportviewerObj = $("#reportviewer").data("ejReportViewer");
    reportviewerObj.refresh(); // To refresh the report.
</script>

{% endhighlight %}

## Events

### destroy
{:#events:destroy}

Fires when the report viewer is destroyed successfully.If you want to perform any operation after destroying the reportviewer control,you can make use of the destroy event.

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
<td class="name">argument</td>
<td class="type"><span class="param-type">object</span></td>
<td class="description last">Event parameters from reportviewer.
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
<td class="name">cancel</td>
<td class="type"><span class="param-type">boolean</span></td>
<td class="description last">true if the event should be canceled; otherwise, false.</td>
</tr>
<tr>
<td class="name">model</td>
<td class="type"><span class="param-type">object</span></td>
<td class="description last">returns the report model.</td>
</tr>
<tr>
<td class="name">type</td>
<td class="type"><span class="param-type">string</span></td>
<td class="description last">returns the name of the event.</td>
</tr>
</tbody>
</table>
</td>
</tr>
</tbody>
</table>

#### Example

{% highlight html %}
 
<div id="reportviewer"></div>
<script>
    $("#reportviewer").ejReportViewer({
        destroy: function (args) {
            // Write a code block to perform any operation after destroy of reportviewer.
        }
    });
</script>

{% endhighlight %}

### drillThrough
{:#events:drillthrough}

Fires during drill through action done in report.If you want to perform any operation when a drill through action is performed, you can make use of the drillThrough event.

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
<td class="name">argument</td>
<td class="type"><span class="param-type">Object</span></td>
<td class="description last">Event parameters from reportviewer.
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
<td class="name">cancel</td>
<td class="type"><span class="param-type">boolean</span></td>
<td class="description last">true if the event should be canceled; otherwise, false.</td>
</tr>
<tr>
<td class="name">actionInfo</td>
<td class="type"><span class="param-type">Object</span></td>
<td class="description last">returns the actionInfo's parameters bookmarkLink, reportName, parameters.</td>
</tr>
<tr>
<td class="name">model</td>
<td class="type"><span class="param-type">object</span></td>
<td class="description last">returns the report model.</td>
</tr>
<tr>
<td class="name">type</td>
<td class="type"><span class="param-type">string</span></td>
<td class="description last">returns the name of the event.</td>
</tr>
</tbody>
</table>
</td>
</tr>
</tbody>
</table>

#### Example

{% highlight html %}
 
<div id="reportviewer"></div> 
<script>        
    $("#reportviewer").ejReportViewer({ 
        drillThrough: function (args) {
            // Write a code block to perform any operation when drill through action occurs in report.
        }
    });                   
</script>

{% endhighlight %}

### renderingBegin
{:#events:renderingbegin}

Fires before report rendering is completed.If you want to perform any operation before the rendering of report,you can make use of the renderingBegin event.

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
<td class="name">argument</td>
<td class="type"><span class="param-type">Object</span></td>
<td class="description last">Event parameters from reportviewer.
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
<td class="name">cancel</td>
<td class="type"><span class="param-type">boolean</span></td>
<td class="description last">true if the event should be canceled; otherwise, false.</td>
</tr>
<tr>
<td class="name">model</td>
<td class="type"><span class="param-type">object</span></td>
<td class="description last">returns the report model.</td>
</tr>
<tr>
<td class="name">type</td>
<td class="type"><span class="param-type">string</span></td>
<td class="description last">returns the name of the event.</td>
</tr>
</tbody>
</table>
</td>
</tr>
</tbody>
</table>

#### Example

{% highlight html %}
 
<div id="reportviewer"></div> 
<script>  
    //rendering begin event for report.               
    $("#reportviewer").ejReportViewer({
        renderingBegin:function(args) {
            // Write a code block to perform any operation before rendering.
        }
    });                 
</script>

{% endhighlight %}

### renderingComplete
{:#events:renderingcomplete}

Fires after report rendering completed.If you want to perform any operation after the rendering of report,you can make use of this renderingComplete event.

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
<td class="name">argument</td>
<td class="type"><span class="param-type">Object</span></td>
<td class="description last">Event parameters from reportviewer.
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
<td class="name">cancel</td>
<td class="type"><span class="param-type">boolean</span></td>
<td class="description last">true if the event should be canceled; otherwise, false.</td>
</tr>
<tr>
<td class="name">model</td>
<td class="type"><span class="param-type">object</span></td>
<td class="description last">returns the report model.</td>
</tr>
<tr>
<td class="name">type</td>
<td class="type"><span class="param-type">string</span></td>
<td class="description last">returns the name of the event.</td>
</tr>
<tr>
<td class="name">reportParameters</td>
<td class="type"><span class="param-type">object</span></td>
<td class="description last">returns the collection of parameters.</td>
</tr>
<tr>
<td class="name">reportParameters</td>
<td class="type"><span class="param-type">object</span></td>
<td class="description last">returns the collection of parameters.</td>
</tr>
</tbody>
</table>
</td>
</tr>
</tbody>
</table>

#### Example

{% highlight html %}
 
<div id="reportviewer"></div> 
<script>        
    //rendering complete event for reportviewer control.
    $("#reportviewer").ejReportViewer({ 
        renderingComplete:function(args) {
            // Write a code block to perform any operation after rendering completed.
        }
    });            
</script>

{% endhighlight %}

### reportError
{:#events:reporterror}

Fires when any error occurred while rendering the report.If you want to perform any operation when an error occurs in the report, you can make use of the reportError event.

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
<td class="name">argument</td>
<td class="type"><span class="param-type">Object</span></td>
<td class="description last">Event parameters from reportviewer.
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
<td class="name">cancel</td>
<td class="type"><span class="param-type">boolean</span></td>
<td class="description last">true if the event should be canceled; otherwise, false.</td>
</tr>
<tr>
<td class="name">error</td>
<td class="type"><span class="param-type">string</span></td>
<td class="description last">returns the error details.</td>
</tr>
<tr>
<td class="name">model</td>
<td class="type"><span class="param-type">object</span></td>
<td class="description last">returns the report model.</td>
</tr>
<tr>
<td class="name">type</td>
<td class="type"><span class="param-type">string</span></td>
<td class="description last">returns the name of the event.</td>
</tr>
</tbody>
</table>
</td>
</tr>
</tbody>
</table>

#### Example

{% highlight html %}
 
<div id="reportviewer"></div> 
<script>        
    $("#reportviewer").ejReportViewer({
        reportError: function (args) {
            // Write a code block to perform any operation when report error occurs.
        }
    });                         
</script>

{% endhighlight %}

### reportExport
{:#events:reportexport}

Fires when the report is being exported.If you want to perform any operation before exporting of report, you can make use of the reportExport event.

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
<td class="name">argument</td>
<td class="type"><span class="param-type">Object</span></td>
<td class="description last">Event parameters from reportviewer.
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
<td class="name">cancel</td>
<td class="type"><span class="param-type">boolean</span></td>
<td class="description last">true if the event should be canceled; otherwise, false.</td>
</tr>
<tr>
<td class="name">model</td>
<td class="type"><span class="param-type">object</span></td>
<td class="description last">returns the report model.</td>
</tr>
<tr>
<td class="name">type</td>
<td class="type"><span class="param-type">string</span></td>
<td class="description last">returns the name of the event.</td>
</tr>
</tbody>
</table>
</td>
</tr>
</tbody>
</table>

#### Example

{% highlight html %}
 
<div id="reportviewer"></div> 
<script>        
    $("#reportviewer").ejReportViewer({ 
        reportExport:  function (args) {
            // Write a code block to perform any action before exporting of report.
        }
    });           
</script>

{% endhighlight %}

### reportLoaded
{:#events:reportloaded}

Fires when the report is loaded.If you want to perform any operation after the successful loading of report, you can make use of the reportLoaded event.

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
<td class="name">
argument</td>
<td class="type"><span class="param-type">Object</span></td>
<td class="description last">event parameters from reportviewer.
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
<td class="name">cancel</td>
<td class="type"><span class="param-type">boolean</span></td>
<td class="description last">true if the event should be canceled; otherwise, false.</td>
</tr>
<tr>
<td class="name">model</td>
<td class="type"><span class="param-type">object</span></td>
<td class="description last">returns the report model.</td>
</tr>
<tr>
<td class="name">type</td>
<td class="type"><span class="param-type">string</span></td>
<td class="description last">returns the name of the event.</td>
</tr>
</tbody>
</table>
</td>
</tr>
</tbody>
</table>

#### Example

{% highlight html %}
 
<div id="reportviewer"></div> 
<script>        
    $("#reportviewer").ejReportViewer({
        reportLoaded: function(args) {
            // Write a code block to perform any action when the report is loaded successfully.
        }
    });             
</script>

{% endhighlight %}

### showError
{:#events:showerror}

Fires when user clicks on a failed report item in the rendered report, before displaying error details dialog. If you want to show custom error detail or perform any action before viewing error detail, you can make use of the showError event.

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
<td class="name">argument</td>
<td class="type"><span class="param-type">Object</span></td>
<td class="description last">Event parameters from reportviewer.
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
<td class="name">cancel</td>
<td class="type"><span class="param-type">boolean</span></td>
<td class="description last">true if the event should be canceled; otherwise, false.</td>
</tr>
<tr>
<td class="name">errorCode</td>
<td class="type"><span class="param-type">string</span></td>
<td class="description last">returns the error code.</td>
</tr>
<tr>
<td class="name">message</td>
<td class="type"><span class="param-type">string</span></td>
<td class="description last">returns the error message.</td>
</tr>
<tr>
<td class="name">detail</td>
<td class="type"><span class="param-type">string</span></td>
<td class="description last">returns the detailed error information.</td>
</tr>
</tbody>
</table>
</td>
</tr>
</tbody>
</table>

#### Example

{% highlight html %}
 
<div id="reportviewer"></div> 
<script>        
    $("#reportviewer").ejReportViewer({
        showError: function (args) {
            // Write a code block to perform any operation when user clicks a failed item in a report.
        }
    });
</script>

{% endhighlight %}

### viewReportClick
{:#events:viewreportclick}

Fires when click the View Report Button.

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
<td class="name">argument</td>
<td class="type"><span class="param-type">Object</span></td>
<td class="description last">Event parameters from reportviewer.
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
<td class="name">cancel</td>
<td class="type"><span class="param-type">boolean</span></td>
<td class="description last">true if the event should be canceled; otherwise, false.</td>
</tr>
<tr>
<td class="name">parameters</td>
<td class="type"><span class="param-type">Object</span></td>
<td class="description last">returns the parameter collection.</td>
</tr>
<tr>
<td class="name">model</td>
<td class="type"><span class="param-type">object</span></td>
<td class="description last">returns the report model.</td>
</tr>
<tr>
<td class="name">type</td>
<td class="type"><span class="param-type">string</span></td>
<td class="description last">returns the name of the event.</td>
</tr>
</tbody>
</table>
</td>
</tr>
</tbody>
</table>

#### Example

{% highlight html %}
 
<div id="reportviewer"></div> 
<script>        
    $("#reportviewer").ejReportViewer({ 
        viewReportClick:  function (args) {
            // Write a code block to perform any operation after destroy of reportviewer.
        }
    });           
</script>

{% endhighlight %}

### exportProgressChanged
{:#events:exportprogresschanged}

Fires when the export progress is changed. To perform any operation when the export progress is changed, use the exportProgressChanged event.

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
<td class="name">
argument</td>
<td class="type"><span class="param-type">Object</span></td>
<td class="description last">Event parameters from reportviewer.
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
<td class="name">format</td>
<td class="type"><span class="param-type">string</span></td>
<td class="description last">returns the export format</td>
</tr>
<tr>
<td class="name">stage</td>
<td class="type"><span class="param-type">string</span></td>
<td class="description last">returns the stage of export processing.</td>
</tr>
<tr>
<td class="name">handled</td>
<td class="type"><span class="param-type">boolean</span></td>
<td class="description last">true if the event should be handled; otherwise, false.</td>
</tr>
<tr>
<td class="name">containerId</td>
<td class="type"><span class="param-type">string</span></td>
<td class="description last">returns ReportViewer container Id.</td>
</tr>
</tbody>
</table>
</td>
</tr>
</tbody>
</table>

#### Example

{% highlight html %}
 
<div id="reportviewer"></div> 
<script>        
    $("#reportviewer").ejReportViewer({
        exportProgressChanged : function(args) {
            // Write a code block to perform any action when the export progress changed.
        }
    });
</script>

{% endhighlight %}

### printProgressChanged
{:#events:printprogresschanged}

Fires when the print progress is changed. To perform any operation when the print progress is changed, use the printProgressChanged event.

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
<td class="name">
argument</td>
<td class="type"><span class="param-type">Object</span></td>
<td class="description last">Event parameters from ReportViewer.
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
<td class="name">stage</td>
<td class="type"><span class="param-type">string</span></td>
<td class="description last">returns the stage of export processing.</td>
</tr>
<tr>
<td class="name">currentPage</td>
<td class="type"><span class="param-type">string</span></td>
<td class="description last">returns the currentPage value</td>
</tr>
<tr>
<td class="name">totalPages</td>
<td class="type"><span class="param-type">string</span></td>
<td class="description last">returns the totalPages value</td>
</tr>
<tr>
<td class="name">handled</td>
<td class="type"><span class="param-type">boolean</span></td>
<td class="description last">true if the event should be handled; otherwise, false.</td>
</tr>
<tr>
<td class="name">containerId</td>
<td class="type"><span class="param-type">string</span></td>
<td class="description last">returns ReportViewer container Id.</td>
</tr>
</tbody>
</table>
</td>
</tr>
</tbody>
</table>

#### Example

{% highlight html %}
 
<div id="reportviewer"></div> 
<script>        
    $("#reportviewer").ejReportViewer({
        printProgressChanged : function(args) {
            // Write a code block to perform any action when the print progress changed.
        }
    });
</script>

{% endhighlight %}

### exportItemClick
{:#events:exportitemclick}

Fires when the export items are clicked. To perform any operation when the export items are clicked, use the exportItemClick event.

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
<td class="name">
argument</td>
<td class="type"><span class="param-type">Object</span></td>
<td class="description last">Event parameters from ReportViewer.
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
<td class="name">value</td>
<td class="type"><span class="param-type">string</span></td>
<td class="description last">returns the export format value.</td>
</tr>
</tbody>
</table>
</td>
</tr>
</tbody>
</table>

#### Example

{% highlight html %}
 
<div id="reportviewer"></div> 
<script>        
    $("#reportviewer").ejReportViewer({
        exportItemClick : function(args) {
            // Write a code block to perform any action when the export item clicked.
        }
    });             
</script>

{% endhighlight %}

### toolbarRendering
{:#events:toolbarrendering}

This event will be triggered on rendering the Report Viewer toolbar.

#### Example 

{% highlight js %}

    $("#reportviewer").ejReportViewer({
        toolbarRendering: function(args) {
            // Write your block of code 
        }
    });

{% endhighlight %}

### toolBarItemClick
{:#events:toolbaritemclick}

Fires when the toolbar items are clicked. To perform any operation when the toolbar items are clicked, use the toolBarItemClick event.

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
<td class="name">
argument</td>
<td class="type"><span class="param-type">Object</span></td>
<td class="description last">Event parameters from ReportViewer.
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
<td class="name">target</td>
<td class="type"><span class="param-type">string</span></td>
<td class="description last">returns the toolbar clicked item name .</td>
</tr>
<tr>
<td class="name">cssClass</td>
<td class="type"><span class="param-type">string</span></td>
<td class="description last">returns the CSS class name specified for the toolbar item</td>
</tr>
<tr>
<td class="name">groupIndex</td>
<td class="type"><span class="param-type">string</span></td>
<td class="description last">returns the Toolbar item rendered group index</td>
</tr>
<tr>
<td class="name">Index</td>
<td class="type"><span class="param-type">string</span></td>
<td class="description last">returns the Toolbar item rendered index</td>
</tr>
<tr>
<td class="name">value</td>
<td class="type"><span class="param-type">string</span></td>
<td class="description last">returns the Toolbar item value.</td>
</tr>
</tbody>
</table>
</td>
</tr>
</tbody>
</table>

#### Example

{% highlight html %}
 
<div id="reportviewer"></div> 
<script>        
    $("#reportviewer").ejReportViewer({
        toolBarItemClick : function(args) {
            // Write a code block to perform any action when the toolbar item clicked.
        }
    });             
</script>

{% endhighlight %}

### hyperlink
{:#events:hyperlink}

Fires when the hyperlink action is performed in the report. To perform any operation during the hyperlink action, use the hyperlink event.

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
<td class="name">argument</td>
<td class="type"><span class="param-type">Object</span></td>
<td class="description last">Event parameters from ReportViewer.
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
<td class="name">cancel</td>
<td class="type"><span class="param-type">boolean</span></td>
<td class="description last">true if the event should be canceled; otherwise, false.</td>
</tr>
<tr>
<td class="name">actionInfo</td>
<td class="type"><span class="param-type">Object</span></td>
<td class="description last">returns the actionInfo's hyperLink detail</td>
</tr>
<tr>
<td class="name">model</td>
<td class="type"><span class="param-type">object</span></td>
<td class="description last">returns the report model.</td>
</tr>
<tr>
<td class="name">type</td>
<td class="type"><span class="param-type">string</span></td>
<td class="description last">returns the name of the event.</td>
</tr>
</tbody>
</table>
</td>
</tr>
</tbody>
</table>

#### Example

{% highlight html %}
 
<div id="reportviewer"></div> 
<script>        
    $("#reportviewer").ejReportViewer({ 
        hyperlink: function (args) {
            // Write a code block to perform any operation when hyperlink action occurs in report.
        }
    });
</script>

{% endhighlight %}

### reportPrint
{:#events:reportprint}

Fires when the report print action is performed in the report. To perform any operation during the report print action, use the ReportPrint event.

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
<td class="name">
argument</td>
<td class="type"><span class="param-type">Object</span></td>
<td class="description last">Event parameters from reportviewer.
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
<td class="name">isStyleLoad</td>
<td class="type"><span class="param-type">boolean</span></td>
<td class="description last">true if you have to load the external style file; otherwise, false.</td>
</tr>
</tbody>
</table>
</td>
</tr>
</tbody>
</table>

#### Example

{% highlight html %}
 
<div id="reportviewer"></div> 
<script>        
    $("#reportviewer").ejReportViewer({
        reportPrint : function(args) {
            // Write a code block to perform any action when the export item clicked.
        }
    });             
</script>

{% endhighlight %}

### ajaxBeforeLoad
{:#events:ajaxbeforeload}

Fires before the ajax request process started.

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
<td class="name">argument</td>
<td class="type"><span class="param-type">Object</span></td>
<td class="description last">Event ajax process from reportviewer.
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
<td class="name">reportViewerToken</td>
<td class="type"><span class="param-type">string</span></td>
<td class="description last">returns the reportViewerToken.</td>
</tr>
<tr>
<td class="name">serviceAuthorizationToken</td>
<td class="type"><span class="param-type">string</span></td>
<td class="description last">returns the serviceAuthorizationToken.</td>
</tr>
<tr>
<td class="name">headerReq</td>
<td class="type"><span class="param-type">Object</span></td>
<td class="description last">Send the headerReq collection.</td>
</tr>
<tr>
<td class="name">headers</td>
<td class="type"><span class="param-type">Object</span></td>
<td class="description last">Send the headers collection.</td>
</tr>
<tr>
<td class="name">data</td>
<td class="type"><span class="param-type">string</span></td>
<td class="description last">Send the custom data.</td>
</tr>
</tbody>
</table>
</td>
</tr>
</tbody>
</table>

#### Example

{% highlight html %}
 
<div id="reportviewer"></div> 
<script>        
    $("#reportviewer").ejReportViewer({ 
        ajaxBeforeLoad:  function (args) {
            // Write a code block to perform any operation after destroy of reportviewer.
        }
    });           
</script>

{% endhighlight %}

### ajaxSuccess
{:#events:ajaxsuccess}

Fires when ajax post call succeed.

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
<td class="name">argument</td>
<td class="type"><span class="param-type">Object</span></td>
<td class="description last">Event ajax process from reportviewer.
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
<td class="name">data</td>
<td class="type"><span class="param-type">object</span></td>
<td class="description last">returns the success data.</td>
</tr>
</tbody>
</table>
</td>
</tr>
</tbody>
</table>

#### Example

{% highlight html %}
 
<div id="reportviewer"></div> 
<script>        
    $("#reportviewer").ejReportViewer({ 
        ajaxSuccess:  function (args) {
            // Write a code block to perform any operation after destroy of reportviewer.
        }
    });           
</script>

{% endhighlight %}

### ajaxError
{:#events:ajaxerror}

Fires when ajax request failed.

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
<td class="name">argument</td>
<td class="type"><span class="param-type">Object</span></td>
<td class="description last">Event ajax process from reportviewer.
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
<td class="name">msg</td>
<td class="type"><span class="param-type">string</span></td>
<td class="description last">returns the error details</td>
</tr>
</tbody>
</table>
</td>
</tr>
</tbody>
</table>

#### Example

{% highlight html %}
 
<div id="reportviewer"></div> 
<script>        
    $("#reportviewer").ejReportViewer({ 
        ajaxError:  function (args) {
            // Write a code block to perform any operation after destroy of reportviewer.
        }
    });           
</script>

{% endhighlight %}

### parameterUpdateStateChange
{:#events:parameterupdatestatechange}

Fires when the dependent parameter value is changing in the parameter block. You can add custom user interface, loading indicator and modify the default progress text, using the ParameterUpdateStateChange event.

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
<td class="name">
argument</td>
<td class="type"><span class="param-type">Object</span></td>
<td class="description last">Event parameters from ReportViewer.
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
<td class="name">cancel</td>
<td class="type"><span class="param-type">boolean</span></td>
<td class="description last">true if the event should be canceled; otherwise, false.</td>
</tr>
<tr>
<td class="name">handled</td>
<td class="type"><span class="param-type">boolean</span></td>
<td class="description last">true, if the event handled by user; otherwise, false.</td>
</tr>
<tr>
<td class="name">state</td>
<td class="type"><span class="param-type">string</span></td>
<td class="description last">The processing state.</td>
</tr>
<tr>
<td class="name">model</td>
<td class="type"><span class="param-type">object</span></td>
<td class="description last">returns the report model</td>
</tr>
<tr>
<td class="name">containerId</td>
<td class="type"><span class="param-type">string</span></td>
<td class="description last">The parameter block id.</td>
</tr>
<tr>
<td class="name">name</td>
<td class="type"><span class="param-type">string</span></td>
<td class="description last">Its only to notify the the current parameter.</td>
</tr>
<tr>
<td class="name">prompt</td>
<td class="type"><span class="param-type">string</span></td>
<td class="description last">Its only to notify the current parameter prompt value.</td>
</tr>
<tr>
<td class="name">progressText</td>
<td class="type"><span class="param-type">string</span></td>
<td class="description last">The progress text that is displayed on the loading indicator.</td>
</tr>
</tbody>
</table>
</td>
</tr>
</tbody>
</table>

#### Example

{% highlight html %}

<div id="reportviewer"></div> 
<script>
    $("#reportviewer").ejReportViewer({
        parameterUpdateStateChange : function(args) {
            // Write a code block to perform any action when the parameter update state change.
        }
    });
</script>

{% endhighlight %}