---
layout: post
title: Properties, Methods and Events of ejHeatMap Widget
description: API reference for ejHeatMap
documentation: API
platform: js-api
keywords: heatmap, ejHeatMap, heatmap api, syncfusion
---

#ejHeatMap
<ts root="datavisualization" />

Essential HeatMap JS represents tabular data values as gradient colors instead of numbers,low and high values are different colors with different gradients.

#### Syntax

  $(element).ejHeatMap();

#### Example

{% highlight html %}
 
    <div id="heatmap"></div>
    <script>
        $("#heatmap").ejHeatMap({});
    </script>

{% endhighlight %}

#### Requires

* module:ej.heatmap.base.js
* module:ej.heatmap.js
* module:ej.core.js
* module:ej.data.js   
* module:ej.globalize.js
* module:ej.touch.js  
* module:ej.scroller.js  


## Members


### width `object`
{:#members:width}

Specifies the width of the heat map.

#### Default Value:

* null

#### Example

{% highlight html %}

    <div id="heatmap"></div>
    <script>
        $("#heatmap").ejHeatMap({
            width: "300"
        });
    </script>

{% endhighlight %}




### height `object`
{:#members:height}

Specifies the width of the heat map.

#### Default Value:

* null

#### Example

{% highlight html %}

    <div id="heatmap"></div>
    <script>
        $("#heatmap").ejHeatMap({
            height: "300"
        });
    </script>

{% endhighlight %}



### id `number`
{:#members:height}

Specifies the name of the heat map.

#### Default Value:

* null

#### Example

{% highlight html %}

    <div id="heatmap"></div>
    <script>
        $("#heatmap").ejHeatMap({
            id: "heatmap"
        });
    </script>

{% endhighlight %}

### showTooltip `boolean`
{:#members:showtooltip}

Enables or disables tooltip of heatmap

#### Default Value:

* true

#### Example

{% highlight html %}

 <div id="heatmap"></div>
    <script>
        $("#heatmap").ejHeatMap({
            showtooltip: true
        });
    </script>

{% endhighlight %}


### toolTipSettings `object`
{:#members:tooltipsettings}

Defines the tooltip that should be shown when the mouse hovers over rows/columns.

#### Default Value:

* null

#### Example

{% highlight js %}

$("#heatmap").ejHeatMap({
    //Defines mouse over tooltip
    toolTipSettings: {
        templateId:"mouseovertoolTipId",
         }
    });
            
{% endhighlight %}

### toolTipSettings.templateId `string`
{:#members:tooltipsettings-templateid}

Defines the tooltip that should be shown when the mouse hovers over rows/columns.

#### Default Value:

* null

#### Example
{% highlight html %}
 <script type="text/x-jsrender" id="mouseovertoolTipId">
        <div class="tooltip-style">
            Custom Tooltip
            <div style="height:0px;width:100%;border:1px solid white;">
            </div>
            <table>
                <tr>
                    <td style="width:50px;">Year  </td>
                    <td>{{:data.Year}}</td>
                </tr>
            </table>
        </div>
    </script>
{% endhighlight %}

{% highlight js %}

$("#heatmap").ejHeatMap({
    //Defines mouse over tooltip
    toolTipSettings: {
        templateId:"mouseovertoolTipId"
         }
    });
            
{% endhighlight %}

### toolTipSettings.associate `enum`
{:#members:tooltipsettings-associate}

<ts name = "ej.datavisualization.HeatMap.Associate"/>

Defines the tooltip of associate that should be shown when the mouse hovers over rows/columns.

<table class="props">
    <thead>
        <tr>
            <th>Name</th>
            <th>Description</th>
       </tr>
   </thead>
    <tbody>
        <tr>
            <td class="name">Target</td>
            <td class="description last">Used to set the associate of tooltip as target</td>
       </tr>
        <tr>
            <td class="name">mouseFollow</td>
            <td class="description last">Used to set the associate of tooltip as mousefollow</td>
       </tr>
        <tr>
            <td class="name">MouseEnter</td>
            <td class="description last">Used to set the associate of tooltip as Mouseenter</td>
       </tr>
    </tbody>
</table>
#### Default Value:

* mouseFollow

#### Example

{% highlight js %}

$("#heatmap").ejHeatMap({
    //Defines mouse over tooltip
    toolTipSettings: {
        templateId:"mouseovertoolTipId",
        associate:"mouseFollow"}
    });
            
{% endhighlight %}

### toolTipSettings.isBalloon `boolean`
{:#members:tooltipsettings-isballoon}

Enables/ disables the balloon for the tooltip to be shown

#### Default Value:

* true

#### Example

{% highlight js %}

$("#heatmap").ejHeatMap({
    //Defines mouse over tooltip
    toolTipSettings: {
        templateId:"mouseovertoolTipId",
        isBalloon:true}
    });
            
{% endhighlight %}

### toolTipSettings.position `object`
{:#members:tooltipsettings-position}

Defines the tooltip of position that should be shown when the mouse hovers over rows/columns.

### toolTipSettings.position.stem `enum`
{:#members:tooltipsettings-position-stem}

<ts name = "ej.datavisualization.HeatMap.position"/>

Defines the horizontal position of tooltip.

<table class="props">
    <thead>
        <tr>
            <th>Name</th>
            <th>Description</th>
       </tr>
   </thead>
    <tbody>
        <tr>
            <td class="name">Left</td>
            <td class="description last">Used to display the tooltip horizontally on left side of rows/columns</td>
       </tr>
        <tr>
            <td class="name">Center</td>
            <td class="description last">Used to display the tooltip horizontally on center side of rows/columns</td>
       </tr>
        <tr>
            <td class="name">Right</td>
            <td class="description last">Used to display the tooltip horizontally on right side of rows/columnsr</td>
       </tr>
     </tbody>

#### Default Value:

* left

#### Example

{% highlight js %}

$("#heatmap").ejHeatMap({
    //Defines mouse over tooltip
    toolTipSettings: {
        templateId:"mouseovertoolTipId",
        associate:"mouseFollow",
        position: {
            stem: { horizontal: "left" }
            };
         }
    });
            
{% endhighlight %}

### toolTipSettings.position.target `enum`
{:#members:tooltipsettings-position-target}

<ts name = "ej.datavisualization.HeatMap.position"/>

Defines the vertical position of tooltip.

 <table class="props">
    <thead>
        <tr>
            <th>Name</th>
            <th>Description</th>
       </tr>
   </thead>
    <tbody>
        <tr>
            <td class="name">Top</td>
            <td class="description last">Used to display the tooltip vertically on top side of rows/columns</td>
       </tr>
        <tr>
            <td class="name">Middle</td>
            <td class="description last">Used to display the tooltip vertically on middle side of rows/columns</td>
       </tr>
        <tr>
            <td class="name">Bottom</td>
            <td class="description last">Used to display the tooltip vertically on bottom side of rows/columnsr</td>
       </tr>
     </tbody>

#### Default Value:

* Middle

#### Example

{% highlight js %}

$("#heatmap").ejHeatMap({
    //Defines mouse over tooltip
    toolTipSettings: {
        templateId:"mouseovertoolTipId",
        associate:"mouseFollow",
        position: {
            target: { vertical: "top" }
            };
         }
    });
            
{% endhighlight %}

### toolTipSettings.trigger `enum`
{:#members:tooltipsettings-trigger}

Defines the tooltip to be triggerred.

<table class="props">
    <thead>
        <tr>
            <th>Name</th>
            <th>Description</th>
       </tr>
   </thead>
    <tbody>
        <tr>
            <td class="name">hover</td>
            <td class="description last">Tooltip can be triggered on mouse hovers</td>
       </tr>
        <tr>
            <td class="name">click</td>
            <td class="description last">Tooltip can be triggered on mouse click</td>
       </tr>
        <tr>
            <td class="name">focus</td>
            <td class="description last">Tooltip can be triggered on mouse focus</td>
       </tr>
    </tbody>
</table>

#### Default Value:

* hover

#### Example

{% highlight js %}

$("#heatmap").ejHeatMap({
    //Defines mouse over tooltip
    toolTipSettings: {
        trigger:"click",
         }
    });
            
{% endhighlight %}
animation: {
                    effect: "none",
                    speed: 0
                },

### toolTipSettings.animation `object`
{:#members:tooltipsettings-animation}

Defines the animation for the tooltip that should be shown when the mouse hovers over rows/columns.

#### Default Value:

* null

#### Example

{% highlight js %}

$("#heatmap").ejHeatMap({
    //Defines mouse over tooltip
    toolTipSettings: {
        animation:"click",
         }
    });
            
{% endhighlight %}

### toolTipSettings.animation.effect `string`
{:#members:tooltipsettings-animation-effect}

Defines the animation effect for the tooltip that should be shown when the mouse hovers over rows/columns.

#### Default Value:

* none

#### Example

{% highlight js %}

$("#heatmap").ejHeatMap({
    //Defines mouse over tooltip
    toolTipSettings: {
        animation:{effect:"none"}
         }
    });
            
{% endhighlight %}

### toolTipSettings.animation.speed `string`
{:#members:tooltipsettings-animation-speed}

Defines the animation speed for the tooltip that should be shown when the mouse hovers over rows/columns.

#### Default Value:

* 0

#### Example

{% highlight js %}

$("#heatmap").ejHeatMap({
    //Defines mouse over tooltip
    toolTipSettings: {
        animation:{effect:"none", speed:0}
         }
    });
            
{% endhighlight %}

### itemsSource `object`
{:#members:itemsSource}

Specifies the source data of the heat map.

#### Default Value:

* []

#### Example

{% highlight html %}

    <div id="heatmap"></div>
    <script>

        var columns = ["Vegie-spread", "Tofuaa", "Alice Mutton", "Konbu", "Flytemysost"]
        var itemSource = [];
        for (var i = 0; i < columns.length; i++) {
            for (var j = 0; j < 6; j++) {
                var value = Math.floor((Math.random() * 100) + 1);
                itemSource.push({ ProductName: columns[i], Year: "Y" + (2011 + j), Value: value })
            }
        }
        $("#heatmap").ejHeatMap({
            itemsSource: itemSource
        });
    </script>

{% endhighlight %}

### heatMapCell `object`
{:#members:heatmapCell}

Specifies the property of the heat map cell.

#### Default Value:

* Null

#### Example

{% highlight html %}

    <div id="heatmap"></div>
    <script>
        $("#heatmap").ejHeatMap({
            heatmapCell: { showColor: true }
        });
    </script>

{% endhighlight %}


### heatMapCell.showContent `enum`
{:#members:heatmapCell-showContent}
 
<ts name = "ej.datavisualization.HeatMap.CellVisibility"/>

Specifies whether the cell content can be visible or not.

<table class="props">
   <thead>
        <tr>
            <th>Name</th>
            <th>Description</th>
       </tr>
   </thead>
   <tbody>
        <tr>
            <td class="name">Visible</td>
            <td class="description last">Display the content of the cell  
            </td>
       </tr>
        <tr>
            <td class="name">Hidden</td>
            <td class="description last">Hide the content of the cell  </td>
       </tr>
   </tbody>
</table>

#### Default Value:

* ej.HeatMap.CellVisibility.Visible

#### Example

{% highlight html %} 

    <div id="heatmap"></div>
    <script>
        $("#heatmap").ejHeatMap({
            heatmapCell: { showContent: ej.HeatMap.CellVisibility.Hidden }
        });
    </script>

{% endhighlight %}


### heatMapCell.showColor `boolean`
{:#members:heatmapCell-showColor}

Specifies whether the cell color can be visible or not.

#### Default Value:

* true

#### Example

{% highlight html %}

    <div id="heatmap"></div>
    <script>
        $("#heatmap").ejHeatMap({
            heatmapCell: { showColor: true }
        });
    </script>

{% endhighlight %}




### isResponsive `boolean`
{:#members:isResponsive}

Specifies can enable responsive mode or not for heat map.

#### Default Value:

* false

#### Example

{% highlight html %}

    <div id="heatmap"></div>
    <script>
        $("#heatmap").ejHeatMap({
            isResponsive: true
        });
    </script>

{% endhighlight %}


### enableVirtualization `boolean`
{:#members:enableVirtualization}

Specifies whether the virtualization can be enable or not.

#### Default Value:

* false

#### Example

{% highlight html %}

    <div id="heatmap"></div>
    <script>
        $("#heatmap").ejHeatMap({
            enableVirtualization: true
        });
    </script>

{% endhighlight %}

 

### defaultColumnStyle `object`
{:#members:defaultColumnStyle}

Specifies the default column properties for all the column style not specified in column properties. 

#### Default Value:

* []

#### Example

{% highlight html %}

    <div id="heatmap"></div>
    <script>
        $("#heatmap").ejHeatMap({
            defaultColumnStyle: {
                textAlign: ej.HeatMap.TextAlign.Left
            }
        });
    </script>

 
{% endhighlight %}

### defaultColumnStyle.textAlign `object`
{:#members:defaultColumnStyle-textAlign}

Specifies the alignment mode of the heat map column.

<ts name = "ej.datavisualization.HeatMap.TextAlign"/>

Enables/disables the bold style

<table class="props">
   <thead>
        <tr>
            <th>Name</th>
            <th>Description</th>
       </tr>
   </thead>
   <tbody>
        <tr>
            <td class="name">Right</td>
            <td class="description last">SAlign right to the heat map cell.
            </td>
       </tr>
        <tr>
            <td class="name">Left</td>
            <td class="description last">Align left to the heat map cell.  </td>
       </tr>
       <tr>
            <td class="name">Center</td>
            <td class="description last">Align center to the heat map cell. </td>
       </tr>
   </tbody>
</table>

#### Default Value:

* ej.HeatMap.TextAlign.Center

#### Example

{% highlight html %} 

    <div id="heatmap"></div>
    <script>
        $("#heatmap").ejHeatMap({
            defaultColumnStyle: {
                textAlign: ej.HeatMap.TextAlign.Left
            }
        });
    </script>


{% endhighlight %}


### defaultColumnStyle.headerTemplateID`string`
{:#members:defaultColumnStyle-headerTemplateID}

Specifies the template id of the heat map column header.

#### Default Value:

* ""

#### Example

{% highlight html %}

    <div id="heatmap"></div>
    <script>
        $("#heatmap").ejHeatMap({
            defaultColumnStyle: {
                headerTemplateID: "columnTemplate"
            }
        });
    </script>
    <script type="text/x-jsrender" id="columnTemplate">
        <img style="width: 45px; height: 40px" src="2.jpg" alt="{{: ProductName }}" />
        <span>{{: ProductName }}</span>
    </script>

{% endhighlight %}


### defaultColumnStyle.templateID`string`
{:#members:defaultColumnStyle-templateID}

Specifies the template id of all individual cell data of the heat map. 

#### Default Value:

* ""

#### Example

{% highlight html %}

    <div id="heatmap"></div>
    <script>
        $("#heatmap").ejHeatMap({
            defaultColumnStyle: {
                templateID: "template"
            }
        });
    </script>
    <script type="text/x-jsrender" id="template">
        <img style="width: 45px; height: 40px" src="2.jpg" alt="{{: ProductName }}" />
        <span>{{: ProductName }}</span>
    </script>

{% endhighlight %}




### legendCollection `array`
{:#members:legendCollection}

Specifies the no of legends can sync with heat map. 

#### Default Value:

* []

#### Example

{% highlight html %}

    <div id="heatmap"></div>
    <script>
        $("#heatmap").ejHeatMap({
            legendCollection: ["heatmap_legend1", "heatmap_legend2"]
        });
    </script>

{% endhighlight %}




### itemsMapping `object`
{:#members:itemsMapping}

Specifies the property and display value of the heat map column.

#### Default Value:

* []

#### Example

{% highlight html %}

    <div id="heatmap"></div>
    <script>
        $("#heatmap").ejHeatMap({
            itemsMapping: {
                column: { "propertyName": "ProductName", "displayName": "Product Name" },
                row: { "propertyName": "Year", "displayName": "Year", }
            }
        });
    </script>
{% endhighlight %}



### itemsMapping.columnStyle `object`
{:#members:itemsMapping-columnStyle}

Column settings for the individual heat map column.

#### Default Value:

* null

#### Example
{% highlight html %}

    <div id="heatmap"></div>
    <script>
        $("#heatmap").ejHeatMap({
            itemsMapping: {
                columnStyle: {
                    textAlign: ej.HeatMap.TextAlign.Left
                }
            }
        });
    </script>

{% endhighlight %}


### itemsMapping.columnStyle.width `number`
{:#members:itemsMapping-columnStyle-width}

Specifies the width of the heat map column.

#### Default Value:

* 0

#### Example

{% highlight html %} 

    <div id="heatmap"></div>
    <script>
        $("#heatmap").ejHeatMap({
            itemsMapping: {
                columnStyle: {
                    width: 100
                }
            }
        });
    </script>

{% endhighlight %}

### itemsMapping.columnStyle.textAlign `string`
{:#members:itemsMapping-columnStyle-textAlign}

Specifies the text align mode of the heat map column.

#### Default Value:

* ej.HeatMap.TextAlign.Center

#### Example

{% highlight html %} 

    <div id="heatmap"></div>
        <script>
            $("#heatmap").ejHeatMap({
                itemsMapping: {
                    columnStyle: {
                        textAlign: ej.HeatMap.TextAlign.Left
                    }
                }
            });
        </script>

{% endhighlight %}

### itemsMapping.columnStyle.headerTemplateID `string`
{:#members:itemsMapping-columnStyle-headerTemplateID}

Specifies the template id of the column header.

#### Default Value:

* ""

#### Example

{% highlight html %} 

    <div id="heatmap"></div>
    <script>
        $("#heatmap").ejHeatMap({
            itemsMapping: {
                columnStyle: {
                    headerTemplateID: "template"
                }
            }
        });
    </script>
    <script type="text/x-jsrender" id="template">
        <img style="width: 45px; height: 40px" src="2.jpg" alt="{{: ProductName }}" />
        <span>{{: ProductName }}</span>
    </script>

{% endhighlight %}

### itemsMapping.columnStyle.templateID `string`
{:#members:itemsMapping-columnStyle-templateID}

Specifies the template id of all individual cell data. 

#### Default Value:

* ""

#### Example

{% highlight html %} 

    <div id="heatmap"></div>
    <script>
        $("#heatmap").ejHeatMap({
            itemsMapping: {
                columnStyle: {
                    templateID: "template"
                }
            }
        });
    </script>
    <script type="text/x-jsrender" id="template">
        <img style="width: 45px; height: 40px" src="2.jpg" alt="{{: ProductName }}" />
        <span>{{: ProductName }}</span>
    </script>

{% endhighlight %}







### itemsMapping.column `object`
{:#members:itemsMapping-column}

Specifies the property and display value of the column.  

#### Default Value:

* null

#### Example

{% highlight html %} 

    <div id="heatmap"></div>
    <script>
        $("#heatmap").ejHeatMap({
            itemsMapping: {
                column: { "propertyName": "ProductName", "displayName": "Product Name" }
            }
        });
    </script>

{% endhighlight %}

### itemsMapping.column.propertyName `string`
{:#members:itemsMapping-column-propertyName}

Specifies the name of the column or row.

#### Default Value:

* ""

#### Example

{% highlight html %} 

    <div id="heatmap"></div>
    <script>
        $("#heatmap").ejHeatMap({
            itemsMapping: {
                column: { "propertyName": "ProductName" }
            }
        });
    </script>

{% endhighlight %}

### itemsMapping.column.displayName `string`
{:#members:itemsMapping-column-displayName}

Specifies the value of the column or row.

#### Default Value:

* ""

#### Example

{% highlight html %} 

    <div id="heatmap"></div>
    <script>
        $("#heatmap").ejHeatMap({
            itemsMapping: {
                column: { "displayName": "Product Name" }
            }
        });
    </script>

{% endhighlight %}






### itemsMapping.row `object`
{:#members:itemsMapping-row}

Specifies the property and display value of the heat map.
row
#### Default Value:

* null

#### Example

{% highlight html %} 

        $("#heatmap").ejHeatMap({
            itemsMapping: {
                row: { "propertyName": "ProductName", "displayName": "Product Name" }
            }
        });

{% endhighlight %}
### itemsMapping.row.propertyName `string`
{:#members:itemsMapping-row-propertyName}

Specifies the name of the column or row.

#### Default Value:

* ""

#### Example

{% highlight html %} 

    <div id="heatmap"></div>
    <script>
        $("#heatmap").ejHeatMap({
            itemsMapping: {
                row: { "propertyName": "ProductName" }
            }
        });
    </script>

{% endhighlight %}

### itemsMapping.row.displayName `string`
{:#members:itemsMapping-row-displayName}

Specifies the value of the column or row.

#### Default Value:

* ""

#### Example

{% highlight html %} 

    <div id="heatmap"></div>
    <script>
        $("#heatmap").ejHeatMap({
            itemsMapping: {
                row: { "displayName": "Product Name" }
            }
        });
    </script>

{% endhighlight %}



### itemsMapping.value `object`
{:#members:itemsMapping-value}

Specifies the property and display value of the column value.

#### Default Value:

* null

#### Example

{% highlight html %} 

    <div id="heatmap"></div>
    <script>
        $("#heatmap").ejHeatMap({
            itemsMapping: {
                value: { "propertyName": "Value" }
            }
        });
    </script>

{% endhighlight %}

### itemsMapping.value.propertyName `string`
{:#members:itemsMapping-value-propertyName}

Specifies the name of the column or row.

#### Default Value:

* ""

#### Example

{% highlight html %} 

    <div id="heatmap"></div>
    <script>
        $("#heatmap").ejHeatMap({
            itemsMapping: {
                value: { "propertyName": "ProductName" }
            }
        });
    </script>

{% endhighlight %}

### itemsMapping.value.displayName `string`
{:#members:itemsMapping-value-displayName}

Specifies the value of the column or row.

#### Default Value:

* ""

#### Example

{% highlight html %} 

    <div id="heatmap"></div>
    <script>
        $("#heatmap").ejHeatMap({
            itemsMapping: {
                value: { "displayName": "Product Name" }
            }
        });
    </script>

{% endhighlight %}



### itemsMapping.headerMapping `object`
{:#members:itemsMapping-headerMapping}

Specifies the property and display value of the header.

#### Default Value:

* null

#### Example

{% highlight html %} 

    <div id="heatmap"></div>
    <script>
        $("#heatmap").ejHeatMap({
            itemsMapping: {
                headerMapping: { "propertyName": "Year", "displayName": "Year" }
            }
        });
    </script>

{% endhighlight %}
### itemsMapping.headerMapping.propertyName `string`
{:#members:itemsMapping-headerMapping-propertyName}

Specifies the name of the column or row. 

#### Default Value:

* ""

#### Example

{% highlight html %} 

    <div id="heatmap"></div>
    <script>
        $("#heatmap").ejHeatMap({
            itemsMapping: {
                headerMapping: { "propertyName": "Year" }
            }
        });
    </script>

{% endhighlight %}

### itemsMapping.headerMapping.displayName `string`
{:#members:itemsMapping-headerMapping-displayName}

Specifies the value of the column or row.

#### Default Value:

* ""

#### Example

{% highlight html %} 

    <div id="heatmap"></div>
    <script>
        $("#heatmap").ejHeatMap({
            itemsMapping: {
                headerMapping: { "displayName": "Year" }
            }
        });
    </script>

{% endhighlight %}
### itemsMapping.headerMapping.columnStyle `object`
{:#members:itemsMapping-headerMapping-columnStyle}

Specifies the property and display value of the header. 

#### Default Value:

* null

#### Example

{% highlight html %} 

    <div id="heatmap"></div>
    <script>
        $("#heatmap").ejHeatMap({
            itemsMapping: {
                headerMapping: {
                    "columnStyle": { width: 105, textAlign: "right" }
                }
            }
        });
    </script>

{% endhighlight %} 

### itemsMapping.columnMapping `array`
{:#members:itemsMapping-columnMapping}

Specifies the property and display value of the collection of column. 

#### Default Value:

* []

#### Example

{% highlight html %} 

    <div id="heatmap"></div>
    <script>
        $("#heatmap").ejHeatMap({
            itemsMapping: {
                columnMapping: [
                   { "propertyName": "property name1", "displayName": "display name1" },
                   { "propertyName": "property name2", "displayName": "display name2" }
                ]
            }
        });
    </script>

{% endhighlight %}
 

### colorMappingCollection `array`
{:#members:colorMappingCollection}

Specifies the color values of the heat map column data.

#### Default Value:

* []

#### Example

{% highlight html %}

    <div id="heatmap"></div>
    <script>
        $("#heatmap").ejHeatMap({
            colorMappingCollection: [
            { value: 0, color: "#8ec8f8", label: { text: "0" } },
            { value: 100, color: "#0d47a1", label: { text: "100" } }
            ]
        });
    </script>

{% endhighlight %}

### colorMappingCollection.color`string`
{:#members:colorMappingCollection-color}

Specifies the color of the heat map column data. 

#### Default Value:

* "white"

#### Example

{% highlight html %}

    <div id="heatmap"></div>
    <script>
        $("#heatmap").ejHeatMap({
            colorMappingCollection: [
            { value: 0, color: "#8ec8f8", label: { text: "0" } },
            { value: 100, color: "#0d47a1", label: { text: "100" } }
            ]
        });
    </script>

{% endhighlight %}

### colorMappingCollection.value `number`
{:#members:colorMappingCollection-value}

Specifies the color values of the heat map column data. 

#### Default Value:

* 0

#### Example

{% highlight html %}

    <div id="heatmap"></div>
    <script>
        $("#heatmap").ejHeatMap({
            colorMappingCollection: [
            { value: 0, color: "#8ec8f8", label: { text: "0" } },
            { value: 100, color: "#0d47a1", label: { text: "100" } }
            ]
        });
    </script>

{% endhighlight %}

### colorMappingCollection.label `object`
{:#members:colorMappingCollection-label}

Specifies the label properties of the heat map color.

#### Default Value:

* null

#### Example

{% highlight html %}

    <div id="heatmap"></div>
    <script>
        $("#heatmap").ejHeatMap({
            colorMappingCollection: [
                { label: { bold: true } }
            ]
        });
    </script>
{% endhighlight %}

### colorMappingCollection.label.bold `boolean`
{:#members:colorMappingCollection-label-bold}

Enables/disables the bold style of the heat map label.

#### Default Value:

* false

#### Example

{% highlight html %}

    <div id="heatmap"></div>
    <script>
        $("#heatmap").ejHeatMap({
            colorMappingCollection: [
                { label: { bold: true } }
            ]
        });
    </script>

{% endhighlight %}

### colorMappingCollection.label.italic `boolean`
{:#members:colorMappingCollection-label-italic}

Enables/disables the italic style of the heat map label.

#### Default Value:

* false

#### Example
{% highlight html %}

    <div id="heatmap"></div>
    <script>
        $("#heatmap").ejHeatMap({
            colorMappingCollection: [
                { label: { italic: true } }
            ]
        });
    </script>

{% endhighlight %}

### colorMappingCollection.label.text`string`
{:#members:colorMappingCollection-label-text}

specifies the text value of the heat map label.

#### Default Value:

* ""

#### Example

{% highlight html %}

    <div id="heatmap"></div>
    <script>
        $("#heatmap").ejHeatMap({
            colorMappingCollection: [
                { label: { text: "10" } }
            ]
        });
    </script>

{% endhighlight %}

### colorMappingCollection.label.textDecoration `enum`
{:#members:colorMappingCollection-label-textDecoration}

<ts name = "ej.datavisualization.HeatMap.TextDecoration "/>

Specifies the text style of the heat map label.

<table class="props">
   <thead>
        <tr>
            <th>Name</th>
            <th>Description</th>
       </tr>
   </thead>
   <tbody>
        <tr>
            <td class="name">Underline</td>
            <td class="description last">Defines a line below the text
            </td>
       </tr>
        <tr>
            <td class="name">Overline</td>
            <td class="description last">Defines a line above the text</td>
       </tr>
        <tr>
            <td class="name">LineThrough</td>
            <td class="description last">Defines a line through the text</td>
       </tr>
        <tr>
            <td class="name">None</td>
            <td class="description last">Defines a normal text. This is default</td>
       </tr>
   </tbody>
</table>

#### Default Value:

* ej.HeatMap.TextDecoration.None

#### Example

{% highlight html %}

    <div id="heatmap"></div>
    <script>
        $("#heatmap").ejHeatMap({
            colorMappingCollection: [
                { label: { textDecoration: ej.HeatMap.TextDecoration.None } }
            ]
        });
    </script>

{% endhighlight %}

### colorMappingCollection.label.fontSize `number`
{:#members:colorMappingCollection-label-fontSize}

Specifies the font size of the heat map label.

#### Default Value:

* 10

#### Example

{% highlight html %}

    <div id="heatmap"></div>
    <script>
        $("#heatmap").ejHeatMap({
            colorMappingCollection: [
                { label: { fontSize: 18 } }
            ]
        });
    </script>

{% endhighlight %}

### colorMappingCollection.label.fontFamily`string`
{:#members:colorMappingCollection-label-fontFamily}

Specifies the font family of the heat map label.

#### Default Value:

* "Arial"

#### Example

{% highlight html %}

    <div id="heatmap"></div>
    <script>
        $("#heatmap").ejHeatMap({
            colorMappingCollection: [
                { label: { fontFamily: "Arial" } }
            ]
        });
    </script>

{% endhighlight %}

### colorMappingCollection.label.fontColor`string`
{:#members:colorMappingCollection-label-fontColor}

Specifies the font color of the heat map label.

#### Default Value:

* "black"

#### Example

{% highlight html %}

    <div id="heatmap"></div>
    <script>
        $("#heatmap").ejHeatMap({
            colorMappingCollection: [
                { label: { fontColor: "red" } }
            ]
        });
    </script>

{% endhighlight %}


## Events

### cellMouseOver
{:#events:cellmouseover}

Triggered when the mouse over on the cell. 

<table class="params">
	<thead>
		<tr>
			<th>Name</th>
			<th>Type</th>
			<th>Description</th>
		</tr>
	</thead>
	<tbody>
		<tr>
			<td class="name">cellValue</td>
			<td class="type">string</td>
			<td class="description last">Value displayed on the cell</td>
		</tr>
		<tr>
			<td class="name">source</td>
			<td class="type">object</td>
			<td class="description last">Returns the HeatMap cell data</td>
		</tr>
		<tr>
			<td class="name">cell</td>
			<td class="type">object</td>
			<td class="description last">Returns the specific HeatMap cell</td>
		</tr>
	</tbody>
</table>

#### Example

{% highlight javascript %}

// cellMouseOver event for HeatMap
$("#heatmapcontent").ejHeatMap({
    cellMouseOver: function(args) {}
});

{% endhighlight %}

### cellMouseEnter
{:#events:cellmouseenter}

Triggered when the mouse over on the cell. 

<table class="params">
	<thead>
		<tr>
			<th>Name</th>
			<th>Type</th>
			<th>Description</th>
		</tr>
	</thead>
	<tbody>
		<tr>
			<td class="name">cellValue</td>
			<td class="type">string</td>
			<td class="description last">Value displayed on the cell</td>
		</tr>
		<tr>
			<td class="name">source</td>
			<td class="type">object</td>
			<td class="description last">Returns the HeatMap cell data</td>
		</tr>
		<tr>
			<td class="name">cell</td>
			<td class="type">object</td>
			<td class="description last">Returns the specific HeatMap cell</td>
		</tr>
	</tbody>
</table>

#### Example

{% highlight javascript %}

// cellMouseEnter event for HeatMap
$("#heatmapcontent").ejHeatMap({
    cellMouseEnter: function(args) {}
});

{% endhighlight %}

### cellMouseLeave
{:#events:cellmouseleave}

Triggered when the mouse over on the cell. 

<table class="params">
	<thead>
		<tr>
			<th>Name</th>
			<th>Type</th>
			<th>Description</th>
		</tr>
	</thead>
	<tbody>
		<tr>
			<td class="name">cellValue</td>
			<td class="type">string</td>
			<td class="description last">Value displayed on the cell</td>
		</tr>
		<tr>
			<td class="name">source</td>
			<td class="type">object</td>
			<td class="description last">Returns the HeatMap cell data</td>
		</tr>
		<tr>
			<td class="name">cell</td>
			<td class="type">object</td>
			<td class="description last">Returns the specific HeatMap cell</td>
		</tr>
	</tbody>
</table>

#### Example

{% highlight javascript %}

// cellMouseLeave event for HeatMap
$("#heatmapcontent").ejHeatMap({
    cellMouseLeave: function(args) {}
});

{% endhighlight %}

### cellSelected
{:#events:cellselected}

Triggered when the mouse over on the cell. 

<table class="params">
	<thead>
		<tr>
			<th>Name</th>
			<th>Type</th>
			<th>Description</th>
		</tr>
	</thead>
	<tbody>
		<tr>
			<td class="name">cellValue</td>
			<td class="type">string</td>
			<td class="description last">Value displayed on the cell</td>
		</tr>
		<tr>
			<td class="name">source</td>
			<td class="type">object</td>
			<td class="description last">Returns the HeatMap cell data</td>
		</tr>
		<tr>
			<td class="name">cell</td>
			<td class="type">object</td>
			<td class="description last">Returns the specific HeatMap cell</td>
		</tr>
	</tbody>
</table>

#### Example

{% highlight javascript %}

// cellSelected event for HeatMap
$("#heatmapcontent").ejHeatMap({
    cellSelected: function(args) {}
});

{% endhighlight %}