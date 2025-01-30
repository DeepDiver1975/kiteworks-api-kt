# UploadsApi

All URIs are relative to *http://localhost*

Method | HTTP request | Description
------------- | ------------- | -------------
[**hostNameRestUploadsIdPost**](UploadsApi.md#hostNameRestUploadsIdPost) | **POST** /{host_name}/rest/uploads/{id} | uploads chunk endpoint
[**restFilesIdActionsInitiateUploadPost**](UploadsApi.md#restFilesIdActionsInitiateUploadPost) | **POST** /rest/files/{id}/actions/initiateUpload | initiates file chunk upload session endpoint
[**restFoldersIdActionsInitiateUploadPost**](UploadsApi.md#restFoldersIdActionsInitiateUploadPost) | **POST** /rest/folders/{id}/actions/initiateUpload | initiates file chunk upload session endpoint
[**restFoldersIdActionsInitiateUploadZipPost**](UploadsApi.md#restFoldersIdActionsInitiateUploadZipPost) | **POST** /rest/folders/{id}/actions/initiateUpload/zip | initiates archive file chunk upload session endpoint
[**restMailIdActionsInitiateUploadPost**](UploadsApi.md#restMailIdActionsInitiateUploadPost) | **POST** /rest/mail/{id}/actions/initiateUpload | initiates file chunk upload session endpoint
[**restPublicMailIdActionsInitiateUploadPost**](UploadsApi.md#restPublicMailIdActionsInitiateUploadPost) | **POST** /rest/public/mail/{id}/actions/initiateUpload | initiates file chunk upload session endpoint
[**restRequestFileRefActionsInitiateUploadPost**](UploadsApi.md#restRequestFileRefActionsInitiateUploadPost) | **POST** /rest/requestFile/{ref}/actions/initiateUpload | initiates file chunk upload session endpoint
[**restUploadsConfigGet**](UploadsApi.md#restUploadsConfigGet) | **GET** /rest/uploads/config | Get upload server configuration
[**restUploadsGet**](UploadsApi.md#restUploadsGet) | **GET** /rest/uploads | Fetch all paused user&#39;s upload sessions
[**restUploadsIdDelete**](UploadsApi.md#restUploadsIdDelete) | **DELETE** /rest/uploads/{id} | Terminate chunk upload session
[**restUploadsIdGet**](UploadsApi.md#restUploadsIdGet) | **GET** /rest/uploads/{id} | Get Upload


<a id="hostNameRestUploadsIdPost"></a>
# **hostNameRestUploadsIdPost**
> Upload hostNameRestUploadsIdPost(id, hostName, compressionMode, compressionSize, originalSize, content, index, lastChunk)

uploads chunk endpoint

uploads chunk to the upload entity

### Example
```kotlin
// Import classes:
//import org.openapitools.client.infrastructure.*
//import org.openapitools.client.models.*

val apiInstance = UploadsApi()
val id : kotlin.Int = 56 // kotlin.Int | The ID of the upload
val hostName : kotlin.String = hostName_example // kotlin.String | Upload host name, can be obtained from GET /uploads/{id} or initiateUpload response
val compressionMode : kotlin.String = compressionMode_example // kotlin.String | The compression mode. Available option \\\"NORMAL\\\", \\\"GZIP\\\" and \\\"ZLIB\\\"
val compressionSize : kotlin.Int = 56 // kotlin.Int | The upload content size after compression
val originalSize : kotlin.Int = 56 // kotlin.Int | The original upload content size before compression
val content : io.ktor.client.request.forms.InputProvider = BINARY_DATA_HERE // io.ktor.client.request.forms.InputProvider | The upload content.
val index : kotlin.Int = 56 // kotlin.Int | The chunk index. Starts from 1
val lastChunk : kotlin.Int = 56 // kotlin.Int | Indicate if this upload is the last chunk of the file.
try {
    val result : Upload = apiInstance.hostNameRestUploadsIdPost(id, hostName, compressionMode, compressionSize, originalSize, content, index, lastChunk)
    println(result)
} catch (e: ClientException) {
    println("4xx response calling UploadsApi#hostNameRestUploadsIdPost")
    e.printStackTrace()
} catch (e: ServerException) {
    println("5xx response calling UploadsApi#hostNameRestUploadsIdPost")
    e.printStackTrace()
}
```

### Parameters

Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **id** | **kotlin.Int**| The ID of the upload |
 **hostName** | **kotlin.String**| Upload host name, can be obtained from GET /uploads/{id} or initiateUpload response |
 **compressionMode** | **kotlin.String**| The compression mode. Available option \\\&quot;NORMAL\\\&quot;, \\\&quot;GZIP\\\&quot; and \\\&quot;ZLIB\\\&quot; |
 **compressionSize** | **kotlin.Int**| The upload content size after compression |
 **originalSize** | **kotlin.Int**| The original upload content size before compression |
 **content** | **io.ktor.client.request.forms.InputProvider**| The upload content. |
 **index** | **kotlin.Int**| The chunk index. Starts from 1 | [optional]
 **lastChunk** | **kotlin.Int**| Indicate if this upload is the last chunk of the file. | [optional]

### Return type

[**Upload**](Upload.md)

### Authorization

No authorization required

### HTTP request headers

 - **Content-Type**: multipart/form-data
 - **Accept**: */*

<a id="restFilesIdActionsInitiateUploadPost"></a>
# **restFilesIdActionsInitiateUploadPost**
> Upload restFilesIdActionsInitiateUploadPost(id, body)

initiates file chunk upload session endpoint

initiates file chunk upload session

### Example
```kotlin
// Import classes:
//import org.openapitools.client.infrastructure.*
//import org.openapitools.client.models.*

val apiInstance = UploadsApi()
val id : kotlin.String = id_example // kotlin.String | The ID of the entity
val body : InitiateUploadPostRequest =  // InitiateUploadPostRequest | 
try {
    val result : Upload = apiInstance.restFilesIdActionsInitiateUploadPost(id, body)
    println(result)
} catch (e: ClientException) {
    println("4xx response calling UploadsApi#restFilesIdActionsInitiateUploadPost")
    e.printStackTrace()
} catch (e: ServerException) {
    println("5xx response calling UploadsApi#restFilesIdActionsInitiateUploadPost")
    e.printStackTrace()
}
```

### Parameters

Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **id** | **kotlin.String**| The ID of the entity |
 **body** | [**InitiateUploadPostRequest**](InitiateUploadPostRequest.md)|  |

### Return type

[**Upload**](Upload.md)

### Authorization

No authorization required

### HTTP request headers

 - **Content-Type**: Not defined
 - **Accept**: */*

<a id="restFoldersIdActionsInitiateUploadPost"></a>
# **restFoldersIdActionsInitiateUploadPost**
> Upload restFoldersIdActionsInitiateUploadPost(id, body)

initiates file chunk upload session endpoint

initiates file chunk upload session

### Example
```kotlin
// Import classes:
//import org.openapitools.client.infrastructure.*
//import org.openapitools.client.models.*

val apiInstance = UploadsApi()
val id : kotlin.String = id_example // kotlin.String | The ID of the entity
val body : InitiateUploadPostRequest =  // InitiateUploadPostRequest | 
try {
    val result : Upload = apiInstance.restFoldersIdActionsInitiateUploadPost(id, body)
    println(result)
} catch (e: ClientException) {
    println("4xx response calling UploadsApi#restFoldersIdActionsInitiateUploadPost")
    e.printStackTrace()
} catch (e: ServerException) {
    println("5xx response calling UploadsApi#restFoldersIdActionsInitiateUploadPost")
    e.printStackTrace()
}
```

### Parameters

Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **id** | **kotlin.String**| The ID of the entity |
 **body** | [**InitiateUploadPostRequest**](InitiateUploadPostRequest.md)|  |

### Return type

[**Upload**](Upload.md)

### Authorization

No authorization required

### HTTP request headers

 - **Content-Type**: Not defined
 - **Accept**: */*

<a id="restFoldersIdActionsInitiateUploadZipPost"></a>
# **restFoldersIdActionsInitiateUploadZipPost**
> Upload restFoldersIdActionsInitiateUploadZipPost(id, body)

initiates archive file chunk upload session endpoint

initiates archive file chunk upload session

### Example
```kotlin
// Import classes:
//import org.openapitools.client.infrastructure.*
//import org.openapitools.client.models.*

val apiInstance = UploadsApi()
val id : kotlin.String = id_example // kotlin.String | The ID of the entity
val body : InitiateUploadPostRequest =  // InitiateUploadPostRequest | 
try {
    val result : Upload = apiInstance.restFoldersIdActionsInitiateUploadZipPost(id, body)
    println(result)
} catch (e: ClientException) {
    println("4xx response calling UploadsApi#restFoldersIdActionsInitiateUploadZipPost")
    e.printStackTrace()
} catch (e: ServerException) {
    println("5xx response calling UploadsApi#restFoldersIdActionsInitiateUploadZipPost")
    e.printStackTrace()
}
```

### Parameters

Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **id** | **kotlin.String**| The ID of the entity |
 **body** | [**InitiateUploadPostRequest**](InitiateUploadPostRequest.md)|  |

### Return type

[**Upload**](Upload.md)

### Authorization

No authorization required

### HTTP request headers

 - **Content-Type**: Not defined
 - **Accept**: */*

<a id="restMailIdActionsInitiateUploadPost"></a>
# **restMailIdActionsInitiateUploadPost**
> Upload restMailIdActionsInitiateUploadPost(id, body)

initiates file chunk upload session endpoint

initiates file chunk upload session

### Example
```kotlin
// Import classes:
//import org.openapitools.client.infrastructure.*
//import org.openapitools.client.models.*

val apiInstance = UploadsApi()
val id : kotlin.String = id_example // kotlin.String | The ID of the entity
val body : InitiateUploadPostRequest =  // InitiateUploadPostRequest | 
try {
    val result : Upload = apiInstance.restMailIdActionsInitiateUploadPost(id, body)
    println(result)
} catch (e: ClientException) {
    println("4xx response calling UploadsApi#restMailIdActionsInitiateUploadPost")
    e.printStackTrace()
} catch (e: ServerException) {
    println("5xx response calling UploadsApi#restMailIdActionsInitiateUploadPost")
    e.printStackTrace()
}
```

### Parameters

Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **id** | **kotlin.String**| The ID of the entity |
 **body** | [**InitiateUploadPostRequest**](InitiateUploadPostRequest.md)|  |

### Return type

[**Upload**](Upload.md)

### Authorization

No authorization required

### HTTP request headers

 - **Content-Type**: Not defined
 - **Accept**: */*

<a id="restPublicMailIdActionsInitiateUploadPost"></a>
# **restPublicMailIdActionsInitiateUploadPost**
> Upload restPublicMailIdActionsInitiateUploadPost(id, body)

initiates file chunk upload session endpoint

initiates file chunk upload session

### Example
```kotlin
// Import classes:
//import org.openapitools.client.infrastructure.*
//import org.openapitools.client.models.*

val apiInstance = UploadsApi()
val id : kotlin.String = id_example // kotlin.String | The ID of the entity
val body : InitiateUploadPostRequest =  // InitiateUploadPostRequest | 
try {
    val result : Upload = apiInstance.restPublicMailIdActionsInitiateUploadPost(id, body)
    println(result)
} catch (e: ClientException) {
    println("4xx response calling UploadsApi#restPublicMailIdActionsInitiateUploadPost")
    e.printStackTrace()
} catch (e: ServerException) {
    println("5xx response calling UploadsApi#restPublicMailIdActionsInitiateUploadPost")
    e.printStackTrace()
}
```

### Parameters

Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **id** | **kotlin.String**| The ID of the entity |
 **body** | [**InitiateUploadPostRequest**](InitiateUploadPostRequest.md)|  |

### Return type

[**Upload**](Upload.md)

### Authorization

No authorization required

### HTTP request headers

 - **Content-Type**: Not defined
 - **Accept**: */*

<a id="restRequestFileRefActionsInitiateUploadPost"></a>
# **restRequestFileRefActionsInitiateUploadPost**
> Upload restRequestFileRefActionsInitiateUploadPost(ref, body)

initiates file chunk upload session endpoint

initiates file chunk upload session

### Example
```kotlin
// Import classes:
//import org.openapitools.client.infrastructure.*
//import org.openapitools.client.models.*

val apiInstance = UploadsApi()
val ref : kotlin.String = ref_example // kotlin.String | The ref of the Request File
val body : InitiateUploadPostRequest =  // InitiateUploadPostRequest | 
try {
    val result : Upload = apiInstance.restRequestFileRefActionsInitiateUploadPost(ref, body)
    println(result)
} catch (e: ClientException) {
    println("4xx response calling UploadsApi#restRequestFileRefActionsInitiateUploadPost")
    e.printStackTrace()
} catch (e: ServerException) {
    println("5xx response calling UploadsApi#restRequestFileRefActionsInitiateUploadPost")
    e.printStackTrace()
}
```

### Parameters

Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **ref** | **kotlin.String**| The ref of the Request File |
 **body** | [**InitiateUploadPostRequest**](InitiateUploadPostRequest.md)|  |

### Return type

[**Upload**](Upload.md)

### Authorization

No authorization required

### HTTP request headers

 - **Content-Type**: Not defined
 - **Accept**: */*

<a id="restUploadsConfigGet"></a>
# **restUploadsConfigGet**
> AcfsConfig restUploadsConfigGet()

Get upload server configuration

Returns the details of the upload server configuration

### Example
```kotlin
// Import classes:
//import org.openapitools.client.infrastructure.*
//import org.openapitools.client.models.*

val apiInstance = UploadsApi()
try {
    val result : AcfsConfig = apiInstance.restUploadsConfigGet()
    println(result)
} catch (e: ClientException) {
    println("4xx response calling UploadsApi#restUploadsConfigGet")
    e.printStackTrace()
} catch (e: ServerException) {
    println("5xx response calling UploadsApi#restUploadsConfigGet")
    e.printStackTrace()
}
```

### Parameters
This endpoint does not need any parameter.

### Return type

[**AcfsConfig**](AcfsConfig.md)

### Authorization

No authorization required

### HTTP request headers

 - **Content-Type**: Not defined
 - **Accept**: */*

<a id="restUploadsGet"></a>
# **restUploadsGet**
> kotlin.collections.List&lt;Upload&gt; restUploadsGet(offset, limit, locateId, with, mode)

Fetch all paused user&#39;s upload sessions

Returns all paused user&#39;s upload sessions

### Example
```kotlin
// Import classes:
//import org.openapitools.client.infrastructure.*
//import org.openapitools.client.models.*

val apiInstance = UploadsApi()
val offset : kotlin.Int = 56 // kotlin.Int | Offset
val limit : kotlin.Int = 56 // kotlin.Int | Limit
val locateId : kotlin.Int = 56 // kotlin.Int | If specified, \"offset\" parameter will be ignored                                             and the page containing entity with this Id will be returned.
val with : kotlin.String = with_example // kotlin.String | With parameters
val mode : kotlin.String = mode_example // kotlin.String | Response mode
try {
    val result : kotlin.collections.List<Upload> = apiInstance.restUploadsGet(offset, limit, locateId, with, mode)
    println(result)
} catch (e: ClientException) {
    println("4xx response calling UploadsApi#restUploadsGet")
    e.printStackTrace()
} catch (e: ServerException) {
    println("5xx response calling UploadsApi#restUploadsGet")
    e.printStackTrace()
}
```

### Parameters

Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **offset** | **kotlin.Int**| Offset | [optional]
 **limit** | **kotlin.Int**| Limit | [optional]
 **locateId** | **kotlin.Int**| If specified, \&quot;offset\&quot; parameter will be ignored                                             and the page containing entity with this Id will be returned. | [optional]
 **with** | **kotlin.String**| With parameters | [optional]
 **mode** | **kotlin.String**| Response mode | [optional]

### Return type

[**kotlin.collections.List&lt;Upload&gt;**](Upload.md)

### Authorization

No authorization required

### HTTP request headers

 - **Content-Type**: Not defined
 - **Accept**: */*

<a id="restUploadsIdDelete"></a>
# **restUploadsIdDelete**
> restUploadsIdDelete(id)

Terminate chunk upload session

Terminates chunk upload session

### Example
```kotlin
// Import classes:
//import org.openapitools.client.infrastructure.*
//import org.openapitools.client.models.*

val apiInstance = UploadsApi()
val id : kotlin.Int = 56 // kotlin.Int | upload id
try {
    apiInstance.restUploadsIdDelete(id)
} catch (e: ClientException) {
    println("4xx response calling UploadsApi#restUploadsIdDelete")
    e.printStackTrace()
} catch (e: ServerException) {
    println("5xx response calling UploadsApi#restUploadsIdDelete")
    e.printStackTrace()
}
```

### Parameters

Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **id** | **kotlin.Int**| upload id |

### Return type

null (empty response body)

### Authorization

No authorization required

### HTTP request headers

 - **Content-Type**: Not defined
 - **Accept**: Not defined

<a id="restUploadsIdGet"></a>
# **restUploadsIdGet**
> Upload restUploadsIdGet(id, with, mode)

Get Upload

Returns the details of the specified upload

### Example
```kotlin
// Import classes:
//import org.openapitools.client.infrastructure.*
//import org.openapitools.client.models.*

val apiInstance = UploadsApi()
val id : kotlin.Int = 56 // kotlin.Int | ID of the upload to retrieve
val with : kotlin.String = with_example // kotlin.String | With parameters
val mode : kotlin.String = mode_example // kotlin.String | Response mode
try {
    val result : Upload = apiInstance.restUploadsIdGet(id, with, mode)
    println(result)
} catch (e: ClientException) {
    println("4xx response calling UploadsApi#restUploadsIdGet")
    e.printStackTrace()
} catch (e: ServerException) {
    println("5xx response calling UploadsApi#restUploadsIdGet")
    e.printStackTrace()
}
```

### Parameters

Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **id** | **kotlin.Int**| ID of the upload to retrieve |
 **with** | **kotlin.String**| With parameters | [optional]
 **mode** | **kotlin.String**| Response mode | [optional]

### Return type

[**Upload**](Upload.md)

### Authorization

No authorization required

### HTTP request headers

 - **Content-Type**: Not defined
 - **Accept**: */*

