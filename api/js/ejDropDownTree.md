---
layout: post
title: Properties, Methods and Events of ejDropDownTree Widget
description: API reference for ejDropDownTree
documentation: API
platform: js-api
keywords: DropDownTree, ejDropDownTree, syncfusion, DropDownTree api
---

# ejDropDownTree


The DropDownTree control provides a list of hierarchical data to choose an item from the list.
It can including other HTML elements such as images, textboxes, check box, radio buttons, and so on.


#### Syntax

{% highlight javascript %}

$('#selectItem').ejDropDownTree();

{% endhighlight %}

#### Example

{% highlight html %}
<input type="text" id="selectItem" />

<div id="itemList">
   <ul id="treeView">
      <li class="expanded">
         United States
         <ul>
            <li>California</li>
            <li>Colorado</li>
            <li>Georgia</li>
         </ul>
      </li>
      <li>
         United Kingdom
         <ul>
            <li>England</li>
            <li>Scotland</li>
            <li>Northern Ireland</li>
         </ul>
      </li>
      <li>
         Asia
         <ul>
            <li>Afghanistan</li>
            <li>Kuwait</li>
            <li>Russia</li>
         </ul>
      </li>
   </ul>
</div>

<script type="text/javascript">
$('#selectItem').ejDropDownTree({
                showPopupOnLoad: true,
                watermarkText: "Please select",
                width: "100%",
                targetId: "itemList"
            });
</script>

{% endhighlight %}

#### Requires


* module:jQuery

* module:jQuery.easing.1.3.js

* module:ej.core.js

* module:ej.data.js

* module:ej.dropdowntree.js

* module:ej.waitingpopup.js

* module:ej.combobox.js

* module:ej.checkbox.js

* module:ej.scroller.js

## Members

### allowKeyboardNavigation  `boolean`
{:#members:allowkeyboardnavigation }

Uses the keyboard for any action, including opening and closing the drop-down tree; navigating, expanding, and collapsing nodes of the dropdown tree; and more.

####  Default Value

* true

#### Example

{% highlight html %}

<input type="text" id="itemList" />

<script type="text/javascript">
        var localData = [
                    { id: 1, name: "Windows Team", hasChild: true, expanded: true },
                    { id: 2, pid: 1, name: "Clark" },
                    { id: 3, pid: 1, name: "Wright" },
                    { id: 4, pid: 1, name: "Lopez" },
                    { id: 7, name: "Web Team", hasChild: true, expanded: true },
                    { id: 8, pid: 7, name: "Joshua" },
                    { id: 9, pid: 7, name: "Matthew" },
                    { id: 10, pid: 7, name: "David" },
                    { id: 11, name: "Build Team", hasChild: true },
                    { id: 12, pid: 11, name: "Ryan" },
                    { id: 13, pid: 11, name: "Justin" },
                    { id: 14, pid: 11, name: "Robert" }];
        $(function () {
            $('#itemList').ejDropDownTree({
                treeViewSettings: {
                    fields: { id: "id", parentId: "pid", value: "id", text: "name", hasChild: "hasChild", dataSource: localData, expanded: "expanded" }
                },
                allowKeyboardNavigation: false
            });
        });
    </script>

{% endhighlight %}

### cssClass  `string`
{:#members:cssclass}

Sets the root CSS class for DropDownTree that allows customization of appearance.

#### Default Value

* ``

#### Example

{% highlight html %}
<input type="text" id="itemList" />
    <script type="text/javascript">
        var localData = [
                   { id: 1, name: "Discover Music", hasChild: true, expanded: true },
                   { id: 2, pid: 1, name: "Hot Singles" },
                   { id: 3, pid: 1, name: "Rising Artists" },
                   { id: 4, pid: 1, name: "Live Music" },
                   { id: 6, pid: 1, name: "Best of 2013 So Far" },
                   { id: 7, name: "Sales and Events", hasChild: true, expanded: true },
                   { id: 8, pid: 7, name: "100 Albums - $5 Each" },
                   { id: 9, pid: 7, name: "Hip-Hop and R&B Sale" },
                   { id: 10, pid: 7, name: "CD Deals" },
                   { id: 11, name: "Categories", hasChild: true },
                   { id: 12, pid: 11, name: "Songs" },
                   { id: 13, pid: 11, name: "Bestselling Albums" },
                   { id: 14, pid: 11, name: "New Releases" },
                   { id: 15, pid: 11, name: "Bestselling Songs" },
                   { id: 16, name: "MP3 Albums", hasChild: true },
                   { id: 17, pid: 16, name: "Rock" },
                   { id: 18, pid: 16, name: "Gospel" },
                   { id: 19, pid: 16, name: "Latin Music" },
                   { id: 20, pid: 16, name: "Jazz" },
                   { id: 21, name: "More in Music", hasChild: true },
                   { id: 22, pid: 21, name: "Music Trade-In" },
                   { id: 23, pid: 21, name: "Redeem a Gift Card" },
                   { id: 24, pid: 21, name: "Band T-Shirts" },
                   { id: 25, pid: 21, name: "Mobile MVC" }];

    
    $(function () {
        $('#itemList).ejDropDownTreeList({
            fields: { id: "id", parentId: "pid", text: "name", hasChild: "hasChild", dataSource: localData, expanded: "expanded" },
            cssClass: 'gradient-lime'
        });
    });
    </script>

{% endhighlight %}

### delimiter `string`
{:#members:delimiter}

Sets the separator when the multiSelectMode with delimiter option or checkbox is enabled. When you enter the delimiter value, the text after the delimiter is considered as a separate word or query. The delimiter string is a single character and must be a symbol. Mostly, the delimiter symbol is used as comma (,), semi-colon (;), or any other special character.

#### Default Value

* ","

#### Example

{% highlight html %}

<input type="text" id="itemList" />

<script type="text/javascript">
        var localData = [
                    { id: 1, name: "Windows Team", hasChild: true, expanded: true },
                    { id: 2, pid: 1, name: "Clark" },
                    { id: 3, pid: 1, name: "Wright" },
                    { id: 4, pid: 1, name: "Lopez" },
                    { id: 6, pid: 1, name: "Anderson" },
                    { id: 7, name: "Web Team", hasChild: true, expanded: true },
                    { id: 8, pid: 7, name: "Joshua" },
                    { id: 9, pid: 7, name: "Matthew" },
                    { id: 10, pid: 7, name: "David" },
                    { id: 11, name: "Build Team", hasChild: true },
                    { id: 12, pid: 11, name: "Ryan" },
                    { id: 13, pid: 11, name: "Justin" },
                    { id: 14, pid: 11, name: "Robert" },
                    { id: 15, pid: 11, name: "Johnson" },
                    { id: 16, name: "WPF Team", hasChild: true },
                    { id: 17, pid: 16, name: "Rock" },
                    { id: 18, pid: 16, name: "Gospel" },
                    { id: 19, pid: 16, name: "Brown" },
                    { id: 20, pid: 16, name: "Miller" }];
        $(function () {
            $('#itemList').ejDropDownTree({
                treeViewSettings: {
                    allowMultiSelection: true,
                    fields: { id: "id", parentId: "pid", value: "id", text: "name", hasChild: "hasChild", dataSource: localData, expanded: "expanded" }
                },
                delimiter: ";"
            });
        });
    </script>

{% endhighlight %}

### enabled  `boolean`
{:#members:enabled}

Indicates whether the DropDownTree control responds to user interaction or not. By default, the control is in the enabled mode and can be disabled by setting this to false.

#### Default Value

* true

#### Example

{% highlight html %}
 
<input type="text" id="itemList" />

<script type="text/javascript">
        var localData = [
                    { id: 1, name: "Windows Team", hasChild: true, expanded: true },
                    { id: 2, pid: 1, name: "Clark" },
                    { id: 3, pid: 1, name: "Wright" },
                    { id: 4, pid: 1, name: "Lopez" },
                    { id: 7, name: "Web Team", hasChild: true, expanded: true },
                    { id: 8, pid: 7, name: "Joshua" },
                    { id: 9, pid: 7, name: "Matthew" },
                    { id: 10, pid: 7, name: "David" },
                    { id: 11, name: "Build Team", hasChild: true },
                    { id: 12, pid: 11, name: "Ryan" },
                    { id: 13, pid: 11, name: "Justin" },
                    { id: 14, pid: 11, name: "Robert" }];
        $(function () {
            $('#itemList').ejDropDownTree({
                treeViewSettings: {
                    fields: { id: "id", parentId: "pid", value: "id", text: "name", hasChild: "hasChild", dataSource: localData, expanded: "expanded" }
                },
                enabled: false
            });
        });
    </script>

{% endhighlight %}

### enableAnimation  `boolean`
{:#members:enableanimation }

The enabled animation property uses the easeOutQuad animation to SlideDown and SlideUp the popup wrapper in 200 and 100 milliseconds, respectively.

#### Default Value

* false

#### Example

{% highlight html %}
 
<input type="text" id="itemList" />

<script type="text/javascript">
        var localData = [
                    { id: 1, name: "Windows Team", hasChild: true, expanded: true },
                    { id: 2, pid: 1, name: "Clark" },
                    { id: 3, pid: 1, name: "Wright" },
                    { id: 4, pid: 1, name: "Lopez" },
                    { id: 7, name: "Web Team", hasChild: true, expanded: true },
                    { id: 8, pid: 7, name: "Joshua" },
                    { id: 9, pid: 7, name: "Matthew" },
                    { id: 10, pid: 7, name: "David" },
                    { id: 11, name: "Build Team", hasChild: true },
                    { id: 12, pid: 11, name: "Ryan" },
                    { id: 13, pid: 11, name: "Justin" },
                    { id: 14, pid: 11, name: "Robert" }];
        $(function () {
            $('#itemList').ejDropDownTree({
                treeViewSettings: {
                    fields: { id: "id", parentId: "pid", value: "id", text: "name", hasChild: "hasChild", dataSource: localData, expanded: "expanded" }
                },
                enableAnimation: true
            });
        });
    </script>

    
{% endhighlight %}

### enablePersistence  `boolean`
{:#members:enablepersistence }

Gets or sets a value that indicates whether to continue the DropDownTree model state in the page using applicable medium, i.e., HTML5 localStorage or cookies.

#### Default Value

* false

#### Example

{% highlight html %}
 
<input type="text" id="itemList" />

<script type="text/javascript">
        var localData = [
                    { id: 1, name: "Windows Team", hasChild: true, expanded: true },
                    { id: 2, pid: 1, name: "Clark" },
                    { id: 3, pid: 1, name: "Wright" },
                    { id: 4, pid: 1, name: "Lopez" },
                    { id: 7, name: "Web Team", hasChild: true, expanded: true },
                    { id: 8, pid: 7, name: "Joshua" },
                    { id: 9, pid: 7, name: "Matthew" },
                    { id: 10, pid: 7, name: "David" },
                    { id: 11, name: "Build Team", hasChild: true },
                    { id: 12, pid: 11, name: "Ryan" },
                    { id: 13, pid: 11, name: "Justin" },
                    { id: 14, pid: 11, name: "Robert" }];
        $(function () {
            $('#itemList').ejDropDownTree({
                treeViewSettings: {
                    fields: { id: "id", parentId: "pid", value: "id", text: "name", hasChild: "hasChild", dataSource: localData, expanded: "expanded" }
                },
                enablePersistence: true
            });
        });
    </script>

    
{% endhighlight %}

### enableRTL  `boolean`
{:#members:enablertl }

Sets the DropDownTree textbox direction from right to left alignment.

#### Default Value

* false

#### Example

{% highlight html %}
 
<input type="text" id="itemList" />

<script type="text/javascript">
        var localData = [
                    { id: 1, name: "Windows Team", hasChild: true, expanded: true },
                    { id: 2, pid: 1, name: "Clark" },
                    { id: 3, pid: 1, name: "Wright" },
                    { id: 4, pid: 1, name: "Lopez" },
                    { id: 7, name: "Web Team", hasChild: true, expanded: true },
                    { id: 8, pid: 7, name: "Joshua" },
                    { id: 9, pid: 7, name: "Matthew" },
                    { id: 10, pid: 7, name: "David" },
                    { id: 11, name: "Build Team", hasChild: true },
                    { id: 12, pid: 11, name: "Ryan" },
                    { id: 13, pid: 11, name: "Justin" },
                    { id: 14, pid: 11, name: "Robert" }];
        $(function () {
            $('#itemList').ejDropDownTree({
                treeViewSettings: {
                    fields: { id: "id", parentId: "pid", value: "id", text: "name", hasChild: "hasChild", dataSource: localData, expanded: "expanded" }
                },
                enableRTL: true
            });
        });
    </script>

    
{% endhighlight %}

### footerTemplate `string`
{:#members:footertemplate }

Creates footer with text or HTML elements for the dropdown items.

#### Default Value

* null

#### Example

{% highlight html %}
    <input type="text" id="empList" />

<script type="text/javascript">
    var treeData = [
           { id: 1, text: "Software Engineer", hasChild: true, expanded: true },
               { id: 2, pid: 1, imgId: "3", text: "Erik Linden", eimg: "3", country: "England" },
               { id: 3, pid: 1, imgId: "8", text: "Louis", eimg: "7", country: "Australia" },
           { id: 4, text: "Tester", hasChild: true, expanded: true },
               { id: 5, pid: 4, imgId: "6", text: "John Linden", eimg: "6", country: "Norway" },
               { id: 6, pid: 4, imgId: "7", text: "Lawrence", eimg: "8", country: "India" }
    ];
    $(function () {
        $('#empList').ejDropDownTree({
            watermarkText: "Please select",
            width: "100%",
            popupSettings: {
                height: "500px"
            },
            footerTemplate: '<div class="e-tree-footer"> <span>End of list</span></div>',
            treeViewSettings: {
                fields: {
                    dataSource: treeData,
                    id: "id", parentId: "pid", text: "text", hasChild: "hasChild"
                },
                template: "#treeTemplate"
            }
        });
    });
</script>

{% endhighlight %}

### fullPathDelimiter  `string`
{:#members:fullpathdelimiter  }

Serves as a patch of the entries comprising the path (that is set in the entry area) of the selected node.

#### Default Value

* '/'

#### Example

{% highlight html %}
    <input type="text" id="itemList" />

<script type="text/javascript">
        var localData = [
                    { id: 1, name: "Windows Team", hasChild: true, expanded: true },
                    { id: 2, pid: 1, name: "Clark" },
                    { id: 3, pid: 1, name: "Wright" },
                    { id: 4, pid: 1, name: "Lopez" },
                    { id: 6, pid: 1, name: "Anderson" },
                    { id: 7, name: "Web Team", hasChild: true, expanded: true },
                    { id: 8, pid: 7, name: "Joshua" },
                    { id: 9, pid: 7, name: "Matthew" },
                    { id: 10, pid: 7, name: "David" },
                    { id: 11, name: "Build Team", hasChild: true },
                    { id: 12, pid: 11, name: "Ryan" },
                    { id: 13, pid: 11, name: "Justin" },
                    { id: 14, pid: 11, name: "Robert" },
                    { id: 15, pid: 11, name: "Johnson" },
                    { id: 16, name: "WPF Team", hasChild: true },
                    { id: 17, pid: 16, name: "Rock" },
                    { id: 18, pid: 16, name: "Gospel" },
                    { id: 19, pid: 16, name: "Brown" },
                    { id: 20, pid: 16, name: "Miller" }];
        $(function () {
            $('#itemList').ejDropDownTree({
                treeViewSettings: {
                    fields: { id: "id", parentId: "pid", value: "id", text: "name", hasChild: "hasChild", dataSource: localData, expanded: "expanded" }
                },
                textMode: "fullPath",
                fullPathDelimiter: "->"
            });
        });
    </script>

{% endhighlight %}

### headerTemplate `string`
{:#members:headertemplate}

Creates header with text or HTML elements for the dropdown items.

#### Default Value

* null

#### Example

{% highlight html %}
    <input type="text" id="empList" />

<script type="text/javascript">
    var treeData = [
           { id: 1, text: "Software Engineer", hasChild: true, expanded: true },
               { id: 2, pid: 1, imgId: "3", text: "Erik Linden", eimg: "3", country: "England" },
               { id: 3, pid: 1, imgId: "8", text: "Louis", eimg: "7", country: "Australia" },
           { id: 4, text: "Tester", hasChild: true, expanded: true },
               { id: 5, pid: 4, imgId: "6", text: "John Linden", eimg: "6", country: "Norway" },
               { id: 6, pid: 4, imgId: "7", text: "Lawrence", eimg: "8", country: "India" }
    ];
    $(function () {
        $('#empList').ejDropDownTree({
            watermarkText: "Please select",
            width: "100%",
            popupSettings: {
                height: "500px"
            },
            headerTemplate: '<div class="e-tree-header"><span>Employees </span></div>',
            treeViewSettings: {
                fields: {
                    dataSource: treeData,
                    id: "id", parentId: "pid", text: "text", hasChild: "hasChild"
                },
                template: "#treeTemplate"
            }
        });
    });
</script>

{% endhighlight %}

### height `string|number`
{:#members:height}

Defines the height of the DropDownTree textbox.

#### Default Value

* ""

#### Example

{% highlight html %}

<input type="text" id="itemList" />

<script type="text/javascript">
        var localData = [
                    { id: 1, name: "Windows Team", hasChild: true, expanded: true },
                    { id: 2, pid: 1, name: "Clark" },
                    { id: 3, pid: 1, name: "Wright" },
                    { id: 4, pid: 1, name: "Lopez" },
                    { id: 7, name: "Web Team", hasChild: true, expanded: true },
                    { id: 8, pid: 7, name: "Joshua" },
                    { id: 9, pid: 7, name: "Matthew" },
                    { id: 10, pid: 7, name: "David" },
                    { id: 11, name: "Build Team", hasChild: true },
                    { id: 12, pid: 11, name: "Ryan" },
                    { id: 13, pid: 11, name: "Justin" },
                    { id: 14, pid: 11, name: "Robert" }];
        $(function () {
            $('#itemList').ejDropDownTree({
                treeViewSettings: {
                    fields: { id: "id", parentId: "pid", value: "id", text: "name", hasChild: "hasChild", dataSource: localData, expanded: "expanded" }
                },
                height: "160px"
            });
        });
    </script>
    
{% endhighlight %}

### locale `string`
{:#members:locale}

Allows you to set a particular country or regional language for the DropDownTree.

#### Default Value

* "en-US"

#### Example

{% highlight html %}

    <input type="text" id="company" />

    $(function () {
        var data = ej.DataManager({ url: "http://mvc.syncfusion.com/services/Northwnd.svc/Customers" });
        $('#company').ejDropDownTree({
            dataSource: data,
            fields: { text: "CompanyName", value: 'ContactName' },
            width: 260,
            showCheckbox: true,
            locale: "de-DE",
            enableFilterSearch: true,
            enablePopupResize: true

        });
    });
    
{% endhighlight %}

### popupSettings `object`
{:#members:popupsettings}

Customizes the height and width of the popup wrapper.

#### Default Value

* {height: '152px',width: 'auto',showPopupOnLoad: false}

### popupSettings.height `string|number`
{:#members:popupsettings-height}

Defines the height of the popup wrapper in the DropDownTree control.

#### Example

{% highlight html %}
<input type="text" id="itemList" />

<script type="text/javascript">
        var localData = [
                    { id: 1, name: "Windows Team", hasChild: true, expanded: true },
                    { id: 2, pid: 1, name: "Clark" },
                    { id: 3, pid: 1, name: "Wright" },
                    { id: 4, pid: 1, name: "Lopez" },
                    { id: 7, name: "Web Team", hasChild: true, expanded: true },
                    { id: 8, pid: 7, name: "Joshua" },
                    { id: 9, pid: 7, name: "Matthew" },
                    { id: 10, pid: 7, name: "David" },
                    { id: 11, name: "Build Team", hasChild: true },
                    { id: 12, pid: 11, name: "Ryan" },
                    { id: 13, pid: 11, name: "Justin" },
                    { id: 14, pid: 11, name: "Robert" }];
        $(function () {
            $('#itemList').ejDropDownTree({
                treeViewSettings: {
                    fields: { id: "id", parentId: "pid", value: "id", text: "name", hasChild: "hasChild", dataSource: localData, expanded: "expanded" }
                },
                popupSettings: {
                         height: "300px"
				}         
              });
        });
    </script>

{% endhighlight %}

### popupSettings.width `string|number`
{:#members:popupsettings-width}

Defines the width of the popup wrapper in the DropDownTree control.

#### Example

{% highlight html %}

<input type="text" id="itemList" />

<script type="text/javascript">
        var localData = [
                    { id: 1, name: "Windows Team", hasChild: true, expanded: true },
                    { id: 2, pid: 1, name: "Clark" },
                    { id: 3, pid: 1, name: "Wright" },
                    { id: 4, pid: 1, name: "Lopez" },
                    { id: 7, name: "Web Team", hasChild: true, expanded: true },
                    { id: 8, pid: 7, name: "Joshua" },
                    { id: 9, pid: 7, name: "Matthew" },
                    { id: 10, pid: 7, name: "David" },
                    { id: 11, name: "Build Team", hasChild: true },
                    { id: 12, pid: 11, name: "Ryan" },
                    { id: 13, pid: 11, name: "Justin" },
                    { id: 14, pid: 11, name: "Robert" }];
        $(function () {
            $('#itemList').ejDropDownTree({
                treeViewSettings: {
                    fields: { id: "id", parentId: "pid", value: "id", text: "name", hasChild: "hasChild", dataSource: localData, expanded: "expanded" }
                },
                popupSettings: {
                         width: "300px"
				}         
              });
        });
    </script>

{% endhighlight %}


### popupSettings.showPopupOnLoad `boolean`
{:#members:popupsettings-showpopuponload}

The DropDownTree control is displayed with the popup.

#### Example

{% highlight html %}

<input type="text" id="itemList" />

<script type="text/javascript">
        var localData = [
                    { id: 1, name: "Windows Team", hasChild: true, expanded: true },
                    { id: 2, pid: 1, name: "Clark" },
                    { id: 3, pid: 1, name: "Wright" },
                    { id: 4, pid: 1, name: "Lopez" },
                    { id: 7, name: "Web Team", hasChild: true, expanded: true },
                    { id: 8, pid: 7, name: "Joshua" },
                    { id: 9, pid: 7, name: "Matthew" },
                    { id: 10, pid: 7, name: "David" },
                    { id: 11, name: "Build Team", hasChild: true },
                    { id: 12, pid: 11, name: "Ryan" },
                    { id: 13, pid: 11, name: "Justin" },
                    { id: 14, pid: 11, name: "Robert" }];
        $(function () {
            $('#itemList').ejDropDownTree({
                treeViewSettings: {
                    fields: { id: "id", parentId: "pid", value: "id", text: "name", hasChild: "hasChild", dataSource: localData, expanded: "expanded" }
                },
                popupSettings: {
                         showPopupOnLoad: true
				}         
              });
        });
    </script>

{% endhighlight %}

### readOnly `boolean`
{:#members:readonly}

Specifies that the DropDownTree textbox values should be read-only.

#### Default Value

* false

#### Example

{% highlight html %}

<input type="text" id="itemList" />

<script type="text/javascript">
        var localData = [
                    { id: 1, name: "Windows Team", hasChild: true, expanded: true },
                    { id: 2, pid: 1, name: "Clark" },
                    { id: 3, pid: 1, name: "Wright" },
                    { id: 4, pid: 1, name: "Lopez" },
                    { id: 7, name: "Web Team", hasChild: true, expanded: true },
                    { id: 8, pid: 7, name: "Joshua" },
                    { id: 9, pid: 7, name: "Matthew" },
                    { id: 10, pid: 7, name: "David" },
                    { id: 11, name: "Build Team", hasChild: true },
                    { id: 12, pid: 11, name: "Ryan" },
                    { id: 13, pid: 11, name: "Justin" },
                    { id: 14, pid: 11, name: "Robert" }];
        $(function () {
            $('#itemList').ejDropDownTree({
                treeViewSettings: {
                    fields: { id: "id", parentId: "pid", value: "id", text: "name", hasChild: "hasChild", dataSource: localData, expanded: "expanded" }
                },
                readOnly: true
            });
        });
    </script>

{% endhighlight %}

### showRoundedCorner `boolean`
{:#members:showroundedcorner}

The DropDownTree's textbox is displayed with rounded corner style.

#### Default Value

* false

#### Example

{% highlight html %}
 
   <input type="text" id="itemList" />

<script type="text/javascript">
        var localData = [
                    { id: 1, name: "Windows Team", hasChild: true, expanded: true },
                    { id: 2, pid: 1, name: "Clark" },
                    { id: 3, pid: 1, name: "Wright" },
                    { id: 4, pid: 1, name: "Lopez" },
                    { id: 7, name: "Web Team", hasChild: true, expanded: true },
                    { id: 8, pid: 7, name: "Joshua" },
                    { id: 9, pid: 7, name: "Matthew" },
                    { id: 10, pid: 7, name: "David" },
                    { id: 11, name: "Build Team", hasChild: true },
                    { id: 12, pid: 11, name: "Ryan" },
                    { id: 13, pid: 11, name: "Justin" },
                    { id: 14, pid: 11, name: "Robert" }];
        $(function () {
            $('#itemList').ejDropDownTree({
                treeViewSettings: {
                    fields: { id: "id", parentId: "pid", value: "id", text: "name", hasChild: "hasChild", dataSource: localData, expanded: "expanded" }
                },
                showRoundedCorner: true
            });
        });
    </script>

{% endhighlight %}

### targetID `string`
{:#members:targetid}

Specifies the targetID for the DropDownTree's items.

#### Default Value

* null

#### Example

{% highlight html %}
 
    <input type="text" id="selectItem" />

                        <div id="itemList">
                            <ul id="treeView">
                                <li class="expanded">
                                    Artwork
                                    <ul>
                                        <li>
                                            Abstract
                                            <ul>
                                                <li>2 Acrylic Mediums</li>
                                                <li>Creative Acrylic</li>
                                                <li>Modern Painting</li>
                                                <li>Canvas Art</li>
                                                <li>Black white</li>
                                            </ul>
                                        </li>
                                        <li>
                                            Children
                                            <ul>
                                                <li>Preschool Crafts</li>
                                                <li>School-age Crafts</li>
                                                <li>Fabulous Toddler</li>
                                            </ul>
                                        </li>
                                    </ul>
                                </li>
                            </ul>
                        </div>

<script type="text/javascript">
        $(function () {
            $('#selectItem').ejDropDownTree({
                targetId: "itemList"
            });
        });
    </script>

{% endhighlight %}

### textMode `enum` 
{:#members:textmode}

<ts name="ej.Textmode"/>

Specifies the delimiter between nodes (indicating their hierarchy). 

<table class="params">
<thead>
<tr>
<th>Option</th>
<th class="last">Description</th>
</tr>
</thead>
<tbody>
<tr>
<td class="option">
none</td>

<td class="description last"> When TextMode property is set to none, only selected/checked node's text is presented. </td>
</tr>
<tr>
<td class="option">
fullPath</td>

<td class="description last">When FullPath option is selected, the full path of the selected node is shown in the control. </td>
</tr>
</tbody>
</table>


#### Default Value

*  `ej.DropDownTree.TextMode.none`

#### Example

{% highlight html %}
 <input type="text" id="itemList" />

<script type="text/javascript">
        var localData = [
                    { id: 1, name: "Windows Team", hasChild: true, expanded: true },
                    { id: 2, pid: 1, name: "Clark" },
                    { id: 3, pid: 1, name: "Wright" },
                    { id: 4, pid: 1, name: "Lopez" },
                    { id: 6, pid: 1, name: "Anderson" },
                    { id: 7, name: "Web Team", hasChild: true, expanded: true },
                    { id: 8, pid: 7, name: "Joshua" },
                    { id: 9, pid: 7, name: "Matthew" },
                    { id: 10, pid: 7, name: "David" },
                    { id: 11, name: "Build Team", hasChild: true },
                    { id: 12, pid: 11, name: "Ryan" },
                    { id: 13, pid: 11, name: "Justin" },
                    { id: 14, pid: 11, name: "Robert" },
                    { id: 15, pid: 11, name: "Johnson" },
                    { id: 16, name: "WPF Team", hasChild: true },
                    { id: 17, pid: 16, name: "Rock" },
                    { id: 18, pid: 16, name: "Gospel" },
                    { id: 19, pid: 16, name: "Brown" },
                    { id: 20, pid: 16, name: "Miller" }];
        $(function () {
            $('#itemList').ejDropDownTree({
                treeViewSettings: {
                    fields: { id: "id", parentId: "pid", value: "id", text: "name", hasChild: "hasChild", dataSource: localData, expanded: "expanded" }
                },
                textMode: "fullPath"
            });
        });
    </script>

{% endhighlight %}

### validationMessage `object`
{:#members:validationmessage}

Sets the jQuery validation error message in the DropDownTree.


#### Default Value

* null

#### Example

{% highlight html %}
 
    <form id="form1">

<input type="text" id="itemList" />
<input type="submit" value="Validate" />
 </form>


<script type="text/javascript">
        var localData = [
                    { id: 1, name: "Windows Team", hasChild: true, expanded: true },
                    { id: 2, pid: 1, name: "Clark" },
                    { id: 3, pid: 1, name: "Wright" },
                    { id: 4, pid: 1, name: "Lopez" },
                    { id: 7, name: "Web Team", hasChild: true, expanded: true },
                    { id: 8, pid: 7, name: "Joshua" },
                    { id: 9, pid: 7, name: "Matthew" },
                    { id: 10, pid: 7, name: "David" },
                    { id: 11, name: "Build Team", hasChild: true },
                    { id: 12, pid: 11, name: "Ryan" },
                    { id: 13, pid: 11, name: "Justin" },
                    { id: 14, pid: 11, name: "Robert" }];
     $.validator.setDefaults({
         ignore: [],
         errorClass: 'e-validation-error', // to get the error message on jQuery validation
         errorPlacement: function (error, element) {
             $(error).insertAfter(element.closest(".e-widget"));
         }
         // any other default options and/or rules
     });
$(function () {
        $('#itemList').ejDropDownTree({
            watermarkText: "Select a car",
            width: "50%",
            targetId: "carsList",
            validationRules: {
                required: true
               
            },
            validationMessage: {
                required: "* Required"
               
            }
        });
    });

    </script>
    
{% endhighlight %}

### validationRules `object`
{:#members:validationrules}

Sets the jQuery validation rules in the DropDownTree.

#### Default Value

* null

#### Example

{% highlight html %}
 
    <form id="form1">

<input type="text" id="itemList" />
<input type="submit" value="Validate" />
 </form>


<script type="text/javascript">
        var localData = [
                    { id: 1, name: "Windows Team", hasChild: true, expanded: true },
                    { id: 2, pid: 1, name: "Clark" },
                    { id: 3, pid: 1, name: "Wright" },
                    { id: 4, pid: 1, name: "Lopez" },
                    { id: 7, name: "Web Team", hasChild: true, expanded: true },
                    { id: 8, pid: 7, name: "Joshua" },
                    { id: 9, pid: 7, name: "Matthew" },
                    { id: 10, pid: 7, name: "David" },
                    { id: 11, name: "Build Team", hasChild: true },
                    { id: 12, pid: 11, name: "Ryan" },
                    { id: 13, pid: 11, name: "Justin" },
                    { id: 14, pid: 11, name: "Robert" }];
     $.validator.setDefaults({
         ignore: [],
         errorClass: 'e-validation-error', // to get the error message on jQuery validation
         errorPlacement: function (error, element) {
             $(error).insertAfter(element.closest(".e-widget"));
         }
         // any other default options and/or rules
     });
$(function () {
        $('#itemList').ejDropDownTree({
            watermarkText: "Select a car",
            width: "50%",
            targetId: "carsList",
            validationRules: {
                required: true
               
            },
            validationMessage: {
                required: "* Required"
               
            }
        });
    });

    </script>
{% endhighlight %}

### value `string`
{:#members:value}

Specifies the value (text content) for the DropDownTree control. For the single selection mode, the selected item's value will be returned in its data type, and for MultiSelectMode, returns the selected items values separated by delimiter in string type.

#### Default Value

* null

#### Example

{% highlight html %}
 
   <input type="text" id="selectCar" />

  
    <script type="text/javascript">
        var localData = [
                   { id: 1, name: "Discover Music", hasChild: true, expanded: true },
                   { id: 2, pid: 1, name: "Hot Singles" },
                   { id: 3, pid: 1, name: "Rising Artists" },
                   { id: 4, pid: 1, name: "Live Music" },
                   { id: 6, pid: 1, name: "Best of 2013 So Far" },
                   { id: 7, name: "Sales and Events", hasChild: true, expanded: true },
                   { id: 8, pid: 7, name: "100 Albums - $5 Each" },
                   { id: 9, pid: 7, name: "Hip-Hop and R&B Sale" },
                   { id: 10, pid: 7, name: "CD Deals" },
                   { id: 11, name: "Categories", hasChild: true },
                   { id: 12, pid: 11, name: "Songs" },
                   { id: 13, pid: 11, name: "Bestselling Albums" },
                   { id: 14, pid: 11, name: "New Releases" },
                   { id: 15, pid: 11, name: "Bestselling Songs" },
                   { id: 16, name: "MP3 Albums", hasChild: true },
                   { id: 17, pid: 16, name: "Rock" },
                   { id: 18, pid: 16, name: "Gospel" },
                   { id: 19, pid: 16, name: "Latin Music" },
                   { id: 20, pid: 16, name: "Jazz" },
                   { id: 21, name: "More in Music", hasChild: true },
                   { id: 22, pid: 21, name: "Music Trade-In" },
                   { id: 23, pid: 21, name: "Redeem a Gift Card" },
                   { id: 24, pid: 21, name: "Band T-Shirts" },
                   { id: 25, pid: 21, name: "Mobile MVC" }];

    
    $(function () {
        $('#selectCar').ejDropDownTreeList({
            fields: { id: "id", parentId: "pid", text: "name", hasChild: "hasChild", dataSource: localData, expanded: "expanded" },
            value: 'Rock'
        });
    });
    </script>

{% endhighlight %}

### watermarkText `string`
{:#members:watermarktext}

Specifies a short hint that describes the expected value of the DropDownTree control.

#### Default Value

* null

#### Example

{% highlight html %}
 
    <input type="text" id="itemList" />

<script type="text/javascript">
        var localData = [
                    { id: 1, name: "Windows Team", hasChild: true, expanded: true },
                    { id: 2, pid: 1, name: "Clark" },
                    { id: 3, pid: 1, name: "Wright" },
                    { id: 4, pid: 1, name: "Lopez" },
                    { id: 7, name: "Web Team", hasChild: true, expanded: true },
                    { id: 8, pid: 7, name: "Joshua" },
                    { id: 9, pid: 7, name: "Matthew" },
                    { id: 10, pid: 7, name: "David" },
                    { id: 11, name: "Build Team", hasChild: true },
                    { id: 12, pid: 11, name: "Ryan" },
                    { id: 13, pid: 11, name: "Justin" },
                    { id: 14, pid: 11, name: "Robert" }];
        $(function () {
            $('#itemList').ejDropDownTree({
                treeViewSettings: {
                    fields: { id: "id", parentId: "pid", value: "id", text: "name", hasChild: "hasChild", dataSource: localData, expanded: "expanded" }
                },
                watermarkText: "Please select"
            });
        });
    </script>

{% endhighlight %}

### width `string|number`
{:#members:width}

Defines the width of the DropDownTree textbox.

#### Default Value

* "100%"

#### Example

{% highlight html %}
 
    <input type="text" id="itemList" />

<script type="text/javascript">
        var localData = [
                    { id: 1, name: "Windows Team", hasChild: true, expanded: true },
                    { id: 2, pid: 1, name: "Clark" },
                    { id: 3, pid: 1, name: "Wright" },
                    { id: 4, pid: 1, name: "Lopez" },
                    { id: 7, name: "Web Team", hasChild: true, expanded: true },
                    { id: 8, pid: 7, name: "Joshua" },
                    { id: 9, pid: 7, name: "Matthew" },
                    { id: 10, pid: 7, name: "David" },
                    { id: 11, name: "Build Team", hasChild: true },
                    { id: 12, pid: 11, name: "Ryan" },
                    { id: 13, pid: 11, name: "Justin" },
                    { id: 14, pid: 11, name: "Robert" }];
        $(function () {
            $('#itemList').ejDropDownTree({
                treeViewSettings: {
                    fields: { id: "id", parentId: "pid", value: "id", text: "name", hasChild: "hasChild", dataSource: localData, expanded: "expanded" }
                },
                width: "150px"
            });
        });
    </script>

{% endhighlight %}

### treeViewSettings `object`
{:#members:treeviewsettings}

Defines the popup settings of the DropDownTree widget. You can use any property which are in [`treeview`](https://help.syncfusion.com/api/js/ejtreeview) using this property.

N> The public method of treeview data is accessed by `[object of the dropdowntree].treeview.[methodname]`.

#### Default Value

* "{}"

#### Example

{% highlight html %}
 
    <input type="text" id="itemList" />

<script type="text/javascript">
        var localData = [
                    { id: 1, name: "Windows Team", hasChild: true, expanded: true },
                    { id: 2, pid: 1, name: "Clark" },
                    { id: 3, pid: 1, name: "Wright" },
                    { id: 4, pid: 1, name: "Lopez" },
                    { id: 7, name: "Web Team", hasChild: true, expanded: true },
                    { id: 8, pid: 7, name: "Joshua" },
                    { id: 9, pid: 7, name: "Matthew" },
                    { id: 10, pid: 7, name: "David" },
                    { id: 11, name: "Build Team", hasChild: true },
                    { id: 12, pid: 11, name: "Ryan" },
                    { id: 13, pid: 11, name: "Justin" },
                    { id: 14, pid: 11, name: "Robert" }];
        $(function () {
            $('#itemList').ejDropDownTree({
                treeViewSettings: {
                    fields: { id: "id", parentId: "pid", value: "id", text: "name", hasChild: "hasChild", dataSource: localData, expanded: "expanded" }
                },
                width: "150px"
            });
        });
    </script>

{% endhighlight %}

## Methods

### checkAll()
{:#methods:checkall}

Checks all the nodes in the DropDownTree.

#### Example

{% highlight html %}
 
<input type="text" id="itemList" />

<script type="text/javascript">
        var localData = [
                    { id: 1, name: "Windows Team", hasChild: true, expanded: true },
                    { id: 2, pid: 1, name: "Clark" },
                    { id: 3, pid: 1, name: "Wright" },
                    { id: 4, pid: 1, name: "Lopez" },
                    { id: 7, name: "Web Team", hasChild: true, expanded: true },
                    { id: 8, pid: 7, name: "Joshua" },
                    { id: 9, pid: 7, name: "Matthew" },
                    { id: 10, pid: 7, name: "David" },
                    { id: 11, name: "Build Team", hasChild: true },
                    { id: 12, pid: 11, name: "Ryan" },
                    { id: 13, pid: 11, name: "Justin" },
                    { id: 14, pid: 11, name: "Robert" }];
        $(function () {
            $('#itemList').ejDropDownTree({
                treeViewSettings: {
                       showCheckbox: true,
                    fields: { id: "id", parentId: "pid", value: "id", text: "name", hasChild: "hasChild", dataSource: localData, expanded: "expanded" }
                },
                value: "Ryan"
            });


    ddTreeObj = $('#itemList').data("ejDropDownTree");
ddTreeObj.checkAll();
        });
    </script>
{% endhighlight %}


{% highlight html %}
 
    <script>
       $('#itemList').ejDropDownTree("checkAll")
    </script>

{% endhighlight %}

### checkNode(node)
{:#methods:checknode}

Checks a node in the DropDownTree.

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
<td class="name">element</td>
<td class="type">string|object|array</td>
<td class="description last"> ID of the DropDownTree node/object of the DropDownTree node/collection 
of the ID/object of the DropDownTree nodes.
</td>
</tr>

</tbody>
</table>

#### Example

{% highlight html %}
 
<input type="text" id="itemList" />

<script type="text/javascript">
        var localData = [
                    { id: 1, name: "Windows Team", hasChild: true, expanded: true },
                    { id: 2, pid: 1, name: "Clark" },
                    { id: 3, pid: 1, name: "Wright" },
                    { id: 4, pid: 1, name: "Lopez" },
                    { id: 7, name: "Web Team", hasChild: true, expanded: true },
                    { id: 8, pid: 7, name: "Joshua" },
                    { id: 9, pid: 7, name: "Matthew" },
                    { id: 10, pid: 7, name: "David" },
                    { id: 11, name: "Build Team", hasChild: true },
                    { id: 12, pid: 11, name: "Ryan" },
                    { id: 13, pid: 11, name: "Justin" },
                    { id: 14, pid: 11, name: "Robert" }];
        $(function () {
            $('#itemList').ejDropDownTree({
                treeViewSettings: {
                     showCheckbox: true,
                    fields: { id: "id", parentId: "pid", value: "id", text: "name", hasChild: "hasChild", dataSource: localData, expanded: "expanded" }
                },
                value: "Ryan"
            });


    ddTreeObj = $('#itemList').data("ejDropDownTree");
ddTreeObj.checkNode($("#1"));
        });
    </script>

{% endhighlight %}


{% highlight html %}
 
    <script>
      $("#itemList").ejDropDownTree("checkNode", $("#1"))
    </script>

{% endhighlight %}

### clearText()
{:#methods:cleartext}

Clears the text in the DropDownTree.

#### Example

{% highlight html %}
 
<input type="text" id="itemList" />

<script type="text/javascript">
        var localData = [
                    { id: 1, name: "Windows Team", hasChild: true, expanded: true },
                    { id: 2, pid: 1, name: "Clark" },
                    { id: 3, pid: 1, name: "Wright" },
                    { id: 4, pid: 1, name: "Lopez" },
                    { id: 7, name: "Web Team", hasChild: true, expanded: true },
                    { id: 8, pid: 7, name: "Joshua" },
                    { id: 9, pid: 7, name: "Matthew" },
                    { id: 10, pid: 7, name: "David" },
                    { id: 11, name: "Build Team", hasChild: true },
                    { id: 12, pid: 11, name: "Ryan" },
                    { id: 13, pid: 11, name: "Justin" },
                    { id: 14, pid: 11, name: "Robert" }];
        $(function () {
            $('#itemList').ejDropDownTree({
                treeViewSettings: {
                    fields: { id: "id", parentId: "pid", value: "id", text: "name", hasChild: "hasChild", dataSource: localData, expanded: "expanded" }
                },
                value: "Ryan"
            });


    ddTreeObj = $('#selectItem').data("ejDropDownTree");
ddTreeObj.clearText();
        });
    </script>

{% endhighlight %}


{% highlight html %}
 
    <script>
       $('#selectItem').ejDropDownTree("clearText")
    </script>

{% endhighlight %}

### destroy()
{:#methods:destroy}

Destroys the DropDownTree control.

#### Example

{% highlight html %}

<input type="text" id="itemList" />

<script type="text/javascript">
        var localData = [
                    { id: 1, name: "Windows Team", hasChild: true, expanded: true },
                    { id: 2, pid: 1, name: "Clark" },
                    { id: 3, pid: 1, name: "Wright" },
                    { id: 4, pid: 1, name: "Lopez" },
                    { id: 7, name: "Web Team", hasChild: true, expanded: true },
                    { id: 8, pid: 7, name: "Joshua" },
                    { id: 9, pid: 7, name: "Matthew" },
                    { id: 10, pid: 7, name: "David" },
                    { id: 11, name: "Build Team", hasChild: true },
                    { id: 12, pid: 11, name: "Ryan" },
                    { id: 13, pid: 11, name: "Justin" },
                    { id: 14, pid: 11, name: "Robert" }];
        $(function () {
            $('#itemList').ejDropDownTree({
                treeViewSettings: {
                    fields: { id: "id", parentId: "pid", value: "id", text: "name", hasChild: "hasChild", dataSource: localData, expanded: "expanded" }
                },
                value: "Ryan"
            });


    ddTreeObj = $('#selectItem').data("ejDropDownTree");
ddTreeObj.destroy();
        });
    </script>


{% endhighlight %}


{% highlight html %}

<script type="text/javascript">
        $('#selectItem').ejDropDownTree("destroy");

    </script>
{% endhighlight %}

### getValue()
{:#methods:getvalue}

Returns the selected value.

#### Example

{% highlight html %}
 
<input type="text" id="itemList" />

<script type="text/javascript">
        var localData = [
                    { id: 1, name: "Windows Team", hasChild: true, expanded: true },
                    { id: 2, pid: 1, name: "Clark" },
                    { id: 3, pid: 1, name: "Wright" },
                    { id: 4, pid: 1, name: "Lopez" },
                    { id: 7, name: "Web Team", hasChild: true, expanded: true },
                    { id: 8, pid: 7, name: "Joshua" },
                    { id: 9, pid: 7, name: "Matthew" },
                    { id: 10, pid: 7, name: "David" },
                    { id: 11, name: "Build Team", hasChild: true },
                    { id: 12, pid: 11, name: "Ryan" },
                    { id: 13, pid: 11, name: "Justin" },
                    { id: 14, pid: 11, name: "Robert" }];
        $(function () {
            $('#itemList').ejDropDownTree({
                treeViewSettings: {
                    fields: { id: "id", parentId: "pid", value: "id", text: "name", hasChild: "hasChild", dataSource: localData, expanded: "expanded" }
                },
                value: "Ryan"
            });


    ddTreeObj = $('#selectItem').data("ejDropDownTree");
ddTreeObj.getValue();
        });
    </script>

{% endhighlight %}


{% highlight html %}
 

    <script>
        $('#selectItem').ejDropDownTree("getValue");
    </script>

{% endhighlight %}

### hidePopup()
{:#methods:hidepopup}

Hides the popup in the DropDownTree.

#### Example

{% highlight html %}
 
<input type="text" id="itemList" />

<script type="text/javascript">
        var localData = [
                    { id: 1, name: "Windows Team", hasChild: true, expanded: true },
                    { id: 2, pid: 1, name: "Clark" },
                    { id: 3, pid: 1, name: "Wright" },
                    { id: 4, pid: 1, name: "Lopez" },
                    { id: 7, name: "Web Team", hasChild: true, expanded: true },
                    { id: 8, pid: 7, name: "Joshua" },
                    { id: 9, pid: 7, name: "Matthew" },
                    { id: 10, pid: 7, name: "David" },
                    { id: 11, name: "Build Team", hasChild: true },
                    { id: 12, pid: 11, name: "Ryan" },
                    { id: 13, pid: 11, name: "Justin" },
                    { id: 14, pid: 11, name: "Robert" }];
        $(function () {
            $('#itemList').ejDropDownTree({
                treeViewSettings: {
                    fields: { id: "id", parentId: "pid", value: "id", text: "name", hasChild: "hasChild", dataSource: localData, expanded: "expanded" }
                },
                value: "Ryan"
            });


    ddTreeObj = $('#selectItem').data("ejDropDownTree");
ddTreeObj.hidePopup();
        });
    </script>

{% endhighlight %}


{% highlight html %}
 

    <script>
        $('#selectItem').ejDropDownTree("hidePopup");
    </script>
    
{% endhighlight %}

### moveNode (sourceNode,destinationNode,index)
{:#methods:movenode}

Moves the DropDownTree node within the same DropDownTree. The new position of the given DropDownTree node will be based on destination node and index position. 

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
<td class="name">sourceNode</td>
<td class="type">string|object</td>
<td class="description last">ID of the DropDownTree node/object of the DropDownTree node.</td>
</tr>
<tr>
<td class="name">destinationNode</td>
<td class="type">string|object</td>
<td class="description last">ID of the DropDownTree node/object of the DropDownTree node.</td>
</tr>
<tr>
<td class="name">index</td>
<td class="type">number</td>
<td class="description last">New index position of the given source node.</td>
</tr>
</tbody>
</table>

#### Example

{% highlight html %}
 
<input type="text" id="itemList" />

<script type="text/javascript">
        var localData = [
                    { id: 1, name: "Windows Team", hasChild: true, expanded: true },
                    { id: 2, pid: 1, name: "Clark" },
                    { id: 3, pid: 1, name: "Wright" },
                    { id: 4, pid: 1, name: "Lopez" },
                    { id: 7, name: "Web Team", hasChild: true, expanded: true },
                    { id: 8, pid: 7, name: "Joshua" },
                    { id: 9, pid: 7, name: "Matthew" },
                    { id: 10, pid: 7, name: "David" },
                    { id: 11, name: "Build Team", hasChild: true },
                    { id: 12, pid: 11, name: "Ryan" },
                    { id: 13, pid: 11, name: "Justin" },
                    { id: 14, pid: 11, name: "Robert" }];
        $(function () {
            $('#itemList').ejDropDownTree({
                treeViewSettings: {
                     showCheckbox: true,
                    fields: { id: "id", parentId: "pid", value: "id", text: "name", hasChild: "hasChild", dataSource: localData, expanded: "expanded" }
                },
                value: "Ryan"
            });


    ddTreeObj = $('#itemList').data("ejDropDownTree");
ddTreeObj.checkNode($("#1"));
obj.moveNode("#1", "#10")
        });
    </script>
{% endhighlight %}


#### Example

{% highlight html %}
 
    <script>
        $('#itemList').ejDropDownTree("moveNode","#1", "#10"); 
    </script>

{% endhighlight %}

### removeAll()
{:#methods:removeall}

Removes all the nodes in the DropDownTree.

#### Example

{% highlight html %}
 
<input type="text" id="itemList" />

<script type="text/javascript">
        var localData = [
                    { id: 1, name: "Windows Team", hasChild: true, expanded: true },
                    { id: 2, pid: 1, name: "Clark" },
                    { id: 3, pid: 1, name: "Wright" },
                    { id: 4, pid: 1, name: "Lopez" },
                    { id: 7, name: "Web Team", hasChild: true, expanded: true },
                    { id: 8, pid: 7, name: "Joshua" },
                    { id: 9, pid: 7, name: "Matthew" },
                    { id: 10, pid: 7, name: "David" },
                    { id: 11, name: "Build Team", hasChild: true },
                    { id: 12, pid: 11, name: "Ryan" },
                    { id: 13, pid: 11, name: "Justin" },
                    { id: 14, pid: 11, name: "Robert" }];
        $(function () {
            $('#itemList').ejDropDownTree({
                treeViewSettings: {
                     showCheckbox: true,
                    fields: { id: "id", parentId: "pid", value: "id", text: "name", hasChild: "hasChild", dataSource: localData, expanded: "expanded" }
                },
                value: "Ryan"
            });


    ddTreeObj = $('#itemList').data("ejDropDownTree");
ddTreeObj.removeAll();
        });
    </script>


{% endhighlight %}


{% highlight html %}
 
    <script>
       $('#itemList').ejDropDownTree("removeAll")
    </script>

{% endhighlight %}

### removeNode(node)
{:#methods:removenode}

Removes a node in the DropDownTree.

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
<td class="name">element</td>
<td class="type">string|object|array</td>
<td class="description last"> ID of the DropDownTree node/object of the DropDownTree node/collection
of the ID/object of the DropDownTree nodes.
</td>
</tr>

</tbody>
</table>

#### Example

{% highlight html %}
 
 <input type="text" id="itemList" />

<script type="text/javascript">
        var localData = [
                    { id: 1, name: "Windows Team", hasChild: true, expanded: true },
                    { id: 2, pid: 1, name: "Clark" },
                    { id: 3, pid: 1, name: "Wright" },
                    { id: 4, pid: 1, name: "Lopez" },
                    { id: 7, name: "Web Team", hasChild: true, expanded: true },
                    { id: 8, pid: 7, name: "Joshua" },
                    { id: 9, pid: 7, name: "Matthew" },
                    { id: 10, pid: 7, name: "David" },
                    { id: 11, name: "Build Team", hasChild: true },
                    { id: 12, pid: 11, name: "Ryan" },
                    { id: 13, pid: 11, name: "Justin" },
                    { id: 14, pid: 11, name: "Robert" }];
        $(function () {
            $('#itemList').ejDropDownTree({
                treeViewSettings: {
                       allowMultiSelection: true,
                    fields: { id: "id", parentId: "pid", value: "id", text: "name", hasChild: "hasChild", dataSource: localData, expanded: "expanded" }
                },
                value: "Ryan"
            });


    ddTreeObj = $('#itemList').data("ejDropDownTree");
ddTreeObj. selectNode($("#3"));
ddTreeObj. removeNode($("#3"));

        });
    </script>

{% endhighlight %}


#### Example

{% highlight html %}
 
    <script>
       $("#itemList").ejDropDownTree("removeNode", $("#1"))
    </script>


{% endhighlight %}

### selectAll()
{:#methods:selectall}

Selects all the DropDownTree nodes when `allowMultiSelection` field is enabled in the treeViewSettings property.

#### Example

{% highlight html %}
 
<input type="text" id="itemList" />

<script type="text/javascript">
        var localData = [
                    { id: 1, name: "Windows Team", hasChild: true, expanded: true },
                    { id: 2, pid: 1, name: "Clark" },
                    { id: 3, pid: 1, name: "Wright" },
                    { id: 4, pid: 1, name: "Lopez" },
                    { id: 7, name: "Web Team", hasChild: true, expanded: true },
                    { id: 8, pid: 7, name: "Joshua" },
                    { id: 9, pid: 7, name: "Matthew" },
                    { id: 10, pid: 7, name: "David" },
                    { id: 11, name: "Build Team", hasChild: true },
                    { id: 12, pid: 11, name: "Ryan" },
                    { id: 13, pid: 11, name: "Justin" },
                    { id: 14, pid: 11, name: "Robert" }];
        $(function () {
            $('#itemList').ejDropDownTree({
                treeViewSettings: {
                       allowMultiSelection: true,
                    fields: { id: "id", parentId: "pid", value: "id", text: "name", hasChild: "hasChild", dataSource: localData, expanded: "expanded" }
                },
                value: "Ryan"
            });


    ddTreeObj = $('#itemList').data("ejDropDownTree");
ddTreeObj.selectAll();
        });
    </script>

{% endhighlight %}


{% highlight html %}
 
    <script>
      $('#itemList').ejDropDownTree('selectAll');
    </script>

{% endhighlight %}

### selectNode(node)
{:#methods:selectnode}

Selects a node in the DropDownTree control. To select the collection of nodes in the DropDownTree control, enable `allowMultiSelection` field of the treeViewSettings property.

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
<td class="name">element</td>
<td class="type">string|object|array</td>
<td class="description last"> ID of the DropDownTree node/object of the DropDownTree node/ collection 
of I the D/object of the DropDownTree nodes.
</td>
</tr>

</tbody>
</table>

#### Example

{% highlight html %}
 
<input type="text" id="itemList" />

<script type="text/javascript">
        var localData = [
                    { id: 1, name: "Windows Team", hasChild: true, expanded: true },
                    { id: 2, pid: 1, name: "Clark" },
                    { id: 3, pid: 1, name: "Wright" },
                    { id: 4, pid: 1, name: "Lopez" },
                    { id: 7, name: "Web Team", hasChild: true, expanded: true },
                    { id: 8, pid: 7, name: "Joshua" },
                    { id: 9, pid: 7, name: "Matthew" },
                    { id: 10, pid: 7, name: "David" },
                    { id: 11, name: "Build Team", hasChild: true },
                    { id: 12, pid: 11, name: "Ryan" },
                    { id: 13, pid: 11, name: "Justin" },
                    { id: 14, pid: 11, name: "Robert" }];
        $(function () {
            $('#itemList').ejDropDownTree({
                treeViewSettings: {
                       allowMultiSelection: true,
                    fields: { id: "id", parentId: "pid", value: "id", text: "name", hasChild: "hasChild", dataSource: localData, expanded: "expanded" }
                },
                value: "Ryan"
            });


    ddTreeObj = $('#itemList').data("ejDropDownTree");
ddTreeObj. selectNode($("#3"));
        });
    </script>

{% endhighlight %}


#### Example

{% highlight html %}
 
    <script>
       $("#itemList").ejDropDownTree("selectNode", $("#1"))
    </script>


{% endhighlight %}

### showPopup()
{:#methods:showpopup}

Shows the DropDownTree control with the popup.

#### Example

{% highlight html %}
 
<input type="text" id="itemList" />

<script type="text/javascript">
        var localData = [
                    { id: 1, name: "Windows Team", hasChild: true, expanded: true },
                    { id: 2, pid: 1, name: "Clark" },
                    { id: 3, pid: 1, name: "Wright" },
                    { id: 4, pid: 1, name: "Lopez" },
                    { id: 7, name: "Web Team", hasChild: true, expanded: true },
                    { id: 8, pid: 7, name: "Joshua" },
                    { id: 9, pid: 7, name: "Matthew" },
                    { id: 10, pid: 7, name: "David" },
                    { id: 11, name: "Build Team", hasChild: true },
                    { id: 12, pid: 11, name: "Ryan" },
                    { id: 13, pid: 11, name: "Justin" },
                    { id: 14, pid: 11, name: "Robert" }];
        $(function () {
            $('#itemList').ejDropDownTree({
                treeViewSettings: {
                    fields: { id: "id", parentId: "pid", value: "id", text: "name", hasChild: "hasChild", dataSource: localData, expanded: "expanded" }
                },
                value: "Ryan"
            });


    ddTreeObj = $('# itemList').data("ejDropDownTree");
ddTreeObj.showPopup();
        });
    </script>

{% endhighlight %}

{% highlight html %}
    <script>
        $('# itemList').ejDropDownTree("showPopup");
    </script>
{% endhighlight %}

### unCheckAll()
{:#methods:uncheckall}

Unchecks all the nodes in the DropDownTree.

#### Example

{% highlight html %}
 
<input type="text" id="itemList" />

<script type="text/javascript">
        var localData = [
                    { id: 1, name: "Windows Team", hasChild: true, expanded: true },
                    { id: 2, pid: 1, name: "Clark" },
                    { id: 3, pid: 1, name: "Wright" },
                    { id: 4, pid: 1, name: "Lopez" },
                    { id: 7, name: "Web Team", hasChild: true, expanded: true },
                    { id: 8, pid: 7, name: "Joshua" },
                    { id: 9, pid: 7, name: "Matthew" },
                    { id: 10, pid: 7, name: "David" },
                    { id: 11, name: "Build Team", hasChild: true },
                    { id: 12, pid: 11, name: "Ryan" },
                    { id: 13, pid: 11, name: "Justin" },
                    { id: 14, pid: 11, name: "Robert" }];
        $(function () {
            $('#itemList').ejDropDownTree({
                treeViewSettings: {
                    showCheckbox: true,
                    fields: { id: "id", parentId: "pid", value: "id", text: "name", hasChild: "hasChild", dataSource: localData, expanded: "expanded" }
                }
            });


    ddTreeObj = $('#itemList').data("ejDropDownTree");
ddTreeObj.unCheckAll ();
        });
    </script>

{% endhighlight %}


{% highlight html %}
 
    <script>
       $('#itemList').ejDropDownTree("unCheckAll")
    </script>

{% endhighlight %}

### unCheckNode(node)
{:#methods:unchecknode}

Unchecks a node in the DropDownTree.

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
<td class="name">element</td>
<td class="type">string|object|array</td>
<td class="description last">ID of the DropDownTree node/object of the DropDownTree node/collection 
of the ID/object of the DropDownTree nodes.
</td>
</tr>

</tbody>
</table>

#### Example

{% highlight html %}
 
input type="text" id="itemList" />

<script type="text/javascript">
        var localData = [
                    { id: 1, name: "Windows Team", hasChild: true, expanded: true },
                    { id: 2, pid: 1, name: "Clark" },
                    { id: 3, pid: 1, name: "Wright" },
                    { id: 4, pid: 1, name: "Lopez" },
                    { id: 7, name: "Web Team", hasChild: true, expanded: true },
                    { id: 8, pid: 7, name: "Joshua" },
                    { id: 9, pid: 7, name: "Matthew" },
                    { id: 10, pid: 7, name: "David" },
                    { id: 11, name: "Build Team", hasChild: true },
                    { id: 12, pid: 11, name: "Ryan" },
                    { id: 13, pid: 11, name: "Justin" },
                    { id: 14, pid: 11, name: "Robert" }];
        $(function () {
            $('#itemList').ejDropDownTree({
                treeViewSettings: {
                    showCheckbox: true,
                    fields: { id: "id", parentId: "pid", value: "id", text: "name", hasChild: "hasChild", dataSource: localData, expanded: "expanded" }
                },
                value: "Ryan"
            });


    ddTreeObj = $('#itemList').data("ejDropDownTree");
ddTreeObj.unCheckNode($('#1'));
        });
    </script>

{% endhighlight %}


{% highlight html %}
 
    <script>
      $("#itemList").ejDropDownTree("unCheckNode", $("#1"))
    </script>

{% endhighlight %}

### unselectAll()
{:#methods:unselectall}

Unselects all the DropDownTree nodes when `allowMultiSelection` field of the treeViewSettings property is enabled.

#### Example

{% highlight html %}
 
<input type="text" id="itemList" />

<script type="text/javascript">
        var localData = [
                    { id: 1, name: "Windows Team", hasChild: true, expanded: true },
                    { id: 2, pid: 1, name: "Clark" },
                    { id: 3, pid: 1, name: "Wright" },
                    { id: 4, pid: 1, name: "Lopez" },
                    { id: 7, name: "Web Team", hasChild: true, expanded: true },
                    { id: 8, pid: 7, name: "Joshua" },
                    { id: 9, pid: 7, name: "Matthew" },
                    { id: 10, pid: 7, name: "David" },
                    { id: 11, name: "Build Team", hasChild: true },
                    { id: 12, pid: 11, name: "Ryan" },
                    { id: 13, pid: 11, name: "Justin" },
                    { id: 14, pid: 11, name: "Robert" }];
        $(function () {
            $('#itemList').ejDropDownTree({
                treeViewSettings: {
                   allowMultiSelection: true,
                    fields: { id: "id", parentId: "pid", value: "id", text: "name", hasChild: "hasChild", dataSource: localData, expanded: "expanded" }
                }
            });


    ddTreeObj = $('#itemList').data("ejDropDownTree");
ddTreeObj.unselectAll ();
        });
    </script>

{% endhighlight %}


{% highlight html %}
 
    <script>
      $('#itemList').ejDropDownTree('unselectAll');
    </script>

{% endhighlight %}

### unselectNode(node)
{:#methods:unselectnode}

Unselects a node in the DropDownTree control. To unselect the collection of nodes in the DropDownTree control, enable `allowMultiSelection` field of the treeViewSettings property.

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
<td class="name">element</td>
<td class="type">string|object|array</td>
<td class="description last"> ID of the DropDownTree node/object of the DropDownTree node/ 
collection of the ID/object of the DropDownTree nodes.
</td>
</tr>

</tbody>
</table>

#### Example

{% highlight html %}
 
<input type="text" id="itemList" />

<script type="text/javascript">
        var localData = [
                    { id: 1, name: "Windows Team", hasChild: true, expanded: true },
                    { id: 2, pid: 1, name: "Clark" },
                    { id: 3, pid: 1, name: "Wright" },
                    { id: 4, pid: 1, name: "Lopez" },
                    { id: 7, name: "Web Team", hasChild: true, expanded: true },
                    { id: 8, pid: 7, name: "Joshua" },
                    { id: 9, pid: 7, name: "Matthew" },
                    { id: 10, pid: 7, name: "David" },
                    { id: 11, name: "Build Team", hasChild: true },
                    { id: 12, pid: 11, name: "Ryan" },
                    { id: 13, pid: 11, name: "Justin" },
                    { id: 14, pid: 11, name: "Robert" }];
        $(function () {
            $('#itemList').ejDropDownTree({
                treeViewSettings: {
                       allowMultiSelection: true,
                    fields: { id: "id", parentId: "pid", value: "id", text: "name", hasChild: "hasChild", dataSource: localData, expanded: "expanded" }
                },
                value: "Ryan"
            });


    ddTreeObj = $('#itemList').data("ejDropDownTree");
ddTreeObj. unselectNode($("#3"));
        });
    </script>

{% endhighlight %}


#### Example

{% highlight html %}
 
    <script>
      $("#itemList").ejDropDownTree("unselectNode", $("#1"));
    </script>


{% endhighlight %}

## Events

### blur
{:#events:blur}

Fires the action when the DropDownTree is about to lose focus.

<table class="params">
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
<td class="description">If the event has to be canceled; otherwise, false.</td>
</tr>
<tr>
<td class="name">type</td>
<td class="type"><span class="param-type">string</span></td>
<td class="description">Event name</td>
</tr>
<tr>
<td class="name">model</td>
<td class="type"><span class="param-type">object</span></td>
<td class="description">DropDownTreeView model.</td>
</tr>
</tbody>
</table>


#### Example

{% highlight html %}
 
<input type="text" id="itemList" />

<script type="text/javascript">

var localData = [
                   { id: 1, name: "Windows Team", hasChild: true, expanded: true },
                    { id: 2, pid: 1, name: "Clark" },
                    { id: 3, pid: 1, name: "Wright" },
                    { id: 4, pid: 1, name: "Lopez" },
                    { id: 7, name: "Web Team", hasChild: true, expanded: true },
                    { id: 8, pid: 7, name: "Joshua" },
                    { id: 9, pid: 7, name: "Matthew" },
                    { id: 10, pid: 7, name: "David" },
                    { id: 11, name: "Build Team", hasChild: true },
                    { id: 12, pid: 11, name: "Ryan" },
                    { id: 13, pid: 11, name: "Justin" },
                    { id: 14, pid: 11, name: "Robert" }];
        $(function () {
            $('#itemList').ejDropDownTree({
                treeViewSettings: {
                    fields: { id: "id", parentId: "pid", value: "id", text: "name", hasChild: "hasChild", dataSource: localData, expanded: "expanded" }
                },
                watermarkText: "Please select",
                width: "100%",
                blur: function (args){
                    //do your changes
                }
           });
       });
    </script>

  {% endhighlight %}

### change
{:#events:change}

Fires the action when the DropDownTree control's value is changed.

<table class="params">
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
<td class="description">If the event has to be canceled; otherwise, false.</td>
</tr>
<tr>
<td class="name">type</td>
<td class="type"><span class="param-type">string</span></td>
<td class="description">Event name</td>
</tr>
<tr>
<td class="name">model</td>
<td class="type"><span class="param-type">object</span></td>
<td class="description">DropDownTreeView model.</td>
</tr>
<tr>
<td class="name">selectedText</td>
<td class="type"><span class="param-type">string</span></td>
<td class="description">Selected item's text.</td>
</tr>
<tr>
<td class="name">text</td>
<td class="type"><span class="param-type">string</span></td>
<td class="description">Selected item's text.</td>
</tr>
<tr>
<td class="name">value</td>
<td class="type"><span class="param-type">string</span></td>
<td class="description">Selected item's value.</td>
</tr>
<tr>
<td class="name">itemId</td>
<td class="type"><span class="param-type">string</span></td>
<td class="description">Selected item's ID.</td>
</tr>
<tr>
<td class="name">isChecked</td>
<td class="type"><span class="param-type">boolean</span></td>
<td class="description">Returns the selected item with checkbox checked or not.</td>
</tr>
</tbody>
</table>


#### Example

{% highlight html %}
 
<input type="text" id="itemList" />

<script type="text/javascript">

var localData = [
                    { id: 1, name: "Windows Team", hasChild: true, expanded: true },
                    { id: 2, pid: 1, name: "Clark" },
                    { id: 3, pid: 1, name: "Wright" },
                    { id: 4, pid: 1, name: "Lopez" },
                    { id: 7, name: "Web Team", hasChild: true, expanded: true },
                    { id: 8, pid: 7, name: "Joshua" },
                    { id: 9, pid: 7, name: "Matthew" },
                    { id: 10, pid: 7, name: "David" },
                    { id: 11, name: "Build Team", hasChild: true },
                    { id: 12, pid: 11, name: "Ryan" },
                    { id: 13, pid: 11, name: "Justin" },
                    { id: 14, pid: 11, name: "Robert" }];
        $(function () {
            $('#itemList').ejDropDownTree({
                treeViewSettings: {
                    fields: { id: "id", parentId: "pid", value: "id", text: "name", hasChild: "hasChild", dataSource: localData, expanded: "expanded" }
                },
                watermarkText: "Please select",
                width: "100%",
                change: function (args){
                    //do your changes
                }
           });
       });
    </script>

  {% endhighlight %}

### checkChange
{:#events:checkchange}

Fires the action when the list item checkbox value is changed.

<table class="params">
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
<td class="description">If the event has to be canceled; otherwise, false.</td>
</tr>
<tr>
<td class="name">type</td>
<td class="type"><span class="param-type">string</span></td>
<td class="description">Event name</td>
</tr>
<tr>
<td class="name">model</td>
<td class="type"><span class="param-type">object</span></td>
<td class="description">DropDownTreeView model.</td>
</tr>
<td class="name">selectedText</td>
<td class="type"><span class="param-type">string</span></td>
<td class="description">Selected item's text.</td>
</tr>
<tr>
<td class="name">text</td>
<td class="type"><span class="param-type">string</span></td>
<td class="description">Selected item's text.</td>
</tr>
<tr>
<td class="name">value</td>
<td class="type"><span class="param-type">string</span></td>
<td class="description">Selected item's value.</td>
</tr>
<tr>
<td class="name">itemId</td>
<td class="type"><span class="param-type">string</span></td>
<td class="description">Selected item's ID.</td>
</tr>
<tr>
<td class="name">isChecked</td>
<td class="type"><span class="param-type">boolean</span></td>
<td class="description">Returns the selected item with checkbox checked or not.</td>
</tr>
</tbody>
</table>


#### Example

{% highlight html %}
 
<input type="text" id="itemList" />

<script type="text/javascript">

var localData = [
                    { id: 1, name: "Windows Team", hasChild: true, expanded: true },
                    { id: 2, pid: 1, name: "Clark" },
                    { id: 3, pid: 1, name: "Wright" },
                    { id: 4, pid: 1, name: "Lopez" },
                    { id: 7, name: "Web Team", hasChild: true, expanded: true },
                    { id: 8, pid: 7, name: "Joshua" },
                    { id: 9, pid: 7, name: "Matthew" },
                    { id: 10, pid: 7, name: "David" },
                    { id: 11, name: "Build Team", hasChild: true },
                    { id: 12, pid: 11, name: "Ryan" },
                    { id: 13, pid: 11, name: "Justin" },
                    { id: 14, pid: 11, name: "Robert" }];
        $(function () {
            $('#itemList').ejDropDownTree({
                treeViewSettings: {
                    showCheckbox: true,
                    fields: { id: "id", parentId: "pid", value: "id", text: "name", hasChild: "hasChild", dataSource: localData, expanded: "expanded" }
                },
                watermarkText: "Please select",
                width: "100%",
                checkChange: function (args){
                    //do your changes
                }
           });
       });
    </script>

  {% endhighlight %}

### close
{:#events:close}

Fires the action once the popup is closed.

<table class="params">
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
<td class="description">If the event has to be canceled; otherwise, false.</td>
</tr>
<tr>
<td class="name">type</td>
<td class="type"><span class="param-type">string</span></td>
<td class="description">Event name</td>
</tr>
<tr>
<td class="name">model</td>
<td class="type"><span class="param-type">object</span></td>
<td class="description">DropDownTreeView model.</td>
</tr>
<tr>
<td class="name">text</td>
<td class="type"><span class="param-type">string</span></td>
<td class="description">Selected item's text.</td>
</tr>
<tr>
<td class="name">value</td>
<td class="type"><span class="param-type">string</span></td>
<td class="description">Selected item's value.</td>
</tr>
</tbody>
</table>


#### Example

{% highlight html %}
 
<input type="text" id="itemList" />

<script type="text/javascript">

var localData = [
                    { id: 1, name: "Windows Team", hasChild: true, expanded: true },
                    { id: 2, pid: 1, name: "Clark" },
                    { id: 3, pid: 1, name: "Wright" },
                    { id: 4, pid: 1, name: "Lopez" },
                    { id: 7, name: "Web Team", hasChild: true, expanded: true },
                    { id: 8, pid: 7, name: "Joshua" },
                    { id: 9, pid: 7, name: "Matthew" },
                    { id: 10, pid: 7, name: "David" },
                    { id: 11, name: "Build Team", hasChild: true },
                    { id: 12, pid: 11, name: "Ryan" },
                    { id: 13, pid: 11, name: "Justin" },
                    { id: 14, pid: 11, name: "Robert" }];
        $(function () {
            $('#itemList').ejDropDownTree({
                treeViewSettings: {
                    fields: { id: "id", parentId: "pid", value: "id", text: "name", hasChild: "hasChild", dataSource: localData, expanded: "expanded" }
                },
                watermarkText: "Please select",
                width: "100%",
                close: function (args){
                    //do your changes
                }
           });
       });
    </script>

  {% endhighlight %}

### Create
{:#events:Create}

Fires the action once the DropDownTree is created.

<table class="params">
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
<td class="description">If the event has to be canceled; otherwise, false.</td>
</tr>
<tr>
<td class="name">type</td>
<td class="type"><span class="param-type">string</span></td>
<td class="description">Event name</td>
</tr>
<tr>
<td class="name">model</td>
<td class="type"><span class="param-type">object</span></td>
<td class="description">DropDownTreeView model.</td>
</tr>
</tbody>
</table>


#### Example

{% highlight html %}
 
<input type="text" id="itemList" />

<script type="text/javascript">

var localData = [
                    { id: 1, name: "Windows Team", hasChild: true, expanded: true },
                    { id: 2, pid: 1, name: "Clark" },
                    { id: 3, pid: 1, name: "Wright" },
                    { id: 4, pid: 1, name: "Lopez" },
                    { id: 7, name: "Web Team", hasChild: true, expanded: true },
                    { id: 8, pid: 7, name: "Joshua" },
                    { id: 9, pid: 7, name: "Matthew" },
                    { id: 10, pid: 7, name: "David" },
                    { id: 11, name: "Build Team", hasChild: true },
                    { id: 12, pid: 11, name: "Ryan" },
                    { id: 13, pid: 11, name: "Justin" },
                    { id: 14, pid: 11, name: "Robert" }];
        $(function () {
            $('#itemList').ejDropDownTree({
                treeViewSettings: {
                    fields: { id: "id", parentId: "pid", value: "id", text: "name", hasChild: "hasChild", dataSource: localData, expanded: "expanded" }
                },
                watermarkText: "Please select",
                width: "100%",
                create: function (args){
                    //do your changes
                }
           });
       });
    </script>

  {% endhighlight %}

### destroy
{:#events:destroy}

Fires the action when DropDownTree is destroyed.

<table class="params">
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
<td class="description">If the event has to be canceled; otherwise, false.</td>
</tr>
<tr>
<td class="name">type</td>
<td class="type"><span class="param-type">string</span></td>
<td class="description">Event name</td>
</tr>
<tr>
<td class="name">model</td>
<td class="type"><span class="param-type">object</span></td>
<td class="description">DropDownTreeView model.</td>
</tr>
</tbody>
</table>


#### Example

{% highlight html %}
 
<input type="text" id="itemList" />

<script type="text/javascript">

var localData = [
                    { id: 1, name: "Windows Team", hasChild: true, expanded: true },
                    { id: 2, pid: 1, name: "Clark" },
                    { id: 3, pid: 1, name: "Wright" },
                    { id: 4, pid: 1, name: "Lopez" },
                    { id: 7, name: "Web Team", hasChild: true, expanded: true },
                    { id: 8, pid: 7, name: "Joshua" },
                    { id: 9, pid: 7, name: "Matthew" },
                    { id: 10, pid: 7, name: "David" },
                    { id: 11, name: "Build Team", hasChild: true },
                    { id: 12, pid: 11, name: "Ryan" },
                    { id: 13, pid: 11, name: "Justin" },
                    { id: 14, pid: 11, name: "Robert" }];
        $(function () {
            $('#itemList').ejDropDownTree({
                treeViewSettings: {
                    fields: { id: "id", parentId: "pid", value: "id", text: "name", hasChild: "hasChild", dataSource: localData, expanded: "expanded" }
                },
                watermarkText: "Please select",
                width: "100%",
                destroy: function (args){
                    //do your changes
                }
           });
       });
    </script>

  {% endhighlight %}

### filtering
{:#events:filtering}

When the enableFilterSearch is enabled, the filtering action is fired as soon as you start typing in the DropDownTree.

<table class="params">
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
<td class="description">If the event has to be canceled; otherwise, false.</td>
</tr>
<tr>
<td class="name">type</td>
<td class="type"><span class="param-type">string</span></td>
<td class="description">Event name</td>
</tr>
<tr>
<td class="name">model</td>
<td class="type"><span class="param-type">object</span></td>
<td class="description">DropDownTreeView model.</td>
</tr>
<tr>
<td class="name">selectedText</td>
<td class="type"><span class="param-type">string</span></td>
<td class="description">Selected item's text.</td>
</tr>
<tr>
<td class="name">searchString</td>
<td class="type"><span class="param-type">string</span></td>
<td class="description">Returns the search string typed in the search box.</td>
</tr>
<tr>
<td class="name">items</td>
<td class="type"><span class="param-type">object</span></td>
<td class="description">Returns the data items of theDropDownTreeView.</td>
</tr>
</tbody>
</table>


#### Example

{% highlight html %}
 
<input type="text" id="itemList" />

<script type="text/javascript">

var localData = [
                    { id: 1, name: "Windows Team", hasChild: true, expanded: true },
                    { id: 2, pid: 1, name: "Clark" },
                    { id: 3, pid: 1, name: "Wright" },
                    { id: 4, pid: 1, name: "Lopez" },
                    { id: 7, name: "Web Team", hasChild: true, expanded: true },
                    { id: 8, pid: 7, name: "Joshua" },
                    { id: 9, pid: 7, name: "Matthew" },
                    { id: 10, pid: 7, name: "David" },
                    { id: 11, name: "Build Team", hasChild: true },
                    { id: 12, pid: 11, name: "Ryan" },
                    { id: 13, pid: 11, name: "Justin" },
                    { id: 14, pid: 11, name: "Robert" }];
        $(function () {
            $('#itemList').ejDropDownTree({
                treeViewSettings: {
                    fields: { id: "id", parentId: "pid", value: "id", text: "name", hasChild: "hasChild", dataSource: localData, expanded: "expanded" }
                },
                watermarkText: "Please select",
                width: "100%",
                filtering: function (args){
                    //do your changes
                }
           });
       });
    </script>

  {% endhighlight %}

### focus
{:#events:focus}

Fires the action when the DropDownTree is focused.

<table class="params">
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
<td class="description">If the event has to be canceled; otherwise, false.</td>
</tr>
<tr>
<td class="name">type</td>
<td class="type"><span class="param-type">string</span></td>
<td class="description">Event name</td>
</tr>
<tr>
<td class="name">model</td>
<td class="type"><span class="param-type">object</span></td>
<td class="description">DropDownTreeView model.</td>
</tr>
</tbody>
</table>


#### Example

{% highlight html %}
 
<input type="text" id="itemList" />

<script type="text/javascript">

var localData = [
                    { id: 1, name: "Windows Team", hasChild: true, expanded: true },
                    { id: 2, pid: 1, name: "Clark" },
                    { id: 3, pid: 1, name: "Wright" },
                    { id: 4, pid: 1, name: "Lopez" },
                    { id: 7, name: "Web Team", hasChild: true, expanded: true },
                    { id: 8, pid: 7, name: "Joshua" },
                    { id: 9, pid: 7, name: "Matthew" },
                    { id: 10, pid: 7, name: "David" },
                    { id: 11, name: "Build Team", hasChild: true },
                    { id: 12, pid: 11, name: "Ryan" },
                    { id: 13, pid: 11, name: "Justin" },
                    { id: 14, pid: 11, name: "Robert" }];
        $(function () {
            $('#itemList').ejDropDownTree({
                treeViewSettings: {
                    fields: { id: "id", parentId: "pid", value: "id", text: "name", hasChild: "hasChild", dataSource: localData, expanded: "expanded" }
                },
                watermarkText: "Please select",
                width: "100%",
                focus: function (args){
                    //do your changes
                }
           });
       });
    </script>

  {% endhighlight %}

### open
{:#events:open}

Fires the action once the popup is opened.

<table class="params">
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
<td class="description">If the event has to be canceled; otherwise, false.</td>
</tr>
<tr>
<td class="name">type</td>
<td class="type"><span class="param-type">string</span></td>
<td class="description">Event name</td>
</tr>
<tr>
<td class="name">model</td>
<td class="type"><span class="param-type">object</span></td>
<td class="description">DropDownTreeView model.</td>
</tr>
<tr>
<td class="name">text</td>
<td class="type"><span class="param-type">string</span></td>
<td class="description">Selected item's text.</td>
</tr>
<tr>
<td class="name">value</td>
<td class="type"><span class="param-type">string</span></td>
<td class="description">Selected item's value.</td>
</tr>
</tbody>
</table>


#### Example

{% highlight html %}
 
<input type="text" id="itemList" />

<script type="text/javascript">

var localData = [
                    { id: 1, name: "Windows Team", hasChild: true, expanded: true },
                    { id: 2, pid: 1, name: "Clark" },
                    { id: 3, pid: 1, name: "Wright" },
                    { id: 4, pid: 1, name: "Lopez" },
                    { id: 7, name: "Web Team", hasChild: true, expanded: true },
                    { id: 8, pid: 7, name: "Joshua" },
                    { id: 9, pid: 7, name: "Matthew" },
                    { id: 10, pid: 7, name: "David" },
                    { id: 11, name: "Build Team", hasChild: true },
                    { id: 12, pid: 11, name: "Ryan" },
                    { id: 13, pid: 11, name: "Justin" },
                    { id: 14, pid: 11, name: "Robert" }];
        $(function () {
            $('#itemList').ejDropDownTree({
                treeViewSettings: {
                    fields: { id: "id", parentId: "pid", value: "id", text: "name", hasChild: "hasChild", dataSource: localData, expanded: "expanded" }
                },
                watermarkText: "Please select",
                width: "100%",
                open: function (args){
                    //do your changes
                }
           });
       });
    </script>

  {% endhighlight %}

### select
{:#events:select}

Fires the action when the list of nodes in the DropDownTree is selected.

<table class="params">
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
<td class="description">If the event has to be canceled; otherwise, false.</td>
</tr>
<tr>
<td class="name">type</td>
<td class="type"><span class="param-type">string</span></td>
<td class="description">Event name</td>
</tr>
<tr>
<td class="name">model</td>
<td class="type"><span class="param-type">object</span></td>
<td class="description">DropDownTreeView model.</td>
</tr>
<td class="name">selectedText</td>
<td class="type"><span class="param-type">string</span></td>
<td class="description">Selected item's text.</td>
</tr>
<tr>
<td class="name">text</td>
<td class="type"><span class="param-type">string</span></td>
<td class="description">Selected item's text.</td>
</tr>
<tr>
<td class="name">value</td>
<td class="type"><span class="param-type">string</span></td>
<td class="description">Selected item's value.</td>
</tr>
<tr>
<td class="name">itemId</td>
<td class="type"><span class="param-type">string</span></td>
<td class="description">Selected item's ID.</td>
</tr>
<tr>
<td class="name">isChecked</td>
<td class="type"><span class="param-type">boolean</span></td>
<td class="description">Returns the selected item with checkbox checked or not.</td>
</tr>
</tbody>
</table>


#### Example

{% highlight html %}
 
<input type="text" id="itemList" />

<script type="text/javascript">

var localData = [
                   { id: 1, name: "Windows Team", hasChild: true, expanded: true },
                    { id: 2, pid: 1, name: "Clark" },
                    { id: 3, pid: 1, name: "Wright" },
                    { id: 4, pid: 1, name: "Lopez" },
                    { id: 7, name: "Web Team", hasChild: true, expanded: true },
                    { id: 8, pid: 7, name: "Joshua" },
                    { id: 9, pid: 7, name: "Matthew" },
                    { id: 10, pid: 7, name: "David" },
                    { id: 11, name: "Build Team", hasChild: true },
                    { id: 12, pid: 11, name: "Ryan" },
                    { id: 13, pid: 11, name: "Justin" },
                    { id: 14, pid: 11, name: "Robert" }];
        $(function () {
            $('#itemList').ejDropDownTree({
                treeViewSettings: {
                    fields: { id: "id", parentId: "pid", value: "id", text: "name", hasChild: "hasChild", dataSource: localData, expanded: "expanded" }
                },
                watermarkText: "Please select",
                width: "100%",
                select: function (args){
                    //do your changes
                }
           });
       });
    </script>

  {% endhighlight %}
