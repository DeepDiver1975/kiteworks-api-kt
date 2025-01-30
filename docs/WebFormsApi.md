# WebFormsApi

All URIs are relative to *http://localhost*

Method | HTTP request | Description
------------- | ------------- | -------------
[**restWebFormsGet**](WebFormsApi.md#restWebFormsGet) | **GET** /rest/webForms | List web forms
[**restWebFormsIdGet**](WebFormsApi.md#restWebFormsIdGet) | **GET** /rest/webForms/{id} | Get a web form


<a id="restWebFormsGet"></a>
# **restWebFormsGet**
> kotlin.collections.List&lt;WebForm&gt; restWebFormsGet(name, nameColonContains, orderBy, with, mode)

List web forms

Returns a list of web forms available to current user.

### Example
```kotlin
// Import classes:
//import org.openapitools.client.infrastructure.*
//import org.openapitools.client.models.*

val apiInstance = WebFormsApi()
val name : kotlin.String = name_example // kotlin.String | Web form name
val nameColonContains : kotlin.String = nameColonContains_example // kotlin.String | Web form name. Search for result that contains specified characters in this parameter.
val orderBy : kotlin.collections.List<kotlin.String> =  // kotlin.collections.List<kotlin.String> | Sorting options
val with : kotlin.String = with_example // kotlin.String | With parameters
val mode : kotlin.String = mode_example // kotlin.String | Response mode
try {
    val result : kotlin.collections.List<WebForm> = apiInstance.restWebFormsGet(name, nameColonContains, orderBy, with, mode)
    println(result)
} catch (e: ClientException) {
    println("4xx response calling WebFormsApi#restWebFormsGet")
    e.printStackTrace()
} catch (e: ServerException) {
    println("5xx response calling WebFormsApi#restWebFormsGet")
    e.printStackTrace()
}
```

### Parameters

Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **name** | **kotlin.String**| Web form name | [optional]
 **nameColonContains** | **kotlin.String**| Web form name. Search for result that contains specified characters in this parameter. | [optional]
 **orderBy** | [**kotlin.collections.List&lt;kotlin.String&gt;**](kotlin.String.md)| Sorting options | [optional]
 **with** | **kotlin.String**| With parameters | [optional]
 **mode** | **kotlin.String**| Response mode | [optional]

### Return type

[**kotlin.collections.List&lt;WebForm&gt;**](WebForm.md)

### Authorization

No authorization required

### HTTP request headers

 - **Content-Type**: Not defined
 - **Accept**: */*

<a id="restWebFormsIdGet"></a>
# **restWebFormsIdGet**
> WebForm restWebFormsIdGet(id, with, mode)

Get a web form

Returns the details of a specified web form

### Example
```kotlin
// Import classes:
//import org.openapitools.client.infrastructure.*
//import org.openapitools.client.models.*

val apiInstance = WebFormsApi()
val id : kotlin.String = id_example // kotlin.String | ID of the web form to be retrieved
val with : kotlin.String = with_example // kotlin.String | With parameters
val mode : kotlin.String = mode_example // kotlin.String | Response mode
try {
    val result : WebForm = apiInstance.restWebFormsIdGet(id, with, mode)
    println(result)
} catch (e: ClientException) {
    println("4xx response calling WebFormsApi#restWebFormsIdGet")
    e.printStackTrace()
} catch (e: ServerException) {
    println("5xx response calling WebFormsApi#restWebFormsIdGet")
    e.printStackTrace()
}
```

### Parameters

Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **id** | **kotlin.String**| ID of the web form to be retrieved |
 **with** | **kotlin.String**| With parameters | [optional]
 **mode** | **kotlin.String**| Response mode | [optional]

### Return type

[**WebForm**](WebForm.md)

### Authorization

No authorization required

### HTTP request headers

 - **Content-Type**: Not defined
 - **Accept**: */*

