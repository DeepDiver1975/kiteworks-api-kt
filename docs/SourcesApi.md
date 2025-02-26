# SourcesApi

All URIs are relative to *http://localhost*

Method | HTTP request | Description
------------- | ------------- | -------------
[**restSourcesActionsLockPatch**](SourcesApi.md#restSourcesActionsLockPatch) | **PATCH** /rest/sources/actions/lock | Lock EC files
[**restSourcesActionsUnlockPatch**](SourcesApi.md#restSourcesActionsUnlockPatch) | **PATCH** /rest/sources/actions/unlock | Unlock EC files
[**restSourcesAuthPost**](SourcesApi.md#restSourcesAuthPost) | **POST** /rest/sources/auth | Login to cloud source
[**restSourcesFilesActionsTransferStatusGet**](SourcesApi.md#restSourcesFilesActionsTransferStatusGet) | **GET** /rest/sources/files/actions/transferStatus | Get kp transfer status.
[**restSourcesFilesIdDelete**](SourcesApi.md#restSourcesFilesIdDelete) | **DELETE** /rest/sources/files/{id} | Delete an EC file.
[**restSourcesFilesIdGet**](SourcesApi.md#restSourcesFilesIdGet) | **GET** /rest/sources/files/{id} | Get info of an EC file.
[**restSourcesFoldersIdDelete**](SourcesApi.md#restSourcesFoldersIdDelete) | **DELETE** /rest/sources/folders/{id} | Delete an EC folder.
[**restSourcesFoldersIdGet**](SourcesApi.md#restSourcesFoldersIdGet) | **GET** /rest/sources/folders/{id} | Get info of an EC folder.
[**restSourcesGet**](SourcesApi.md#restSourcesGet) | **GET** /rest/sources | Return user&#39;s sources
[**restSourcesIdAuthGet**](SourcesApi.md#restSourcesIdAuthGet) | **GET** /rest/sources/{id}/auth | Get url with redirect to cloud ECM auth
[**restSourcesIdAuthPost**](SourcesApi.md#restSourcesIdAuthPost) | **POST** /rest/sources/{id}/auth | Login to on-premise source
[**restSourcesIdAuthStatusGet**](SourcesApi.md#restSourcesIdAuthStatusGet) | **GET** /rest/sources/{id}/authStatus | Get cloud ECM auth status
[**restSourcesIdChildrenGet**](SourcesApi.md#restSourcesIdChildrenGet) | **GET** /rest/sources/{id}/children | Returns the content of the specified ECM source
[**restSourcesIdDelete**](SourcesApi.md#restSourcesIdDelete) | **DELETE** /rest/sources/{id} | Deletes specified source
[**restSourcesIdExternalEditGet**](SourcesApi.md#restSourcesIdExternalEditGet) | **GET** /rest/sources/{id}/externalEdit | Get access token for external file edit.
[**restSourcesIdFoldersGet**](SourcesApi.md#restSourcesIdFoldersGet) | **GET** /rest/sources/{id}/folders | Returns the list of folders of the specified ECM folder
[**restSourcesIdGet**](SourcesApi.md#restSourcesIdGet) | **GET** /rest/sources/{id} | Returns requested ECM source
[**restSourcesIdPreviewGet**](SourcesApi.md#restSourcesIdPreviewGet) | **GET** /rest/sources/{id}/preview | Retrieve information about the kitepoint file preview.
[**restSourcesParentFilesGet**](SourcesApi.md#restSourcesParentFilesGet) | **GET** /rest/sources/{parent}/files | Returns the list of files of the specified ECM folder
[**restSourcesPost**](SourcesApi.md#restSourcesPost) | **POST** /rest/sources | Add user ECM source


<a id="restSourcesActionsLockPatch"></a>
# **restSourcesActionsLockPatch**
> restSourcesActionsLockPatch(idColonIn, partialSuccess, mode)

Lock EC files

Lock EC files

### Example
```kotlin
// Import classes:
//import org.openapitools.client.infrastructure.*
//import org.openapitools.client.models.*

val apiInstance = SourcesApi()
val idColonIn : kotlin.Int = 56 // kotlin.Int | Array of values which are going to be changed.
val partialSuccess : kotlin.Boolean = true // kotlin.Boolean | Whether to perform action on valid items even if some ones fail
val mode : kotlin.String = mode_example // kotlin.String | Response mode
try {
    apiInstance.restSourcesActionsLockPatch(idColonIn, partialSuccess, mode)
} catch (e: ClientException) {
    println("4xx response calling SourcesApi#restSourcesActionsLockPatch")
    e.printStackTrace()
} catch (e: ServerException) {
    println("5xx response calling SourcesApi#restSourcesActionsLockPatch")
    e.printStackTrace()
}
```

### Parameters

Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **idColonIn** | **kotlin.Int**| Array of values which are going to be changed. |
 **partialSuccess** | **kotlin.Boolean**| Whether to perform action on valid items even if some ones fail | [optional]
 **mode** | **kotlin.String**| Response mode | [optional]

### Return type

null (empty response body)

### Authorization

No authorization required

### HTTP request headers

 - **Content-Type**: Not defined
 - **Accept**: Not defined

<a id="restSourcesActionsUnlockPatch"></a>
# **restSourcesActionsUnlockPatch**
> restSourcesActionsUnlockPatch(idColonIn, partialSuccess, mode)

Unlock EC files

Unlock EC files

### Example
```kotlin
// Import classes:
//import org.openapitools.client.infrastructure.*
//import org.openapitools.client.models.*

val apiInstance = SourcesApi()
val idColonIn : kotlin.Int = 56 // kotlin.Int | Array of values which are going to be changed.
val partialSuccess : kotlin.Boolean = true // kotlin.Boolean | Whether to perform action on valid items even if some ones fail
val mode : kotlin.String = mode_example // kotlin.String | Response mode
try {
    apiInstance.restSourcesActionsUnlockPatch(idColonIn, partialSuccess, mode)
} catch (e: ClientException) {
    println("4xx response calling SourcesApi#restSourcesActionsUnlockPatch")
    e.printStackTrace()
} catch (e: ServerException) {
    println("5xx response calling SourcesApi#restSourcesActionsUnlockPatch")
    e.printStackTrace()
}
```

### Parameters

Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **idColonIn** | **kotlin.Int**| Array of values which are going to be changed. |
 **partialSuccess** | **kotlin.Boolean**| Whether to perform action on valid items even if some ones fail | [optional]
 **mode** | **kotlin.String**| Response mode | [optional]

### Return type

null (empty response body)

### Authorization

No authorization required

### HTTP request headers

 - **Content-Type**: Not defined
 - **Accept**: Not defined

<a id="restSourcesAuthPost"></a>
# **restSourcesAuthPost**
> restSourcesAuthPost(body)

Login to cloud source

Get tokens after ECM auth

### Example
```kotlin
// Import classes:
//import org.openapitools.client.infrastructure.*
//import org.openapitools.client.models.*

val apiInstance = SourcesApi()
val body : CloudSourceLoginPost =  // CloudSourceLoginPost | Login params
try {
    apiInstance.restSourcesAuthPost(body)
} catch (e: ClientException) {
    println("4xx response calling SourcesApi#restSourcesAuthPost")
    e.printStackTrace()
} catch (e: ServerException) {
    println("5xx response calling SourcesApi#restSourcesAuthPost")
    e.printStackTrace()
}
```

### Parameters

Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **body** | [**CloudSourceLoginPost**](CloudSourceLoginPost.md)| Login params |

### Return type

null (empty response body)

### Authorization

No authorization required

### HTTP request headers

 - **Content-Type**: Not defined
 - **Accept**: Not defined

<a id="restSourcesFilesActionsTransferStatusGet"></a>
# **restSourcesFilesActionsTransferStatusGet**
> kotlin.collections.List&lt;KPTransferStatus&gt; restSourcesFilesActionsTransferStatusGet(transactionId, transactionIdColonIn, mode)

Get kp transfer status.

Get status of transfer to EC

### Example
```kotlin
// Import classes:
//import org.openapitools.client.infrastructure.*
//import org.openapitools.client.models.*

val apiInstance = SourcesApi()
val transactionId : kotlin.Int = 56 // kotlin.Int | Transaction ID of download
val transactionIdColonIn : kotlin.Int = 56 // kotlin.Int | Transaction ID of download. Search for results that contain any of specified values of this parameter.
val mode : kotlin.String = mode_example // kotlin.String | Response mode
try {
    val result : kotlin.collections.List<KPTransferStatus> = apiInstance.restSourcesFilesActionsTransferStatusGet(transactionId, transactionIdColonIn, mode)
    println(result)
} catch (e: ClientException) {
    println("4xx response calling SourcesApi#restSourcesFilesActionsTransferStatusGet")
    e.printStackTrace()
} catch (e: ServerException) {
    println("5xx response calling SourcesApi#restSourcesFilesActionsTransferStatusGet")
    e.printStackTrace()
}
```

### Parameters

Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **transactionId** | **kotlin.Int**| Transaction ID of download | [optional]
 **transactionIdColonIn** | **kotlin.Int**| Transaction ID of download. Search for results that contain any of specified values of this parameter. | [optional]
 **mode** | **kotlin.String**| Response mode | [optional]

### Return type

[**kotlin.collections.List&lt;KPTransferStatus&gt;**](KPTransferStatus.md)

### Authorization

No authorization required

### HTTP request headers

 - **Content-Type**: Not defined
 - **Accept**: */*

<a id="restSourcesFilesIdDelete"></a>
# **restSourcesFilesIdDelete**
> restSourcesFilesIdDelete(id, forceDelete, mode)

Delete an EC file.

Delete an EC file.

### Example
```kotlin
// Import classes:
//import org.openapitools.client.infrastructure.*
//import org.openapitools.client.models.*

val apiInstance = SourcesApi()
val id : kotlin.String = id_example // kotlin.String | ID of EC file
val forceDelete : kotlin.Boolean = true // kotlin.Boolean | If set to True user can delete file which only in his use
val mode : kotlin.String = mode_example // kotlin.String | Response mode
try {
    apiInstance.restSourcesFilesIdDelete(id, forceDelete, mode)
} catch (e: ClientException) {
    println("4xx response calling SourcesApi#restSourcesFilesIdDelete")
    e.printStackTrace()
} catch (e: ServerException) {
    println("5xx response calling SourcesApi#restSourcesFilesIdDelete")
    e.printStackTrace()
}
```

### Parameters

Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **id** | **kotlin.String**| ID of EC file |
 **forceDelete** | **kotlin.Boolean**| If set to True user can delete file which only in his use | [optional]
 **mode** | **kotlin.String**| Response mode | [optional]

### Return type

null (empty response body)

### Authorization

No authorization required

### HTTP request headers

 - **Content-Type**: Not defined
 - **Accept**: Not defined

<a id="restSourcesFilesIdGet"></a>
# **restSourcesFilesIdGet**
> SourceFile restSourcesFilesIdGet(id, with, mode)

Get info of an EC file.

Get info of an EC file.

### Example
```kotlin
// Import classes:
//import org.openapitools.client.infrastructure.*
//import org.openapitools.client.models.*

val apiInstance = SourcesApi()
val id : kotlin.String = id_example // kotlin.String | ID of EC file
val with : kotlin.String = with_example // kotlin.String | With parameters
val mode : kotlin.String = mode_example // kotlin.String | Response mode
try {
    val result : SourceFile = apiInstance.restSourcesFilesIdGet(id, with, mode)
    println(result)
} catch (e: ClientException) {
    println("4xx response calling SourcesApi#restSourcesFilesIdGet")
    e.printStackTrace()
} catch (e: ServerException) {
    println("5xx response calling SourcesApi#restSourcesFilesIdGet")
    e.printStackTrace()
}
```

### Parameters

Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **id** | **kotlin.String**| ID of EC file |
 **with** | **kotlin.String**| With parameters | [optional]
 **mode** | **kotlin.String**| Response mode | [optional]

### Return type

[**SourceFile**](SourceFile.md)

### Authorization

No authorization required

### HTTP request headers

 - **Content-Type**: Not defined
 - **Accept**: */*

<a id="restSourcesFoldersIdDelete"></a>
# **restSourcesFoldersIdDelete**
> restSourcesFoldersIdDelete(id)

Delete an EC folder.

Delete an EC folder.

### Example
```kotlin
// Import classes:
//import org.openapitools.client.infrastructure.*
//import org.openapitools.client.models.*

val apiInstance = SourcesApi()
val id : kotlin.String = id_example // kotlin.String | ID of EC folder
try {
    apiInstance.restSourcesFoldersIdDelete(id)
} catch (e: ClientException) {
    println("4xx response calling SourcesApi#restSourcesFoldersIdDelete")
    e.printStackTrace()
} catch (e: ServerException) {
    println("5xx response calling SourcesApi#restSourcesFoldersIdDelete")
    e.printStackTrace()
}
```

### Parameters

Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **id** | **kotlin.String**| ID of EC folder |

### Return type

null (empty response body)

### Authorization

No authorization required

### HTTP request headers

 - **Content-Type**: Not defined
 - **Accept**: Not defined

<a id="restSourcesFoldersIdGet"></a>
# **restSourcesFoldersIdGet**
> SourceFolder restSourcesFoldersIdGet(id, with, mode)

Get info of an EC folder.

Get info of an EC folder.

### Example
```kotlin
// Import classes:
//import org.openapitools.client.infrastructure.*
//import org.openapitools.client.models.*

val apiInstance = SourcesApi()
val id : kotlin.String = id_example // kotlin.String | ID of EC folder
val with : kotlin.String = with_example // kotlin.String | With parameters
val mode : kotlin.String = mode_example // kotlin.String | Response mode
try {
    val result : SourceFolder = apiInstance.restSourcesFoldersIdGet(id, with, mode)
    println(result)
} catch (e: ClientException) {
    println("4xx response calling SourcesApi#restSourcesFoldersIdGet")
    e.printStackTrace()
} catch (e: ServerException) {
    println("5xx response calling SourcesApi#restSourcesFoldersIdGet")
    e.printStackTrace()
}
```

### Parameters

Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **id** | **kotlin.String**| ID of EC folder |
 **with** | **kotlin.String**| With parameters | [optional]
 **mode** | **kotlin.String**| Response mode | [optional]

### Return type

[**SourceFolder**](SourceFolder.md)

### Authorization

No authorization required

### HTTP request headers

 - **Content-Type**: Not defined
 - **Accept**: */*

<a id="restSourcesGet"></a>
# **restSourcesGet**
> Sources restSourcesGet(includeKw, searchType, limit, query, includeContainer, offset)

Return user&#39;s sources

Return user&#39;s sources

### Example
```kotlin
// Import classes:
//import org.openapitools.client.infrastructure.*
//import org.openapitools.client.models.*

val apiInstance = SourcesApi()
val includeKw : kotlin.Boolean = true // kotlin.Boolean | 
val searchType : kotlin.String = searchType_example // kotlin.String | 
val limit : kotlin.Int = 56 // kotlin.Int | 
val query : kotlin.String = query_example // kotlin.String | 
val includeContainer : kotlin.Boolean = true // kotlin.Boolean | 
val offset : kotlin.Int = 56 // kotlin.Int | 
try {
    val result : Sources = apiInstance.restSourcesGet(includeKw, searchType, limit, query, includeContainer, offset)
    println(result)
} catch (e: ClientException) {
    println("4xx response calling SourcesApi#restSourcesGet")
    e.printStackTrace()
} catch (e: ServerException) {
    println("5xx response calling SourcesApi#restSourcesGet")
    e.printStackTrace()
}
```

### Parameters

Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **includeKw** | **kotlin.Boolean**|  | [optional]
 **searchType** | **kotlin.String**|  | [optional]
 **limit** | **kotlin.Int**|  | [optional]
 **query** | **kotlin.String**|  | [optional]
 **includeContainer** | **kotlin.Boolean**|  | [optional]
 **offset** | **kotlin.Int**|  | [optional]

### Return type

[**Sources**](Sources.md)

### Authorization

No authorization required

### HTTP request headers

 - **Content-Type**: Not defined
 - **Accept**: */*

<a id="restSourcesIdAuthGet"></a>
# **restSourcesIdAuthGet**
> EcmAuth restSourcesIdAuthGet(id)

Get url with redirect to cloud ECM auth

Get url with redirect to cloud ECM auth

### Example
```kotlin
// Import classes:
//import org.openapitools.client.infrastructure.*
//import org.openapitools.client.models.*

val apiInstance = SourcesApi()
val id : kotlin.Int = 56 // kotlin.Int | The source ID
try {
    val result : EcmAuth = apiInstance.restSourcesIdAuthGet(id)
    println(result)
} catch (e: ClientException) {
    println("4xx response calling SourcesApi#restSourcesIdAuthGet")
    e.printStackTrace()
} catch (e: ServerException) {
    println("5xx response calling SourcesApi#restSourcesIdAuthGet")
    e.printStackTrace()
}
```

### Parameters

Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **id** | **kotlin.Int**| The source ID |

### Return type

[**EcmAuth**](EcmAuth.md)

### Authorization

No authorization required

### HTTP request headers

 - **Content-Type**: Not defined
 - **Accept**: */*

<a id="restSourcesIdAuthPost"></a>
# **restSourcesIdAuthPost**
> restSourcesIdAuthPost(id, body)

Login to on-premise source

Login to on-premise source

### Example
```kotlin
// Import classes:
//import org.openapitools.client.infrastructure.*
//import org.openapitools.client.models.*

val apiInstance = SourcesApi()
val id : kotlin.String = id_example // kotlin.String | The source ID
val body : OnPremiseSourceLoginPost =  // OnPremiseSourceLoginPost | Login params
try {
    apiInstance.restSourcesIdAuthPost(id, body)
} catch (e: ClientException) {
    println("4xx response calling SourcesApi#restSourcesIdAuthPost")
    e.printStackTrace()
} catch (e: ServerException) {
    println("5xx response calling SourcesApi#restSourcesIdAuthPost")
    e.printStackTrace()
}
```

### Parameters

Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **id** | **kotlin.String**| The source ID |
 **body** | [**OnPremiseSourceLoginPost**](OnPremiseSourceLoginPost.md)| Login params |

### Return type

null (empty response body)

### Authorization

No authorization required

### HTTP request headers

 - **Content-Type**: Not defined
 - **Accept**: Not defined

<a id="restSourcesIdAuthStatusGet"></a>
# **restSourcesIdAuthStatusGet**
> restSourcesIdAuthStatusGet(id)

Get cloud ECM auth status

Get cloud ECM auth status

### Example
```kotlin
// Import classes:
//import org.openapitools.client.infrastructure.*
//import org.openapitools.client.models.*

val apiInstance = SourcesApi()
val id : kotlin.Int = 56 // kotlin.Int | The source ID
try {
    apiInstance.restSourcesIdAuthStatusGet(id)
} catch (e: ClientException) {
    println("4xx response calling SourcesApi#restSourcesIdAuthStatusGet")
    e.printStackTrace()
} catch (e: ServerException) {
    println("5xx response calling SourcesApi#restSourcesIdAuthStatusGet")
    e.printStackTrace()
}
```

### Parameters

Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **id** | **kotlin.Int**| The source ID |

### Return type

null (empty response body)

### Authorization

No authorization required

### HTTP request headers

 - **Content-Type**: Not defined
 - **Accept**: Not defined

<a id="restSourcesIdChildrenGet"></a>
# **restSourcesIdChildrenGet**
> kotlin.collections.List&lt;SourceContent&gt; restSourcesIdChildrenGet(id, name, nameColonContains, description, descriptionColonContains, created, createdColonGt, createdColonGte, createdColonLt, createdColonLte, modified, modifiedColonGt, modifiedColonGte, modifiedColonLt, modifiedColonLte, deleted, type, orderBy, offset, limit, with, mode)

Returns the content of the specified ECM source

Returns the content of the requested source.

### Example
```kotlin
// Import classes:
//import org.openapitools.client.infrastructure.*
//import org.openapitools.client.models.*

val apiInstance = SourcesApi()
val id : kotlin.String = id_example // kotlin.String | ID of the source folder to be retrieved
val name : kotlin.String = name_example // kotlin.String | Object name
val nameColonContains : kotlin.String = nameColonContains_example // kotlin.String | Object name. Search for result that contains specified characters in this parameter.
val description : kotlin.String = description_example // kotlin.String | Object description
val descriptionColonContains : kotlin.String = descriptionColonContains_example // kotlin.String | Object description. Search for result that contains specified characters in this parameter.
val created : kotlin.String = 2013-10-20 // kotlin.String | Object creation date
val createdColonGt : kotlin.String = 2013-10-20 // kotlin.String | Object creation date. Search for result that has this parameter value greater than specified.
val createdColonGte : kotlin.String = 2013-10-20 // kotlin.String | Object creation date. Search for result that has this parameter value greater or equal to the specified.
val createdColonLt : kotlin.String = 2013-10-20 // kotlin.String | Object creation date. Search for result that has this parameter value less than specified.
val createdColonLte : kotlin.String = 2013-10-20 // kotlin.String | Object creation date. Search for result that has this parameter value less or equal to the specified.
val modified : kotlin.String = 2013-10-20 // kotlin.String | Object modification date
val modifiedColonGt : kotlin.String = 2013-10-20 // kotlin.String | Object modification date. Search for result that has this parameter value greater than specified.
val modifiedColonGte : kotlin.String = 2013-10-20 // kotlin.String | Object modification date. Search for result that has this parameter value greater or equal to the specified.
val modifiedColonLt : kotlin.String = 2013-10-20 // kotlin.String | Object modification date. Search for result that has this parameter value less than specified.
val modifiedColonLte : kotlin.String = 2013-10-20 // kotlin.String | Object modification date. Search for result that has this parameter value less or equal to the specified.
val deleted : kotlin.Boolean = true // kotlin.Boolean | Indicates that object is deleted
val type : kotlin.String = type_example // kotlin.String | Object type to return
val orderBy : kotlin.collections.List<kotlin.String> =  // kotlin.collections.List<kotlin.String> | Sorting options
val offset : kotlin.Int = 56 // kotlin.Int | Offset
val limit : kotlin.Int = 56 // kotlin.Int | Limit
val with : kotlin.String = with_example // kotlin.String | With parameters
val mode : kotlin.String = mode_example // kotlin.String | Response mode
try {
    val result : kotlin.collections.List<SourceContent> = apiInstance.restSourcesIdChildrenGet(id, name, nameColonContains, description, descriptionColonContains, created, createdColonGt, createdColonGte, createdColonLt, createdColonLte, modified, modifiedColonGt, modifiedColonGte, modifiedColonLt, modifiedColonLte, deleted, type, orderBy, offset, limit, with, mode)
    println(result)
} catch (e: ClientException) {
    println("4xx response calling SourcesApi#restSourcesIdChildrenGet")
    e.printStackTrace()
} catch (e: ServerException) {
    println("5xx response calling SourcesApi#restSourcesIdChildrenGet")
    e.printStackTrace()
}
```

### Parameters

Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **id** | **kotlin.String**| ID of the source folder to be retrieved |
 **name** | **kotlin.String**| Object name | [optional]
 **nameColonContains** | **kotlin.String**| Object name. Search for result that contains specified characters in this parameter. | [optional]
 **description** | **kotlin.String**| Object description | [optional]
 **descriptionColonContains** | **kotlin.String**| Object description. Search for result that contains specified characters in this parameter. | [optional]
 **created** | **kotlin.String**| Object creation date | [optional]
 **createdColonGt** | **kotlin.String**| Object creation date. Search for result that has this parameter value greater than specified. | [optional]
 **createdColonGte** | **kotlin.String**| Object creation date. Search for result that has this parameter value greater or equal to the specified. | [optional]
 **createdColonLt** | **kotlin.String**| Object creation date. Search for result that has this parameter value less than specified. | [optional]
 **createdColonLte** | **kotlin.String**| Object creation date. Search for result that has this parameter value less or equal to the specified. | [optional]
 **modified** | **kotlin.String**| Object modification date | [optional]
 **modifiedColonGt** | **kotlin.String**| Object modification date. Search for result that has this parameter value greater than specified. | [optional]
 **modifiedColonGte** | **kotlin.String**| Object modification date. Search for result that has this parameter value greater or equal to the specified. | [optional]
 **modifiedColonLt** | **kotlin.String**| Object modification date. Search for result that has this parameter value less than specified. | [optional]
 **modifiedColonLte** | **kotlin.String**| Object modification date. Search for result that has this parameter value less or equal to the specified. | [optional]
 **deleted** | **kotlin.Boolean**| Indicates that object is deleted | [optional]
 **type** | **kotlin.String**| Object type to return | [optional]
 **orderBy** | [**kotlin.collections.List&lt;kotlin.String&gt;**](kotlin.String.md)| Sorting options | [optional]
 **offset** | **kotlin.Int**| Offset | [optional]
 **limit** | **kotlin.Int**| Limit | [optional]
 **with** | **kotlin.String**| With parameters | [optional]
 **mode** | **kotlin.String**| Response mode | [optional]

### Return type

[**kotlin.collections.List&lt;SourceContent&gt;**](SourceContent.md)

### Authorization

No authorization required

### HTTP request headers

 - **Content-Type**: Not defined
 - **Accept**: */*

<a id="restSourcesIdDelete"></a>
# **restSourcesIdDelete**
> restSourcesIdDelete(id)

Deletes specified source

Deletes specified source.

### Example
```kotlin
// Import classes:
//import org.openapitools.client.infrastructure.*
//import org.openapitools.client.models.*

val apiInstance = SourcesApi()
val id : kotlin.String = id_example // kotlin.String | ID of the source to be deleted.
try {
    apiInstance.restSourcesIdDelete(id)
} catch (e: ClientException) {
    println("4xx response calling SourcesApi#restSourcesIdDelete")
    e.printStackTrace()
} catch (e: ServerException) {
    println("5xx response calling SourcesApi#restSourcesIdDelete")
    e.printStackTrace()
}
```

### Parameters

Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **id** | **kotlin.String**| ID of the source to be deleted. |

### Return type

null (empty response body)

### Authorization

No authorization required

### HTTP request headers

 - **Content-Type**: Not defined
 - **Accept**: Not defined

<a id="restSourcesIdExternalEditGet"></a>
# **restSourcesIdExternalEditGet**
> RefreshToken restSourcesIdExternalEditGet(id, with, mode)

Get access token for external file edit.

Retrieve refresh token for external file edit.

### Example
```kotlin
// Import classes:
//import org.openapitools.client.infrastructure.*
//import org.openapitools.client.models.*

val apiInstance = SourcesApi()
val id : kotlin.Int = 56 // kotlin.Int | ID of the file
val with : kotlin.String = with_example // kotlin.String | With parameters
val mode : kotlin.String = mode_example // kotlin.String | Response mode
try {
    val result : RefreshToken = apiInstance.restSourcesIdExternalEditGet(id, with, mode)
    println(result)
} catch (e: ClientException) {
    println("4xx response calling SourcesApi#restSourcesIdExternalEditGet")
    e.printStackTrace()
} catch (e: ServerException) {
    println("5xx response calling SourcesApi#restSourcesIdExternalEditGet")
    e.printStackTrace()
}
```

### Parameters

Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **id** | **kotlin.Int**| ID of the file |
 **with** | **kotlin.String**| With parameters | [optional]
 **mode** | **kotlin.String**| Response mode | [optional]

### Return type

[**RefreshToken**](RefreshToken.md)

### Authorization

No authorization required

### HTTP request headers

 - **Content-Type**: Not defined
 - **Accept**: */*

<a id="restSourcesIdFoldersGet"></a>
# **restSourcesIdFoldersGet**
> kotlin.collections.List&lt;SourceContent&gt; restSourcesIdFoldersGet(id, name, nameColonContains, description, descriptionColonContains, created, createdColonGt, createdColonGte, createdColonLt, createdColonLte, modified, modifiedColonGt, modifiedColonGte, modifiedColonLt, modifiedColonLte, deleted, orderBy, offset, limit, with, mode)

Returns the list of folders of the specified ECM folder

Returns the content of the requested source.

### Example
```kotlin
// Import classes:
//import org.openapitools.client.infrastructure.*
//import org.openapitools.client.models.*

val apiInstance = SourcesApi()
val id : kotlin.String = id_example // kotlin.String | ID of the source folder to be retrieved
val name : kotlin.String = name_example // kotlin.String | Object name
val nameColonContains : kotlin.String = nameColonContains_example // kotlin.String | Object name. Search for result that contains specified characters in this parameter.
val description : kotlin.String = description_example // kotlin.String | Object description
val descriptionColonContains : kotlin.String = descriptionColonContains_example // kotlin.String | Object description. Search for result that contains specified characters in this parameter.
val created : kotlin.String = 2013-10-20 // kotlin.String | Object creation date
val createdColonGt : kotlin.String = 2013-10-20 // kotlin.String | Object creation date. Search for result that has this parameter value greater than specified.
val createdColonGte : kotlin.String = 2013-10-20 // kotlin.String | Object creation date. Search for result that has this parameter value greater or equal to the specified.
val createdColonLt : kotlin.String = 2013-10-20 // kotlin.String | Object creation date. Search for result that has this parameter value less than specified.
val createdColonLte : kotlin.String = 2013-10-20 // kotlin.String | Object creation date. Search for result that has this parameter value less or equal to the specified.
val modified : kotlin.String = 2013-10-20 // kotlin.String | Object modification date
val modifiedColonGt : kotlin.String = 2013-10-20 // kotlin.String | Object modification date. Search for result that has this parameter value greater than specified.
val modifiedColonGte : kotlin.String = 2013-10-20 // kotlin.String | Object modification date. Search for result that has this parameter value greater or equal to the specified.
val modifiedColonLt : kotlin.String = 2013-10-20 // kotlin.String | Object modification date. Search for result that has this parameter value less than specified.
val modifiedColonLte : kotlin.String = 2013-10-20 // kotlin.String | Object modification date. Search for result that has this parameter value less or equal to the specified.
val deleted : kotlin.Boolean = true // kotlin.Boolean | Indicates that object is deleted
val orderBy : kotlin.collections.List<kotlin.String> =  // kotlin.collections.List<kotlin.String> | Sorting options
val offset : kotlin.Int = 56 // kotlin.Int | Offset
val limit : kotlin.Int = 56 // kotlin.Int | Limit
val with : kotlin.String = with_example // kotlin.String | With parameters
val mode : kotlin.String = mode_example // kotlin.String | Response mode
try {
    val result : kotlin.collections.List<SourceContent> = apiInstance.restSourcesIdFoldersGet(id, name, nameColonContains, description, descriptionColonContains, created, createdColonGt, createdColonGte, createdColonLt, createdColonLte, modified, modifiedColonGt, modifiedColonGte, modifiedColonLt, modifiedColonLte, deleted, orderBy, offset, limit, with, mode)
    println(result)
} catch (e: ClientException) {
    println("4xx response calling SourcesApi#restSourcesIdFoldersGet")
    e.printStackTrace()
} catch (e: ServerException) {
    println("5xx response calling SourcesApi#restSourcesIdFoldersGet")
    e.printStackTrace()
}
```

### Parameters

Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **id** | **kotlin.String**| ID of the source folder to be retrieved |
 **name** | **kotlin.String**| Object name | [optional]
 **nameColonContains** | **kotlin.String**| Object name. Search for result that contains specified characters in this parameter. | [optional]
 **description** | **kotlin.String**| Object description | [optional]
 **descriptionColonContains** | **kotlin.String**| Object description. Search for result that contains specified characters in this parameter. | [optional]
 **created** | **kotlin.String**| Object creation date | [optional]
 **createdColonGt** | **kotlin.String**| Object creation date. Search for result that has this parameter value greater than specified. | [optional]
 **createdColonGte** | **kotlin.String**| Object creation date. Search for result that has this parameter value greater or equal to the specified. | [optional]
 **createdColonLt** | **kotlin.String**| Object creation date. Search for result that has this parameter value less than specified. | [optional]
 **createdColonLte** | **kotlin.String**| Object creation date. Search for result that has this parameter value less or equal to the specified. | [optional]
 **modified** | **kotlin.String**| Object modification date | [optional]
 **modifiedColonGt** | **kotlin.String**| Object modification date. Search for result that has this parameter value greater than specified. | [optional]
 **modifiedColonGte** | **kotlin.String**| Object modification date. Search for result that has this parameter value greater or equal to the specified. | [optional]
 **modifiedColonLt** | **kotlin.String**| Object modification date. Search for result that has this parameter value less than specified. | [optional]
 **modifiedColonLte** | **kotlin.String**| Object modification date. Search for result that has this parameter value less or equal to the specified. | [optional]
 **deleted** | **kotlin.Boolean**| Indicates that object is deleted | [optional]
 **orderBy** | [**kotlin.collections.List&lt;kotlin.String&gt;**](kotlin.String.md)| Sorting options | [optional]
 **offset** | **kotlin.Int**| Offset | [optional]
 **limit** | **kotlin.Int**| Limit | [optional]
 **with** | **kotlin.String**| With parameters | [optional]
 **mode** | **kotlin.String**| Response mode | [optional]

### Return type

[**kotlin.collections.List&lt;SourceContent&gt;**](SourceContent.md)

### Authorization

No authorization required

### HTTP request headers

 - **Content-Type**: Not defined
 - **Accept**: */*

<a id="restSourcesIdGet"></a>
# **restSourcesIdGet**
> Source restSourcesIdGet(id, with, mode)

Returns requested ECM source

Returns requested source.

### Example
```kotlin
// Import classes:
//import org.openapitools.client.infrastructure.*
//import org.openapitools.client.models.*

val apiInstance = SourcesApi()
val id : kotlin.String = id_example // kotlin.String | ID of the source to be retrieved
val with : kotlin.String = with_example // kotlin.String | With parameters
val mode : kotlin.String = mode_example // kotlin.String | Response mode
try {
    val result : Source = apiInstance.restSourcesIdGet(id, with, mode)
    println(result)
} catch (e: ClientException) {
    println("4xx response calling SourcesApi#restSourcesIdGet")
    e.printStackTrace()
} catch (e: ServerException) {
    println("5xx response calling SourcesApi#restSourcesIdGet")
    e.printStackTrace()
}
```

### Parameters

Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **id** | **kotlin.String**| ID of the source to be retrieved |
 **with** | **kotlin.String**| With parameters | [optional]
 **mode** | **kotlin.String**| Response mode | [optional]

### Return type

[**Source**](Source.md)

### Authorization

No authorization required

### HTTP request headers

 - **Content-Type**: Not defined
 - **Accept**: */*

<a id="restSourcesIdPreviewGet"></a>
# **restSourcesIdPreviewGet**
> KitepointPreview restSourcesIdPreviewGet(id)

Retrieve information about the kitepoint file preview.

Retrieve information about the kitepoint file preview.

### Example
```kotlin
// Import classes:
//import org.openapitools.client.infrastructure.*
//import org.openapitools.client.models.*

val apiInstance = SourcesApi()
val id : kotlin.Int = 56 // kotlin.Int | ID of the kitepoint file
try {
    val result : KitepointPreview = apiInstance.restSourcesIdPreviewGet(id)
    println(result)
} catch (e: ClientException) {
    println("4xx response calling SourcesApi#restSourcesIdPreviewGet")
    e.printStackTrace()
} catch (e: ServerException) {
    println("5xx response calling SourcesApi#restSourcesIdPreviewGet")
    e.printStackTrace()
}
```

### Parameters

Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **id** | **kotlin.Int**| ID of the kitepoint file |

### Return type

[**KitepointPreview**](KitepointPreview.md)

### Authorization

No authorization required

### HTTP request headers

 - **Content-Type**: Not defined
 - **Accept**: */*

<a id="restSourcesParentFilesGet"></a>
# **restSourcesParentFilesGet**
> kotlin.collections.List&lt;SourceContent&gt; restSourcesParentFilesGet(parent, name, nameColonContains, description, descriptionColonContains, created, createdColonGt, createdColonGte, createdColonLt, createdColonLte, modified, modifiedColonGt, modifiedColonGte, modifiedColonLt, modifiedColonLte, deleted, orderBy, offset, limit, with, mode)

Returns the list of files of the specified ECM folder

Returns the list of files of the requested ECM folder.

### Example
```kotlin
// Import classes:
//import org.openapitools.client.infrastructure.*
//import org.openapitools.client.models.*

val apiInstance = SourcesApi()
val parent : kotlin.String = parent_example // kotlin.String | ID of the source folder to be retrieved
val name : kotlin.String = name_example // kotlin.String | Object name
val nameColonContains : kotlin.String = nameColonContains_example // kotlin.String | Object name. Search for result that contains specified characters in this parameter.
val description : kotlin.String = description_example // kotlin.String | Object description
val descriptionColonContains : kotlin.String = descriptionColonContains_example // kotlin.String | Object description. Search for result that contains specified characters in this parameter.
val created : kotlin.String = 2013-10-20 // kotlin.String | Object creation date
val createdColonGt : kotlin.String = 2013-10-20 // kotlin.String | Object creation date. Search for result that has this parameter value greater than specified.
val createdColonGte : kotlin.String = 2013-10-20 // kotlin.String | Object creation date. Search for result that has this parameter value greater or equal to the specified.
val createdColonLt : kotlin.String = 2013-10-20 // kotlin.String | Object creation date. Search for result that has this parameter value less than specified.
val createdColonLte : kotlin.String = 2013-10-20 // kotlin.String | Object creation date. Search for result that has this parameter value less or equal to the specified.
val modified : kotlin.String = 2013-10-20 // kotlin.String | Object modification date
val modifiedColonGt : kotlin.String = 2013-10-20 // kotlin.String | Object modification date. Search for result that has this parameter value greater than specified.
val modifiedColonGte : kotlin.String = 2013-10-20 // kotlin.String | Object modification date. Search for result that has this parameter value greater or equal to the specified.
val modifiedColonLt : kotlin.String = 2013-10-20 // kotlin.String | Object modification date. Search for result that has this parameter value less than specified.
val modifiedColonLte : kotlin.String = 2013-10-20 // kotlin.String | Object modification date. Search for result that has this parameter value less or equal to the specified.
val deleted : kotlin.Boolean = true // kotlin.Boolean | Indicates that object is deleted
val orderBy : kotlin.collections.List<kotlin.String> =  // kotlin.collections.List<kotlin.String> | Sorting options
val offset : kotlin.Int = 56 // kotlin.Int | Offset
val limit : kotlin.Int = 56 // kotlin.Int | Limit
val with : kotlin.String = with_example // kotlin.String | With parameters
val mode : kotlin.String = mode_example // kotlin.String | Response mode
try {
    val result : kotlin.collections.List<SourceContent> = apiInstance.restSourcesParentFilesGet(parent, name, nameColonContains, description, descriptionColonContains, created, createdColonGt, createdColonGte, createdColonLt, createdColonLte, modified, modifiedColonGt, modifiedColonGte, modifiedColonLt, modifiedColonLte, deleted, orderBy, offset, limit, with, mode)
    println(result)
} catch (e: ClientException) {
    println("4xx response calling SourcesApi#restSourcesParentFilesGet")
    e.printStackTrace()
} catch (e: ServerException) {
    println("5xx response calling SourcesApi#restSourcesParentFilesGet")
    e.printStackTrace()
}
```

### Parameters

Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **parent** | **kotlin.String**| ID of the source folder to be retrieved |
 **name** | **kotlin.String**| Object name | [optional]
 **nameColonContains** | **kotlin.String**| Object name. Search for result that contains specified characters in this parameter. | [optional]
 **description** | **kotlin.String**| Object description | [optional]
 **descriptionColonContains** | **kotlin.String**| Object description. Search for result that contains specified characters in this parameter. | [optional]
 **created** | **kotlin.String**| Object creation date | [optional]
 **createdColonGt** | **kotlin.String**| Object creation date. Search for result that has this parameter value greater than specified. | [optional]
 **createdColonGte** | **kotlin.String**| Object creation date. Search for result that has this parameter value greater or equal to the specified. | [optional]
 **createdColonLt** | **kotlin.String**| Object creation date. Search for result that has this parameter value less than specified. | [optional]
 **createdColonLte** | **kotlin.String**| Object creation date. Search for result that has this parameter value less or equal to the specified. | [optional]
 **modified** | **kotlin.String**| Object modification date | [optional]
 **modifiedColonGt** | **kotlin.String**| Object modification date. Search for result that has this parameter value greater than specified. | [optional]
 **modifiedColonGte** | **kotlin.String**| Object modification date. Search for result that has this parameter value greater or equal to the specified. | [optional]
 **modifiedColonLt** | **kotlin.String**| Object modification date. Search for result that has this parameter value less than specified. | [optional]
 **modifiedColonLte** | **kotlin.String**| Object modification date. Search for result that has this parameter value less or equal to the specified. | [optional]
 **deleted** | **kotlin.Boolean**| Indicates that object is deleted | [optional]
 **orderBy** | [**kotlin.collections.List&lt;kotlin.String&gt;**](kotlin.String.md)| Sorting options | [optional]
 **offset** | **kotlin.Int**| Offset | [optional]
 **limit** | **kotlin.Int**| Limit | [optional]
 **with** | **kotlin.String**| With parameters | [optional]
 **mode** | **kotlin.String**| Response mode | [optional]

### Return type

[**kotlin.collections.List&lt;SourceContent&gt;**](SourceContent.md)

### Authorization

No authorization required

### HTTP request headers

 - **Content-Type**: Not defined
 - **Accept**: */*

<a id="restSourcesPost"></a>
# **restSourcesPost**
> restSourcesPost(body, returnEntity, mode)

Add user ECM source

Add user source.

### Example
```kotlin
// Import classes:
//import org.openapitools.client.infrastructure.*
//import org.openapitools.client.models.*

val apiInstance = SourcesApi()
val body : SourcePost =  // SourcePost | source details
val returnEntity : kotlin.Boolean = true // kotlin.Boolean | Return information about newly created entity
val mode : kotlin.String = mode_example // kotlin.String | Response mode
try {
    apiInstance.restSourcesPost(body, returnEntity, mode)
} catch (e: ClientException) {
    println("4xx response calling SourcesApi#restSourcesPost")
    e.printStackTrace()
} catch (e: ServerException) {
    println("5xx response calling SourcesApi#restSourcesPost")
    e.printStackTrace()
}
```

### Parameters

Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **body** | [**SourcePost**](SourcePost.md)| source details |
 **returnEntity** | **kotlin.Boolean**| Return information about newly created entity | [optional]
 **mode** | **kotlin.String**| Response mode | [optional]

### Return type

null (empty response body)

### Authorization

No authorization required

### HTTP request headers

 - **Content-Type**: Not defined
 - **Accept**: Not defined

