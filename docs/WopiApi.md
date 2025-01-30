# WopiApi

All URIs are relative to *http://localhost*

Method | HTTP request | Description
------------- | ------------- | -------------
[**restWopiContainersFolderTokenPost**](WopiApi.md#restWopiContainersFolderTokenPost) | **POST** /rest/wopi/containers/{folder}/token | Generate WopiAccessToken for folder
[**restWopiFilesFileTokenPost**](WopiApi.md#restWopiFilesFileTokenPost) | **POST** /rest/wopi/files/{file}/token | Generate WopiAccessToken for file


<a id="restWopiContainersFolderTokenPost"></a>
# **restWopiContainersFolderTokenPost**
> WopiAccessToken restWopiContainersFolderTokenPost(folder)

Generate WopiAccessToken for folder

Generate WopiAccessToken for folder

### Example
```kotlin
// Import classes:
//import org.openapitools.client.infrastructure.*
//import org.openapitools.client.models.*

val apiInstance = WopiApi()
val folder : kotlin.Int = 56 // kotlin.Int | ID of the folder
try {
    val result : WopiAccessToken = apiInstance.restWopiContainersFolderTokenPost(folder)
    println(result)
} catch (e: ClientException) {
    println("4xx response calling WopiApi#restWopiContainersFolderTokenPost")
    e.printStackTrace()
} catch (e: ServerException) {
    println("5xx response calling WopiApi#restWopiContainersFolderTokenPost")
    e.printStackTrace()
}
```

### Parameters

Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **folder** | **kotlin.Int**| ID of the folder |

### Return type

[**WopiAccessToken**](WopiAccessToken.md)

### Authorization

No authorization required

### HTTP request headers

 - **Content-Type**: Not defined
 - **Accept**: */*

<a id="restWopiFilesFileTokenPost"></a>
# **restWopiFilesFileTokenPost**
> WopiAccessToken restWopiFilesFileTokenPost(file)

Generate WopiAccessToken for file

Generate WopiAccessToken for file

### Example
```kotlin
// Import classes:
//import org.openapitools.client.infrastructure.*
//import org.openapitools.client.models.*

val apiInstance = WopiApi()
val file : kotlin.Int = 56 // kotlin.Int | ID of the file
try {
    val result : WopiAccessToken = apiInstance.restWopiFilesFileTokenPost(file)
    println(result)
} catch (e: ClientException) {
    println("4xx response calling WopiApi#restWopiFilesFileTokenPost")
    e.printStackTrace()
} catch (e: ServerException) {
    println("5xx response calling WopiApi#restWopiFilesFileTokenPost")
    e.printStackTrace()
}
```

### Parameters

Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **file** | **kotlin.Int**| ID of the file |

### Return type

[**WopiAccessToken**](WopiAccessToken.md)

### Authorization

No authorization required

### HTTP request headers

 - **Content-Type**: Not defined
 - **Accept**: */*

