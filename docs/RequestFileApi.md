# RequestFileApi

All URIs are relative to *http://localhost*

Method | HTTP request | Description
------------- | ------------- | -------------
[**restFoldersIdActionsRequestFilePost**](RequestFileApi.md#restFoldersIdActionsRequestFilePost) | **POST** /rest/folders/{id}/actions/requestFile | Send a Request File to Folder
[**restMailActionsRequestFilePost**](RequestFileApi.md#restMailActionsRequestFilePost) | **POST** /rest/mail/actions/requestFile | Send a Request File to Inbox
[**restRequestFileRefActionsFilePost**](RequestFileApi.md#restRequestFileRefActionsFilePost) | **POST** /rest/requestFile/{ref}/actions/file | upload content
[**restRequestFileRefCommentObjectIdPost**](RequestFileApi.md#restRequestFileRefCommentObjectIdPost) | **POST** /rest/requestFile/{ref}/comment/{object_id} | Create a Comment on a file
[**restRequestFileRefDelete**](RequestFileApi.md#restRequestFileRefDelete) | **DELETE** /rest/requestFile/{ref} | Expire the request file
[**restRequestFileRefGet**](RequestFileApi.md#restRequestFileRefGet) | **GET** /rest/requestFile/{ref} | Returns Request File Info by ref
[**restRequestFileRefPreviewObjectIdGet**](RequestFileApi.md#restRequestFileRefPreviewObjectIdGet) | **GET** /rest/requestFile/{ref}/preview/{object_id} | Retrieve information about the file preview.
[**restRequestFileRefReplyPost**](RequestFileApi.md#restRequestFileRefReplyPost) | **POST** /rest/requestFile/{ref}/reply | Reply to Request File
[**restRequestFileRefSourcesGet**](RequestFileApi.md#restRequestFileRefSourcesGet) | **GET** /rest/requestFile/{ref}/sources | Retrieve Request File attached files included by the requester
[**restRequestFileRefSourcesObjectIdContentGet**](RequestFileApi.md#restRequestFileRefSourcesObjectIdContentGet) | **GET** /rest/requestFile/{ref}/sources/{object_id}/content | Read source file content
[**restRequestFileRefSourcesObjectIdGet**](RequestFileApi.md#restRequestFileRefSourcesObjectIdGet) | **GET** /rest/requestFile/{ref}/sources/{object_id} | Read file info
[**restRequestFileRefUploadsGet**](RequestFileApi.md#restRequestFileRefUploadsGet) | **GET** /rest/requestFile/{ref}/uploads | Retrieve Request File uploaded files by the login uploader
[**restRequestFileRefUploadsObjectIdContentGet**](RequestFileApi.md#restRequestFileRefUploadsObjectIdContentGet) | **GET** /rest/requestFile/{ref}/uploads/{object_id}/content | Read source file content
[**restRequestFileRefUploadsObjectIdDelete**](RequestFileApi.md#restRequestFileRefUploadsObjectIdDelete) | **DELETE** /rest/requestFile/{ref}/uploads/{object_id} | Delete uploaded file
[**restRequestFileRefUploadsObjectIdGet**](RequestFileApi.md#restRequestFileRefUploadsObjectIdGet) | **GET** /rest/requestFile/{ref}/uploads/{object_id} | Read uploaded file info
[**restRequestFileUsersUserIdDelete**](RequestFileApi.md#restRequestFileUsersUserIdDelete) | **DELETE** /rest/requestFile/users/{userId} | Delete request files sent by the the specified user


<a id="restFoldersIdActionsRequestFilePost"></a>
# **restFoldersIdActionsRequestFilePost**
> restFoldersIdActionsRequestFilePost(id, body)

Send a Request File to Folder

Send a Request File to Folder

### Example
```kotlin
// Import classes:
//import org.openapitools.client.infrastructure.*
//import org.openapitools.client.models.*

val apiInstance = RequestFileApi()
val id : kotlin.String = id_example // kotlin.String | The ID of the entity
val body : RequestFileToFolderPostRequest =  // RequestFileToFolderPostRequest | 
try {
    apiInstance.restFoldersIdActionsRequestFilePost(id, body)
} catch (e: ClientException) {
    println("4xx response calling RequestFileApi#restFoldersIdActionsRequestFilePost")
    e.printStackTrace()
} catch (e: ServerException) {
    println("5xx response calling RequestFileApi#restFoldersIdActionsRequestFilePost")
    e.printStackTrace()
}
```

### Parameters

Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **id** | **kotlin.String**| The ID of the entity |
 **body** | [**RequestFileToFolderPostRequest**](RequestFileToFolderPostRequest.md)|  |

### Return type

null (empty response body)

### Authorization

No authorization required

### HTTP request headers

 - **Content-Type**: Not defined
 - **Accept**: Not defined

<a id="restMailActionsRequestFilePost"></a>
# **restMailActionsRequestFilePost**
> restMailActionsRequestFilePost(body)

Send a Request File to Inbox

Send a Request File to Inbox

### Example
```kotlin
// Import classes:
//import org.openapitools.client.infrastructure.*
//import org.openapitools.client.models.*

val apiInstance = RequestFileApi()
val body : RequestFileToInboxPostRequest =  // RequestFileToInboxPostRequest | 
try {
    apiInstance.restMailActionsRequestFilePost(body)
} catch (e: ClientException) {
    println("4xx response calling RequestFileApi#restMailActionsRequestFilePost")
    e.printStackTrace()
} catch (e: ServerException) {
    println("5xx response calling RequestFileApi#restMailActionsRequestFilePost")
    e.printStackTrace()
}
```

### Parameters

Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **body** | [**RequestFileToInboxPostRequest**](RequestFileToInboxPostRequest.md)|  |

### Return type

null (empty response body)

### Authorization

No authorization required

### HTTP request headers

 - **Content-Type**: Not defined
 - **Accept**: Not defined

<a id="restRequestFileRefActionsFilePost"></a>
# **restRequestFileRefActionsFilePost**
> restRequestFileRefActionsFilePost(ref, body, returnEntity, mode, clientCreated, clientModified)

upload content

uploads file content to a request folder

### Example
```kotlin
// Import classes:
//import org.openapitools.client.infrastructure.*
//import org.openapitools.client.models.*

val apiInstance = RequestFileApi()
val ref : kotlin.String = ref_example // kotlin.String | Request file short link
val body : io.ktor.client.request.forms.InputProvider = BINARY_DATA_HERE // io.ktor.client.request.forms.InputProvider | file content
val returnEntity : kotlin.Boolean = true // kotlin.Boolean | Return information about newly created entity
val mode : kotlin.String = mode_example // kotlin.String | Response mode
val clientCreated : kotlin.String = 2013-10-20 // kotlin.String | Client created field for the file
val clientModified : kotlin.String = 2013-10-20 // kotlin.String | Client modified field for the file
try {
    apiInstance.restRequestFileRefActionsFilePost(ref, body, returnEntity, mode, clientCreated, clientModified)
} catch (e: ClientException) {
    println("4xx response calling RequestFileApi#restRequestFileRefActionsFilePost")
    e.printStackTrace()
} catch (e: ServerException) {
    println("5xx response calling RequestFileApi#restRequestFileRefActionsFilePost")
    e.printStackTrace()
}
```

### Parameters

Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **ref** | **kotlin.String**| Request file short link |
 **body** | **io.ktor.client.request.forms.InputProvider**| file content |
 **returnEntity** | **kotlin.Boolean**| Return information about newly created entity | [optional]
 **mode** | **kotlin.String**| Response mode | [optional]
 **clientCreated** | **kotlin.String**| Client created field for the file | [optional]
 **clientModified** | **kotlin.String**| Client modified field for the file | [optional]

### Return type

null (empty response body)

### Authorization

No authorization required

### HTTP request headers

 - **Content-Type**: multipart/form-data
 - **Accept**: Not defined

<a id="restRequestFileRefCommentObjectIdPost"></a>
# **restRequestFileRefCommentObjectIdPost**
> restRequestFileRefCommentObjectIdPost(ref, objectId, body, returnEntity, mode)

Create a Comment on a file

Create a Comment on a file.

### Example
```kotlin
// Import classes:
//import org.openapitools.client.infrastructure.*
//import org.openapitools.client.models.*

val apiInstance = RequestFileApi()
val ref : kotlin.String = ref_example // kotlin.String | The request file shortlink
val objectId : kotlin.String = objectId_example // kotlin.String | Object ID of the file being commented on
val body : CommentPost =  // CommentPost | The comment details
val returnEntity : kotlin.Boolean = true // kotlin.Boolean | Return information about newly created entity
val mode : kotlin.String = mode_example // kotlin.String | Response mode
try {
    apiInstance.restRequestFileRefCommentObjectIdPost(ref, objectId, body, returnEntity, mode)
} catch (e: ClientException) {
    println("4xx response calling RequestFileApi#restRequestFileRefCommentObjectIdPost")
    e.printStackTrace()
} catch (e: ServerException) {
    println("5xx response calling RequestFileApi#restRequestFileRefCommentObjectIdPost")
    e.printStackTrace()
}
```

### Parameters

Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **ref** | **kotlin.String**| The request file shortlink |
 **objectId** | **kotlin.String**| Object ID of the file being commented on |
 **body** | [**CommentPost**](CommentPost.md)| The comment details |
 **returnEntity** | **kotlin.Boolean**| Return information about newly created entity | [optional]
 **mode** | **kotlin.String**| Response mode | [optional]

### Return type

null (empty response body)

### Authorization

No authorization required

### HTTP request headers

 - **Content-Type**: Not defined
 - **Accept**: Not defined

<a id="restRequestFileRefDelete"></a>
# **restRequestFileRefDelete**
> RequestFile restRequestFileRefDelete(ref)

Expire the request file

Expire the request file by setting deleted to true

### Example
```kotlin
// Import classes:
//import org.openapitools.client.infrastructure.*
//import org.openapitools.client.models.*

val apiInstance = RequestFileApi()
val ref : kotlin.String = ref_example // kotlin.String | the shortlink of request file to expire
try {
    val result : RequestFile = apiInstance.restRequestFileRefDelete(ref)
    println(result)
} catch (e: ClientException) {
    println("4xx response calling RequestFileApi#restRequestFileRefDelete")
    e.printStackTrace()
} catch (e: ServerException) {
    println("5xx response calling RequestFileApi#restRequestFileRefDelete")
    e.printStackTrace()
}
```

### Parameters

Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **ref** | **kotlin.String**| the shortlink of request file to expire |

### Return type

[**RequestFile**](RequestFile.md)

### Authorization

No authorization required

### HTTP request headers

 - **Content-Type**: Not defined
 - **Accept**: */*

<a id="restRequestFileRefGet"></a>
# **restRequestFileRefGet**
> RequestFile restRequestFileRefGet(ref, read)

Returns Request File Info by ref

Returns Request File Info by ref

### Example
```kotlin
// Import classes:
//import org.openapitools.client.infrastructure.*
//import org.openapitools.client.models.*

val apiInstance = RequestFileApi()
val ref : kotlin.String = ref_example // kotlin.String | The ref of the Request File
val read : kotlin.Boolean = true // kotlin.Boolean | To log view event, default to true
try {
    val result : RequestFile = apiInstance.restRequestFileRefGet(ref, read)
    println(result)
} catch (e: ClientException) {
    println("4xx response calling RequestFileApi#restRequestFileRefGet")
    e.printStackTrace()
} catch (e: ServerException) {
    println("5xx response calling RequestFileApi#restRequestFileRefGet")
    e.printStackTrace()
}
```

### Parameters

Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **ref** | **kotlin.String**| The ref of the Request File |
 **read** | **kotlin.Boolean**| To log view event, default to true | [optional]

### Return type

[**RequestFile**](RequestFile.md)

### Authorization

No authorization required

### HTTP request headers

 - **Content-Type**: Not defined
 - **Accept**: */*

<a id="restRequestFileRefPreviewObjectIdGet"></a>
# **restRequestFileRefPreviewObjectIdGet**
> Preview restRequestFileRefPreviewObjectIdGet(ref, objectId)

Retrieve information about the file preview.

Retrieve information about the file preview.

### Example
```kotlin
// Import classes:
//import org.openapitools.client.infrastructure.*
//import org.openapitools.client.models.*

val apiInstance = RequestFileApi()
val ref : kotlin.String = ref_example // kotlin.String | The request file shortlink
val objectId : kotlin.String = objectId_example // kotlin.String | ID of the file
try {
    val result : Preview = apiInstance.restRequestFileRefPreviewObjectIdGet(ref, objectId)
    println(result)
} catch (e: ClientException) {
    println("4xx response calling RequestFileApi#restRequestFileRefPreviewObjectIdGet")
    e.printStackTrace()
} catch (e: ServerException) {
    println("5xx response calling RequestFileApi#restRequestFileRefPreviewObjectIdGet")
    e.printStackTrace()
}
```

### Parameters

Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **ref** | **kotlin.String**| The request file shortlink |
 **objectId** | **kotlin.String**| ID of the file |

### Return type

[**Preview**](Preview.md)

### Authorization

No authorization required

### HTTP request headers

 - **Content-Type**: Not defined
 - **Accept**: */*

<a id="restRequestFileRefReplyPost"></a>
# **restRequestFileRefReplyPost**
> restRequestFileRefReplyPost(ref, body)

Reply to Request File

Reply to Request File

### Example
```kotlin
// Import classes:
//import org.openapitools.client.infrastructure.*
//import org.openapitools.client.models.*

val apiInstance = RequestFileApi()
val ref : kotlin.String = ref_example // kotlin.String | The ref of the Request File
val body : RequestFileReplyPostRequest =  // RequestFileReplyPostRequest | 
try {
    apiInstance.restRequestFileRefReplyPost(ref, body)
} catch (e: ClientException) {
    println("4xx response calling RequestFileApi#restRequestFileRefReplyPost")
    e.printStackTrace()
} catch (e: ServerException) {
    println("5xx response calling RequestFileApi#restRequestFileRefReplyPost")
    e.printStackTrace()
}
```

### Parameters

Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **ref** | **kotlin.String**| The ref of the Request File |
 **body** | [**RequestFileReplyPostRequest**](RequestFileReplyPostRequest.md)|  |

### Return type

null (empty response body)

### Authorization

No authorization required

### HTTP request headers

 - **Content-Type**: Not defined
 - **Accept**: Not defined

<a id="restRequestFileRefSourcesGet"></a>
# **restRequestFileRefSourcesGet**
> RequestFileSource restRequestFileRefSourcesGet(ref)

Retrieve Request File attached files included by the requester

Returns attached files included by the requester.

### Example
```kotlin
// Import classes:
//import org.openapitools.client.infrastructure.*
//import org.openapitools.client.models.*

val apiInstance = RequestFileApi()
val ref : kotlin.String = ref_example // kotlin.String | the shortlink of request file to retrieve for
try {
    val result : RequestFileSource = apiInstance.restRequestFileRefSourcesGet(ref)
    println(result)
} catch (e: ClientException) {
    println("4xx response calling RequestFileApi#restRequestFileRefSourcesGet")
    e.printStackTrace()
} catch (e: ServerException) {
    println("5xx response calling RequestFileApi#restRequestFileRefSourcesGet")
    e.printStackTrace()
}
```

### Parameters

Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **ref** | **kotlin.String**| the shortlink of request file to retrieve for |

### Return type

[**RequestFileSource**](RequestFileSource.md)

### Authorization

No authorization required

### HTTP request headers

 - **Content-Type**: Not defined
 - **Accept**: */*

<a id="restRequestFileRefSourcesObjectIdContentGet"></a>
# **restRequestFileRefSourcesObjectIdContentGet**
> Content restRequestFileRefSourcesObjectIdContentGet(ref, objectId, range)

Read source file content

Read content of a source file

### Example
```kotlin
// Import classes:
//import org.openapitools.client.infrastructure.*
//import org.openapitools.client.models.*

val apiInstance = RequestFileApi()
val ref : kotlin.String = ref_example // kotlin.String | Request file short link
val objectId : kotlin.String = objectId_example // kotlin.String | ID of the file
val range : kotlin.String = range_example // kotlin.String | Bytes range to retrieve. Example: bytes=0-1024
try {
    val result : Content = apiInstance.restRequestFileRefSourcesObjectIdContentGet(ref, objectId, range)
    println(result)
} catch (e: ClientException) {
    println("4xx response calling RequestFileApi#restRequestFileRefSourcesObjectIdContentGet")
    e.printStackTrace()
} catch (e: ServerException) {
    println("5xx response calling RequestFileApi#restRequestFileRefSourcesObjectIdContentGet")
    e.printStackTrace()
}
```

### Parameters

Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **ref** | **kotlin.String**| Request file short link |
 **objectId** | **kotlin.String**| ID of the file |
 **range** | **kotlin.String**| Bytes range to retrieve. Example: bytes&#x3D;0-1024 | [optional]

### Return type

[**Content**](Content.md)

### Authorization

No authorization required

### HTTP request headers

 - **Content-Type**: Not defined
 - **Accept**: */*

<a id="restRequestFileRefSourcesObjectIdGet"></a>
# **restRequestFileRefSourcesObjectIdGet**
> Content restRequestFileRefSourcesObjectIdGet(ref, objectId, with, mode)

Read file info

Read properties of a source file

### Example
```kotlin
// Import classes:
//import org.openapitools.client.infrastructure.*
//import org.openapitools.client.models.*

val apiInstance = RequestFileApi()
val ref : kotlin.String = ref_example // kotlin.String | The shortlink of the request file
val objectId : kotlin.String = objectId_example // kotlin.String | ID of the source file
val with : kotlin.String = with_example // kotlin.String | With parameters
val mode : kotlin.String = mode_example // kotlin.String | Response mode
try {
    val result : Content = apiInstance.restRequestFileRefSourcesObjectIdGet(ref, objectId, with, mode)
    println(result)
} catch (e: ClientException) {
    println("4xx response calling RequestFileApi#restRequestFileRefSourcesObjectIdGet")
    e.printStackTrace()
} catch (e: ServerException) {
    println("5xx response calling RequestFileApi#restRequestFileRefSourcesObjectIdGet")
    e.printStackTrace()
}
```

### Parameters

Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **ref** | **kotlin.String**| The shortlink of the request file |
 **objectId** | **kotlin.String**| ID of the source file |
 **with** | **kotlin.String**| With parameters | [optional]
 **mode** | **kotlin.String**| Response mode | [optional]

### Return type

[**Content**](Content.md)

### Authorization

No authorization required

### HTTP request headers

 - **Content-Type**: Not defined
 - **Accept**: */*

<a id="restRequestFileRefUploadsGet"></a>
# **restRequestFileRefUploadsGet**
> RequestFileUpload restRequestFileRefUploadsGet(ref)

Retrieve Request File uploaded files by the login uploader

Returns uploaded files by the login uploader.

### Example
```kotlin
// Import classes:
//import org.openapitools.client.infrastructure.*
//import org.openapitools.client.models.*

val apiInstance = RequestFileApi()
val ref : kotlin.String = ref_example // kotlin.String | the shortlink of request file to retrieve for
try {
    val result : RequestFileUpload = apiInstance.restRequestFileRefUploadsGet(ref)
    println(result)
} catch (e: ClientException) {
    println("4xx response calling RequestFileApi#restRequestFileRefUploadsGet")
    e.printStackTrace()
} catch (e: ServerException) {
    println("5xx response calling RequestFileApi#restRequestFileRefUploadsGet")
    e.printStackTrace()
}
```

### Parameters

Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **ref** | **kotlin.String**| the shortlink of request file to retrieve for |

### Return type

[**RequestFileUpload**](RequestFileUpload.md)

### Authorization

No authorization required

### HTTP request headers

 - **Content-Type**: Not defined
 - **Accept**: */*

<a id="restRequestFileRefUploadsObjectIdContentGet"></a>
# **restRequestFileRefUploadsObjectIdContentGet**
> Content restRequestFileRefUploadsObjectIdContentGet(ref, objectId, range)

Read source file content

Read content of a source file

### Example
```kotlin
// Import classes:
//import org.openapitools.client.infrastructure.*
//import org.openapitools.client.models.*

val apiInstance = RequestFileApi()
val ref : kotlin.String = ref_example // kotlin.String | id
val objectId : kotlin.String = objectId_example // kotlin.String | ID of the file
val range : kotlin.String = range_example // kotlin.String | Bytes range to retrieve. Example: bytes=0-1024
try {
    val result : Content = apiInstance.restRequestFileRefUploadsObjectIdContentGet(ref, objectId, range)
    println(result)
} catch (e: ClientException) {
    println("4xx response calling RequestFileApi#restRequestFileRefUploadsObjectIdContentGet")
    e.printStackTrace()
} catch (e: ServerException) {
    println("5xx response calling RequestFileApi#restRequestFileRefUploadsObjectIdContentGet")
    e.printStackTrace()
}
```

### Parameters

Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **ref** | **kotlin.String**| id |
 **objectId** | **kotlin.String**| ID of the file |
 **range** | **kotlin.String**| Bytes range to retrieve. Example: bytes&#x3D;0-1024 | [optional]

### Return type

[**Content**](Content.md)

### Authorization

No authorization required

### HTTP request headers

 - **Content-Type**: Not defined
 - **Accept**: */*

<a id="restRequestFileRefUploadsObjectIdDelete"></a>
# **restRequestFileRefUploadsObjectIdDelete**
> Content restRequestFileRefUploadsObjectIdDelete(ref, objectId)

Delete uploaded file

Delete an uploaded file

### Example
```kotlin
// Import classes:
//import org.openapitools.client.infrastructure.*
//import org.openapitools.client.models.*

val apiInstance = RequestFileApi()
val ref : kotlin.String = ref_example // kotlin.String | weblink
val objectId : kotlin.String = objectId_example // kotlin.String | ID of the uploaded file
try {
    val result : Content = apiInstance.restRequestFileRefUploadsObjectIdDelete(ref, objectId)
    println(result)
} catch (e: ClientException) {
    println("4xx response calling RequestFileApi#restRequestFileRefUploadsObjectIdDelete")
    e.printStackTrace()
} catch (e: ServerException) {
    println("5xx response calling RequestFileApi#restRequestFileRefUploadsObjectIdDelete")
    e.printStackTrace()
}
```

### Parameters

Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **ref** | **kotlin.String**| weblink |
 **objectId** | **kotlin.String**| ID of the uploaded file |

### Return type

[**Content**](Content.md)

### Authorization

No authorization required

### HTTP request headers

 - **Content-Type**: Not defined
 - **Accept**: */*

<a id="restRequestFileRefUploadsObjectIdGet"></a>
# **restRequestFileRefUploadsObjectIdGet**
> Content restRequestFileRefUploadsObjectIdGet(ref, objectId, with, mode)

Read uploaded file info

Read properties of a uploaded file

### Example
```kotlin
// Import classes:
//import org.openapitools.client.infrastructure.*
//import org.openapitools.client.models.*

val apiInstance = RequestFileApi()
val ref : kotlin.String = ref_example // kotlin.String | weblink
val objectId : kotlin.String = objectId_example // kotlin.String | ID of the uploaded file
val with : kotlin.String = with_example // kotlin.String | With parameters
val mode : kotlin.String = mode_example // kotlin.String | Response mode
try {
    val result : Content = apiInstance.restRequestFileRefUploadsObjectIdGet(ref, objectId, with, mode)
    println(result)
} catch (e: ClientException) {
    println("4xx response calling RequestFileApi#restRequestFileRefUploadsObjectIdGet")
    e.printStackTrace()
} catch (e: ServerException) {
    println("5xx response calling RequestFileApi#restRequestFileRefUploadsObjectIdGet")
    e.printStackTrace()
}
```

### Parameters

Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **ref** | **kotlin.String**| weblink |
 **objectId** | **kotlin.String**| ID of the uploaded file |
 **with** | **kotlin.String**| With parameters | [optional]
 **mode** | **kotlin.String**| Response mode | [optional]

### Return type

[**Content**](Content.md)

### Authorization

No authorization required

### HTTP request headers

 - **Content-Type**: Not defined
 - **Accept**: */*

<a id="restRequestFileUsersUserIdDelete"></a>
# **restRequestFileUsersUserIdDelete**
> RequestFile restRequestFileUsersUserIdDelete(userId, requestFileIdColonIn, mode)

Delete request files sent by the the specified user

Delete request files sent by the the specified user

### Example
```kotlin
// Import classes:
//import org.openapitools.client.infrastructure.*
//import org.openapitools.client.models.*

val apiInstance = RequestFileApi()
val userId : kotlin.String = userId_example // kotlin.String | The user ID of request file
val requestFileIdColonIn : kotlin.Int = 56 // kotlin.Int | Search for results that contain any of specified values of this parameter.
val mode : kotlin.String = mode_example // kotlin.String | Response mode
try {
    val result : RequestFile = apiInstance.restRequestFileUsersUserIdDelete(userId, requestFileIdColonIn, mode)
    println(result)
} catch (e: ClientException) {
    println("4xx response calling RequestFileApi#restRequestFileUsersUserIdDelete")
    e.printStackTrace()
} catch (e: ServerException) {
    println("5xx response calling RequestFileApi#restRequestFileUsersUserIdDelete")
    e.printStackTrace()
}
```

### Parameters

Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **userId** | **kotlin.String**| The user ID of request file |
 **requestFileIdColonIn** | **kotlin.Int**| Search for results that contain any of specified values of this parameter. | [optional]
 **mode** | **kotlin.String**| Response mode | [optional]

### Return type

[**RequestFile**](RequestFile.md)

### Authorization

No authorization required

### HTTP request headers

 - **Content-Type**: Not defined
 - **Accept**: */*

