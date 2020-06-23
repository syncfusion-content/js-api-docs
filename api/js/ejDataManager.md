---
layout: post
title: Essential JS ejDataManager Widget | Syncfusion
description: You can learn about how to use Properties, options, methods and events of Essential JS ejDataManager widget here.
documentation: UG
platform: js-api
metaname: 
metacontent: 
---

# API Reference for ejDataManager
<ts  isFrameWork="true" />

Communicates with data source and returns the desired result based on the Query provided.


#### Syntax

{% highlight html %}

var dataManager = new ej.DataManager(datasource, query, adaptor)

{% endhighlight %}

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
<td class="name">datasource</td>
<td class="type"><span class="param-type">Object</span></td>
<td class="description last">Sets the data source to create the Data Manager.</td>
</tr>
<tr>
<td class="name">query</td>
<td class="type"><span class="param-type">ej.Query</span></td>
<td class="description last">Sets the default query for the data source.</td>
</tr>
<tr>
<td class="name">adaptor</td>
<td class="type"><span class="param-type">Object</span></td>
<td class="description last">Configures the adaptor based on the data source type of the Data Manager.</td>
</tr>
</tbody>
</table>

#### Example
{:.example}

{% highlight html %}

    <style>
        .table,tr,td{ border:1px solid; padding:3px;}
    </style>
    <table class="table" style="border-collapse:collapse">
        <tbody></tbody>
    </table>

    <script>
        var dataManger = ej.DataManager(window.gridData);
        var tableBody = ""; 
        for(var i=0;i<5;i++)
        { 
            row="dataManger.dataSource.json[0];;" 
            tableBody="" +="String.format("<tr><td>{0}</td><td>{1}</td><td>{2}</td><td>{3}</td><td>{4}</td></tr>"," row.OrderID,="" row.CustomerID,="" row.EmployeeID,="" row.ShipCity,="" row.freight);
            $(".table="" tbody").html(tableBody);
        }
    </script>

{% endhighlight %}
 
## Callback Functions

### beforeSend(request, settings)
{:#callbackfunctions:beforesend}

Custom headers can be set using pre-request callback beforeSend as follows. The setRequestHeader method can be used to modify the XMLHTTPRequest.

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
<td class="name">request</td>
<td class="type"><span class="param-type">Object</span></td>
<td class="description last">Sets the default query for the data source.</td>
</tr>
<tr>
<td class="name">settings</td>
<td class="type"><span class="param-type">Object</span></td>
<td class="description last">A set of key/value pairs that configure the AJAX request.</td>
</tr>
</tbody>
</table>

#### Example
{:.example}

{% highlight html %}

    <div class="datatable" style="padding:10px">
        <table id="table1" class="table table-striped table-bordered" style="width:700px" >
            <thead>
            <tr>
                <th>Order ID</th>
                <th>Customer ID</th>
                <th>Employee ID</th>
            </tr>
            </thead>
            <tbody></tbody>
        </table>
    </div>
    <script type="text/javascript">
        $(function () {
            var customAdaptor = new ej.UrlAdaptor().extend({
                beforeSend: function (request, settings) {
                    settings.setRequestHeader("myData1", "Syncfusion");
                    settings.setRequestHeader("myData2", 23243);
                
                }
            });

            var dataManager1 = ej.DataManager({ url: "TreeViewFeatures.aspx/Data", adaptor: new customAdaptor() });
            var query = ej.Query().take(3).skip(2);
            var execute = dataManager1.executeQuery(query) // executing query
                    .done(function (e) {
                        renderTable(e.result);
                    });
        });
    </script>
  
{% endhighlight %}

### done(args)
{:#callbackfunctions:done}

A function to be called if the request succeeds.

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
<td class="name">result</td>
<td class="type"><span class="param-type">Object</span></td>
<td class="description last">Contains filtered results on the data based on query.</td>
</tr>
<tr>
<td class="name">query</td>
<td class="type"><span class="param-type">ej.Query</span></td>
<td class="description last">A set of key/value pairs that configure the AJAX request.</td>
</tr>
<tr>
<td class="name">xhr</td>
<td class="type"><span class="param-type">Object</span></td>
<td class="description last">XMLHTTPRequest object.</td>
</tr>
<tr>
<td class="name">actual</td>
<td class="type"><span class="param-type">Object</span></td>
<td class="description last">Contains all the records as it is from the data source.</td>
</tr>
<tr>
<td class="name">getKnockoutModel</td>
<td class="type"><span class="param-type">function</span></td>
<td class="description last">The DataManager contains a default method to subscribe the view model properties as KO observable. This is done at the success of the executeQuery using the getKnockoutModel. You can also provide computed properties to the view model using the getKnockoutModel.</td>
</tr>
<tr>
<td class="name">getTableModel</td>
<td class="type"><span class="param-type">function</span></td>
<td class="description last">The DataManager contains a default support to bind a TableModel to the element. You can make the data observable using the getTableModel method. The getTableModel method also accept extra properties or properties with computed value that can be added to the TableModel. In the view, you can create a simple view by using the bindings getTableModel</td>
</tr>
<tr>
<td class="name">count</td>
<td class="type"><span class="param-type">number</span></td>
<td class="description last">Contains total count of records when the requiresCount() method is enabled in the ej.Query()</td>
</tr>
<tr>
<td class="name">request</td>
<td class="type"><span class="param-type">Object</span></td>
<td class="description last">Contains all the necessary data before posting a request</td>
</tr>
<tr>
<td class="name">aggregates</td>
<td class="type"><span class="param-type">Object</span></td>
<td class="description last">Aggregates data such as sum, average , min and max</td>
</tr>
<tr>
<td class="name">virtualSelectRecords</td>
<td class="type"><span class="param-type">Object</span></td>
<td class="description last">It will have virtually loaded records, when the lazy loading or virtual scrolling is enabled.</td>
</tr>
</tbody>
</table>

#### Example
{:.example}

{% highlight html %}

    <div class="datatable">
        <table id="table1" class="table table-striped table-bordered" style="width:700px">
            <thead>
                <tr>
                    <th>ItemID</th>
                    <th>ItemName</th>
                    <th>ItemType</th>
                </tr>
            </thead>
            <tbody></tbody>
        </table>
    </div>

<script type="text/javascript">
    $(function () {

        var dataManager = ej.DataManager({
            url: "http://mvc.syncfusion.com/Services/Northwnd.svc/Foods",
            crossDomain: true
        });
        var query = ej.Query()
            .sortBy("ItemID", "descending", false)
                .select("ItemID", "ItemName", "ItemType")
        var updateData = { ItemID: 14, ItemName: "Grapes Juice", ItemType: "Veg" };
        dataManager.update("ItemID", updateData);
        // executing query
        var dataSource = dataManager.executeQuery(query).done(function (args) {
            // Result is successful
            renderTable(args.result);
        });
    });

    // This function can be better replaced with any template engine. We used this for simplicity in demo.
    function renderTable(data) {
        var tableBody = "", row;
        for (var i = 0; i < data.length; i++) {
            row = data[i];
            tableBody += String.format("<tr><td>{0}</td><td>{1}</td><td>{2}</td></tr>", row.ItemID, row.ItemName, row.ItemType);
        }
        $(".table tbody").html(tableBody);
    }
</script>

{% endhighlight %}

### fail(args)
{:#callbackfunctions:fail}

A function to be called if the request fails.

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
<td class="name">query</td>
<td class="type"><span class="param-type">ej.Query</span></td>
<td class="description last">A set of key/value pairs that configure the AJAX request.</td>
</tr>
<tr>
<td class="name">error</td>
<td class="type"><span class="param-type">Object</span></td>
<td class="description last">When an HTTP error occurs, error thrown receives error status of HTTP object.</td>
</tr>
</tbody>
</table>

#### Example
{:.example}

{% highlight html %}

    <div class="datatable">
        <table id="table1" class="table table-striped table-bordered" style="width:700px">
            <thead>
                <tr>
                    <th>ItemID</th>
                    <th>ItemName</th>
                    <th>ItemType</th>
                </tr>
            </thead>
            <tbody></tbody>
        </table>
    </div>

<script type="text/javascript">
    $(function () {

        var dataManager = ej.DataManager({
            url: "http://mvc.syncfusion.com/Services/Northwnd.svc/Foods",
            crossDomain: true
        });
        var query = ej.Query()
            .sortBy("ItemID", "descending", false)
                .select("ItemID", "ItemName", "ItemType")
        var updateData = { ItemID: 14, ItemName: "Grapes Juice", ItemType: "Veg" };
        dataManager.update("ItemID", updateData);
        // executing query
        var dataSource = dataManager.executeQuery(query).done(function (args) {

        renderTable(args.result);
        }).fail(function (args) {
            // handling of error
        });

    });

    // This function can be better replaced with any template engine. We used this for simplicity in demo.
    function renderTable(data) {
        var tableBody = "", row;
        for (var i = 0; i < data.length; i++) {
            row = data[i];
            tableBody += String.format("<tr><td>{0}</td><td>{1}</td><td>{2}</td></tr>", row.ItemID, row.ItemName, row.ItemType);
        }
        $(".table tbody").html(tableBody);
    }
</script>

{% endhighlight %}

### always(args)
{:#callbackfunctions:always}

A function to be called when the request finishes (after success and error callbacks are executed).

If the request is success, arguments list will be as below.

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
<td class="name">result</td>
<td class="type"><span class="param-type">Object</span></td>
<td class="description last">Contains filtered results on the data based on query.</td>
</tr>
<tr>
<td class="name">query</td>
<td class="type"><span class="param-type">ej.Query</span></td>
<td class="description last">A set of key/value pairs that configure the AJAX request.</td>
</tr>
<tr>
<td class="name">xhr</td>
<td class="type"><span class="param-type">Object</span></td>
<td class="description last">XMLHTTPRequest object.</td>
</tr>
<tr>
<td class="name">actual</td>
<td class="type"><span class="param-type">Object</span></td>
<td class="description last">Contains all the records as it is from the data source.</td>
</tr>
<tr>
<td class="name">getKnockoutModel</td>
<td class="type"><span class="param-type">function</span></td>
<td class="description last">The DataManager contains a default method to subscribe the view model properties as KO observable. This is done at the success of the executeQuery using the getKnockoutModel. You can also provide computed properties to the view model using the getKnockoutModel.</td>
</tr>
<tr>
<td class="name">getTableModel</td>
<td class="type"><span class="param-type">function</span></td>
<td class="description last">The DataManager contains a default support to bind a TableModel to the element. You can make the data observable using the getTableModel method. The getTableModel method also accept extra properties or properties with computed value that can be added to the TableModel. In the view, you can create a simple view by using the bindings getTableModel</td>
</tr>
<tr>
<td class="name">count</td>
<td class="type"><span class="param-type">number</span></td>
<td class="description last">Contains total count of records when the requiresCount() method is enabled in the ej.Query()</td>
</tr>
<tr>
<td class="name">request</td>
<td class="type"><span class="param-type">Object</span></td>
<td class="description last">Contains all the necessary data before posting a request</td>
</tr>
<tr>
<td class="name">aggregates</td>
<td class="type"><span class="param-type">Object</span></td>
<td class="description last">Aggregates data such as sum, average , min and max</td>
</tr>
<tr>
<td class="name">virtualSelectRecords</td>
<td class="type"><span class="param-type">Object</span></td>
<td class="description last">It will have virtually loaded records, when the lazy loading or virtual scrolling is enabled.</td>
</tr>
</tbody>
</table>

If the request is fail, the argument list will be as below.

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
<td class="name">query</td>
<td class="type"><span class="param-type">ej.Query</span></td>
<td class="description last">A set of key/value pairs that configure the AJAX request.</td>
</tr>
<tr>
<td class="name">error</td>
<td class="type"><span class="param-type">Object</span></td>
<td class="description last">When an HTTP error occurs, error thrown receives error status of HTTP object.</td>
</tr>
</tbody>
</table>

#### Example
{:.example}

{% highlight html %}

    <div class="datatable">
        <table id="table1" class="table table-striped table-bordered" style="width:700px">
            <thead>
                <tr>
                    <th>ItemID</th>
                    <th>ItemName</th>
                    <th>ItemType</th>
                </tr>
            </thead>
            <tbody></tbody>
        </table>
    </div>

<script type="text/javascript">
    $(function () {

        var dataManager = ej.DataManager({
            url: "http://mvc.syncfusion.com/Services/Northwnd.svc/Foods",
            crossDomain: true
        });
        var query = ej.Query()
            .sortBy("ItemID", "descending", false)
                .select("ItemID", "ItemName", "ItemType")
        var updateData = { ItemID: 14, ItemName: "Grapes Juice", ItemType: "Veg" };
        dataManager.update("ItemID", updateData);
        // executing query
        var dataSource = dataManager.executeQuery(query).always(function (args) {
                // if it is success result can be obtained otherwise it display the error report
                renderTable(args.result);
        });
    });

    // This function can be better replaced with any template engine. We used this for simplicity in demo.
    function renderTable(data) {
        var tableBody = "", row;
        for (var i = 0; i < data.length; i++) {
            row = data[i];
            tableBody += String.format("<tr><td>{0}</td><td>{1}</td><td>{2}</td></tr>", row.ItemID, row.ItemName, row.ItemType);
        }
        $(".table tbody").html(tableBody);
    }
</script>

{% endhighlight %}


## Methods

### executeLocal(query)
{:#methods:executelocal}

This method does not execute more than one operation at a time; it waits for one operation to complete, and then executes the next operation.

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
<td class="name">query</td>
<td class="type"><span class="param-type">ej.Query</span></td>
<td class="description last">Sets the default query for the data source.</td>
</tr>
</tbody>
</table>

#### Returns:
{:#methods:returns:}

JQueryPromise

#### Example
{:.example}

{% highlight html %}

    <div class="datatable">
        <table id="table1" class="table table-striped table-bordered" style="width:700px">
            <thead>
                <tr>
                    <th>Order ID</th>
                    <th>Customer ID</th>
                    <th>Employee ID</th>
                </tr>
            </thead>
            <tbody></tbody>
        </table>
    </div>

<script type="text/javascript">
    $(function () {

        var data = [{ OrderID: 10248, CustomerID: "VINET", EmployeeID: 5 },
                        { OrderID: 10249, CustomerID: "AANAR", EmployeeID: 9 },
                        { OrderID: 10250, CustomerID: "VICTE", EmployeeID: 2 },
                        { OrderID: 10251, CustomerID: "TOMSP", EmployeeID: 7 },
                        { OrderID: 10252, CustomerID: "SUPRD", EmployeeID: 6 }];
        var dataManager = ej.DataManager(data);
        var query = ej.Query()
            .from("Orders")
            .sortBy("OrderID", "descending", false)
        // executing query
        var dataSource = dataManager.executeLocal(query);
        renderTable(dataSource);

    });

    // This function can be better replaced with any template engine. We used this for simplicity in demo.
    function renderTable(data) {
        var tableBody = "", row;
        for (var i = 0; i < data.length; i++) {
            row = data[i];
            tableBody += String.format("<tr><td>{0}</td><td>{1}</td><td>{2}</td></tr>", row.OrderID, row.CustomerID, row.EmployeeID);
        }
        $(".table tbody").html(tableBody);
    }
</script>

{% endhighlight %}

### executeQuery(query, done, fail, always)
{:#methods:executequery}

The executeQuery property is used to process the data based on the query on URL Binding.

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
<td class="name">query</td>
<td class="type"><span class="param-type">ej.Query</span></td>
<td class="description last">Sets the default query for the data source.</td>
</tr>
<tr>
<td class="name">done</td>
<td class="type"><span class="param-type">function</span></td>
<td class="description last">A function to be called if the request succeeds.</td>
</tr>
<tr>
<td class="name">fail</td>
<td class="type"><span class="param-type">function</span></td>
<td class="description last">A function to be called if the request fails.</td>
</tr>
<tr>
<td class="name">always</td>
<td class="type"><span class="param-type">function</span></td>
<td class="description last">A function to be called when the request finishes (after success and error callbacks are executed).</td>
</tr>
</tbody>
</table>

#### Returns:
{:#methods:returns:}

JQueryPromise

#### Example
{:.example}

{% highlight html %}

<script>

    var dataManager = ej.DataManager("http://mvc.syncfusion.com/Services/Northwnd.svc/");
    var query =  ej.Query().select(["OrderID", "CustomerID", "ShipName"]).from("Orders").take(3);
    var promise = dataManager.executeQuery(query);
    promise.done(function(e){});
    promise.fail(function(e){});

</script>

{% endhighlight %}


### insert(data, tableName, query)
{:#methods:insert}

Inserts a data item in the data table.

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
<td class="type"><span class="param-type">Object</span></td>
<td class="description last">JSON data or JSON array</td>
</tr>
<tr>
<td class="name">tableName</td>
<td class="type"><span class="param-type">string</span></td>
<td class="description last">Name of the table</td>
</tr>
<tr>
<td class="name">query</td>
<td class="type"><span class="param-type">ej.Query</span></td>
<td class="description last">Sets the default query for the data source.</td>
</tr>
</tbody>
</table>
 
#### Returns:
{:#methods:returns:}

Object
 
#### Example
{:.example}

{% highlight html %}

    <div class="datatable">
        <table id="table1" class="table table-striped table-bordered" style="width:700px">
            <thead>
                <tr>
                    <th>Order ID</th>
                    <th>Customer ID</th>
                    <th>Employee ID</th>
                </tr>
            </thead>
            <tbody></tbody>
        </table>
    </div>

<script type="text/javascript">

    $(function () {

        var data = [{ OrderID: 10248, CustomerID: "VINET", EmployeeID: 5 },
                        { OrderID: 10249, CustomerID: "AANAR", EmployeeID: 9 },
                        { OrderID: 10250, CustomerID: "VICTE", EmployeeID: 2 },
                        { OrderID: 10251, CustomerID: "TOMSP", EmployeeID: 7 },
                        { OrderID: 10252, CustomerID: "SUPRD", EmployeeID: 6 }];
        var dataManager = ej.DataManager(data);
        var query = ej.Query()
            .from("Orders")
            .sortBy("OrderID", "descending", false)
        var record = { OrderID: 10253, CustomerID: "STRPQ", EmployeeID: 4 };
        dataManager.insert(record);
        // executing query
        var dataSource = dataManager.executeLocal(query);
        renderTable(dataSource);

    });

    // This function can be better replaced with any template engine. We used this for simplicity in demo.
    function renderTable(data) {
        var tableBody = "", row;
        for (var i = 0; i < data.length; i++) {
            row = data[i];
            tableBody += String.format("<tr><td>{0}</td><td>{1}</td><td>{2}</td></tr>", row.OrderID, row.CustomerID, row.EmployeeID);
        }
        $(".table tbody").html(tableBody);
    }

</script>

{% endhighlight %}
 
 
### remove(keyField, value, tableName, query)
{:#methods:remove}

It is used to remove the data from the dataSource.

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
<td class="name">keyField</td>
<td class="type"><span class="param-type">string</span></td>
<td class="description last">KeyColumn to find the data</td>
</tr>
<tr>
<td class="name">value</td>
<td class="type"><span class="param-type">string</span></td>
<td class="description last">Specified value for the keyField</td>
</tr>
<tr>
<td class="name">tableName </td>
<td class="type"><span class="param-type">string</span></td>
<td class="description last">Name of the source table</td>
</tr>
<tr>
<td class="name">query</td>
<td class="type"><span class="param-type">ej.Query</span></td>
<td class="description last">Sets the default query for the data source.</td>
</tr>
</tbody>
</table>

#### Returns:
{:#methods:returns:}

Object

#### Example
{:.example}

{% highlight html %}

    <div class="datatable">
        <table id="table1" class="table table-striped table-bordered" style="width:700px">
            <thead>
                <tr>
                    <th>Order ID</th>
                    <th>Customer ID</th>
                    <th>Employee ID</th>
                </tr>
            </thead>
            <tbody></tbody>
        </table>
    </div>

<script type="text/javascript">

    $(function () {
        var query = ej.Query().sortByDesc("EmployeeID");
        var data = [{ OrderID: 10248, CustomerID: "VINET", EmployeeID: 5 },
                        { OrderID: 10249, CustomerID: "AANAR", EmployeeID: 9 },
                        { OrderID: 10250, CustomerID: "VICTE", EmployeeID: 2 },
                        { OrderID: 10251, CustomerID: "TOMSP", EmployeeID: 7 },
                        { OrderID: 10252, CustomerID: "SUPRD", EmployeeID: 6 }];
        var dataManager = ej.DataManager(data);
        dataManager.remove("OrderID", 10252, data);
        var dataSource = dataManager.executeLocal(query);
        renderTable(dataSource);

    });

    function renderTable(data) {
        var tableBody = "", row;
        for (var i = 0; i < data.length; i++) {
            row = data[i];
            tableBody += String.format("<tr><td>{0}</td><td>{1}</td><td>{2}</td></tr>", row.OrderID, row.CustomerID, row.EmployeeID);
        }
        $(".table tbody").html(tableBody);
    }

</script>

{% endhighlight %}


### saveChanges(changes, key, tableName, query)
{:#methods:savechanges}

This method is used to save the changes to the corresponding table. You can add a new record, edit an existing record, or delete a record by using this method.

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
<td class="name">changes</td>
<td class="type"><span class="param-type">Object</span></td>
<td class="description last">Specified values for the Data Table</td>
</tr>
<tr>
<td class="name">key</td>
<td class="type"><span class="param-type">String</span></td>
<td class="description last">KeyColumn to find the data</td>
</tr>
<tr>
<td class="name">tableName </td>
<td class="type"><span class="param-type">string</span></td>
<td class="description last">Name of the source table</td>
</tr>
<tr>
<td class="name">query</td>
<td class="type"><span class="param-type">ej.Query</span></td>
<td class="description last">Sets the default query for the data source.</td>
</tr>
</tbody>
</table>

#### Returns:
{:#methods:returns:}

Object

#### Example
{:.example}

{% highlight html %}

    <div class="datatable">
        <table id="table1" class="table table-striped table-bordered" style="width:700px">
            <thead>
                <tr>
                    <th>Order ID</th>
                    <th>Customer ID</th>
                    <th>Employee ID</th>
                </tr>
            </thead>
            <tbody></tbody>
        </table>
    </div>

<script type="text/javascript">
    $(function () {

        var data = [{ OrderID: 10248, CustomerID: "VINET", EmployeeID: 5 },
                        { OrderID: 10249, CustomerID: "AANAR", EmployeeID: 9 },
                        { OrderID: 10250, CustomerID: "VICTE", EmployeeID: 2 },
                        { OrderID: 10251, CustomerID: "TOMSP", EmployeeID: 7 },
                        { OrderID: 10252, CustomerID: "SUPRD", EmployeeID: 6 }];

        var newData = { "added": [{ OrderID: 10258, CustomerID: "JOHN", EmployeeID: 25 }], "deleted": {} , "changed":{} };
        
        var dataManager = ej.DataManager(data);
            var query = ej.Query()
                        .from("Orders")
                        .sortBy("OrderID", "descending", false)

            var dataManagerObj = dataManager.saveChanges(newData);
        
            renderTable(data);
    });

    // This function can be better replaced with any template engine. We used this for simplicity in demo.
    function renderTable(data) {
        var tableBody = "", row;
        for (var i = 0; i < data.length; i++) {
            row = data[i];
            tableBody += String.format("<tr><td>{0}</td><td>{1}</td><td>{2}</td></tr>", row.OrderID, row.CustomerID, row.EmployeeID);
        }
        $(".table tbody").html(tableBody);
    }
</script>

{% endhighlight %}

### update(keyField, value, tableName, query)
{:#methods:update}

Updates existing record and saves the changes to the table.

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
<td class="name">keyField</td>
<td class="type"><span class="param-type">String</span></td>
<td class="description last">KeyColumn to find the data</td>
</tr>
<tr>
<td class="name">value</td>
<td class="type"><span class="param-type">String</span></td>
<td class="description last">Specified value for the keyField</td>
</tr>
<tr>
<td class="name">tableName</td>
<td class="type"><span class="param-type">String</span></td>
<td class="description last">Name of the source table</td>
</tr>
<tr>
<td class="name">query</td>
<td class="type"><span class="param-type">ej.Query</span></td>
<td class="description last">Sets the default query for the data source.</td>
</tr>
</tbody>
</table>

#### Returns:
{:#methods:returns:}

Object

#### Example
{:.example}

{% highlight html %}

    <div class="datatable">
        <table id="table1" class="table table-striped table-bordered" style="width:700px">
            <thead>
                <tr>
                    <th>Order ID</th>
                    <th>Customer ID</th>
                    <th>Employee ID</th>
                </tr>
            </thead>
            <tbody></tbody>
        </table>
    </div>

<script type="text/javascript">
    $(function () {
        var query = ej.Query().sortByDesc("EmployeeID");
        var data = [{ OrderID: 10248, CustomerID: "VINET", EmployeeID: 5 },
                    { OrderID: 10249, CustomerID: "AANAR", EmployeeID: 9 },
                    { OrderID: 10250, CustomerID: "VICTE", EmployeeID: 2 },
                    { OrderID: 10251, CustomerID: "TOMSP", EmployeeID: 7 },
                    { OrderID: 10252, CustomerID: "SUPRD", EmployeeID: 6 }];
        var updateData = { OrderID: 10252, CustomerID: "ZAUDS", EmployeeID: 4 };
        var dataManger = ej.DataManager(data);
        dataManger.update("OrderID", updateData, data);
        var result = dataManger.executeLocal(query);
        renderTable(result);

    });

    function renderTable(data) {
        var tableBody = "", row;
        for (var i = 0; i < data.length; i++) {
            row = data[i];
            tableBody += String.format("<tr><td>{0}</td><td>{1}</td><td>{2}</td></tr>", row.OrderID, row.CustomerID, row.EmployeeID);
        }
        $(".table tbody").html(tableBody);
    }
</script>

{% endhighlight %}