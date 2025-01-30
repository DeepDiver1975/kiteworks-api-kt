# ExternalDLApi

All URIs are relative to *http://localhost*

Method | HTTP request | Description
------------- | ------------- | -------------
[**restExternalDLDelete**](ExternalDLApi.md#restExternalDLDelete) | **DELETE** /rest/externalDL | Delete external DL
[**restExternalDLGet**](ExternalDLApi.md#restExternalDLGet) | **GET** /rest/externalDL | Get external DL
[**restExternalDLPost**](ExternalDLApi.md#restExternalDLPost) | **POST** /rest/externalDL | Add external DL


<a id="restExternalDLDelete"></a>
# **restExternalDLDelete**
> ExternalDLs restExternalDLDelete(body)

Delete external DL

Delete external DL

### Example
```kotlin
// Import classes:
//import org.openapitools.client.infrastructure.*
//import org.openapitools.client.models.*

val apiInstance = ExternalDLApi()
val body : ExternalDLUpdateRequest =  // ExternalDLUpdateRequest | 
try {
    val result : ExternalDLs = apiInstance.restExternalDLDelete(body)
    println(result)
} catch (e: ClientException) {
    println("4xx response calling ExternalDLApi#restExternalDLDelete")
    e.printStackTrace()
} catch (e: ServerException) {
    println("5xx response calling ExternalDLApi#restExternalDLDelete")
    e.printStackTrace()
}
```

### Parameters

Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **body** | [**ExternalDLUpdateRequest**](ExternalDLUpdateRequest.md)|  |

### Return type

[**ExternalDLs**](ExternalDLs.md)

### Authorization

No authorization required

### HTTP request headers

 - **Content-Type**: Not defined
 - **Accept**: */*

<a id="restExternalDLGet"></a>
# **restExternalDLGet**
> ExternalDLs restExternalDLGet(search)

Get external DL

Get external DL

### Example
```kotlin
// Import classes:
//import org.openapitools.client.infrastructure.*
//import org.openapitools.client.models.*

val apiInstance = ExternalDLApi()
val search : kotlin.String = search_example // kotlin.String | 
try {
    val result : ExternalDLs = apiInstance.restExternalDLGet(search)
    println(result)
} catch (e: ClientException) {
    println("4xx response calling ExternalDLApi#restExternalDLGet")
    e.printStackTrace()
} catch (e: ServerException) {
    println("5xx response calling ExternalDLApi#restExternalDLGet")
    e.printStackTrace()
}
```

### Parameters

Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **search** | **kotlin.String**|  | [optional]

### Return type

[**ExternalDLs**](ExternalDLs.md)

### Authorization

No authorization required

### HTTP request headers

 - **Content-Type**: Not defined
 - **Accept**: */*

<a id="restExternalDLPost"></a>
# **restExternalDLPost**
> ExternalDLs restExternalDLPost(body)

Add external DL

Add external DL

### Example
```kotlin
// Import classes:
//import org.openapitools.client.infrastructure.*
//import org.openapitools.client.models.*

val apiInstance = ExternalDLApi()
val body : ExternalDLUpdateRequest =  // ExternalDLUpdateRequest | 
try {
    val result : ExternalDLs = apiInstance.restExternalDLPost(body)
    println(result)
} catch (e: ClientException) {
    println("4xx response calling ExternalDLApi#restExternalDLPost")
    e.printStackTrace()
} catch (e: ServerException) {
    println("5xx response calling ExternalDLApi#restExternalDLPost")
    e.printStackTrace()
}
```

### Parameters

Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **body** | [**ExternalDLUpdateRequest**](ExternalDLUpdateRequest.md)|  |

### Return type

[**ExternalDLs**](ExternalDLs.md)

### Authorization

No authorization required

### HTTP request headers

 - **Content-Type**: Not defined
 - **Accept**: */*

