---
layout: post
title: Properties, Methods and Events of ejPager Widget
description: Methods,members and events avaliable in ejPager
documentation: API
platform: js-api
keywords: ejPager, API, Essential JS Pager
metaname: 
metacontent: 
---

# Pager

Custom Design for HTML Pager control.


#### Syntax

{% highlight javascript %}

$(element).ejPager()

{% endhighlight %}



#### Example

{% highlight html %}
 
<div id="pager"></div> 
 
<script>
// Create ejPager
pagerModel = {pageSize:5,pageCount:5,currentPage:1}
$("#pager").ejPager(pagerModel);     
</script>

{% endhighlight %}


#### Requires

* module:jQuery
* module:ej.core.js
* module:ej.touch.js
* module:ej.pager.js


## Members


### customText `string`
{:#members:customText}

Gets or sets a value that indicates whether to display the custom text message in Pager.

#### Default Value:
{:.param}
* ""

#### Example
{:.example}
{% highlight html %}
<div id="pager"></div> 
<script>
$("#pager").ejPager({customText ="custom pager text"})
});
</script>

{% endhighlight %}


### currentPage `number`
{:#members:currentpage}

Gets or sets a value that indicates whether to define which page to display currently in pager.

#### Default Value:
{:.param}
* 1

#### Example
{:.example}
{% highlight html %}
<div id="pager"></div> 
<script>
$("#pager").ejPager({currentPage: 1 })
});
</script>
{% endhighlight %}


### enableExternalMessage `boolean`
{:#members:enableExternalMessage}

Gets or sets a value that indicates whether to display the external Message in Pager.

#### Default Value:
{:.param}
* false

#### Example
{:.example}
{% highlight html %}
<div id="pager"></div> 
<script>
$("#pager").ejPager({enableExternalMessage: true })
});
</script>

{% endhighlight %}


### enableQueryString `boolean`
{:#members:enablequerystring}

Gets or sets a value that indicates whether to pass the current page information as a query string along with the URL while navigating to other page.

#### Default Value:
{:.param}
* false

#### Example
{:.example}
{% highlight html %}
<div id="pager"></div> 
<script>
$("#pager").ejPager({enableQueryString: true })
});
</script>

{% endhighlight %}



### enableRTL `boolean`
{:#members:enablertl}

Align content in the pager control from right to left by setting the property as true.

#### Default Value:
{:.param}
* false

#### Example
{:.example}
{% highlight html %}
<div id="pager"></div> 
<script>
$("#pager").ejPager({enableRTL:true})
});
</script>
{% endhighlight %}


### externalMessage `string`
{:#members:externalMessage}

Gets or sets a value that indicates whether to display the external Message in Pager.

#### Default Value:
{:.param}
* ""

#### Example
{:.example}
{% highlight html %}
<div id="pager"></div> 
<script>
$("#pager").ejPager({enableExternalMessage: true, externalMessage:"external message in Pager" })
});
</script>

{% endhighlight %}

N> `enableExternalMessage` default value as false. so We must enable `enableExternalMessage` set as true when enable externalMessage.


### locale `string`
{:#members:locale}

Gets or sets a value that indicates whether to customizing the user interface (UI) as locale-specific in order to display regional data i.e. in a language and culture specific to a particular country or region.

#### Default Value:
{:.param}
* "en-US"

#### Example
{:.example}
{% highlight html %} 
<div id="pager"></div> 
<script>
ej.Pager.locale["es-ES"] = {
   pagerInfo: "{0} de {1} p&aacute;ginas ({2} art&iacute;culos)"
};
$("#pager").ejPager({locale: "es-ES"})
});
</script>
{% endhighlight %}


### pageCount `number`
{:#members:pagecount}

Gets or sets a value that indicates whether to define the number of pages displayed in the pager for navigation.

#### Default Value:
{:.param}
* 10

#### Example
{:.example}
{% highlight html %}
<div id="pager"></div> 
<script>
$("#pager").ejPager({pageCount: 5 })
});
</script>
{% endhighlight %}


### pageSize `number`

{:#members:pagesize}

Gets or sets a value that indicates whether to define the number of records displayed per page.

#### Default Value
{:.param}
* 12

#### Example
{:.example}
{% highlight html %}
<div id="pager"></div> 
<script>
$("#pager").ejPager({pageSize: 2 })
});
</script>
{% endhighlight %}


### pageSizeList `Array`

{:#members:pagesizelist}

It allows to have multiple choices of pageSize values for Pager control. The "[pageSize](https://help.syncfusion.com/api/js/ejpager#members:pagesize)" API value of the pager will be updated depending upon the value being selected from the dropdown.

#### Default Value
{:.param}
* null

#### Example

{:.example}
{% highlight html %}

<div id="pager"></div> 

<script>
// Set pageSizeList value during initialization.
$("#pager").ejPager({pageSizeList: [1,2,3] })

</script>

{% endhighlight %}


### totalPages `number`
{:#members:totalpages}

Get or sets a value of total number of pages in the pager. The totalPages value is calculated based on page size and total records.

#### Default Value:
{:.param}
* null

#### Example
{:.example}
{% highlight html %}
<div id="pager"></div> 
<script>
$("#pager").ejPager({totalPages: 1 })
});
</script>
{% endhighlight %}

### totalRecordsCount `number`
{:#members:totalrecordscount}

Get the value of total number of records which is bound to a data item. 

#### Default Value:
{:.param}
* null

#### Example
{:.example}
{% highlight html %}
<div id="pager"></div> 
<script>
$("#pager").ejPager({totalRecordsCount: 10 })
});
</script>
{% endhighlight %}

### showPageInfo `boolean`
{:#members:showpageinfo}

Shows or hides the current page information in pager footer.

#### Default Value:
{:.param}
* true

#### Example
{:.example}

{% highlight html %}

<div id="pager"></div> 
<script>
$("#pager").ejPager({showPageInfo:false})
});
</script>

{% endhighlight %}


## Methods

### gotoPage(pageIndex)
{:#methods:gotopage}

Send a paging request to specified page through the pager control.

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
<td class="name">pageIndex</td>
<td class="type">number</td>
<td class="description last">Specifies the index to be navigated</td>
</tr>
</tbody>
</table>

#### Example

{:.example}


{% highlight html %}


<div class="frame">
    <ul id="sliderContent">
    <li><img class="image" src="http://jsplayground.syncfusion.com/{{ site.releaseversion }}/themes/web/content/images/rotator/nature.jpg" title="Nature" /></li>
    <li><img class="image" src="http://jsplayground.syncfusion.com/{{ site.releaseversion }}/themes/web/content/images/rotator/bird.jpg" title="Beautiful Bird" /></li>
    <li><img class="image" src="http://jsplayground.syncfusion.com/{{ site.releaseversion }}/themes/web/content/images/rotator/sculpture.jpg" title="Amazing Sculptures" /></li>
    <li><img class="image" src="http://jsplayground.syncfusion.com/{{ site.releaseversion }}/themes/web/content/images/rotator/seaview.jpg"  title="Sea-View"/></li>
    <li><img class="image" src="http://jsplayground.syncfusion.com/{{ site.releaseversion }}/themes/web/content/images/rotator/snowfall.jpg"  title="Snow Fall"/></li>
    <li><img class="image" src="http://jsplayground.syncfusion.com/{{ site.releaseversion }}/themes/web/content/images/rotator/card.jpg"  title="Credit Card"/></li>
    <li><img class="image" src="http://jsplayground.syncfusion.com/{{ site.releaseversion }}/themes/web/content/images/rotator/night.jpg"  title="Colorful Night"/></li>
    </ul>
</div>
<script type="text/javascript">
    $(function () {
    // declaration
    $("#sliderContent").ejRotator({
        slideWidth: "600px",
        frameSpace: "0px",
        showPager: true,
    });
    var obj = $("#sliderContent").ejRotator("instance")
    $('.e-pager-wrap').css('display', 'none')
    $("<div id='pager' style='width:600px'></div>").appendTo($("body"));
    $('#pager').ejPager({
        pageSize:1, totalPages: 7, totalRecordsCount:7, pageCount: 3, click: "page" })
                        
    });
    function page(args) {
    if(!ej.isNullOrUndefined(args.event)){
        this.goToPage(args.model.currentPage); // pager moved to the specified page
        this.refreshPager(); // refresh the pager control
        var obj = $("#sliderContent").ejRotator("instance").gotoIndex(args.currentPage);
    }
    }
</script>
<style type="text/css" class="cssStyles">
    .frame {
    width: 600px;
    }
    #sliderContent > li .image {
    width: 600px;
    height: 350px;
    }
</style>

{% endhighlight %}


### refreshPager()
{:#methods:refreshpager}

`refreshPager()` helps to refresh the model value of pager control.

#### Example

{% highlight html %}
 
<div id="pager"></div> 
 
<script>
$('#pager').ejPager();
var pgObj = $("#pager").data("ejPager");
pgObj.refreshPager(); 
</script>

{% endhighlight %}



## Events

### click
{:#events:click}

Triggered when pager numeric item is clicked in pager control.

<table class="params">
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
<td class="description">Returns the cancel option value.</td>
</tr>
<tr>
<td class="name">currentPage</td>
<td class="type"><span class="param-type">number</span></td>
<td class="description">Returns the current page index.</td>
</tr>
<tr>
<td class="name">model</td>
<td class="type"><span class="param-type">object</span></td>
<td class="description">Returns the pager model.</td>
</tr>
<tr>
<td class="name">type</td>
<td class="type"><span class="param-type">string</span></td>
<td class="description">Returns the name of event</td>
</tr>
<tr>
<td class="name">event</td>
<td class="type"><span class="param-type">object</span></td>
<td class="description">Returns current action event type and its target.</td>
</tr>
</tbody>
</table>

####Example
{:.example}

{% highlight html %}

<div id="pager"></div> 
<script>
$("#pager").ejPager({
   click: function (args) {}
});
</script>

{% endhighlight %}
