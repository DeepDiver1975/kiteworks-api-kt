# SourceTypesApi

All URIs are relative to *http://localhost*

Method | HTTP request | Description
------------- | ------------- | -------------
[**restSourceTypesGet**](SourceTypesApi.md#restSourceTypesGet) | **GET** /rest/sourceTypes | List all ECM source types
[**restSourceTypesIdGet**](SourceTypesApi.md#restSourceTypesIdGet) | **GET** /rest/sourceTypes/{id} | Returns requested ECM source type


<a id="restSourceTypesGet"></a>
# **restSourceTypesGet**
> kotlin.collections.List&lt;SourceType&gt; restSourceTypesGet(mode, orderBy)

List all ECM source types

Returns a list of available ECM source types.

### Example
```kotlin
// Import classes:
//import org.openapitools.client.infrastructure.*
//import org.openapitools.client.models.*

val apiInstance = SourceTypesApi()
val mode : kotlin.Boolean = true // kotlin.Boolean | Mode
val orderBy : kotlin.collections.List<kotlin.String> =  // kotlin.collections.List<kotlin.String> | Sorting options
try {
    val result : kotlin.collections.List<SourceType> = apiInstance.restSourceTypesGet(mode, orderBy)
    println(result)
} catch (e: ClientException) {
    println("4xx response calling SourceTypesApi#restSourceTypesGet")
    e.printStackTrace()
} catch (e: ServerException) {
    println("5xx response calling SourceTypesApi#restSourceTypesGet")
    e.printStackTrace()
}
```

### Parameters

Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **mode** | **kotlin.Boolean**| Mode | [optional]
 **orderBy** | [**kotlin.collections.List&lt;kotlin.String&gt;**](kotlin.String.md)| Sorting options | [optional]

### Return type

[**kotlin.collections.List&lt;SourceType&gt;**](SourceType.md)

### Authorization

No authorization required

### HTTP request headers

 - **Content-Type**: Not defined
 - **Accept**: */*

<a id="restSourceTypesIdGet"></a>
# **restSourceTypesIdGet**
> SourceType restSourceTypesIdGet(id)

Returns requested ECM source type

Returns requested source type.

### Example
```kotlin
// Import classes:
//import org.openapitools.client.infrastructure.*
//import org.openapitools.client.models.*

val apiInstance = SourceTypesApi()
val id : kotlin.Int = 56 // kotlin.Int | ID of the sourceType to be retrieved
try {
    val result : SourceType = apiInstance.restSourceTypesIdGet(id)
    println(result)
} catch (e: ClientException) {
    println("4xx response calling SourceTypesApi#restSourceTypesIdGet")
    e.printStackTrace()
} catch (e: ServerException) {
    println("5xx response calling SourceTypesApi#restSourceTypesIdGet")
    e.printStackTrace()
}
```

### Parameters

Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **id** | **kotlin.Int**| ID of the sourceType to be retrieved |

### Return type

[**SourceType**](SourceType.md)

### Authorization

No authorization required

### HTTP request headers

 - **Content-Type**: Not defined
 - **Accept**: */*

