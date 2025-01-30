# DliApi

All URIs are relative to *http://localhost*

Method | HTTP request | Description
------------- | ------------- | -------------
[**restDliExportsGet**](DliApi.md#restDliExportsGet) | **GET** /rest/dli/exports | Return the list of all exports for all users
[**restDliExportsIdContentGet**](DliApi.md#restDliExportsIdContentGet) | **GET** /rest/dli/exports/{id}/content | Download the generated export.
[**restDliExportsIdDelete**](DliApi.md#restDliExportsIdDelete) | **DELETE** /rest/dli/exports/{id} | Delete the specified export.
[**restDliExportsIdGet**](DliApi.md#restDliExportsIdGet) | **GET** /rest/dli/exports/{id} | Return information of an export such as status, download url, user ID, etc.
[**restDliExportsUsersIdPost**](DliApi.md#restDliExportsUsersIdPost) | **POST** /rest/dli/exports/users/{id} | Start generating export for the specified user
[**restDliFilesFileIdUsersUserIdActivitiesGet**](DliApi.md#restDliFilesFileIdUsersUserIdActivitiesGet) | **GET** /rest/dli/files/{fileId}/users/{userId}/activities | Return the list of Activities for this file
[**restDliFilesIdContentGet**](DliApi.md#restDliFilesIdContentGet) | **GET** /rest/dli/files/{id}/content | Read file content
[**restDliFilesIdGet**](DliApi.md#restDliFilesIdGet) | **GET** /rest/dli/files/{id} | Retrieve information about the file specified.
[**restDliFilesIdPathGet**](DliApi.md#restDliFilesIdPathGet) | **GET** /rest/dli/files/{id}/path | Gets the file path by its ID
[**restDliFilesIdPreviewGet**](DliApi.md#restDliFilesIdPreviewGet) | **GET** /rest/dli/files/{id}/preview | Retrieve information about the file preview.
[**restDliFilesIdVersionsGet**](DliApi.md#restDliFilesIdVersionsGet) | **GET** /rest/dli/files/{id}/versions | List versions
[**restDliFilesIdVersionsVersionIdContentGet**](DliApi.md#restDliFilesIdVersionsVersionIdContentGet) | **GET** /rest/dli/files/{id}/versions/{version_id}/content | Download specified version
[**restDliFilesIdVersionsVersionIdGet**](DliApi.md#restDliFilesIdVersionsVersionIdGet) | **GET** /rest/dli/files/{id}/versions/{version_id} | Allow DLI admin to get specified version
[**restDliFoldersFolderIdUsersUserIdActivitiesGet**](DliApi.md#restDliFoldersFolderIdUsersUserIdActivitiesGet) | **GET** /rest/dli/folders/{folderId}/users/{userId}/activities | Return the list of activities for this folder of the specified user
[**restDliFoldersIdGet**](DliApi.md#restDliFoldersIdGet) | **GET** /rest/dli/folders/{id} | Retrieve folder information.
[**restDliMailIdAttachmentsGet**](DliApi.md#restDliMailIdAttachmentsGet) | **GET** /rest/dli/mail/{id}/attachments | List email attachments
[**restDliMailIdRecipientsGet**](DliApi.md#restDliMailIdRecipientsGet) | **GET** /rest/dli/mail/{id}/recipients | List Recipients
[**restDliUsersIdActivitiesGet**](DliApi.md#restDliUsersIdActivitiesGet) | **GET** /rest/dli/users/{id}/activities | Return the list of all activities of the specified user
[**restDliUsersIdMailGet**](DliApi.md#restDliUsersIdMailGet) | **GET** /rest/dli/users/{id}/mail | Retrieve information about the mail specified be a user


<a id="restDliExportsGet"></a>
# **restDliExportsGet**
> kotlin.collections.List&lt;Export&gt; restDliExportsGet(userId, userIdColonIn, status, statusColonContains, offset, limit, with, mode)

Return the list of all exports for all users

Return the list of all exports for all users

### Example
```kotlin
// Import classes:
//import org.openapitools.client.infrastructure.*
//import org.openapitools.client.models.*

val apiInstance = DliApi()
val userId : kotlin.String = userId_example // kotlin.String | Unique identifier of user
val userIdColonIn : kotlin.String = userIdColonIn_example // kotlin.String | Unique identifier of user. Search for results that contain any of specified values of this parameter.
val status : kotlin.String = status_example // kotlin.String | Status of the generated report
val statusColonContains : kotlin.String = statusColonContains_example // kotlin.String | Status of the generated report. Search for result that contains specified characters in this parameter.
val offset : kotlin.Int = 56 // kotlin.Int | Offset
val limit : kotlin.Int = 56 // kotlin.Int | Limit
val with : kotlin.String = with_example // kotlin.String | With parameters
val mode : kotlin.String = mode_example // kotlin.String | Response mode
try {
    val result : kotlin.collections.List<Export> = apiInstance.restDliExportsGet(userId, userIdColonIn, status, statusColonContains, offset, limit, with, mode)
    println(result)
} catch (e: ClientException) {
    println("4xx response calling DliApi#restDliExportsGet")
    e.printStackTrace()
} catch (e: ServerException) {
    println("5xx response calling DliApi#restDliExportsGet")
    e.printStackTrace()
}
```

### Parameters

Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **userId** | **kotlin.String**| Unique identifier of user | [optional]
 **userIdColonIn** | **kotlin.String**| Unique identifier of user. Search for results that contain any of specified values of this parameter. | [optional]
 **status** | **kotlin.String**| Status of the generated report | [optional]
 **statusColonContains** | **kotlin.String**| Status of the generated report. Search for result that contains specified characters in this parameter. | [optional]
 **offset** | **kotlin.Int**| Offset | [optional]
 **limit** | **kotlin.Int**| Limit | [optional]
 **with** | **kotlin.String**| With parameters | [optional]
 **mode** | **kotlin.String**| Response mode | [optional]

### Return type

[**kotlin.collections.List&lt;Export&gt;**](Export.md)

### Authorization

No authorization required

### HTTP request headers

 - **Content-Type**: Not defined
 - **Accept**: */*

<a id="restDliExportsIdContentGet"></a>
# **restDliExportsIdContentGet**
> kotlin.collections.List&lt;Export&gt; restDliExportsIdContentGet(id)

Download the generated export.

Download the generated export.

### Example
```kotlin
// Import classes:
//import org.openapitools.client.infrastructure.*
//import org.openapitools.client.models.*

val apiInstance = DliApi()
val id : kotlin.Int = 56 // kotlin.Int | ID of the export
try {
    val result : kotlin.collections.List<Export> = apiInstance.restDliExportsIdContentGet(id)
    println(result)
} catch (e: ClientException) {
    println("4xx response calling DliApi#restDliExportsIdContentGet")
    e.printStackTrace()
} catch (e: ServerException) {
    println("5xx response calling DliApi#restDliExportsIdContentGet")
    e.printStackTrace()
}
```

### Parameters

Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **id** | **kotlin.Int**| ID of the export |

### Return type

[**kotlin.collections.List&lt;Export&gt;**](Export.md)

### Authorization

No authorization required

### HTTP request headers

 - **Content-Type**: Not defined
 - **Accept**: */*

<a id="restDliExportsIdDelete"></a>
# **restDliExportsIdDelete**
> kotlin.collections.List&lt;Export&gt; restDliExportsIdDelete(id)

Delete the specified export.

Delete the specified export.

### Example
```kotlin
// Import classes:
//import org.openapitools.client.infrastructure.*
//import org.openapitools.client.models.*

val apiInstance = DliApi()
val id : kotlin.Int = 56 // kotlin.Int | ID of the export
try {
    val result : kotlin.collections.List<Export> = apiInstance.restDliExportsIdDelete(id)
    println(result)
} catch (e: ClientException) {
    println("4xx response calling DliApi#restDliExportsIdDelete")
    e.printStackTrace()
} catch (e: ServerException) {
    println("5xx response calling DliApi#restDliExportsIdDelete")
    e.printStackTrace()
}
```

### Parameters

Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **id** | **kotlin.Int**| ID of the export |

### Return type

[**kotlin.collections.List&lt;Export&gt;**](Export.md)

### Authorization

No authorization required

### HTTP request headers

 - **Content-Type**: Not defined
 - **Accept**: */*

<a id="restDliExportsIdGet"></a>
# **restDliExportsIdGet**
> kotlin.collections.List&lt;Export&gt; restDliExportsIdGet(id)

Return information of an export such as status, download url, user ID, etc.

Return information of an export such as status, download url, user ID, etc.

### Example
```kotlin
// Import classes:
//import org.openapitools.client.infrastructure.*
//import org.openapitools.client.models.*

val apiInstance = DliApi()
val id : kotlin.Int = 56 // kotlin.Int | ID of the export
try {
    val result : kotlin.collections.List<Export> = apiInstance.restDliExportsIdGet(id)
    println(result)
} catch (e: ClientException) {
    println("4xx response calling DliApi#restDliExportsIdGet")
    e.printStackTrace()
} catch (e: ServerException) {
    println("5xx response calling DliApi#restDliExportsIdGet")
    e.printStackTrace()
}
```

### Parameters

Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **id** | **kotlin.Int**| ID of the export |

### Return type

[**kotlin.collections.List&lt;Export&gt;**](Export.md)

### Authorization

No authorization required

### HTTP request headers

 - **Content-Type**: Not defined
 - **Accept**: */*

<a id="restDliExportsUsersIdPost"></a>
# **restDliExportsUsersIdPost**
> kotlin.collections.List&lt;Export&gt; restDliExportsUsersIdPost(id, body, returnEntity, mode)

Start generating export for the specified user

Start generating export for the specified user

### Example
```kotlin
// Import classes:
//import org.openapitools.client.infrastructure.*
//import org.openapitools.client.models.*

val apiInstance = DliApi()
val id : kotlin.String = id_example // kotlin.String | ID of the user
val body : ExportPost =  // ExportPost | report types, start date, and end date
val returnEntity : kotlin.Boolean = true // kotlin.Boolean | Return information about newly created entity
val mode : kotlin.String = mode_example // kotlin.String | Response mode
try {
    val result : kotlin.collections.List<Export> = apiInstance.restDliExportsUsersIdPost(id, body, returnEntity, mode)
    println(result)
} catch (e: ClientException) {
    println("4xx response calling DliApi#restDliExportsUsersIdPost")
    e.printStackTrace()
} catch (e: ServerException) {
    println("5xx response calling DliApi#restDliExportsUsersIdPost")
    e.printStackTrace()
}
```

### Parameters

Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **id** | **kotlin.String**| ID of the user |
 **body** | [**ExportPost**](ExportPost.md)| report types, start date, and end date |
 **returnEntity** | **kotlin.Boolean**| Return information about newly created entity | [optional]
 **mode** | **kotlin.String**| Response mode | [optional]

### Return type

[**kotlin.collections.List&lt;Export&gt;**](Export.md)

### Authorization

No authorization required

### HTTP request headers

 - **Content-Type**: Not defined
 - **Accept**: */*

<a id="restDliFilesFileIdUsersUserIdActivitiesGet"></a>
# **restDliFilesFileIdUsersUserIdActivitiesGet**
> kotlin.collections.List&lt;ActivityAdmin&gt; restDliFilesFileIdUsersUserIdActivitiesGet(fileId, userId, noDayBack, startDate, endDate, filter, search, type, transactionId, orderBy, offset, limit, with, mode)

Return the list of Activities for this file

Return the list of Activities for this file.

### Example
```kotlin
// Import classes:
//import org.openapitools.client.infrastructure.*
//import org.openapitools.client.models.*

val apiInstance = DliApi()
val fileId : kotlin.String = fileId_example // kotlin.String | ID of the file
val userId : kotlin.String = userId_example // kotlin.String | User Id
val noDayBack : kotlin.Int = 56 // kotlin.Int | Number of days back to search
val startDate : java.time.LocalDate = 2013-10-20 // java.time.LocalDate | Start date
val endDate : java.time.LocalDate = 2013-10-20 // java.time.LocalDate | End date
val filter : kotlin.String = filter_example // kotlin.String | All or my activities
val search : kotlin.String = search_example // kotlin.String | Search by mail body, subject and sender/recipients
val type : kotlin.String = type_example // kotlin.String | Activity type
val transactionId : kotlin.String = transactionId_example // kotlin.String | Transaction ID associated with the activities
val orderBy : kotlin.collections.List<kotlin.String> =  // kotlin.collections.List<kotlin.String> | Sorting options
val offset : kotlin.Int = 56 // kotlin.Int | Offset
val limit : kotlin.Int = 56 // kotlin.Int | Limit
val with : kotlin.String = with_example // kotlin.String | With parameters
val mode : kotlin.String = mode_example // kotlin.String | Response mode
try {
    val result : kotlin.collections.List<ActivityAdmin> = apiInstance.restDliFilesFileIdUsersUserIdActivitiesGet(fileId, userId, noDayBack, startDate, endDate, filter, search, type, transactionId, orderBy, offset, limit, with, mode)
    println(result)
} catch (e: ClientException) {
    println("4xx response calling DliApi#restDliFilesFileIdUsersUserIdActivitiesGet")
    e.printStackTrace()
} catch (e: ServerException) {
    println("5xx response calling DliApi#restDliFilesFileIdUsersUserIdActivitiesGet")
    e.printStackTrace()
}
```

### Parameters

Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **fileId** | **kotlin.String**| ID of the file |
 **userId** | **kotlin.String**| User Id |
 **noDayBack** | **kotlin.Int**| Number of days back to search | [optional]
 **startDate** | **java.time.LocalDate**| Start date | [optional]
 **endDate** | **java.time.LocalDate**| End date | [optional]
 **filter** | **kotlin.String**| All or my activities | [optional]
 **search** | **kotlin.String**| Search by mail body, subject and sender/recipients | [optional]
 **type** | **kotlin.String**| Activity type | [optional]
 **transactionId** | **kotlin.String**| Transaction ID associated with the activities | [optional]
 **orderBy** | [**kotlin.collections.List&lt;kotlin.String&gt;**](kotlin.String.md)| Sorting options | [optional]
 **offset** | **kotlin.Int**| Offset | [optional]
 **limit** | **kotlin.Int**| Limit | [optional]
 **with** | **kotlin.String**| With parameters | [optional]
 **mode** | **kotlin.String**| Response mode | [optional]

### Return type

[**kotlin.collections.List&lt;ActivityAdmin&gt;**](ActivityAdmin.md)

### Authorization

No authorization required

### HTTP request headers

 - **Content-Type**: Not defined
 - **Accept**: */*

<a id="restDliFilesIdContentGet"></a>
# **restDliFilesIdContentGet**
> restDliFilesIdContentGet(id, range)

Read file content

Read content of file

### Example
```kotlin
// Import classes:
//import org.openapitools.client.infrastructure.*
//import org.openapitools.client.models.*

val apiInstance = DliApi()
val id : kotlin.String = id_example // kotlin.String | ID of the file
val range : kotlin.String = range_example // kotlin.String | Bytes range to retrieve. Example: bytes=0-1024
try {
    apiInstance.restDliFilesIdContentGet(id, range)
} catch (e: ClientException) {
    println("4xx response calling DliApi#restDliFilesIdContentGet")
    e.printStackTrace()
} catch (e: ServerException) {
    println("5xx response calling DliApi#restDliFilesIdContentGet")
    e.printStackTrace()
}
```

### Parameters

Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **id** | **kotlin.String**| ID of the file |
 **range** | **kotlin.String**| Bytes range to retrieve. Example: bytes&#x3D;0-1024 | [optional]

### Return type

null (empty response body)

### Authorization

No authorization required

### HTTP request headers

 - **Content-Type**: Not defined
 - **Accept**: Not defined

<a id="restDliFilesIdGet"></a>
# **restDliFilesIdGet**
> org.openapitools.client.infrastructure.OctetByteArray restDliFilesIdGet(id, with, mode)

Retrieve information about the file specified.

Retrieve information about the file specified. This includes file name,                created date, modified date, file deleted, locked, fingerprint, and links to file,                folder, and owner.

### Example
```kotlin
// Import classes:
//import org.openapitools.client.infrastructure.*
//import org.openapitools.client.models.*

val apiInstance = DliApi()
val id : kotlin.String = id_example // kotlin.String | ID of the file
val with : kotlin.String = with_example // kotlin.String | With parameters
val mode : kotlin.String = mode_example // kotlin.String | Response mode
try {
    val result : org.openapitools.client.infrastructure.OctetByteArray = apiInstance.restDliFilesIdGet(id, with, mode)
    println(result)
} catch (e: ClientException) {
    println("4xx response calling DliApi#restDliFilesIdGet")
    e.printStackTrace()
} catch (e: ServerException) {
    println("5xx response calling DliApi#restDliFilesIdGet")
    e.printStackTrace()
}
```

### Parameters

Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **id** | **kotlin.String**| ID of the file |
 **with** | **kotlin.String**| With parameters | [optional]
 **mode** | **kotlin.String**| Response mode | [optional]

### Return type

[**org.openapitools.client.infrastructure.OctetByteArray**](org.openapitools.client.infrastructure.OctetByteArray.md)

### Authorization

No authorization required

### HTTP request headers

 - **Content-Type**: Not defined
 - **Accept**: */*

<a id="restDliFilesIdPathGet"></a>
# **restDliFilesIdPathGet**
> restDliFilesIdPathGet(id, mode)

Gets the file path by its ID

Gets the file path by its ID

### Example
```kotlin
// Import classes:
//import org.openapitools.client.infrastructure.*
//import org.openapitools.client.models.*

val apiInstance = DliApi()
val id : kotlin.String = id_example // kotlin.String | ID of the file
val mode : kotlin.String = mode_example // kotlin.String | Response mode
try {
    apiInstance.restDliFilesIdPathGet(id, mode)
} catch (e: ClientException) {
    println("4xx response calling DliApi#restDliFilesIdPathGet")
    e.printStackTrace()
} catch (e: ServerException) {
    println("5xx response calling DliApi#restDliFilesIdPathGet")
    e.printStackTrace()
}
```

### Parameters

Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **id** | **kotlin.String**| ID of the file |
 **mode** | **kotlin.String**| Response mode | [optional]

### Return type

null (empty response body)

### Authorization

No authorization required

### HTTP request headers

 - **Content-Type**: Not defined
 - **Accept**: Not defined

<a id="restDliFilesIdPreviewGet"></a>
# **restDliFilesIdPreviewGet**
> Preview restDliFilesIdPreviewGet(id)

Retrieve information about the file preview.

Retrieve information about the file preview.

### Example
```kotlin
// Import classes:
//import org.openapitools.client.infrastructure.*
//import org.openapitools.client.models.*

val apiInstance = DliApi()
val id : kotlin.String = id_example // kotlin.String | ID of the file
try {
    val result : Preview = apiInstance.restDliFilesIdPreviewGet(id)
    println(result)
} catch (e: ClientException) {
    println("4xx response calling DliApi#restDliFilesIdPreviewGet")
    e.printStackTrace()
} catch (e: ServerException) {
    println("5xx response calling DliApi#restDliFilesIdPreviewGet")
    e.printStackTrace()
}
```

### Parameters

Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **id** | **kotlin.String**| ID of the file |

### Return type

[**Preview**](Preview.md)

### Authorization

No authorization required

### HTTP request headers

 - **Content-Type**: Not defined
 - **Accept**: */*

<a id="restDliFilesIdVersionsGet"></a>
# **restDliFilesIdVersionsGet**
> kotlin.collections.List&lt;Version&gt; restDliFilesIdVersionsGet(id, created, createdColonGt, createdColonGte, createdColonLt, createdColonLte, orderBy, offset, limit, locateId, with, mode)

List versions

Returns a list of versions for a given file

### Example
```kotlin
// Import classes:
//import org.openapitools.client.infrastructure.*
//import org.openapitools.client.models.*

val apiInstance = DliApi()
val id : kotlin.String = id_example // kotlin.String | Object id of file to retrieve versions for
val created : kotlin.Int = 56 // kotlin.Int | File Version creation date
val createdColonGt : kotlin.Int = 56 // kotlin.Int | File Version creation date. Search for result that has this parameter value greater than specified.
val createdColonGte : kotlin.Int = 56 // kotlin.Int | File Version creation date. Search for result that has this parameter value greater or equal to the specified.
val createdColonLt : kotlin.Int = 56 // kotlin.Int | File Version creation date. Search for result that has this parameter value less than specified.
val createdColonLte : kotlin.Int = 56 // kotlin.Int | File Version creation date. Search for result that has this parameter value less or equal to the specified.
val orderBy : kotlin.collections.List<kotlin.String> =  // kotlin.collections.List<kotlin.String> | Sorting options
val offset : kotlin.Int = 56 // kotlin.Int | Offset
val limit : kotlin.Int = 56 // kotlin.Int | Limit
val locateId : kotlin.Int = 56 // kotlin.Int | If specified, \"offset\" parameter will be ignored                                             and the page containing entity with this Id will be returned.
val with : kotlin.String = with_example // kotlin.String | With parameters
val mode : kotlin.String = mode_example // kotlin.String | Response mode
try {
    val result : kotlin.collections.List<Version> = apiInstance.restDliFilesIdVersionsGet(id, created, createdColonGt, createdColonGte, createdColonLt, createdColonLte, orderBy, offset, limit, locateId, with, mode)
    println(result)
} catch (e: ClientException) {
    println("4xx response calling DliApi#restDliFilesIdVersionsGet")
    e.printStackTrace()
} catch (e: ServerException) {
    println("5xx response calling DliApi#restDliFilesIdVersionsGet")
    e.printStackTrace()
}
```

### Parameters

Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **id** | **kotlin.String**| Object id of file to retrieve versions for |
 **created** | **kotlin.Int**| File Version creation date | [optional]
 **createdColonGt** | **kotlin.Int**| File Version creation date. Search for result that has this parameter value greater than specified. | [optional]
 **createdColonGte** | **kotlin.Int**| File Version creation date. Search for result that has this parameter value greater or equal to the specified. | [optional]
 **createdColonLt** | **kotlin.Int**| File Version creation date. Search for result that has this parameter value less than specified. | [optional]
 **createdColonLte** | **kotlin.Int**| File Version creation date. Search for result that has this parameter value less or equal to the specified. | [optional]
 **orderBy** | [**kotlin.collections.List&lt;kotlin.String&gt;**](kotlin.String.md)| Sorting options | [optional]
 **offset** | **kotlin.Int**| Offset | [optional]
 **limit** | **kotlin.Int**| Limit | [optional]
 **locateId** | **kotlin.Int**| If specified, \&quot;offset\&quot; parameter will be ignored                                             and the page containing entity with this Id will be returned. | [optional]
 **with** | **kotlin.String**| With parameters | [optional]
 **mode** | **kotlin.String**| Response mode | [optional]

### Return type

[**kotlin.collections.List&lt;Version&gt;**](Version.md)

### Authorization

No authorization required

### HTTP request headers

 - **Content-Type**: Not defined
 - **Accept**: */*

<a id="restDliFilesIdVersionsVersionIdContentGet"></a>
# **restDliFilesIdVersionsVersionIdContentGet**
> restDliFilesIdVersionsVersionIdContentGet(id, versionId, range)

Download specified version

Download specified version

### Example
```kotlin
// Import classes:
//import org.openapitools.client.infrastructure.*
//import org.openapitools.client.models.*

val apiInstance = DliApi()
val id : kotlin.String = id_example // kotlin.String | ID of the file
val versionId : kotlin.String = versionId_example // kotlin.String | version ID for which to retrieve content
val range : kotlin.String = range_example // kotlin.String | Bytes range to retrieve. Example: bytes=0-1024
try {
    apiInstance.restDliFilesIdVersionsVersionIdContentGet(id, versionId, range)
} catch (e: ClientException) {
    println("4xx response calling DliApi#restDliFilesIdVersionsVersionIdContentGet")
    e.printStackTrace()
} catch (e: ServerException) {
    println("5xx response calling DliApi#restDliFilesIdVersionsVersionIdContentGet")
    e.printStackTrace()
}
```

### Parameters

Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **id** | **kotlin.String**| ID of the file |
 **versionId** | **kotlin.String**| version ID for which to retrieve content |
 **range** | **kotlin.String**| Bytes range to retrieve. Example: bytes&#x3D;0-1024 | [optional]

### Return type

null (empty response body)

### Authorization

No authorization required

### HTTP request headers

 - **Content-Type**: Not defined
 - **Accept**: Not defined

<a id="restDliFilesIdVersionsVersionIdGet"></a>
# **restDliFilesIdVersionsVersionIdGet**
> Version restDliFilesIdVersionsVersionIdGet(id, versionId)

Allow DLI admin to get specified version

Returns the specified version of a file

### Example
```kotlin
// Import classes:
//import org.openapitools.client.infrastructure.*
//import org.openapitools.client.models.*

val apiInstance = DliApi()
val id : kotlin.String = id_example // kotlin.String | Object id of file to retrieve versions for
val versionId : kotlin.String = versionId_example // kotlin.String | version ID
try {
    val result : Version = apiInstance.restDliFilesIdVersionsVersionIdGet(id, versionId)
    println(result)
} catch (e: ClientException) {
    println("4xx response calling DliApi#restDliFilesIdVersionsVersionIdGet")
    e.printStackTrace()
} catch (e: ServerException) {
    println("5xx response calling DliApi#restDliFilesIdVersionsVersionIdGet")
    e.printStackTrace()
}
```

### Parameters

Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **id** | **kotlin.String**| Object id of file to retrieve versions for |
 **versionId** | **kotlin.String**| version ID |

### Return type

[**Version**](Version.md)

### Authorization

No authorization required

### HTTP request headers

 - **Content-Type**: Not defined
 - **Accept**: */*

<a id="restDliFoldersFolderIdUsersUserIdActivitiesGet"></a>
# **restDliFoldersFolderIdUsersUserIdActivitiesGet**
> kotlin.collections.List&lt;ActivityAdmin&gt; restDliFoldersFolderIdUsersUserIdActivitiesGet(folderId, userId, noDayBack, startDate, endDate, filter, search, type, transactionId, orderBy, offset, limit, with, mode)

Return the list of activities for this folder of the specified user

Return the list of activities for this folder of the specified user

### Example
```kotlin
// Import classes:
//import org.openapitools.client.infrastructure.*
//import org.openapitools.client.models.*

val apiInstance = DliApi()
val folderId : kotlin.String = folderId_example // kotlin.String | ID of the folder
val userId : kotlin.String = userId_example // kotlin.String | User Id
val noDayBack : kotlin.Int = 56 // kotlin.Int | Number of days back to search
val startDate : java.time.LocalDate = 2013-10-20 // java.time.LocalDate | Start date
val endDate : java.time.LocalDate = 2013-10-20 // java.time.LocalDate | End date
val filter : kotlin.String = filter_example // kotlin.String | All or my activities
val search : kotlin.String = search_example // kotlin.String | Search by mail body, subject and sender/recipients
val type : kotlin.String = type_example // kotlin.String | Activity type
val transactionId : kotlin.String = transactionId_example // kotlin.String | Transaction ID associated with the activities
val orderBy : kotlin.collections.List<kotlin.String> =  // kotlin.collections.List<kotlin.String> | Sorting options
val offset : kotlin.Int = 56 // kotlin.Int | Offset
val limit : kotlin.Int = 56 // kotlin.Int | Limit
val with : kotlin.String = with_example // kotlin.String | With parameters
val mode : kotlin.String = mode_example // kotlin.String | Response mode
try {
    val result : kotlin.collections.List<ActivityAdmin> = apiInstance.restDliFoldersFolderIdUsersUserIdActivitiesGet(folderId, userId, noDayBack, startDate, endDate, filter, search, type, transactionId, orderBy, offset, limit, with, mode)
    println(result)
} catch (e: ClientException) {
    println("4xx response calling DliApi#restDliFoldersFolderIdUsersUserIdActivitiesGet")
    e.printStackTrace()
} catch (e: ServerException) {
    println("5xx response calling DliApi#restDliFoldersFolderIdUsersUserIdActivitiesGet")
    e.printStackTrace()
}
```

### Parameters

Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **folderId** | **kotlin.String**| ID of the folder |
 **userId** | **kotlin.String**| User Id |
 **noDayBack** | **kotlin.Int**| Number of days back to search | [optional]
 **startDate** | **java.time.LocalDate**| Start date | [optional]
 **endDate** | **java.time.LocalDate**| End date | [optional]
 **filter** | **kotlin.String**| All or my activities | [optional]
 **search** | **kotlin.String**| Search by mail body, subject and sender/recipients | [optional]
 **type** | **kotlin.String**| Activity type | [optional]
 **transactionId** | **kotlin.String**| Transaction ID associated with the activities | [optional]
 **orderBy** | [**kotlin.collections.List&lt;kotlin.String&gt;**](kotlin.String.md)| Sorting options | [optional]
 **offset** | **kotlin.Int**| Offset | [optional]
 **limit** | **kotlin.Int**| Limit | [optional]
 **with** | **kotlin.String**| With parameters | [optional]
 **mode** | **kotlin.String**| Response mode | [optional]

### Return type

[**kotlin.collections.List&lt;ActivityAdmin&gt;**](ActivityAdmin.md)

### Authorization

No authorization required

### HTTP request headers

 - **Content-Type**: Not defined
 - **Accept**: */*

<a id="restDliFoldersIdGet"></a>
# **restDliFoldersIdGet**
> Folder restDliFoldersIdGet(id, with, mode)

Retrieve folder information.

Return folder information for the specified folder. e.g.:                   I want to know creation date, get a link to the folder,                   find out if the folder was deleted, etc.

### Example
```kotlin
// Import classes:
//import org.openapitools.client.infrastructure.*
//import org.openapitools.client.models.*

val apiInstance = DliApi()
val id : kotlin.String = id_example // kotlin.String | ID of the folder
val with : kotlin.String = with_example // kotlin.String | With parameters
val mode : kotlin.String = mode_example // kotlin.String | Response mode
try {
    val result : Folder = apiInstance.restDliFoldersIdGet(id, with, mode)
    println(result)
} catch (e: ClientException) {
    println("4xx response calling DliApi#restDliFoldersIdGet")
    e.printStackTrace()
} catch (e: ServerException) {
    println("5xx response calling DliApi#restDliFoldersIdGet")
    e.printStackTrace()
}
```

### Parameters

Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **id** | **kotlin.String**| ID of the folder |
 **with** | **kotlin.String**| With parameters | [optional]
 **mode** | **kotlin.String**| Response mode | [optional]

### Return type

[**Folder**](Folder.md)

### Authorization

No authorization required

### HTTP request headers

 - **Content-Type**: Not defined
 - **Accept**: */*

<a id="restDliMailIdAttachmentsGet"></a>
# **restDliMailIdAttachmentsGet**
> kotlin.collections.List&lt;Attachment&gt; restDliMailIdAttachmentsGet(id, ref, offset, limit, locateId, with, mode)

List email attachments

Returns a list of attachments for a given mail.                        e.g.: I want to the id&#39;s of all the attachments for a mail I sent.

### Example
```kotlin
// Import classes:
//import org.openapitools.client.infrastructure.*
//import org.openapitools.client.models.*

val apiInstance = DliApi()
val id : kotlin.String = id_example // kotlin.String | Mail id to retrieve attachments for
val ref : kotlin.String = ref_example // kotlin.String | The email reference code (Mandatory if the email can be accessed without authentication)
val offset : kotlin.Int = 56 // kotlin.Int | Offset
val limit : kotlin.Int = 56 // kotlin.Int | Limit
val locateId : kotlin.Int = 56 // kotlin.Int | If specified, \"offset\" parameter will be ignored                                             and the page containing entity with this Id will be returned.
val with : kotlin.String = with_example // kotlin.String | With parameters
val mode : kotlin.String = mode_example // kotlin.String | Response mode
try {
    val result : kotlin.collections.List<Attachment> = apiInstance.restDliMailIdAttachmentsGet(id, ref, offset, limit, locateId, with, mode)
    println(result)
} catch (e: ClientException) {
    println("4xx response calling DliApi#restDliMailIdAttachmentsGet")
    e.printStackTrace()
} catch (e: ServerException) {
    println("5xx response calling DliApi#restDliMailIdAttachmentsGet")
    e.printStackTrace()
}
```

### Parameters

Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **id** | **kotlin.String**| Mail id to retrieve attachments for |
 **ref** | **kotlin.String**| The email reference code (Mandatory if the email can be accessed without authentication) | [optional]
 **offset** | **kotlin.Int**| Offset | [optional]
 **limit** | **kotlin.Int**| Limit | [optional]
 **locateId** | **kotlin.Int**| If specified, \&quot;offset\&quot; parameter will be ignored                                             and the page containing entity with this Id will be returned. | [optional]
 **with** | **kotlin.String**| With parameters | [optional]
 **mode** | **kotlin.String**| Response mode | [optional]

### Return type

[**kotlin.collections.List&lt;Attachment&gt;**](Attachment.md)

### Authorization

No authorization required

### HTTP request headers

 - **Content-Type**: Not defined
 - **Accept**: */*

<a id="restDliMailIdRecipientsGet"></a>
# **restDliMailIdRecipientsGet**
> kotlin.collections.List&lt;Recipient&gt; restDliMailIdRecipientsGet(id, type, ref, orderBy, offset, limit, locateId, with, mode)

List Recipients

Returns a list of recipients for a given email

### Example
```kotlin
// Import classes:
//import org.openapitools.client.infrastructure.*
//import org.openapitools.client.models.*

val apiInstance = DliApi()
val id : kotlin.String = id_example // kotlin.String | ID of the email
val type : kotlin.collections.List<kotlin.String> =  // kotlin.collections.List<kotlin.String> | Type for Recipient. TO,CC,BCC
val ref : kotlin.String = ref_example // kotlin.String | The email reference (Mandatory if the email can be accessed without authentication)
val orderBy : kotlin.collections.List<kotlin.String> =  // kotlin.collections.List<kotlin.String> | Sorting options
val offset : kotlin.Int = 56 // kotlin.Int | Offset
val limit : kotlin.Int = 56 // kotlin.Int | Limit
val locateId : kotlin.Int = 56 // kotlin.Int | If specified, \"offset\" parameter will be ignored                                             and the page containing entity with this Id will be returned.
val with : kotlin.String = with_example // kotlin.String | With parameters
val mode : kotlin.String = mode_example // kotlin.String | Response mode
try {
    val result : kotlin.collections.List<Recipient> = apiInstance.restDliMailIdRecipientsGet(id, type, ref, orderBy, offset, limit, locateId, with, mode)
    println(result)
} catch (e: ClientException) {
    println("4xx response calling DliApi#restDliMailIdRecipientsGet")
    e.printStackTrace()
} catch (e: ServerException) {
    println("5xx response calling DliApi#restDliMailIdRecipientsGet")
    e.printStackTrace()
}
```

### Parameters

Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **id** | **kotlin.String**| ID of the email |
 **type** | [**kotlin.collections.List&lt;kotlin.String&gt;**](kotlin.String.md)| Type for Recipient. TO,CC,BCC | [optional]
 **ref** | **kotlin.String**| The email reference (Mandatory if the email can be accessed without authentication) | [optional]
 **orderBy** | [**kotlin.collections.List&lt;kotlin.String&gt;**](kotlin.String.md)| Sorting options | [optional]
 **offset** | **kotlin.Int**| Offset | [optional]
 **limit** | **kotlin.Int**| Limit | [optional]
 **locateId** | **kotlin.Int**| If specified, \&quot;offset\&quot; parameter will be ignored                                             and the page containing entity with this Id will be returned. | [optional]
 **with** | **kotlin.String**| With parameters | [optional]
 **mode** | **kotlin.String**| Response mode | [optional]

### Return type

[**kotlin.collections.List&lt;Recipient&gt;**](Recipient.md)

### Authorization

No authorization required

### HTTP request headers

 - **Content-Type**: Not defined
 - **Accept**: */*

<a id="restDliUsersIdActivitiesGet"></a>
# **restDliUsersIdActivitiesGet**
> kotlin.collections.List&lt;ActivityAdmin&gt; restDliUsersIdActivitiesGet(id, noDayBack, startDate, endDate, filter, search, type, transactionId, orderBy, offset, limit, with, mode)

Return the list of all activities of the specified user

Return the list of all activities of the specified user

### Example
```kotlin
// Import classes:
//import org.openapitools.client.infrastructure.*
//import org.openapitools.client.models.*

val apiInstance = DliApi()
val id : kotlin.String = id_example // kotlin.String | ID of the user
val noDayBack : kotlin.Int = 56 // kotlin.Int | Number of days back to search
val startDate : java.time.LocalDate = 2013-10-20 // java.time.LocalDate | Start date
val endDate : java.time.LocalDate = 2013-10-20 // java.time.LocalDate | End date
val filter : kotlin.String = filter_example // kotlin.String | All or my activities
val search : kotlin.String = search_example // kotlin.String | Search by mail body, subject and sender/recipients
val type : kotlin.String = type_example // kotlin.String | Activity type
val transactionId : kotlin.String = transactionId_example // kotlin.String | Transaction ID associated with the activities
val orderBy : kotlin.collections.List<kotlin.String> =  // kotlin.collections.List<kotlin.String> | Sorting options
val offset : kotlin.Int = 56 // kotlin.Int | Offset
val limit : kotlin.Int = 56 // kotlin.Int | Limit
val with : kotlin.String = with_example // kotlin.String | With parameters
val mode : kotlin.String = mode_example // kotlin.String | Response mode
try {
    val result : kotlin.collections.List<ActivityAdmin> = apiInstance.restDliUsersIdActivitiesGet(id, noDayBack, startDate, endDate, filter, search, type, transactionId, orderBy, offset, limit, with, mode)
    println(result)
} catch (e: ClientException) {
    println("4xx response calling DliApi#restDliUsersIdActivitiesGet")
    e.printStackTrace()
} catch (e: ServerException) {
    println("5xx response calling DliApi#restDliUsersIdActivitiesGet")
    e.printStackTrace()
}
```

### Parameters

Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **id** | **kotlin.String**| ID of the user |
 **noDayBack** | **kotlin.Int**| Number of days back to search | [optional]
 **startDate** | **java.time.LocalDate**| Start date | [optional]
 **endDate** | **java.time.LocalDate**| End date | [optional]
 **filter** | **kotlin.String**| All or my activities | [optional]
 **search** | **kotlin.String**| Search by mail body, subject and sender/recipients | [optional]
 **type** | **kotlin.String**| Activity type | [optional]
 **transactionId** | **kotlin.String**| Transaction ID associated with the activities | [optional]
 **orderBy** | [**kotlin.collections.List&lt;kotlin.String&gt;**](kotlin.String.md)| Sorting options | [optional]
 **offset** | **kotlin.Int**| Offset | [optional]
 **limit** | **kotlin.Int**| Limit | [optional]
 **with** | **kotlin.String**| With parameters | [optional]
 **mode** | **kotlin.String**| Response mode | [optional]

### Return type

[**kotlin.collections.List&lt;ActivityAdmin&gt;**](ActivityAdmin.md)

### Authorization

No authorization required

### HTTP request headers

 - **Content-Type**: Not defined
 - **Accept**: */*

<a id="restDliUsersIdMailGet"></a>
# **restDliUsersIdMailGet**
> kotlin.collections.List&lt;Email&gt; restDliUsersIdMailGet(id, senderId, senderIdColonIn, isRecipient, read, date, dateColonGt, dateColonGte, dateColonLt, dateColonLte, modifiedDate, modifiedDateColonGt, modifiedDateColonGte, modifiedDateColonLt, modifiedDateColonLte, deleted, emailPackageId, emailPackageIdColonIn, templateId, templateIdColonIn, status, isPreview, isUserSent, bucket, returnCustomWebForm, customWebFormOnly, webFormId, webFormIdColonContains, orderBy, offset, limit, locateId, with, mode)

Retrieve information about the mail specified be a user

Retrieve information about the mail specified by one user

### Example
```kotlin
// Import classes:
//import org.openapitools.client.infrastructure.*
//import org.openapitools.client.models.*

val apiInstance = DliApi()
val id : kotlin.String = id_example // kotlin.String | ID of the user
val senderId : kotlin.String = senderId_example // kotlin.String | Unique identifier of User who sent Email
val senderIdColonIn : kotlin.String = senderIdColonIn_example // kotlin.String | Unique identifier of User who sent Email. Search for results that contain any of specified values of this parameter.
val isRecipient : kotlin.Boolean = true // kotlin.Boolean | Unique identifier of User who receive Email
val read : kotlin.Boolean = true // kotlin.Boolean | Whether the email is read or not by current user
val date : java.time.LocalDate = 2013-10-20 // java.time.LocalDate | Email creation date
val dateColonGt : java.time.LocalDate = 2013-10-20 // java.time.LocalDate | Email creation date. Search for result that has this parameter value greater than specified.
val dateColonGte : java.time.LocalDate = 2013-10-20 // java.time.LocalDate | Email creation date. Search for result that has this parameter value greater or equal to the specified.
val dateColonLt : java.time.LocalDate = 2013-10-20 // java.time.LocalDate | Email creation date. Search for result that has this parameter value less than specified.
val dateColonLte : java.time.LocalDate = 2013-10-20 // java.time.LocalDate | Email creation date. Search for result that has this parameter value less or equal to the specified.
val modifiedDate : java.time.LocalDate = 2013-10-20 // java.time.LocalDate | Email modification date
val modifiedDateColonGt : java.time.LocalDate = 2013-10-20 // java.time.LocalDate | Email modification date. Search for result that has this parameter value greater than specified.
val modifiedDateColonGte : java.time.LocalDate = 2013-10-20 // java.time.LocalDate | Email modification date. Search for result that has this parameter value greater or equal to the specified.
val modifiedDateColonLt : java.time.LocalDate = 2013-10-20 // java.time.LocalDate | Email modification date. Search for result that has this parameter value less than specified.
val modifiedDateColonLte : java.time.LocalDate = 2013-10-20 // java.time.LocalDate | Email modification date. Search for result that has this parameter value less or equal to the specified.
val deleted : kotlin.Boolean = true // kotlin.Boolean | Indicates that Email is deleted
val emailPackageId : kotlin.String = emailPackageId_example // kotlin.String | Email Package unique identifier
val emailPackageIdColonIn : kotlin.String = emailPackageIdColonIn_example // kotlin.String | Email Package unique identifier. Search for results that contain any of specified values of this parameter.
val templateId : kotlin.Int = 56 // kotlin.Int | Email Template unique identifier
val templateIdColonIn : kotlin.Int = 56 // kotlin.Int | Email Template unique identifier. Search for results that contain any of specified values of this parameter.
val status : kotlin.collections.List<kotlin.String> =  // kotlin.collections.List<kotlin.String> | Email status
val isPreview : kotlin.Boolean = true // kotlin.Boolean | Whether the email is a preview email
val isUserSent : kotlin.Boolean = true // kotlin.Boolean | Whether the email was sent by some user
val bucket : kotlin.String = bucket_example // kotlin.String | Email bucket
val returnCustomWebForm : kotlin.Boolean = true // kotlin.Boolean | Return all emails include those with the custom web form
val customWebFormOnly : kotlin.Boolean = true // kotlin.Boolean | Return only emails with the custom web form
val webFormId : kotlin.String = webFormId_example // kotlin.String | Email web form ID
val webFormIdColonContains : kotlin.String = webFormIdColonContains_example // kotlin.String | Email web form ID. Search for result that contains specified characters in this parameter.
val orderBy : kotlin.collections.List<kotlin.String> =  // kotlin.collections.List<kotlin.String> | Sorting options
val offset : kotlin.Int = 56 // kotlin.Int | Offset
val limit : kotlin.Int = 56 // kotlin.Int | Limit
val locateId : kotlin.Int = 56 // kotlin.Int | If specified, \"offset\" parameter will be ignored                                             and the page containing entity with this Id will be returned.
val with : kotlin.String = with_example // kotlin.String | With parameters
val mode : kotlin.String = mode_example // kotlin.String | Response mode
try {
    val result : kotlin.collections.List<Email> = apiInstance.restDliUsersIdMailGet(id, senderId, senderIdColonIn, isRecipient, read, date, dateColonGt, dateColonGte, dateColonLt, dateColonLte, modifiedDate, modifiedDateColonGt, modifiedDateColonGte, modifiedDateColonLt, modifiedDateColonLte, deleted, emailPackageId, emailPackageIdColonIn, templateId, templateIdColonIn, status, isPreview, isUserSent, bucket, returnCustomWebForm, customWebFormOnly, webFormId, webFormIdColonContains, orderBy, offset, limit, locateId, with, mode)
    println(result)
} catch (e: ClientException) {
    println("4xx response calling DliApi#restDliUsersIdMailGet")
    e.printStackTrace()
} catch (e: ServerException) {
    println("5xx response calling DliApi#restDliUsersIdMailGet")
    e.printStackTrace()
}
```

### Parameters

Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **id** | **kotlin.String**| ID of the user |
 **senderId** | **kotlin.String**| Unique identifier of User who sent Email | [optional]
 **senderIdColonIn** | **kotlin.String**| Unique identifier of User who sent Email. Search for results that contain any of specified values of this parameter. | [optional]
 **isRecipient** | **kotlin.Boolean**| Unique identifier of User who receive Email | [optional]
 **read** | **kotlin.Boolean**| Whether the email is read or not by current user | [optional]
 **date** | **java.time.LocalDate**| Email creation date | [optional]
 **dateColonGt** | **java.time.LocalDate**| Email creation date. Search for result that has this parameter value greater than specified. | [optional]
 **dateColonGte** | **java.time.LocalDate**| Email creation date. Search for result that has this parameter value greater or equal to the specified. | [optional]
 **dateColonLt** | **java.time.LocalDate**| Email creation date. Search for result that has this parameter value less than specified. | [optional]
 **dateColonLte** | **java.time.LocalDate**| Email creation date. Search for result that has this parameter value less or equal to the specified. | [optional]
 **modifiedDate** | **java.time.LocalDate**| Email modification date | [optional]
 **modifiedDateColonGt** | **java.time.LocalDate**| Email modification date. Search for result that has this parameter value greater than specified. | [optional]
 **modifiedDateColonGte** | **java.time.LocalDate**| Email modification date. Search for result that has this parameter value greater or equal to the specified. | [optional]
 **modifiedDateColonLt** | **java.time.LocalDate**| Email modification date. Search for result that has this parameter value less than specified. | [optional]
 **modifiedDateColonLte** | **java.time.LocalDate**| Email modification date. Search for result that has this parameter value less or equal to the specified. | [optional]
 **deleted** | **kotlin.Boolean**| Indicates that Email is deleted | [optional]
 **emailPackageId** | **kotlin.String**| Email Package unique identifier | [optional]
 **emailPackageIdColonIn** | **kotlin.String**| Email Package unique identifier. Search for results that contain any of specified values of this parameter. | [optional]
 **templateId** | **kotlin.Int**| Email Template unique identifier | [optional]
 **templateIdColonIn** | **kotlin.Int**| Email Template unique identifier. Search for results that contain any of specified values of this parameter. | [optional]
 **status** | [**kotlin.collections.List&lt;kotlin.String&gt;**](kotlin.String.md)| Email status | [optional]
 **isPreview** | **kotlin.Boolean**| Whether the email is a preview email | [optional]
 **isUserSent** | **kotlin.Boolean**| Whether the email was sent by some user | [optional]
 **bucket** | **kotlin.String**| Email bucket | [optional]
 **returnCustomWebForm** | **kotlin.Boolean**| Return all emails include those with the custom web form | [optional]
 **customWebFormOnly** | **kotlin.Boolean**| Return only emails with the custom web form | [optional]
 **webFormId** | **kotlin.String**| Email web form ID | [optional]
 **webFormIdColonContains** | **kotlin.String**| Email web form ID. Search for result that contains specified characters in this parameter. | [optional]
 **orderBy** | [**kotlin.collections.List&lt;kotlin.String&gt;**](kotlin.String.md)| Sorting options | [optional]
 **offset** | **kotlin.Int**| Offset | [optional]
 **limit** | **kotlin.Int**| Limit | [optional]
 **locateId** | **kotlin.Int**| If specified, \&quot;offset\&quot; parameter will be ignored                                             and the page containing entity with this Id will be returned. | [optional]
 **with** | **kotlin.String**| With parameters | [optional]
 **mode** | **kotlin.String**| Response mode | [optional]

### Return type

[**kotlin.collections.List&lt;Email&gt;**](Email.md)

### Authorization

No authorization required

### HTTP request headers

 - **Content-Type**: Not defined
 - **Accept**: */*

