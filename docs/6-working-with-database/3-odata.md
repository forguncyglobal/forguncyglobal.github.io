---
layout: default
title: OData
parent: Working with Database
permalink: /working-with-database/OData/
nav_order: 3
---

# {{ page.title }}

- [OData Overview](#odata-overview)
- [OData Functions](#odata-functions)
- [OData Generation Tool](#odata-generation-tool)

## OData Overview

OData is a protocol that standardizes data access methods in web applications. Specifications were developed mainly by Microsoft, IBM, SAP, and Citrix.

Forguncy only supports OData. It retrieves table data using OData resource paths. Table data here refers to table or view data. It also supports some OData query options, operators and functions. There are four ways to retrieve data using OData.

|**Server-side API**|You can retrieve table data using an OData resource path by using the GetTableData method (String) overload.|
|**Web APIs**|By using the getTableDataByOData method, you can get the table data using the OData resource path. |
|**URLs**|You can get table data using OData with the URL rules <br/> *http://server name or IP address/application path/OData/GetData/OData resource path* <br/> Note: You cannot use the URL method unless you are logged into the Forguncy application. |
|**Function**|By using the OData function, you can get the table data with the conditions specified by OData.|

Below is the sample of using C# code to get authentication for the Forguncy application and retrieving table data using OData by URL:

### Form Authentication

public  string GetOData( string baseUrl, string odataParam, CookieContainer loginCookie) <br/>
{<br/>
    HttpWebRequest rq = HttpWebRequest.Create(baseUrl + "OData/GetData/" + odataParam) as HttpWebRequest;<br/>
    rq.CookieContainer = loginCookie;<br/>
    rq.Method = WebRequestMethods.Http.Get;<br/>
    var response = rq.GetResponse();<br/>
     return  new StreamReader(response.GetResponseStream()).ReadToEnd();<br/>
}<br/>
CookieContainer GetLoginCookie( string baseUrl, string userName, string passWord)<br/>
{<br/>
    var login = baseUrl + "Account/Login" ;<br/>
    HttpWebRequest rq = HttpWebRequest.Create(login) as HttpWebRequest;<br/>
    rq.CookieContainer = new CookieContainer();<br/>
    rq.Method = WebRequestMethods.Http.Post;<br/>
    rq. Accept = "application/json" ;<br/>
    rq.ContentType = "application/json" ;<br/>
     var loginStr = "{userName:\"" + userName + "\", password:\"" + passWord + "\",rememberMe:true }" ;<br/>
     var data = Encoding. UTF8.GetBytes(loginStr);<br/>
     using (Stream stream = rq.GetRequestStream())<br/>
    {<br/>
        stream.Write(data, 0, data.Length);<br/>
    }<br/>
    var response = rq.GetResponse();<br/>
     return rq.CookieContainer;<br/>
}<br/>
//test code<br/>
 var baseUrl = "http://localhost:42515/Forguncy/" ;<br/>
 var loginCookie = GetLoginCookie(baseUrl, "Administrator" , "123456" );<br/>
Console.WriteLine(GetOData(baseUrl, "table" , loginCookie));<br/>
Console.WriteLine(GetOData(baseUrl, "table(2)" , loginCookie));
{:.note}

### Windows Authentication

public  static  string GetODataWindows( string baseUrl, string odataParam, string userName, string password, string domain)<br/>
{<br/>
    HttpWebRequest rq = HttpWebRequest.Create(baseUrl + "OData/GetData/" + odataParam) as HttpWebRequest;<br/>
    rq.Credentials = new NetworkCredential(userName, password, domain);<br/>
    rq.Method = WebRequestMethods.Http.Get;<br/>
    var response = rq.GetResponse();<br/>
     return  new StreamReader(response.GetResponseStream()).ReadToEnd();<br/>
}<br/>
// test code<br/>
 Console.WriteLine(GetOData(baseUrl, "table" , "budoutaro" , "123456" , "abccompany" ));
 {:.note}

## OData Functions

OData functions are specific functions in Forguncy that do not exist in Excel. 

When setting an OData function to a cell, it is possible to construct an OData path using the GUI by using the [OData generation tool](#OData-generation-tool).

## OData Generation Tool

You can create a new OData path or read and change the OData path written in the active cell.

If you open the OData Generator with multiple OData functions in the active cell, only the first one will be loaded and the rest will be discarded. If there is an error in the OData function or an exception error occurs while loading, nothing will be loaded when you open the OData generation tool.

When changing the OData path written in the active cell, if the path contains an else condition of IF / IsBlank, the path may not be analyzed correctly and an incorrect result may be displayed. Such as:

|Description on the active cell|"=ODATA("Table 1?$select=*&$filter=ID eq "&IF(ISBLANK(AP6),"null",AP6+1))"|
|Display result when read by OData generation tool|"=ODATA("Table 1?$select=*&$filter=ID eq "&IF(ISBLANK(AP6),"null",AP6)"|

- Go to **Formula** tab and click **OData Generation Tool**.

![odata-generator](/assets/images/product-images/odata-generator.png)
{:.dropshadow}

- Select the target table.

![odata-builder-select-table](/assets/images/product-images/odata-builder-select-table.png)
{:.dropshadow}

- On the **Select** tab, choose *Column*, *Count*, or *Value*.
    Select *Column* to retrieve by specifying the field. All fields are checked by default. Uncheck if necessary. An OData path of the form "$select=ID" is generated. If you select multiple fields, the field names are separated by commas.

    ![odata-builder-columns](/assets/images/product-images/odata-builder-columns.png)
    {:.dropshadow}

    Select *Count* to get the number of columns in the table. An OData path of the form *$count* is generated.

    ![odata-builder-count](/assets/images/product-images/odata-builder-count.png)
    {:.dropshadow}

    To retrieve only values, select Get Values ​​Only and set the target field and value. An OData path of the form *Value* is generated.

    ![odata-builder-value](/assets/images/product-images/odata-builder-value.png)
    {:.dropshadow}

- On the Query tab, specify your query criteria.
    Click *New Condition* and specify the query criteria. An OData path of the form *$filter* is generated.

    ![odata-builder-query](/assets/images/product-images/odata-builder-query.png)
    {:.dropshadow}

- On the *Top* tab, specify the first record to retrieve. An OData path of the form *$top* is generated.

    ![odata-builder-top](/assets/images/product-images/odata-builder-top.png)
    {:.dropshadow}

- On the *OrderBy* tab, specify the sorting for the displayed table. Click *New Condition* and select the *column* and *order* for sorting. An OData path of the form *$orderby* is generated.

    ![odata-builder-orderBy](/assets/images/product-images/odata-builder-orderBy.png)
    {:.dropshadow}

- Click the **Copy** button to copy the OData path to the clipboard. 
- Click **OK** to set the cell as an OData function.