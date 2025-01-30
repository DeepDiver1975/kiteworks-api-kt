# AccessVerificationsApi

All URIs are relative to *http://localhost*

Method | HTTP request | Description
------------- | ------------- | -------------
[**restAccessVerificationsIdGet**](AccessVerificationsApi.md#restAccessVerificationsIdGet) | **GET** /rest/accessVerifications/{id} | Get access verification
[**restAccessVerificationsIdPost**](AccessVerificationsApi.md#restAccessVerificationsIdPost) | **POST** /rest/accessVerifications/{id} | Submit access verification


<a id="restAccessVerificationsIdGet"></a>
# **restAccessVerificationsIdGet**
> AccessVerification restAccessVerificationsIdGet(id)

Get access verification

Get access verification

### Example
```kotlin
// Import classes:
//import org.openapitools.client.infrastructure.*
//import org.openapitools.client.models.*

val apiInstance = AccessVerificationsApi()
val id : kotlin.String = id_example // kotlin.String | The ID of the entity
try {
    val result : AccessVerification = apiInstance.restAccessVerificationsIdGet(id)
    println(result)
} catch (e: ClientException) {
    println("4xx response calling AccessVerificationsApi#restAccessVerificationsIdGet")
    e.printStackTrace()
} catch (e: ServerException) {
    println("5xx response calling AccessVerificationsApi#restAccessVerificationsIdGet")
    e.printStackTrace()
}
```

### Parameters

Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **id** | **kotlin.String**| The ID of the entity |

### Return type

[**AccessVerification**](AccessVerification.md)

### Authorization

No authorization required

### HTTP request headers

 - **Content-Type**: Not defined
 - **Accept**: */*

<a id="restAccessVerificationsIdPost"></a>
# **restAccessVerificationsIdPost**
> DownloadLink restAccessVerificationsIdPost(id, body)

Submit access verification

Submit access verification

### Example
```kotlin
// Import classes:
//import org.openapitools.client.infrastructure.*
//import org.openapitools.client.models.*

val apiInstance = AccessVerificationsApi()
val id : kotlin.String = id_example // kotlin.String | The ID of the entity
val body : AccessVerificationPostRequest =  // AccessVerificationPostRequest | 
try {
    val result : DownloadLink = apiInstance.restAccessVerificationsIdPost(id, body)
    println(result)
} catch (e: ClientException) {
    println("4xx response calling AccessVerificationsApi#restAccessVerificationsIdPost")
    e.printStackTrace()
} catch (e: ServerException) {
    println("5xx response calling AccessVerificationsApi#restAccessVerificationsIdPost")
    e.printStackTrace()
}
```

### Parameters

Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **id** | **kotlin.String**| The ID of the entity |
 **body** | [**AccessVerificationPostRequest**](AccessVerificationPostRequest.md)|  |

### Return type

[**DownloadLink**](DownloadLink.md)

### Authorization

No authorization required

### HTTP request headers

 - **Content-Type**: Not defined
 - **Accept**: */*

