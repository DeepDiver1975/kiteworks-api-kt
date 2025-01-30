# ShortLinksApi

All URIs are relative to *http://localhost*

Method | HTTP request | Description
------------- | ------------- | -------------
[**restShortLinksRefGet**](ShortLinksApi.md#restShortLinksRefGet) | **GET** /rest/shortLinks/{ref} | Short Link


<a id="restShortLinksRefGet"></a>
# **restShortLinksRefGet**
> Shortlink restShortLinksRefGet(ref, mode)

Short Link

Returns properties of a short link including the associated entity ID.

### Example
```kotlin
// Import classes:
//import org.openapitools.client.infrastructure.*
//import org.openapitools.client.models.*

val apiInstance = ShortLinksApi()
val ref : kotlin.String = ref_example // kotlin.String | The ref value of the short link
val mode : kotlin.String = mode_example // kotlin.String | Response mode
try {
    val result : Shortlink = apiInstance.restShortLinksRefGet(ref, mode)
    println(result)
} catch (e: ClientException) {
    println("4xx response calling ShortLinksApi#restShortLinksRefGet")
    e.printStackTrace()
} catch (e: ServerException) {
    println("5xx response calling ShortLinksApi#restShortLinksRefGet")
    e.printStackTrace()
}
```

### Parameters

Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **ref** | **kotlin.String**| The ref value of the short link |
 **mode** | **kotlin.String**| Response mode | [optional]

### Return type

[**Shortlink**](Shortlink.md)

### Authorization

No authorization required

### HTTP request headers

 - **Content-Type**: Not defined
 - **Accept**: */*

