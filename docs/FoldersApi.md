# FoldersApi

All URIs are relative to *http://localhost*

Method | HTTP request | Description
------------- | ------------- | -------------
[**restAdminFoldersPut**](FoldersApi.md#restAdminFoldersPut) | **PUT** /rest/admin/folders | Bulk update folders
[**restFoldersActionsFavoriteDelete**](FoldersApi.md#restFoldersActionsFavoriteDelete) | **DELETE** /rest/folders/actions/favorite | Removes specified folders from favorites
[**restFoldersActionsFavoritePost**](FoldersApi.md#restFoldersActionsFavoritePost) | **POST** /rest/folders/actions/favorite | Set multiple folders as favorite
[**restFoldersActionsPermanentDelete**](FoldersApi.md#restFoldersActionsPermanentDelete) | **DELETE** /rest/folders/actions/permanent | Permanently delete the specified folders.
[**restFoldersActionsRecoverPatch**](FoldersApi.md#restFoldersActionsRecoverPatch) | **PATCH** /rest/folders/actions/recover | Recover deleted folders.
[**restFoldersActionsScanPost**](FoldersApi.md#restFoldersActionsScanPost) | **POST** /rest/folders/actions/scan | Triggers on demand AV/DLP scan on multiple folders.
[**restFoldersDelete**](FoldersApi.md#restFoldersDelete) | **DELETE** /rest/folders | Deletes list of folders
[**restFoldersIdActionsMovePost**](FoldersApi.md#restFoldersIdActionsMovePost) | **POST** /rest/folders/{id}/actions/move | Move the folder
[**restFoldersIdActionsPermanentDelete**](FoldersApi.md#restFoldersIdActionsPermanentDelete) | **DELETE** /rest/folders/{id}/actions/permanent | Permanently delete the specified folder.
[**restFoldersIdActionsRecoverPatch**](FoldersApi.md#restFoldersIdActionsRecoverPatch) | **PATCH** /rest/folders/{id}/actions/recover | Recover deleted folder.
[**restFoldersIdActionsScanPost**](FoldersApi.md#restFoldersIdActionsScanPost) | **POST** /rest/folders/{id}/actions/scan | Triggers on demand AV/DLP folder scan.
[**restFoldersIdActionsSendMessagePost**](FoldersApi.md#restFoldersIdActionsSendMessagePost) | **POST** /rest/folders/{id}/actions/sendMessage | Create a send message email entry
[**restFoldersIdActivitiesActionsExportCSVGet**](FoldersApi.md#restFoldersIdActivitiesActionsExportCSVGet) | **GET** /rest/folders/{id}/activities/actions/exportCSV | Get activities list
[**restFoldersIdActivitiesGet**](FoldersApi.md#restFoldersIdActivitiesGet) | **GET** /rest/folders/{id}/activities | Get activities list
[**restFoldersIdChildrenGet**](FoldersApi.md#restFoldersIdChildrenGet) | **GET** /rest/folders/{id}/children | Return the list of folder children. Folders fetched at first, then files.
[**restFoldersIdCommentsGet**](FoldersApi.md#restFoldersIdCommentsGet) | **GET** /rest/folders/{id}/comments | Return the list of Comments for this folder
[**restFoldersIdDelete**](FoldersApi.md#restFoldersIdDelete) | **DELETE** /rest/folders/{id} | Folder for deletion
[**restFoldersIdFoldersGet**](FoldersApi.md#restFoldersIdFoldersGet) | **GET** /rest/folders/{id}/folders | List children folders of specified parent
[**restFoldersIdFoldersPost**](FoldersApi.md#restFoldersIdFoldersPost) | **POST** /rest/folders/{id}/folders | Create a new folder
[**restFoldersIdGet**](FoldersApi.md#restFoldersIdGet) | **GET** /rest/folders/{id} | Get the folder
[**restFoldersIdMembersGet**](FoldersApi.md#restFoldersIdMembersGet) | **GET** /rest/folders/{id}/members | List folder members
[**restFoldersIdMembersLdapGroupGet**](FoldersApi.md#restFoldersIdMembersLdapGroupGet) | **GET** /rest/folders/{id}/members/ldapGroup | List LDAP group members
[**restFoldersIdMembersLdapGroupLdapGroupIdDelete**](FoldersApi.md#restFoldersIdMembersLdapGroupLdapGroupIdDelete) | **DELETE** /rest/folders/{id}/members/ldapGroup/{ldap_group_id} | Deletes group member
[**restFoldersIdMembersLdapGroupLdapGroupIdGet**](FoldersApi.md#restFoldersIdMembersLdapGroupLdapGroupIdGet) | **GET** /rest/folders/{id}/members/ldapGroup/{ldap_group_id} | Display group member
[**restFoldersIdMembersLdapGroupLdapGroupIdPut**](FoldersApi.md#restFoldersIdMembersLdapGroupLdapGroupIdPut) | **PUT** /rest/folders/{id}/members/ldapGroup/{ldap_group_id} | update group members
[**restFoldersIdMembersMeDelete**](FoldersApi.md#restFoldersIdMembersMeDelete) | **DELETE** /rest/folders/{id}/members/me | Remove ownself from the folder
[**restFoldersIdMembersMemberUserIdDelete**](FoldersApi.md#restFoldersIdMembersMemberUserIdDelete) | **DELETE** /rest/folders/{id}/members/{member_user_id} | Deletes member
[**restFoldersIdMembersMemberUserIdGet**](FoldersApi.md#restFoldersIdMembersMemberUserIdGet) | **GET** /rest/folders/{id}/members/{member_user_id} | Display member
[**restFoldersIdMembersMemberUserIdPut**](FoldersApi.md#restFoldersIdMembersMemberUserIdPut) | **PUT** /rest/folders/{id}/members/{member_user_id} | update members
[**restFoldersIdMembersPost**](FoldersApi.md#restFoldersIdMembersPost) | **POST** /rest/folders/{id}/members | Add multiple members
[**restFoldersIdPut**](FoldersApi.md#restFoldersIdPut) | **PUT** /rest/folders/{id} | Update a folder
[**restFoldersIdQuotaGet**](FoldersApi.md#restFoldersIdQuotaGet) | **GET** /rest/folders/{id}/quota | Get the folder quota
[**restFoldersIdTasksGet**](FoldersApi.md#restFoldersIdTasksGet) | **GET** /rest/folders/{id}/tasks | Get Tasks for a folder
[**restFoldersIdTreeGet**](FoldersApi.md#restFoldersIdTreeGet) | **GET** /rest/folders/{id}/tree | Gets the folder path by its ID
[**restFoldersParentFilesGet**](FoldersApi.md#restFoldersParentFilesGet) | **GET** /rest/folders/{parent}/files | Returns the list of files in the specified folder.
[**restFoldersSharedGet**](FoldersApi.md#restFoldersSharedGet) | **GET** /rest/folders/shared | List top level shared folders
[**restFoldersTopGet**](FoldersApi.md#restFoldersTopGet) | **GET** /rest/folders/top | Return the list of top level and shared folders.
[**restPermissionsFolderFolderIdGet**](FoldersApi.md#restPermissionsFolderFolderIdGet) | **GET** /rest/permissions/folder/{folder_id} | Return the list of permissions available on a folder


<a id="restAdminFoldersPut"></a>
# **restAdminFoldersPut**
> Folders restAdminFoldersPut(body, mode, with, returnEntity)

Bulk update folders

Bulk update folders

### Example
```kotlin
// Import classes:
//import org.openapitools.client.infrastructure.*
//import org.openapitools.client.models.*

val apiInstance = FoldersApi()
val body : AdminFolderPutRequest =  // AdminFolderPutRequest | 
val mode : kotlin.String = mode_example // kotlin.String | 
val with : kotlin.String = with_example // kotlin.String | 
val returnEntity : kotlin.Boolean = true // kotlin.Boolean | 
try {
    val result : Folders = apiInstance.restAdminFoldersPut(body, mode, with, returnEntity)
    println(result)
} catch (e: ClientException) {
    println("4xx response calling FoldersApi#restAdminFoldersPut")
    e.printStackTrace()
} catch (e: ServerException) {
    println("5xx response calling FoldersApi#restAdminFoldersPut")
    e.printStackTrace()
}
```

### Parameters

Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **body** | [**AdminFolderPutRequest**](AdminFolderPutRequest.md)|  |
 **mode** | **kotlin.String**|  | [optional]
 **with** | **kotlin.String**|  | [optional]
 **returnEntity** | **kotlin.Boolean**|  | [optional]

### Return type

[**Folders**](Folders.md)

### Authorization

No authorization required

### HTTP request headers

 - **Content-Type**: Not defined
 - **Accept**: */*

<a id="restFoldersActionsFavoriteDelete"></a>
# **restFoldersActionsFavoriteDelete**
> restFoldersActionsFavoriteDelete(idColonIn, partialSuccess, mode)

Removes specified folders from favorites

Removes specified folders from favorites

### Example
```kotlin
// Import classes:
//import org.openapitools.client.infrastructure.*
//import org.openapitools.client.models.*

val apiInstance = FoldersApi()
val idColonIn : kotlin.String = idColonIn_example // kotlin.String | Array of values which are going to be changed.
val partialSuccess : kotlin.Boolean = true // kotlin.Boolean | Whether to perform action on valid items even if some ones fail
val mode : kotlin.String = mode_example // kotlin.String | Response mode
try {
    apiInstance.restFoldersActionsFavoriteDelete(idColonIn, partialSuccess, mode)
} catch (e: ClientException) {
    println("4xx response calling FoldersApi#restFoldersActionsFavoriteDelete")
    e.printStackTrace()
} catch (e: ServerException) {
    println("5xx response calling FoldersApi#restFoldersActionsFavoriteDelete")
    e.printStackTrace()
}
```

### Parameters

Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **idColonIn** | **kotlin.String**| Array of values which are going to be changed. |
 **partialSuccess** | **kotlin.Boolean**| Whether to perform action on valid items even if some ones fail | [optional]
 **mode** | **kotlin.String**| Response mode | [optional]

### Return type

null (empty response body)

### Authorization

No authorization required

### HTTP request headers

 - **Content-Type**: Not defined
 - **Accept**: Not defined

<a id="restFoldersActionsFavoritePost"></a>
# **restFoldersActionsFavoritePost**
> restFoldersActionsFavoritePost(idColonIn, partialSuccess, returnEntity, mode)

Set multiple folders as favorite

Set multiple folders as favorite

### Example
```kotlin
// Import classes:
//import org.openapitools.client.infrastructure.*
//import org.openapitools.client.models.*

val apiInstance = FoldersApi()
val idColonIn : kotlin.String = idColonIn_example // kotlin.String | Array of values which are going to be changed.
val partialSuccess : kotlin.Boolean = true // kotlin.Boolean | Whether to perform action on valid items even if some ones fail
val returnEntity : kotlin.Boolean = true // kotlin.Boolean | Return information about newly created entity
val mode : kotlin.String = mode_example // kotlin.String | Response mode
try {
    apiInstance.restFoldersActionsFavoritePost(idColonIn, partialSuccess, returnEntity, mode)
} catch (e: ClientException) {
    println("4xx response calling FoldersApi#restFoldersActionsFavoritePost")
    e.printStackTrace()
} catch (e: ServerException) {
    println("5xx response calling FoldersApi#restFoldersActionsFavoritePost")
    e.printStackTrace()
}
```

### Parameters

Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **idColonIn** | **kotlin.String**| Array of values which are going to be changed. |
 **partialSuccess** | **kotlin.Boolean**| Whether to perform action on valid items even if some ones fail | [optional]
 **returnEntity** | **kotlin.Boolean**| Return information about newly created entity | [optional]
 **mode** | **kotlin.String**| Response mode | [optional]

### Return type

null (empty response body)

### Authorization

No authorization required

### HTTP request headers

 - **Content-Type**: Not defined
 - **Accept**: Not defined

<a id="restFoldersActionsPermanentDelete"></a>
# **restFoldersActionsPermanentDelete**
> restFoldersActionsPermanentDelete(idColonIn, partialSuccess, mode)

Permanently delete the specified folders.

Permanently delete the specified folders.                These folders will no longer be accessible by any means.

### Example
```kotlin
// Import classes:
//import org.openapitools.client.infrastructure.*
//import org.openapitools.client.models.*

val apiInstance = FoldersApi()
val idColonIn : kotlin.String = idColonIn_example // kotlin.String | Array of values which are going to be changed.
val partialSuccess : kotlin.Boolean = true // kotlin.Boolean | Whether to perform action on valid items even if some ones fail
val mode : kotlin.String = mode_example // kotlin.String | Response mode
try {
    apiInstance.restFoldersActionsPermanentDelete(idColonIn, partialSuccess, mode)
} catch (e: ClientException) {
    println("4xx response calling FoldersApi#restFoldersActionsPermanentDelete")
    e.printStackTrace()
} catch (e: ServerException) {
    println("5xx response calling FoldersApi#restFoldersActionsPermanentDelete")
    e.printStackTrace()
}
```

### Parameters

Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **idColonIn** | **kotlin.String**| Array of values which are going to be changed. |
 **partialSuccess** | **kotlin.Boolean**| Whether to perform action on valid items even if some ones fail | [optional]
 **mode** | **kotlin.String**| Response mode | [optional]

### Return type

null (empty response body)

### Authorization

No authorization required

### HTTP request headers

 - **Content-Type**: Not defined
 - **Accept**: Not defined

<a id="restFoldersActionsRecoverPatch"></a>
# **restFoldersActionsRecoverPatch**
> restFoldersActionsRecoverPatch(idColonIn, partialSuccess, returnEntity, mode)

Recover deleted folders.

Recover deleted folders and their children files and folders.

### Example
```kotlin
// Import classes:
//import org.openapitools.client.infrastructure.*
//import org.openapitools.client.models.*

val apiInstance = FoldersApi()
val idColonIn : kotlin.String = idColonIn_example // kotlin.String | Array of values which are going to be changed.
val partialSuccess : kotlin.Boolean = true // kotlin.Boolean | Whether to perform action on valid items even if some ones fail
val returnEntity : kotlin.Boolean = true // kotlin.Boolean | Return information about newly created entity
val mode : kotlin.String = mode_example // kotlin.String | Response mode
try {
    apiInstance.restFoldersActionsRecoverPatch(idColonIn, partialSuccess, returnEntity, mode)
} catch (e: ClientException) {
    println("4xx response calling FoldersApi#restFoldersActionsRecoverPatch")
    e.printStackTrace()
} catch (e: ServerException) {
    println("5xx response calling FoldersApi#restFoldersActionsRecoverPatch")
    e.printStackTrace()
}
```

### Parameters

Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **idColonIn** | **kotlin.String**| Array of values which are going to be changed. |
 **partialSuccess** | **kotlin.Boolean**| Whether to perform action on valid items even if some ones fail | [optional]
 **returnEntity** | **kotlin.Boolean**| Return information about newly created entity | [optional]
 **mode** | **kotlin.String**| Response mode | [optional]

### Return type

null (empty response body)

### Authorization

No authorization required

### HTTP request headers

 - **Content-Type**: Not defined
 - **Accept**: Not defined

<a id="restFoldersActionsScanPost"></a>
# **restFoldersActionsScanPost**
> restFoldersActionsScanPost(returnEntity, idColonIn, with, mode)

Triggers on demand AV/DLP scan on multiple folders.

Attempts to trigger an AV/DLP scan on requested folders.

### Example
```kotlin
// Import classes:
//import org.openapitools.client.infrastructure.*
//import org.openapitools.client.models.*

val apiInstance = FoldersApi()
val returnEntity : kotlin.Boolean = true // kotlin.Boolean | Return information about newly created entity
val idColonIn : kotlin.String = idColonIn_example // kotlin.String | List of IDs of entities to scan. Search for results that contain any of specified values of this parameter.
val with : kotlin.String = with_example // kotlin.String | With parameters
val mode : kotlin.String = mode_example // kotlin.String | Response mode
try {
    apiInstance.restFoldersActionsScanPost(returnEntity, idColonIn, with, mode)
} catch (e: ClientException) {
    println("4xx response calling FoldersApi#restFoldersActionsScanPost")
    e.printStackTrace()
} catch (e: ServerException) {
    println("5xx response calling FoldersApi#restFoldersActionsScanPost")
    e.printStackTrace()
}
```

### Parameters

Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **returnEntity** | **kotlin.Boolean**| Return information about newly created entity | [optional]
 **idColonIn** | **kotlin.String**| List of IDs of entities to scan. Search for results that contain any of specified values of this parameter. | [optional]
 **with** | **kotlin.String**| With parameters | [optional]
 **mode** | **kotlin.String**| Response mode | [optional]

### Return type

null (empty response body)

### Authorization

No authorization required

### HTTP request headers

 - **Content-Type**: Not defined
 - **Accept**: Not defined

<a id="restFoldersDelete"></a>
# **restFoldersDelete**
> restFoldersDelete(idColonIn, partialSuccess, mode)

Deletes list of folders

Deletes list of folders.

### Example
```kotlin
// Import classes:
//import org.openapitools.client.infrastructure.*
//import org.openapitools.client.models.*

val apiInstance = FoldersApi()
val idColonIn : kotlin.String = idColonIn_example // kotlin.String | Array of values which are going to be changed.
val partialSuccess : kotlin.Boolean = true // kotlin.Boolean | Whether to perform action on valid items even if some ones fail
val mode : kotlin.String = mode_example // kotlin.String | Response mode
try {
    apiInstance.restFoldersDelete(idColonIn, partialSuccess, mode)
} catch (e: ClientException) {
    println("4xx response calling FoldersApi#restFoldersDelete")
    e.printStackTrace()
} catch (e: ServerException) {
    println("5xx response calling FoldersApi#restFoldersDelete")
    e.printStackTrace()
}
```

### Parameters

Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **idColonIn** | **kotlin.String**| Array of values which are going to be changed. |
 **partialSuccess** | **kotlin.Boolean**| Whether to perform action on valid items even if some ones fail | [optional]
 **mode** | **kotlin.String**| Response mode | [optional]

### Return type

null (empty response body)

### Authorization

No authorization required

### HTTP request headers

 - **Content-Type**: Not defined
 - **Accept**: Not defined

<a id="restFoldersIdActionsMovePost"></a>
# **restFoldersIdActionsMovePost**
> Folder1 restFoldersIdActionsMovePost(id, body, mode, with, returnEntity)

Move the folder

Move the folder

### Example
```kotlin
// Import classes:
//import org.openapitools.client.infrastructure.*
//import org.openapitools.client.models.*

val apiInstance = FoldersApi()
val id : kotlin.String = id_example // kotlin.String | The ID of the entity
val body : DestinationFolderIdRequest =  // DestinationFolderIdRequest | 
val mode : kotlin.String = mode_example // kotlin.String | 
val with : kotlin.String = with_example // kotlin.String | 
val returnEntity : kotlin.Boolean = true // kotlin.Boolean | 
try {
    val result : Folder1 = apiInstance.restFoldersIdActionsMovePost(id, body, mode, with, returnEntity)
    println(result)
} catch (e: ClientException) {
    println("4xx response calling FoldersApi#restFoldersIdActionsMovePost")
    e.printStackTrace()
} catch (e: ServerException) {
    println("5xx response calling FoldersApi#restFoldersIdActionsMovePost")
    e.printStackTrace()
}
```

### Parameters

Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **id** | **kotlin.String**| The ID of the entity |
 **body** | [**DestinationFolderIdRequest**](DestinationFolderIdRequest.md)|  |
 **mode** | **kotlin.String**|  | [optional]
 **with** | **kotlin.String**|  | [optional]
 **returnEntity** | **kotlin.Boolean**|  | [optional]

### Return type

[**Folder1**](Folder1.md)

### Authorization

No authorization required

### HTTP request headers

 - **Content-Type**: Not defined
 - **Accept**: */*

<a id="restFoldersIdActionsPermanentDelete"></a>
# **restFoldersIdActionsPermanentDelete**
> restFoldersIdActionsPermanentDelete(id)

Permanently delete the specified folder.

Permanently delete the specified folder.                This folder will no longer be accessible by any means.

### Example
```kotlin
// Import classes:
//import org.openapitools.client.infrastructure.*
//import org.openapitools.client.models.*

val apiInstance = FoldersApi()
val id : kotlin.String = id_example // kotlin.String | ID of the folder
try {
    apiInstance.restFoldersIdActionsPermanentDelete(id)
} catch (e: ClientException) {
    println("4xx response calling FoldersApi#restFoldersIdActionsPermanentDelete")
    e.printStackTrace()
} catch (e: ServerException) {
    println("5xx response calling FoldersApi#restFoldersIdActionsPermanentDelete")
    e.printStackTrace()
}
```

### Parameters

Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **id** | **kotlin.String**| ID of the folder |

### Return type

null (empty response body)

### Authorization

No authorization required

### HTTP request headers

 - **Content-Type**: Not defined
 - **Accept**: Not defined

<a id="restFoldersIdActionsRecoverPatch"></a>
# **restFoldersIdActionsRecoverPatch**
> Folder restFoldersIdActionsRecoverPatch(id, returnEntity, mode)

Recover deleted folder.

Recover the specified folder. This un-marks the folder for deletion.

### Example
```kotlin
// Import classes:
//import org.openapitools.client.infrastructure.*
//import org.openapitools.client.models.*

val apiInstance = FoldersApi()
val id : kotlin.String = id_example // kotlin.String | ID of the folder
val returnEntity : kotlin.Boolean = true // kotlin.Boolean | Return information about newly created entity
val mode : kotlin.String = mode_example // kotlin.String | Response mode
try {
    val result : Folder = apiInstance.restFoldersIdActionsRecoverPatch(id, returnEntity, mode)
    println(result)
} catch (e: ClientException) {
    println("4xx response calling FoldersApi#restFoldersIdActionsRecoverPatch")
    e.printStackTrace()
} catch (e: ServerException) {
    println("5xx response calling FoldersApi#restFoldersIdActionsRecoverPatch")
    e.printStackTrace()
}
```

### Parameters

Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **id** | **kotlin.String**| ID of the folder |
 **returnEntity** | **kotlin.Boolean**| Return information about newly created entity | [optional]
 **mode** | **kotlin.String**| Response mode | [optional]

### Return type

[**Folder**](Folder.md)

### Authorization

No authorization required

### HTTP request headers

 - **Content-Type**: Not defined
 - **Accept**: */*

<a id="restFoldersIdActionsScanPost"></a>
# **restFoldersIdActionsScanPost**
> restFoldersIdActionsScanPost(id, returnEntity, folderIdColonIn, fileIdColonIn, with, mode)

Triggers on demand AV/DLP folder scan.

Attempts to trigger an AV/DLP scan on requested folder.

### Example
```kotlin
// Import classes:
//import org.openapitools.client.infrastructure.*
//import org.openapitools.client.models.*

val apiInstance = FoldersApi()
val id : kotlin.String = id_example // kotlin.String | ID of the folder
val returnEntity : kotlin.Boolean = true // kotlin.Boolean | Return information about newly created entity
val folderIdColonIn : kotlin.Int = 56 // kotlin.Int | List of folder IDs of entities to scan. Search for results that contain any of specified values of this parameter.
val fileIdColonIn : kotlin.Int = 56 // kotlin.Int | List of file IDs of entities to scan. Search for results that contain any of specified values of this parameter.
val with : kotlin.String = with_example // kotlin.String | With parameters
val mode : kotlin.String = mode_example // kotlin.String | Response mode
try {
    apiInstance.restFoldersIdActionsScanPost(id, returnEntity, folderIdColonIn, fileIdColonIn, with, mode)
} catch (e: ClientException) {
    println("4xx response calling FoldersApi#restFoldersIdActionsScanPost")
    e.printStackTrace()
} catch (e: ServerException) {
    println("5xx response calling FoldersApi#restFoldersIdActionsScanPost")
    e.printStackTrace()
}
```

### Parameters

Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **id** | **kotlin.String**| ID of the folder |
 **returnEntity** | **kotlin.Boolean**| Return information about newly created entity | [optional]
 **folderIdColonIn** | **kotlin.Int**| List of folder IDs of entities to scan. Search for results that contain any of specified values of this parameter. | [optional]
 **fileIdColonIn** | **kotlin.Int**| List of file IDs of entities to scan. Search for results that contain any of specified values of this parameter. | [optional]
 **with** | **kotlin.String**| With parameters | [optional]
 **mode** | **kotlin.String**| Response mode | [optional]

### Return type

null (empty response body)

### Authorization

No authorization required

### HTTP request headers

 - **Content-Type**: Not defined
 - **Accept**: Not defined

<a id="restFoldersIdActionsSendMessagePost"></a>
# **restFoldersIdActionsSendMessagePost**
> restFoldersIdActionsSendMessagePost(id, body, returnEntity, mode)

Create a send message email entry

Creates a send message email entry

### Example
```kotlin
// Import classes:
//import org.openapitools.client.infrastructure.*
//import org.openapitools.client.models.*

val apiInstance = FoldersApi()
val id : kotlin.String = id_example // kotlin.String | ID of the folder
val body : SendMessagePost =  // SendMessagePost | The email details
val returnEntity : kotlin.Boolean = true // kotlin.Boolean | Return information about newly created entity
val mode : kotlin.String = mode_example // kotlin.String | Response mode
try {
    apiInstance.restFoldersIdActionsSendMessagePost(id, body, returnEntity, mode)
} catch (e: ClientException) {
    println("4xx response calling FoldersApi#restFoldersIdActionsSendMessagePost")
    e.printStackTrace()
} catch (e: ServerException) {
    println("5xx response calling FoldersApi#restFoldersIdActionsSendMessagePost")
    e.printStackTrace()
}
```

### Parameters

Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **id** | **kotlin.String**| ID of the folder |
 **body** | [**SendMessagePost**](SendMessagePost.md)| The email details |
 **returnEntity** | **kotlin.Boolean**| Return information about newly created entity | [optional]
 **mode** | **kotlin.String**| Response mode | [optional]

### Return type

null (empty response body)

### Authorization

No authorization required

### HTTP request headers

 - **Content-Type**: Not defined
 - **Accept**: Not defined

<a id="restFoldersIdActivitiesActionsExportCSVGet"></a>
# **restFoldersIdActivitiesActionsExportCSVGet**
> org.openapitools.client.infrastructure.OctetByteArray restFoldersIdActivitiesActionsExportCSVGet(id, fileId, endTime, endDate, filter, startTime, with, startDate, noDayBack, limit, mode, transactionId, orderBy, search, nested, offset, type, returnEntity)

Get activities list

Get activities list

### Example
```kotlin
// Import classes:
//import org.openapitools.client.infrastructure.*
//import org.openapitools.client.models.*

val apiInstance = FoldersApi()
val id : kotlin.String = id_example // kotlin.String | The ID of the entity
val fileId : kotlin.String = fileId_example // kotlin.String | File ID inside the folder
val endTime : kotlin.Int = 56 // kotlin.Int | End time in unix timestamp
val endDate : kotlin.String = endDate_example // kotlin.String | End date
val filter : kotlin.String = filter_example // kotlin.String | All or my activities
val startTime : kotlin.Int = 56 // kotlin.Int | Start time in unix timestamp
val with : kotlin.String = with_example // kotlin.String | 
val startDate : kotlin.String = startDate_example // kotlin.String | Start date
val noDayBack : kotlin.Int = 56 // kotlin.Int | Number of days back to search
val limit : kotlin.Int = 56 // kotlin.Int | 
val mode : kotlin.String = mode_example // kotlin.String | 
val transactionId : kotlin.String = transactionId_example // kotlin.String | Transaction ID associated with the activities
val orderBy : kotlin.String = orderBy_example // kotlin.String | Order By
val search : kotlin.String = search_example // kotlin.String | Search by mail body, subject and sender/recipients
val nested : kotlin.Boolean = true // kotlin.Boolean | Include nested folders
val offset : kotlin.Int = 56 // kotlin.Int | 
val type : kotlin.String = type_example // kotlin.String | Activity type
val returnEntity : kotlin.Boolean = true // kotlin.Boolean | 
try {
    val result : org.openapitools.client.infrastructure.OctetByteArray = apiInstance.restFoldersIdActivitiesActionsExportCSVGet(id, fileId, endTime, endDate, filter, startTime, with, startDate, noDayBack, limit, mode, transactionId, orderBy, search, nested, offset, type, returnEntity)
    println(result)
} catch (e: ClientException) {
    println("4xx response calling FoldersApi#restFoldersIdActivitiesActionsExportCSVGet")
    e.printStackTrace()
} catch (e: ServerException) {
    println("5xx response calling FoldersApi#restFoldersIdActivitiesActionsExportCSVGet")
    e.printStackTrace()
}
```

### Parameters

Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **id** | **kotlin.String**| The ID of the entity |
 **fileId** | **kotlin.String**| File ID inside the folder | [optional]
 **endTime** | **kotlin.Int**| End time in unix timestamp | [optional]
 **endDate** | **kotlin.String**| End date | [optional]
 **filter** | **kotlin.String**| All or my activities | [optional]
 **startTime** | **kotlin.Int**| Start time in unix timestamp | [optional]
 **with** | **kotlin.String**|  | [optional]
 **startDate** | **kotlin.String**| Start date | [optional]
 **noDayBack** | **kotlin.Int**| Number of days back to search | [optional]
 **limit** | **kotlin.Int**|  | [optional]
 **mode** | **kotlin.String**|  | [optional]
 **transactionId** | **kotlin.String**| Transaction ID associated with the activities | [optional]
 **orderBy** | **kotlin.String**| Order By | [optional]
 **search** | **kotlin.String**| Search by mail body, subject and sender/recipients | [optional]
 **nested** | **kotlin.Boolean**| Include nested folders | [optional]
 **offset** | **kotlin.Int**|  | [optional]
 **type** | **kotlin.String**| Activity type | [optional]
 **returnEntity** | **kotlin.Boolean**|  | [optional]

### Return type

[**org.openapitools.client.infrastructure.OctetByteArray**](org.openapitools.client.infrastructure.OctetByteArray.md)

### Authorization

No authorization required

### HTTP request headers

 - **Content-Type**: Not defined
 - **Accept**: */*

<a id="restFoldersIdActivitiesGet"></a>
# **restFoldersIdActivitiesGet**
> ActivityList restFoldersIdActivitiesGet(id, fileId, endTime, endDate, filter, startTime, with, startDate, noDayBack, limit, mode, transactionId, orderBy, search, nested, offset, type, returnEntity)

Get activities list

Get activities list

### Example
```kotlin
// Import classes:
//import org.openapitools.client.infrastructure.*
//import org.openapitools.client.models.*

val apiInstance = FoldersApi()
val id : kotlin.String = id_example // kotlin.String | The ID of the entity
val fileId : kotlin.String = fileId_example // kotlin.String | File ID inside the folder
val endTime : kotlin.Int = 56 // kotlin.Int | End time in unix timestamp
val endDate : kotlin.String = endDate_example // kotlin.String | End date
val filter : kotlin.String = filter_example // kotlin.String | All or my activities
val startTime : kotlin.Int = 56 // kotlin.Int | Start time in unix timestamp
val with : kotlin.String = with_example // kotlin.String | 
val startDate : kotlin.String = startDate_example // kotlin.String | Start date
val noDayBack : kotlin.Int = 56 // kotlin.Int | Number of days back to search
val limit : kotlin.Int = 56 // kotlin.Int | 
val mode : kotlin.String = mode_example // kotlin.String | 
val transactionId : kotlin.String = transactionId_example // kotlin.String | Transaction ID associated with the activities
val orderBy : kotlin.String = orderBy_example // kotlin.String | Order By
val search : kotlin.String = search_example // kotlin.String | Search by mail body, subject and sender/recipients
val nested : kotlin.Boolean = true // kotlin.Boolean | Include nested folders
val offset : kotlin.Int = 56 // kotlin.Int | 
val type : kotlin.String = type_example // kotlin.String | Activity type
val returnEntity : kotlin.Boolean = true // kotlin.Boolean | 
try {
    val result : ActivityList = apiInstance.restFoldersIdActivitiesGet(id, fileId, endTime, endDate, filter, startTime, with, startDate, noDayBack, limit, mode, transactionId, orderBy, search, nested, offset, type, returnEntity)
    println(result)
} catch (e: ClientException) {
    println("4xx response calling FoldersApi#restFoldersIdActivitiesGet")
    e.printStackTrace()
} catch (e: ServerException) {
    println("5xx response calling FoldersApi#restFoldersIdActivitiesGet")
    e.printStackTrace()
}
```

### Parameters

Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **id** | **kotlin.String**| The ID of the entity |
 **fileId** | **kotlin.String**| File ID inside the folder | [optional]
 **endTime** | **kotlin.Int**| End time in unix timestamp | [optional]
 **endDate** | **kotlin.String**| End date | [optional]
 **filter** | **kotlin.String**| All or my activities | [optional]
 **startTime** | **kotlin.Int**| Start time in unix timestamp | [optional]
 **with** | **kotlin.String**|  | [optional]
 **startDate** | **kotlin.String**| Start date | [optional]
 **noDayBack** | **kotlin.Int**| Number of days back to search | [optional]
 **limit** | **kotlin.Int**|  | [optional]
 **mode** | **kotlin.String**|  | [optional]
 **transactionId** | **kotlin.String**| Transaction ID associated with the activities | [optional]
 **orderBy** | **kotlin.String**| Order By | [optional]
 **search** | **kotlin.String**| Search by mail body, subject and sender/recipients | [optional]
 **nested** | **kotlin.Boolean**| Include nested folders | [optional]
 **offset** | **kotlin.Int**|  | [optional]
 **type** | **kotlin.String**| Activity type | [optional]
 **returnEntity** | **kotlin.Boolean**|  | [optional]

### Return type

[**ActivityList**](ActivityList.md)

### Authorization

No authorization required

### HTTP request headers

 - **Content-Type**: Not defined
 - **Accept**: */*

<a id="restFoldersIdChildrenGet"></a>
# **restFoldersIdChildrenGet**
> kotlin.collections.List&lt;Folder&gt; restFoldersIdChildrenGet(id, fileId, deleted, extensions, with, limit, mode, regex, orderBy, offset, returnEntity)

Return the list of folder children. Folders fetched at first, then files.

Return the list of folder children. Folders fetched at first, then files.

### Example
```kotlin
// Import classes:
//import org.openapitools.client.infrastructure.*
//import org.openapitools.client.models.*

val apiInstance = FoldersApi()
val id : kotlin.String = id_example // kotlin.String | The ID of the entity
val fileId : kotlin.String = fileId_example // kotlin.String | 
val deleted : kotlin.Boolean = true // kotlin.Boolean | Don't show deleted, true - show only deleted, none - show both
val extensions : kotlin.String = extensions_example // kotlin.String | Comma delimited whitelist of extensions to filter files by
val with : kotlin.String = with_example // kotlin.String | 
val limit : kotlin.Int = 56 // kotlin.Int | 
val mode : kotlin.String = mode_example // kotlin.String | 
val regex : kotlin.String = regex_example // kotlin.String | Regex pattern to filter files by
val orderBy : kotlin.String = orderBy_example // kotlin.String | Sorting options. Accepts id, name, modified, created, size. Sample format is id:asc
val offset : kotlin.Int = 56 // kotlin.Int | 
val returnEntity : kotlin.Boolean = true // kotlin.Boolean | 
try {
    val result : kotlin.collections.List<Folder> = apiInstance.restFoldersIdChildrenGet(id, fileId, deleted, extensions, with, limit, mode, regex, orderBy, offset, returnEntity)
    println(result)
} catch (e: ClientException) {
    println("4xx response calling FoldersApi#restFoldersIdChildrenGet")
    e.printStackTrace()
} catch (e: ServerException) {
    println("5xx response calling FoldersApi#restFoldersIdChildrenGet")
    e.printStackTrace()
}
```

### Parameters

Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **id** | **kotlin.String**| The ID of the entity |
 **fileId** | **kotlin.String**|  | [optional]
 **deleted** | **kotlin.Boolean**| Don&#39;t show deleted, true - show only deleted, none - show both | [optional]
 **extensions** | **kotlin.String**| Comma delimited whitelist of extensions to filter files by | [optional]
 **with** | **kotlin.String**|  | [optional]
 **limit** | **kotlin.Int**|  | [optional]
 **mode** | **kotlin.String**|  | [optional]
 **regex** | **kotlin.String**| Regex pattern to filter files by | [optional]
 **orderBy** | **kotlin.String**| Sorting options. Accepts id, name, modified, created, size. Sample format is id:asc | [optional]
 **offset** | **kotlin.Int**|  | [optional]
 **returnEntity** | **kotlin.Boolean**|  | [optional]

### Return type

[**kotlin.collections.List&lt;Folder&gt;**](Folder.md)

### Authorization

No authorization required

### HTTP request headers

 - **Content-Type**: Not defined
 - **Accept**: */*

<a id="restFoldersIdCommentsGet"></a>
# **restFoldersIdCommentsGet**
> kotlin.collections.List&lt;Comment&gt; restFoldersIdCommentsGet(id, parentId, parentIdColonIn, userId, userIdColonIn, created, createdColonGt, createdColonGte, createdColonLt, createdColonLte, modified, modifiedColonGt, modifiedColonGte, modifiedColonLt, modifiedColonLte, contentsColonContains, orderBy, offset, limit, with, mode)

Return the list of Comments for this folder

Returns all comments made on this folder.

### Example
```kotlin
// Import classes:
//import org.openapitools.client.infrastructure.*
//import org.openapitools.client.models.*

val apiInstance = FoldersApi()
val id : kotlin.String = id_example // kotlin.String | ID of the parent folder
val parentId : kotlin.Int = 56 // kotlin.Int | Parent Comment unique identifier
val parentIdColonIn : kotlin.Int = 56 // kotlin.Int | Parent Comment unique identifier. Search for results that contain any of specified values of this parameter.
val userId : kotlin.String = userId_example // kotlin.String | Unique identifier of comment author
val userIdColonIn : kotlin.String = userIdColonIn_example // kotlin.String | Unique identifier of comment author. Search for results that contain any of specified values of this parameter.
val created : kotlin.String = 2013-10-20 // kotlin.String | Comment creation date
val createdColonGt : kotlin.String = 2013-10-20 // kotlin.String | Comment creation date. Search for result that has this parameter value greater than specified.
val createdColonGte : kotlin.String = 2013-10-20 // kotlin.String | Comment creation date. Search for result that has this parameter value greater or equal to the specified.
val createdColonLt : kotlin.String = 2013-10-20 // kotlin.String | Comment creation date. Search for result that has this parameter value less than specified.
val createdColonLte : kotlin.String = 2013-10-20 // kotlin.String | Comment creation date. Search for result that has this parameter value less or equal to the specified.
val modified : kotlin.String = 2013-10-20 // kotlin.String | Comment modification date
val modifiedColonGt : kotlin.String = 2013-10-20 // kotlin.String | Comment modification date. Search for result that has this parameter value greater than specified.
val modifiedColonGte : kotlin.String = 2013-10-20 // kotlin.String | Comment modification date. Search for result that has this parameter value greater or equal to the specified.
val modifiedColonLt : kotlin.String = 2013-10-20 // kotlin.String | Comment modification date. Search for result that has this parameter value less than specified.
val modifiedColonLte : kotlin.String = 2013-10-20 // kotlin.String | Comment modification date. Search for result that has this parameter value less or equal to the specified.
val contentsColonContains : kotlin.String = contentsColonContains_example // kotlin.String | Comment content. Search for result that contains specified characters in this parameter.
val orderBy : kotlin.collections.List<kotlin.String> =  // kotlin.collections.List<kotlin.String> | Sorting options
val offset : kotlin.Int = 56 // kotlin.Int | Offset
val limit : kotlin.Int = 56 // kotlin.Int | Limit
val with : kotlin.String = with_example // kotlin.String | With parameters
val mode : kotlin.String = mode_example // kotlin.String | Response mode
try {
    val result : kotlin.collections.List<Comment> = apiInstance.restFoldersIdCommentsGet(id, parentId, parentIdColonIn, userId, userIdColonIn, created, createdColonGt, createdColonGte, createdColonLt, createdColonLte, modified, modifiedColonGt, modifiedColonGte, modifiedColonLt, modifiedColonLte, contentsColonContains, orderBy, offset, limit, with, mode)
    println(result)
} catch (e: ClientException) {
    println("4xx response calling FoldersApi#restFoldersIdCommentsGet")
    e.printStackTrace()
} catch (e: ServerException) {
    println("5xx response calling FoldersApi#restFoldersIdCommentsGet")
    e.printStackTrace()
}
```

### Parameters

Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **id** | **kotlin.String**| ID of the parent folder |
 **parentId** | **kotlin.Int**| Parent Comment unique identifier | [optional]
 **parentIdColonIn** | **kotlin.Int**| Parent Comment unique identifier. Search for results that contain any of specified values of this parameter. | [optional]
 **userId** | **kotlin.String**| Unique identifier of comment author | [optional]
 **userIdColonIn** | **kotlin.String**| Unique identifier of comment author. Search for results that contain any of specified values of this parameter. | [optional]
 **created** | **kotlin.String**| Comment creation date | [optional]
 **createdColonGt** | **kotlin.String**| Comment creation date. Search for result that has this parameter value greater than specified. | [optional]
 **createdColonGte** | **kotlin.String**| Comment creation date. Search for result that has this parameter value greater or equal to the specified. | [optional]
 **createdColonLt** | **kotlin.String**| Comment creation date. Search for result that has this parameter value less than specified. | [optional]
 **createdColonLte** | **kotlin.String**| Comment creation date. Search for result that has this parameter value less or equal to the specified. | [optional]
 **modified** | **kotlin.String**| Comment modification date | [optional]
 **modifiedColonGt** | **kotlin.String**| Comment modification date. Search for result that has this parameter value greater than specified. | [optional]
 **modifiedColonGte** | **kotlin.String**| Comment modification date. Search for result that has this parameter value greater or equal to the specified. | [optional]
 **modifiedColonLt** | **kotlin.String**| Comment modification date. Search for result that has this parameter value less than specified. | [optional]
 **modifiedColonLte** | **kotlin.String**| Comment modification date. Search for result that has this parameter value less or equal to the specified. | [optional]
 **contentsColonContains** | **kotlin.String**| Comment content. Search for result that contains specified characters in this parameter. | [optional]
 **orderBy** | [**kotlin.collections.List&lt;kotlin.String&gt;**](kotlin.String.md)| Sorting options | [optional]
 **offset** | **kotlin.Int**| Offset | [optional]
 **limit** | **kotlin.Int**| Limit | [optional]
 **with** | **kotlin.String**| With parameters | [optional]
 **mode** | **kotlin.String**| Response mode | [optional]

### Return type

[**kotlin.collections.List&lt;Comment&gt;**](Comment.md)

### Authorization

No authorization required

### HTTP request headers

 - **Content-Type**: Not defined
 - **Accept**: */*

<a id="restFoldersIdDelete"></a>
# **restFoldersIdDelete**
> restFoldersIdDelete(id)

Folder for deletion

Marks the specified folder for deletion. The folder is still accessible as a deleted folder until it expires and is deleted permanently.

### Example
```kotlin
// Import classes:
//import org.openapitools.client.infrastructure.*
//import org.openapitools.client.models.*

val apiInstance = FoldersApi()
val id : kotlin.String = id_example // kotlin.String | The ID of the entity
try {
    apiInstance.restFoldersIdDelete(id)
} catch (e: ClientException) {
    println("4xx response calling FoldersApi#restFoldersIdDelete")
    e.printStackTrace()
} catch (e: ServerException) {
    println("5xx response calling FoldersApi#restFoldersIdDelete")
    e.printStackTrace()
}
```

### Parameters

Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **id** | **kotlin.String**| The ID of the entity |

### Return type

null (empty response body)

### Authorization

No authorization required

### HTTP request headers

 - **Content-Type**: Not defined
 - **Accept**: Not defined

<a id="restFoldersIdFoldersGet"></a>
# **restFoldersIdFoldersGet**
> kotlin.collections.List&lt;Folder&gt; restFoldersIdFoldersGet(id, name, nameColonContains, userId, userIdColonIn, created, createdColonGt, createdColonGte, createdColonLt, createdColonLte, modified, modifiedColonGt, modifiedColonGte, modifiedColonLt, modifiedColonLte, deleted, expire, expireColonGt, expireColonGte, expireColonLt, expireColonLte, fileLifetime, fileLifetimeColonGt, fileLifetimeColonGte, fileLifetimeColonLt, fileLifetimeColonLte, secure, descriptionColonContains, orderBy, offset, limit, locateId, with, mode)

List children folders of specified parent

Return the list of folders in the specified folder including its metadata.

### Example
```kotlin
// Import classes:
//import org.openapitools.client.infrastructure.*
//import org.openapitools.client.models.*

val apiInstance = FoldersApi()
val id : kotlin.String = id_example // kotlin.String | ID of the parent folder
val name : kotlin.String = name_example // kotlin.String | Folder name
val nameColonContains : kotlin.String = nameColonContains_example // kotlin.String | Folder name. Search for result that contains specified characters in this parameter.
val userId : kotlin.String = userId_example // kotlin.String | Unique identifier of Object creator
val userIdColonIn : kotlin.String = userIdColonIn_example // kotlin.String | Unique identifier of Object creator. Search for results that contain any of specified values of this parameter.
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
val expire : kotlin.Int = 56 // kotlin.Int | Expiration date
val expireColonGt : kotlin.Int = 56 // kotlin.Int | Expiration date. Search for result that has this parameter value greater than specified.
val expireColonGte : kotlin.Int = 56 // kotlin.Int | Expiration date. Search for result that has this parameter value greater or equal to the specified.
val expireColonLt : kotlin.Int = 56 // kotlin.Int | Expiration date. Search for result that has this parameter value less than specified.
val expireColonLte : kotlin.Int = 56 // kotlin.Int | Expiration date. Search for result that has this parameter value less or equal to the specified.
val fileLifetime : kotlin.Int = 56 // kotlin.Int | Folder lifetime
val fileLifetimeColonGt : kotlin.Int = 56 // kotlin.Int | Folder lifetime. Search for result that has this parameter value greater than specified.
val fileLifetimeColonGte : kotlin.Int = 56 // kotlin.Int | Folder lifetime. Search for result that has this parameter value greater or equal to the specified.
val fileLifetimeColonLt : kotlin.Int = 56 // kotlin.Int | Folder lifetime. Search for result that has this parameter value less than specified.
val fileLifetimeColonLte : kotlin.Int = 56 // kotlin.Int | Folder lifetime. Search for result that has this parameter value less or equal to the specified.
val secure : kotlin.Boolean = true // kotlin.Boolean | Folder secure flag
val descriptionColonContains : kotlin.String = descriptionColonContains_example // kotlin.String | Folder description. Search for result that contains specified characters in this parameter.
val orderBy : kotlin.collections.List<kotlin.String> =  // kotlin.collections.List<kotlin.String> | Sorting options
val offset : kotlin.Int = 56 // kotlin.Int | Offset
val limit : kotlin.Int = 56 // kotlin.Int | Limit
val locateId : kotlin.Int = 56 // kotlin.Int | If specified, \"offset\" parameter will be ignored                                             and the page containing entity with this Id will be returned.
val with : kotlin.String = with_example // kotlin.String | With parameters
val mode : kotlin.String = mode_example // kotlin.String | Response mode
try {
    val result : kotlin.collections.List<Folder> = apiInstance.restFoldersIdFoldersGet(id, name, nameColonContains, userId, userIdColonIn, created, createdColonGt, createdColonGte, createdColonLt, createdColonLte, modified, modifiedColonGt, modifiedColonGte, modifiedColonLt, modifiedColonLte, deleted, expire, expireColonGt, expireColonGte, expireColonLt, expireColonLte, fileLifetime, fileLifetimeColonGt, fileLifetimeColonGte, fileLifetimeColonLt, fileLifetimeColonLte, secure, descriptionColonContains, orderBy, offset, limit, locateId, with, mode)
    println(result)
} catch (e: ClientException) {
    println("4xx response calling FoldersApi#restFoldersIdFoldersGet")
    e.printStackTrace()
} catch (e: ServerException) {
    println("5xx response calling FoldersApi#restFoldersIdFoldersGet")
    e.printStackTrace()
}
```

### Parameters

Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **id** | **kotlin.String**| ID of the parent folder |
 **name** | **kotlin.String**| Folder name | [optional]
 **nameColonContains** | **kotlin.String**| Folder name. Search for result that contains specified characters in this parameter. | [optional]
 **userId** | **kotlin.String**| Unique identifier of Object creator | [optional]
 **userIdColonIn** | **kotlin.String**| Unique identifier of Object creator. Search for results that contain any of specified values of this parameter. | [optional]
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
 **expire** | **kotlin.Int**| Expiration date | [optional]
 **expireColonGt** | **kotlin.Int**| Expiration date. Search for result that has this parameter value greater than specified. | [optional]
 **expireColonGte** | **kotlin.Int**| Expiration date. Search for result that has this parameter value greater or equal to the specified. | [optional]
 **expireColonLt** | **kotlin.Int**| Expiration date. Search for result that has this parameter value less than specified. | [optional]
 **expireColonLte** | **kotlin.Int**| Expiration date. Search for result that has this parameter value less or equal to the specified. | [optional]
 **fileLifetime** | **kotlin.Int**| Folder lifetime | [optional]
 **fileLifetimeColonGt** | **kotlin.Int**| Folder lifetime. Search for result that has this parameter value greater than specified. | [optional]
 **fileLifetimeColonGte** | **kotlin.Int**| Folder lifetime. Search for result that has this parameter value greater or equal to the specified. | [optional]
 **fileLifetimeColonLt** | **kotlin.Int**| Folder lifetime. Search for result that has this parameter value less than specified. | [optional]
 **fileLifetimeColonLte** | **kotlin.Int**| Folder lifetime. Search for result that has this parameter value less or equal to the specified. | [optional]
 **secure** | **kotlin.Boolean**| Folder secure flag | [optional]
 **descriptionColonContains** | **kotlin.String**| Folder description. Search for result that contains specified characters in this parameter. | [optional]
 **orderBy** | [**kotlin.collections.List&lt;kotlin.String&gt;**](kotlin.String.md)| Sorting options | [optional]
 **offset** | **kotlin.Int**| Offset | [optional]
 **limit** | **kotlin.Int**| Limit | [optional]
 **locateId** | **kotlin.Int**| If specified, \&quot;offset\&quot; parameter will be ignored                                             and the page containing entity with this Id will be returned. | [optional]
 **with** | **kotlin.String**| With parameters | [optional]
 **mode** | **kotlin.String**| Response mode | [optional]

### Return type

[**kotlin.collections.List&lt;Folder&gt;**](Folder.md)

### Authorization

No authorization required

### HTTP request headers

 - **Content-Type**: Not defined
 - **Accept**: */*

<a id="restFoldersIdFoldersPost"></a>
# **restFoldersIdFoldersPost**
> Folder1 restFoldersIdFoldersPost(id, body, mode, with, returnEntity)

Create a new folder

Create a new folder under the specified parent_id

### Example
```kotlin
// Import classes:
//import org.openapitools.client.infrastructure.*
//import org.openapitools.client.models.*

val apiInstance = FoldersApi()
val id : kotlin.String = id_example // kotlin.String | The ID of the entity
val body : FolderCreatePostRequest =  // FolderCreatePostRequest | 
val mode : kotlin.String = mode_example // kotlin.String | 
val with : kotlin.String = with_example // kotlin.String | 
val returnEntity : kotlin.Boolean = true // kotlin.Boolean | 
try {
    val result : Folder1 = apiInstance.restFoldersIdFoldersPost(id, body, mode, with, returnEntity)
    println(result)
} catch (e: ClientException) {
    println("4xx response calling FoldersApi#restFoldersIdFoldersPost")
    e.printStackTrace()
} catch (e: ServerException) {
    println("5xx response calling FoldersApi#restFoldersIdFoldersPost")
    e.printStackTrace()
}
```

### Parameters

Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **id** | **kotlin.String**| The ID of the entity |
 **body** | [**FolderCreatePostRequest**](FolderCreatePostRequest.md)|  |
 **mode** | **kotlin.String**|  | [optional]
 **with** | **kotlin.String**|  | [optional]
 **returnEntity** | **kotlin.Boolean**|  | [optional]

### Return type

[**Folder1**](Folder1.md)

### Authorization

No authorization required

### HTTP request headers

 - **Content-Type**: Not defined
 - **Accept**: */*

<a id="restFoldersIdGet"></a>
# **restFoldersIdGet**
> Folder1 restFoldersIdGet(id, mode, with, returnEntity)

Get the folder

Get the folder

### Example
```kotlin
// Import classes:
//import org.openapitools.client.infrastructure.*
//import org.openapitools.client.models.*

val apiInstance = FoldersApi()
val id : kotlin.String = id_example // kotlin.String | The ID of the entity
val mode : kotlin.String = mode_example // kotlin.String | 
val with : kotlin.String = with_example // kotlin.String | 
val returnEntity : kotlin.Boolean = true // kotlin.Boolean | 
try {
    val result : Folder1 = apiInstance.restFoldersIdGet(id, mode, with, returnEntity)
    println(result)
} catch (e: ClientException) {
    println("4xx response calling FoldersApi#restFoldersIdGet")
    e.printStackTrace()
} catch (e: ServerException) {
    println("5xx response calling FoldersApi#restFoldersIdGet")
    e.printStackTrace()
}
```

### Parameters

Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **id** | **kotlin.String**| The ID of the entity |
 **mode** | **kotlin.String**|  | [optional]
 **with** | **kotlin.String**|  | [optional]
 **returnEntity** | **kotlin.Boolean**|  | [optional]

### Return type

[**Folder1**](Folder1.md)

### Authorization

No authorization required

### HTTP request headers

 - **Content-Type**: Not defined
 - **Accept**: */*

<a id="restFoldersIdMembersGet"></a>
# **restFoldersIdMembersGet**
> Members restFoldersIdMembersGet(id, orderBy, groupIdColonIn, with, roleId, limit, mode, userId, userIdColonIn, roleIdColonIn, type, offset, groupId, returnEntity)

List folder members

Returns a list of members in the folder.

### Example
```kotlin
// Import classes:
//import org.openapitools.client.infrastructure.*
//import org.openapitools.client.models.*

val apiInstance = FoldersApi()
val id : kotlin.String = id_example // kotlin.String | The ID of the entity
val orderBy : kotlin.String = orderBy_example // kotlin.String | 
val groupIdColonIn : kotlin.collections.List<kotlin.String> =  // kotlin.collections.List<kotlin.String> | 
val with : kotlin.String = with_example // kotlin.String | 
val roleId : kotlin.Int = 56 // kotlin.Int | 
val limit : kotlin.Int = 56 // kotlin.Int | 
val mode : kotlin.String = mode_example // kotlin.String | 
val userId : kotlin.String = userId_example // kotlin.String | 
val userIdColonIn : kotlin.collections.List<kotlin.String> =  // kotlin.collections.List<kotlin.String> | Member id list recommended request size <= 100
val roleIdColonIn : kotlin.collections.List<kotlin.String> =  // kotlin.collections.List<kotlin.String> | 
val type : kotlin.String = type_example // kotlin.String | 
val offset : kotlin.Int = 56 // kotlin.Int | 
val groupId : kotlin.Int = 56 // kotlin.Int | 
val returnEntity : kotlin.Boolean = true // kotlin.Boolean | 
try {
    val result : Members = apiInstance.restFoldersIdMembersGet(id, orderBy, groupIdColonIn, with, roleId, limit, mode, userId, userIdColonIn, roleIdColonIn, type, offset, groupId, returnEntity)
    println(result)
} catch (e: ClientException) {
    println("4xx response calling FoldersApi#restFoldersIdMembersGet")
    e.printStackTrace()
} catch (e: ServerException) {
    println("5xx response calling FoldersApi#restFoldersIdMembersGet")
    e.printStackTrace()
}
```

### Parameters

Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **id** | **kotlin.String**| The ID of the entity |
 **orderBy** | **kotlin.String**|  | [optional]
 **groupIdColonIn** | [**kotlin.collections.List&lt;kotlin.String&gt;**](kotlin.String.md)|  | [optional]
 **with** | **kotlin.String**|  | [optional]
 **roleId** | **kotlin.Int**|  | [optional]
 **limit** | **kotlin.Int**|  | [optional]
 **mode** | **kotlin.String**|  | [optional]
 **userId** | **kotlin.String**|  | [optional]
 **userIdColonIn** | [**kotlin.collections.List&lt;kotlin.String&gt;**](kotlin.String.md)| Member id list recommended request size &lt;&#x3D; 100 | [optional]
 **roleIdColonIn** | [**kotlin.collections.List&lt;kotlin.String&gt;**](kotlin.String.md)|  | [optional]
 **type** | **kotlin.String**|  | [optional]
 **offset** | **kotlin.Int**|  | [optional]
 **groupId** | **kotlin.Int**|  | [optional]
 **returnEntity** | **kotlin.Boolean**|  | [optional]

### Return type

[**Members**](Members.md)

### Authorization

No authorization required

### HTTP request headers

 - **Content-Type**: Not defined
 - **Accept**: */*

<a id="restFoldersIdMembersLdapGroupGet"></a>
# **restFoldersIdMembersLdapGroupGet**
> kotlin.collections.List&lt;MemberGroup&gt; restFoldersIdMembersLdapGroupGet(id, groupId, groupIdColonIn, roleId, roleIdColonIn, orderBy, offset, limit, with, mode)

List LDAP group members

Returns a list of LDAP group members in the folder.                        This returns LDAP name, email, and privileges.

### Example
```kotlin
// Import classes:
//import org.openapitools.client.infrastructure.*
//import org.openapitools.client.models.*

val apiInstance = FoldersApi()
val id : kotlin.String = id_example // kotlin.String | ID of the folder
val groupId : kotlin.Int = 56 // kotlin.Int | Unique identifier of group
val groupIdColonIn : kotlin.Int = 56 // kotlin.Int | Unique identifier of group. Search for results that contain any of specified values of this parameter.
val roleId : kotlin.Int = 56 // kotlin.Int | Unique identifier of role
val roleIdColonIn : kotlin.Int = 56 // kotlin.Int | Unique identifier of role. Search for results that contain any of specified values of this parameter.
val orderBy : kotlin.collections.List<kotlin.String> =  // kotlin.collections.List<kotlin.String> | Sorting options
val offset : kotlin.Int = 56 // kotlin.Int | Offset
val limit : kotlin.Int = 56 // kotlin.Int | Limit
val with : kotlin.String = with_example // kotlin.String | With parameters
val mode : kotlin.String = mode_example // kotlin.String | Response mode
try {
    val result : kotlin.collections.List<MemberGroup> = apiInstance.restFoldersIdMembersLdapGroupGet(id, groupId, groupIdColonIn, roleId, roleIdColonIn, orderBy, offset, limit, with, mode)
    println(result)
} catch (e: ClientException) {
    println("4xx response calling FoldersApi#restFoldersIdMembersLdapGroupGet")
    e.printStackTrace()
} catch (e: ServerException) {
    println("5xx response calling FoldersApi#restFoldersIdMembersLdapGroupGet")
    e.printStackTrace()
}
```

### Parameters

Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **id** | **kotlin.String**| ID of the folder |
 **groupId** | **kotlin.Int**| Unique identifier of group | [optional]
 **groupIdColonIn** | **kotlin.Int**| Unique identifier of group. Search for results that contain any of specified values of this parameter. | [optional]
 **roleId** | **kotlin.Int**| Unique identifier of role | [optional]
 **roleIdColonIn** | **kotlin.Int**| Unique identifier of role. Search for results that contain any of specified values of this parameter. | [optional]
 **orderBy** | [**kotlin.collections.List&lt;kotlin.String&gt;**](kotlin.String.md)| Sorting options | [optional]
 **offset** | **kotlin.Int**| Offset | [optional]
 **limit** | **kotlin.Int**| Limit | [optional]
 **with** | **kotlin.String**| With parameters | [optional]
 **mode** | **kotlin.String**| Response mode | [optional]

### Return type

[**kotlin.collections.List&lt;MemberGroup&gt;**](MemberGroup.md)

### Authorization

No authorization required

### HTTP request headers

 - **Content-Type**: Not defined
 - **Accept**: */*

<a id="restFoldersIdMembersLdapGroupLdapGroupIdDelete"></a>
# **restFoldersIdMembersLdapGroupLdapGroupIdDelete**
> restFoldersIdMembersLdapGroupLdapGroupIdDelete(id, ldapGroupId, downgradeNested)

Deletes group member

Deletes group member in the folder

### Example
```kotlin
// Import classes:
//import org.openapitools.client.infrastructure.*
//import org.openapitools.client.models.*

val apiInstance = FoldersApi()
val id : kotlin.String = id_example // kotlin.String | The ID of the entity
val ldapGroupId : kotlin.Int = 56 // kotlin.Int | The ldap group ID
val downgradeNested : kotlin.Boolean = true // kotlin.Boolean | 
try {
    apiInstance.restFoldersIdMembersLdapGroupLdapGroupIdDelete(id, ldapGroupId, downgradeNested)
} catch (e: ClientException) {
    println("4xx response calling FoldersApi#restFoldersIdMembersLdapGroupLdapGroupIdDelete")
    e.printStackTrace()
} catch (e: ServerException) {
    println("5xx response calling FoldersApi#restFoldersIdMembersLdapGroupLdapGroupIdDelete")
    e.printStackTrace()
}
```

### Parameters

Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **id** | **kotlin.String**| The ID of the entity |
 **ldapGroupId** | **kotlin.Int**| The ldap group ID |
 **downgradeNested** | **kotlin.Boolean**|  | [optional]

### Return type

null (empty response body)

### Authorization

No authorization required

### HTTP request headers

 - **Content-Type**: Not defined
 - **Accept**: Not defined

<a id="restFoldersIdMembersLdapGroupLdapGroupIdGet"></a>
# **restFoldersIdMembersLdapGroupLdapGroupIdGet**
> Member restFoldersIdMembersLdapGroupLdapGroupIdGet(id, ldapGroupId, with, mode)

Display group member

Display the specified group member in the folder

### Example
```kotlin
// Import classes:
//import org.openapitools.client.infrastructure.*
//import org.openapitools.client.models.*

val apiInstance = FoldersApi()
val id : kotlin.String = id_example // kotlin.String | ID of the folder
val ldapGroupId : kotlin.Int = 56 // kotlin.Int | id of the group member
val with : kotlin.String = with_example // kotlin.String | With parameters
val mode : kotlin.String = mode_example // kotlin.String | Response mode
try {
    val result : Member = apiInstance.restFoldersIdMembersLdapGroupLdapGroupIdGet(id, ldapGroupId, with, mode)
    println(result)
} catch (e: ClientException) {
    println("4xx response calling FoldersApi#restFoldersIdMembersLdapGroupLdapGroupIdGet")
    e.printStackTrace()
} catch (e: ServerException) {
    println("5xx response calling FoldersApi#restFoldersIdMembersLdapGroupLdapGroupIdGet")
    e.printStackTrace()
}
```

### Parameters

Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **id** | **kotlin.String**| ID of the folder |
 **ldapGroupId** | **kotlin.Int**| id of the group member |
 **with** | **kotlin.String**| With parameters | [optional]
 **mode** | **kotlin.String**| Response mode | [optional]

### Return type

[**Member**](Member.md)

### Authorization

No authorization required

### HTTP request headers

 - **Content-Type**: Not defined
 - **Accept**: */*

<a id="restFoldersIdMembersLdapGroupLdapGroupIdPut"></a>
# **restFoldersIdMembersLdapGroupLdapGroupIdPut**
> restFoldersIdMembersLdapGroupLdapGroupIdPut(id, ldapGroupId, body, returnEntity, downgradeNested, mode)

update group members

updates group members in the folder

### Example
```kotlin
// Import classes:
//import org.openapitools.client.infrastructure.*
//import org.openapitools.client.models.*

val apiInstance = FoldersApi()
val id : kotlin.String = id_example // kotlin.String | ID of the folder
val ldapGroupId : kotlin.Int = 56 // kotlin.Int | id of the group member
val body : MemberGroupPut =  // MemberGroupPut | members and roles details
val returnEntity : kotlin.Boolean = true // kotlin.Boolean | Return information about newly created entity
val downgradeNested : kotlin.Boolean = true // kotlin.Boolean | Downgrade member role for nested folders
val mode : kotlin.String = mode_example // kotlin.String | Response mode
try {
    apiInstance.restFoldersIdMembersLdapGroupLdapGroupIdPut(id, ldapGroupId, body, returnEntity, downgradeNested, mode)
} catch (e: ClientException) {
    println("4xx response calling FoldersApi#restFoldersIdMembersLdapGroupLdapGroupIdPut")
    e.printStackTrace()
} catch (e: ServerException) {
    println("5xx response calling FoldersApi#restFoldersIdMembersLdapGroupLdapGroupIdPut")
    e.printStackTrace()
}
```

### Parameters

Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **id** | **kotlin.String**| ID of the folder |
 **ldapGroupId** | **kotlin.Int**| id of the group member |
 **body** | [**MemberGroupPut**](MemberGroupPut.md)| members and roles details |
 **returnEntity** | **kotlin.Boolean**| Return information about newly created entity | [optional]
 **downgradeNested** | **kotlin.Boolean**| Downgrade member role for nested folders | [optional]
 **mode** | **kotlin.String**| Response mode | [optional]

### Return type

null (empty response body)

### Authorization

No authorization required

### HTTP request headers

 - **Content-Type**: Not defined
 - **Accept**: Not defined

<a id="restFoldersIdMembersMeDelete"></a>
# **restFoldersIdMembersMeDelete**
> restFoldersIdMembersMeDelete(id, downgradeNested)

Remove ownself from the folder

Remove ownself from the folder

### Example
```kotlin
// Import classes:
//import org.openapitools.client.infrastructure.*
//import org.openapitools.client.models.*

val apiInstance = FoldersApi()
val id : kotlin.String = id_example // kotlin.String | The ID of the entity
val downgradeNested : kotlin.Boolean = true // kotlin.Boolean | 
try {
    apiInstance.restFoldersIdMembersMeDelete(id, downgradeNested)
} catch (e: ClientException) {
    println("4xx response calling FoldersApi#restFoldersIdMembersMeDelete")
    e.printStackTrace()
} catch (e: ServerException) {
    println("5xx response calling FoldersApi#restFoldersIdMembersMeDelete")
    e.printStackTrace()
}
```

### Parameters

Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **id** | **kotlin.String**| The ID of the entity |
 **downgradeNested** | **kotlin.Boolean**|  | [optional]

### Return type

null (empty response body)

### Authorization

No authorization required

### HTTP request headers

 - **Content-Type**: Not defined
 - **Accept**: Not defined

<a id="restFoldersIdMembersMemberUserIdDelete"></a>
# **restFoldersIdMembersMemberUserIdDelete**
> restFoldersIdMembersMemberUserIdDelete(id, memberUserId, downgradeNested)

Deletes member

Deletes member in the folder

### Example
```kotlin
// Import classes:
//import org.openapitools.client.infrastructure.*
//import org.openapitools.client.models.*

val apiInstance = FoldersApi()
val id : kotlin.String = id_example // kotlin.String | The ID of the entity
val memberUserId : kotlin.String = memberUserId_example // kotlin.String | The member user ID
val downgradeNested : kotlin.Boolean = true // kotlin.Boolean | 
try {
    apiInstance.restFoldersIdMembersMemberUserIdDelete(id, memberUserId, downgradeNested)
} catch (e: ClientException) {
    println("4xx response calling FoldersApi#restFoldersIdMembersMemberUserIdDelete")
    e.printStackTrace()
} catch (e: ServerException) {
    println("5xx response calling FoldersApi#restFoldersIdMembersMemberUserIdDelete")
    e.printStackTrace()
}
```

### Parameters

Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **id** | **kotlin.String**| The ID of the entity |
 **memberUserId** | **kotlin.String**| The member user ID |
 **downgradeNested** | **kotlin.Boolean**|  | [optional]

### Return type

null (empty response body)

### Authorization

No authorization required

### HTTP request headers

 - **Content-Type**: Not defined
 - **Accept**: Not defined

<a id="restFoldersIdMembersMemberUserIdGet"></a>
# **restFoldersIdMembersMemberUserIdGet**
> Member restFoldersIdMembersMemberUserIdGet(id, memberUserId, with, mode)

Display member

Display the specified member in the folder

### Example
```kotlin
// Import classes:
//import org.openapitools.client.infrastructure.*
//import org.openapitools.client.models.*

val apiInstance = FoldersApi()
val id : kotlin.String = id_example // kotlin.String | ID of the folder
val memberUserId : kotlin.String = memberUserId_example // kotlin.String | ID of the member
val with : kotlin.String = with_example // kotlin.String | With parameters
val mode : kotlin.String = mode_example // kotlin.String | Response mode
try {
    val result : Member = apiInstance.restFoldersIdMembersMemberUserIdGet(id, memberUserId, with, mode)
    println(result)
} catch (e: ClientException) {
    println("4xx response calling FoldersApi#restFoldersIdMembersMemberUserIdGet")
    e.printStackTrace()
} catch (e: ServerException) {
    println("5xx response calling FoldersApi#restFoldersIdMembersMemberUserIdGet")
    e.printStackTrace()
}
```

### Parameters

Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **id** | **kotlin.String**| ID of the folder |
 **memberUserId** | **kotlin.String**| ID of the member |
 **with** | **kotlin.String**| With parameters | [optional]
 **mode** | **kotlin.String**| Response mode | [optional]

### Return type

[**Member**](Member.md)

### Authorization

No authorization required

### HTTP request headers

 - **Content-Type**: Not defined
 - **Accept**: */*

<a id="restFoldersIdMembersMemberUserIdPut"></a>
# **restFoldersIdMembersMemberUserIdPut**
> restFoldersIdMembersMemberUserIdPut(id, memberUserId, body, returnEntity, downgradeNested, mode)

update members

updates members in the folder

### Example
```kotlin
// Import classes:
//import org.openapitools.client.infrastructure.*
//import org.openapitools.client.models.*

val apiInstance = FoldersApi()
val id : kotlin.String = id_example // kotlin.String | ID of the folder
val memberUserId : kotlin.String = memberUserId_example // kotlin.String | ID of the member
val body : MemberPut =  // MemberPut | members and roles details
val returnEntity : kotlin.Boolean = true // kotlin.Boolean | Return information about newly created entity
val downgradeNested : kotlin.Boolean = true // kotlin.Boolean | Downgrade member role for nested folders
val mode : kotlin.String = mode_example // kotlin.String | Response mode
try {
    apiInstance.restFoldersIdMembersMemberUserIdPut(id, memberUserId, body, returnEntity, downgradeNested, mode)
} catch (e: ClientException) {
    println("4xx response calling FoldersApi#restFoldersIdMembersMemberUserIdPut")
    e.printStackTrace()
} catch (e: ServerException) {
    println("5xx response calling FoldersApi#restFoldersIdMembersMemberUserIdPut")
    e.printStackTrace()
}
```

### Parameters

Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **id** | **kotlin.String**| ID of the folder |
 **memberUserId** | **kotlin.String**| ID of the member |
 **body** | [**MemberPut**](MemberPut.md)| members and roles details |
 **returnEntity** | **kotlin.Boolean**| Return information about newly created entity | [optional]
 **downgradeNested** | **kotlin.Boolean**| Downgrade member role for nested folders | [optional]
 **mode** | **kotlin.String**| Response mode | [optional]

### Return type

null (empty response body)

### Authorization

No authorization required

### HTTP request headers

 - **Content-Type**: Not defined
 - **Accept**: Not defined

<a id="restFoldersIdMembersPost"></a>
# **restFoldersIdMembersPost**
> FolderAddMembers restFoldersIdMembersPost(id, body, partialSuccess, downgradeNested, with, mode, updateIfExists, returnEntity)

Add multiple members

Add multiple members to the folder

### Example
```kotlin
// Import classes:
//import org.openapitools.client.infrastructure.*
//import org.openapitools.client.models.*

val apiInstance = FoldersApi()
val id : kotlin.String = id_example // kotlin.String | The ID of the entity
val body : FolderMemberPostRequest =  // FolderMemberPostRequest | 
val partialSuccess : kotlin.Boolean = true // kotlin.Boolean | 
val downgradeNested : kotlin.Boolean = true // kotlin.Boolean | 
val with : kotlin.String = with_example // kotlin.String | 
val mode : kotlin.String = mode_example // kotlin.String | 
val updateIfExists : kotlin.Boolean = true // kotlin.Boolean | 
val returnEntity : kotlin.Boolean = true // kotlin.Boolean | 
try {
    val result : FolderAddMembers = apiInstance.restFoldersIdMembersPost(id, body, partialSuccess, downgradeNested, with, mode, updateIfExists, returnEntity)
    println(result)
} catch (e: ClientException) {
    println("4xx response calling FoldersApi#restFoldersIdMembersPost")
    e.printStackTrace()
} catch (e: ServerException) {
    println("5xx response calling FoldersApi#restFoldersIdMembersPost")
    e.printStackTrace()
}
```

### Parameters

Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **id** | **kotlin.String**| The ID of the entity |
 **body** | [**FolderMemberPostRequest**](FolderMemberPostRequest.md)|  |
 **partialSuccess** | **kotlin.Boolean**|  | [optional]
 **downgradeNested** | **kotlin.Boolean**|  | [optional]
 **with** | **kotlin.String**|  | [optional]
 **mode** | **kotlin.String**|  | [optional]
 **updateIfExists** | **kotlin.Boolean**|  | [optional]
 **returnEntity** | **kotlin.Boolean**|  | [optional]

### Return type

[**FolderAddMembers**](FolderAddMembers.md)

### Authorization

No authorization required

### HTTP request headers

 - **Content-Type**: Not defined
 - **Accept**: */*

<a id="restFoldersIdPut"></a>
# **restFoldersIdPut**
> Folder1 restFoldersIdPut(id, body, mode, with, returnEntity)

Update a folder

Update folder

### Example
```kotlin
// Import classes:
//import org.openapitools.client.infrastructure.*
//import org.openapitools.client.models.*

val apiInstance = FoldersApi()
val id : kotlin.String = id_example // kotlin.String | The ID of the entity
val body : FolderUpdatePutRequest =  // FolderUpdatePutRequest | 
val mode : kotlin.String = mode_example // kotlin.String | 
val with : kotlin.String = with_example // kotlin.String | 
val returnEntity : kotlin.Boolean = true // kotlin.Boolean | 
try {
    val result : Folder1 = apiInstance.restFoldersIdPut(id, body, mode, with, returnEntity)
    println(result)
} catch (e: ClientException) {
    println("4xx response calling FoldersApi#restFoldersIdPut")
    e.printStackTrace()
} catch (e: ServerException) {
    println("5xx response calling FoldersApi#restFoldersIdPut")
    e.printStackTrace()
}
```

### Parameters

Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **id** | **kotlin.String**| The ID of the entity |
 **body** | [**FolderUpdatePutRequest**](FolderUpdatePutRequest.md)|  |
 **mode** | **kotlin.String**|  | [optional]
 **with** | **kotlin.String**|  | [optional]
 **returnEntity** | **kotlin.Boolean**|  | [optional]

### Return type

[**Folder1**](Folder1.md)

### Authorization

No authorization required

### HTTP request headers

 - **Content-Type**: Not defined
 - **Accept**: */*

<a id="restFoldersIdQuotaGet"></a>
# **restFoldersIdQuotaGet**
> FolderQuota restFoldersIdQuotaGet(id, fileId)

Get the folder quota

Get the folder quota

### Example
```kotlin
// Import classes:
//import org.openapitools.client.infrastructure.*
//import org.openapitools.client.models.*

val apiInstance = FoldersApi()
val id : kotlin.String = id_example // kotlin.String | The ID of the entity
val fileId : kotlin.String = fileId_example // kotlin.String | 
try {
    val result : FolderQuota = apiInstance.restFoldersIdQuotaGet(id, fileId)
    println(result)
} catch (e: ClientException) {
    println("4xx response calling FoldersApi#restFoldersIdQuotaGet")
    e.printStackTrace()
} catch (e: ServerException) {
    println("5xx response calling FoldersApi#restFoldersIdQuotaGet")
    e.printStackTrace()
}
```

### Parameters

Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **id** | **kotlin.String**| The ID of the entity |
 **fileId** | **kotlin.String**|  | [optional]

### Return type

[**FolderQuota**](FolderQuota.md)

### Authorization

No authorization required

### HTTP request headers

 - **Content-Type**: Not defined
 - **Accept**: */*

<a id="restFoldersIdTasksGet"></a>
# **restFoldersIdTasksGet**
> kotlin.collections.List&lt;Task&gt; restFoldersIdTasksGet(id, assigneeId, assigneeIdColonIn, due, dueColonGt, dueColonGte, dueColonLt, dueColonLte, parentId, parentIdColonIn, userId, userIdColonIn, created, createdColonGt, createdColonGte, createdColonLt, createdColonLte, modified, modifiedColonGt, modifiedColonGte, modifiedColonLt, modifiedColonLte, contentsColonContains, status, deleted, orderBy, offset, limit, with, mode)

Get Tasks for a folder

Returns all tasks for a folder

### Example
```kotlin
// Import classes:
//import org.openapitools.client.infrastructure.*
//import org.openapitools.client.models.*

val apiInstance = FoldersApi()
val id : kotlin.String = id_example // kotlin.String | Folder object ID of the task to retrieve
val assigneeId : kotlin.String = assigneeId_example // kotlin.String | Assigned User unique identifier
val assigneeIdColonIn : kotlin.String = assigneeIdColonIn_example // kotlin.String | Assigned User unique identifier. Search for results that contain any of specified values of this parameter.
val due : kotlin.String = 2013-10-20 // kotlin.String | Task due date
val dueColonGt : kotlin.String = 2013-10-20 // kotlin.String | Task due date. Search for result that has this parameter value greater than specified.
val dueColonGte : kotlin.String = 2013-10-20 // kotlin.String | Task due date. Search for result that has this parameter value greater or equal to the specified.
val dueColonLt : kotlin.String = 2013-10-20 // kotlin.String | Task due date. Search for result that has this parameter value less than specified.
val dueColonLte : kotlin.String = 2013-10-20 // kotlin.String | Task due date. Search for result that has this parameter value less or equal to the specified.
val parentId : kotlin.Int = 56 // kotlin.Int | Parent Comment identifier
val parentIdColonIn : kotlin.Int = 56 // kotlin.Int | Parent Comment identifier. Search for results that contain any of specified values of this parameter.
val userId : kotlin.String = userId_example // kotlin.String | Identifier of User who created a Task
val userIdColonIn : kotlin.String = userIdColonIn_example // kotlin.String | Identifier of User who created a Task. Search for results that contain any of specified values of this parameter.
val created : kotlin.String = 2013-10-20 // kotlin.String | Task creation date
val createdColonGt : kotlin.String = 2013-10-20 // kotlin.String | Task creation date. Search for result that has this parameter value greater than specified.
val createdColonGte : kotlin.String = 2013-10-20 // kotlin.String | Task creation date. Search for result that has this parameter value greater or equal to the specified.
val createdColonLt : kotlin.String = 2013-10-20 // kotlin.String | Task creation date. Search for result that has this parameter value less than specified.
val createdColonLte : kotlin.String = 2013-10-20 // kotlin.String | Task creation date. Search for result that has this parameter value less or equal to the specified.
val modified : kotlin.String = 2013-10-20 // kotlin.String | Task modification date
val modifiedColonGt : kotlin.String = 2013-10-20 // kotlin.String | Task modification date. Search for result that has this parameter value greater than specified.
val modifiedColonGte : kotlin.String = 2013-10-20 // kotlin.String | Task modification date. Search for result that has this parameter value greater or equal to the specified.
val modifiedColonLt : kotlin.String = 2013-10-20 // kotlin.String | Task modification date. Search for result that has this parameter value less than specified.
val modifiedColonLte : kotlin.String = 2013-10-20 // kotlin.String | Task modification date. Search for result that has this parameter value less or equal to the specified.
val contentsColonContains : kotlin.String = contentsColonContains_example // kotlin.String | Task content. Search for result that contains specified characters in this parameter.
val status : kotlin.collections.List<kotlin.String> =  // kotlin.collections.List<kotlin.String> | Task status
val deleted : kotlin.Boolean = true // kotlin.Boolean | Whether the task has been deleted
val orderBy : kotlin.collections.List<kotlin.String> =  // kotlin.collections.List<kotlin.String> | Sorting options
val offset : kotlin.Int = 56 // kotlin.Int | Offset
val limit : kotlin.Int = 56 // kotlin.Int | Limit
val with : kotlin.String = with_example // kotlin.String | With parameters
val mode : kotlin.String = mode_example // kotlin.String | Response mode
try {
    val result : kotlin.collections.List<Task> = apiInstance.restFoldersIdTasksGet(id, assigneeId, assigneeIdColonIn, due, dueColonGt, dueColonGte, dueColonLt, dueColonLte, parentId, parentIdColonIn, userId, userIdColonIn, created, createdColonGt, createdColonGte, createdColonLt, createdColonLte, modified, modifiedColonGt, modifiedColonGte, modifiedColonLt, modifiedColonLte, contentsColonContains, status, deleted, orderBy, offset, limit, with, mode)
    println(result)
} catch (e: ClientException) {
    println("4xx response calling FoldersApi#restFoldersIdTasksGet")
    e.printStackTrace()
} catch (e: ServerException) {
    println("5xx response calling FoldersApi#restFoldersIdTasksGet")
    e.printStackTrace()
}
```

### Parameters

Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **id** | **kotlin.String**| Folder object ID of the task to retrieve |
 **assigneeId** | **kotlin.String**| Assigned User unique identifier | [optional]
 **assigneeIdColonIn** | **kotlin.String**| Assigned User unique identifier. Search for results that contain any of specified values of this parameter. | [optional]
 **due** | **kotlin.String**| Task due date | [optional]
 **dueColonGt** | **kotlin.String**| Task due date. Search for result that has this parameter value greater than specified. | [optional]
 **dueColonGte** | **kotlin.String**| Task due date. Search for result that has this parameter value greater or equal to the specified. | [optional]
 **dueColonLt** | **kotlin.String**| Task due date. Search for result that has this parameter value less than specified. | [optional]
 **dueColonLte** | **kotlin.String**| Task due date. Search for result that has this parameter value less or equal to the specified. | [optional]
 **parentId** | **kotlin.Int**| Parent Comment identifier | [optional]
 **parentIdColonIn** | **kotlin.Int**| Parent Comment identifier. Search for results that contain any of specified values of this parameter. | [optional]
 **userId** | **kotlin.String**| Identifier of User who created a Task | [optional]
 **userIdColonIn** | **kotlin.String**| Identifier of User who created a Task. Search for results that contain any of specified values of this parameter. | [optional]
 **created** | **kotlin.String**| Task creation date | [optional]
 **createdColonGt** | **kotlin.String**| Task creation date. Search for result that has this parameter value greater than specified. | [optional]
 **createdColonGte** | **kotlin.String**| Task creation date. Search for result that has this parameter value greater or equal to the specified. | [optional]
 **createdColonLt** | **kotlin.String**| Task creation date. Search for result that has this parameter value less than specified. | [optional]
 **createdColonLte** | **kotlin.String**| Task creation date. Search for result that has this parameter value less or equal to the specified. | [optional]
 **modified** | **kotlin.String**| Task modification date | [optional]
 **modifiedColonGt** | **kotlin.String**| Task modification date. Search for result that has this parameter value greater than specified. | [optional]
 **modifiedColonGte** | **kotlin.String**| Task modification date. Search for result that has this parameter value greater or equal to the specified. | [optional]
 **modifiedColonLt** | **kotlin.String**| Task modification date. Search for result that has this parameter value less than specified. | [optional]
 **modifiedColonLte** | **kotlin.String**| Task modification date. Search for result that has this parameter value less or equal to the specified. | [optional]
 **contentsColonContains** | **kotlin.String**| Task content. Search for result that contains specified characters in this parameter. | [optional]
 **status** | [**kotlin.collections.List&lt;kotlin.String&gt;**](kotlin.String.md)| Task status | [optional]
 **deleted** | **kotlin.Boolean**| Whether the task has been deleted | [optional]
 **orderBy** | [**kotlin.collections.List&lt;kotlin.String&gt;**](kotlin.String.md)| Sorting options | [optional]
 **offset** | **kotlin.Int**| Offset | [optional]
 **limit** | **kotlin.Int**| Limit | [optional]
 **with** | **kotlin.String**| With parameters | [optional]
 **mode** | **kotlin.String**| Response mode | [optional]

### Return type

[**kotlin.collections.List&lt;Task&gt;**](Task.md)

### Authorization

No authorization required

### HTTP request headers

 - **Content-Type**: Not defined
 - **Accept**: */*

<a id="restFoldersIdTreeGet"></a>
# **restFoldersIdTreeGet**
> restFoldersIdTreeGet(id, mode)

Gets the folder path by its ID

Gets the folder path by its ID

### Example
```kotlin
// Import classes:
//import org.openapitools.client.infrastructure.*
//import org.openapitools.client.models.*

val apiInstance = FoldersApi()
val id : kotlin.String = id_example // kotlin.String | ID of the folder
val mode : kotlin.String = mode_example // kotlin.String | Response mode
try {
    apiInstance.restFoldersIdTreeGet(id, mode)
} catch (e: ClientException) {
    println("4xx response calling FoldersApi#restFoldersIdTreeGet")
    e.printStackTrace()
} catch (e: ServerException) {
    println("5xx response calling FoldersApi#restFoldersIdTreeGet")
    e.printStackTrace()
}
```

### Parameters

Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **id** | **kotlin.String**| ID of the folder |
 **mode** | **kotlin.String**| Response mode | [optional]

### Return type

null (empty response body)

### Authorization

No authorization required

### HTTP request headers

 - **Content-Type**: Not defined
 - **Accept**: Not defined

<a id="restFoldersParentFilesGet"></a>
# **restFoldersParentFilesGet**
> FolderChildrenFiles restFoldersParentFilesGet(parent, modifiedColonGte, created, mode, modifiedColonLte, expireColonGt, modifiedColonGt, expireColonLt, expireColonLte, expireColonGte, createdColonLt, nameColonContains, expire, userId, userIdColonIn, modifiedColonLt, orderBy, createdColonGt, returnEntity, createdColonLte, with, limit, isPushed, deleted, name, createdColonGte, modified, offset)

Returns the list of files in the specified folder.

Returns the list of files in the specified folder.

### Example
```kotlin
// Import classes:
//import org.openapitools.client.infrastructure.*
//import org.openapitools.client.models.*

val apiInstance = FoldersApi()
val parent : kotlin.String = parent_example // kotlin.String | The ID of the parent folder
val modifiedColonGte : kotlin.String = modifiedColonGte_example // kotlin.String | Object modified date. Search for result that has this parameter value greater or equal to the specified.
val created : kotlin.String = created_example // kotlin.String | Object creation date
val mode : kotlin.String = mode_example // kotlin.String | 
val modifiedColonLte : kotlin.String = modifiedColonLte_example // kotlin.String | Object modified date. Search for result that has this parameter value less or equal to the specified.
val expireColonGt : kotlin.String = expireColonGt_example // kotlin.String | Expiration date. Search for result that has this parameter value greater than specified.
val modifiedColonGt : kotlin.String = modifiedColonGt_example // kotlin.String | Object modified date. Search for result that has this parameter value greater than specified.
val expireColonLt : kotlin.String = expireColonLt_example // kotlin.String | Expiration date. Search for result that has this parameter value less than specified.
val expireColonLte : kotlin.String = expireColonLte_example // kotlin.String | Expiration date. Search for result that has this parameter value less or equal to the specified.
val expireColonGte : kotlin.String = expireColonGte_example // kotlin.String | Expiration date. Search for result that has this parameter value greater or equal to the specified.
val createdColonLt : kotlin.String = createdColonLt_example // kotlin.String | Email creation date. Search for result that has this parameter value less than specified.
val nameColonContains : kotlin.String = nameColonContains_example // kotlin.String | Object name. Search for result that contains specified characters in this parameter.
val expire : kotlin.String = expire_example // kotlin.String | Object modified date
val userId : kotlin.String = userId_example // kotlin.String | Unique identifier of Object creator
val userIdColonIn : kotlin.collections.List<kotlin.String> =  // kotlin.collections.List<kotlin.String> | Unique identifier of Object creator recommended request size <= 100
val modifiedColonLt : kotlin.String = modifiedColonLt_example // kotlin.String | Object modified date. Search for result that has this parameter value less than specified.
val orderBy : kotlin.String = orderBy_example // kotlin.String | Sorting options. Accepts id, name, modified, created, size. Sample format is id:asc
val createdColonGt : kotlin.String = createdColonGt_example // kotlin.String | Object creation date. Search for result that has this parameter value greater than specified.
val returnEntity : kotlin.Boolean = true // kotlin.Boolean | 
val createdColonLte : kotlin.String = createdColonLte_example // kotlin.String | Email creation date. Search for result that has this parameter value less or equal to the specified.
val with : kotlin.String = with_example // kotlin.String | 
val limit : kotlin.Int = 56 // kotlin.Int | 
val isPushed : kotlin.Boolean = true // kotlin.Boolean | Whether the file is pushed
val deleted : kotlin.Boolean = true // kotlin.Boolean | Don't show deleted, true - show only deleted, none - show both
val name : kotlin.String = name_example // kotlin.String | Object name
val createdColonGte : kotlin.String = createdColonGte_example // kotlin.String | Object creation date. Search for result that has this parameter value greater or equal to the specified.
val modified : kotlin.String = modified_example // kotlin.String | Object modified date
val offset : kotlin.Int = 56 // kotlin.Int | 
try {
    val result : FolderChildrenFiles = apiInstance.restFoldersParentFilesGet(parent, modifiedColonGte, created, mode, modifiedColonLte, expireColonGt, modifiedColonGt, expireColonLt, expireColonLte, expireColonGte, createdColonLt, nameColonContains, expire, userId, userIdColonIn, modifiedColonLt, orderBy, createdColonGt, returnEntity, createdColonLte, with, limit, isPushed, deleted, name, createdColonGte, modified, offset)
    println(result)
} catch (e: ClientException) {
    println("4xx response calling FoldersApi#restFoldersParentFilesGet")
    e.printStackTrace()
} catch (e: ServerException) {
    println("5xx response calling FoldersApi#restFoldersParentFilesGet")
    e.printStackTrace()
}
```

### Parameters

Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **parent** | **kotlin.String**| The ID of the parent folder |
 **modifiedColonGte** | **kotlin.String**| Object modified date. Search for result that has this parameter value greater or equal to the specified. | [optional]
 **created** | **kotlin.String**| Object creation date | [optional]
 **mode** | **kotlin.String**|  | [optional]
 **modifiedColonLte** | **kotlin.String**| Object modified date. Search for result that has this parameter value less or equal to the specified. | [optional]
 **expireColonGt** | **kotlin.String**| Expiration date. Search for result that has this parameter value greater than specified. | [optional]
 **modifiedColonGt** | **kotlin.String**| Object modified date. Search for result that has this parameter value greater than specified. | [optional]
 **expireColonLt** | **kotlin.String**| Expiration date. Search for result that has this parameter value less than specified. | [optional]
 **expireColonLte** | **kotlin.String**| Expiration date. Search for result that has this parameter value less or equal to the specified. | [optional]
 **expireColonGte** | **kotlin.String**| Expiration date. Search for result that has this parameter value greater or equal to the specified. | [optional]
 **createdColonLt** | **kotlin.String**| Email creation date. Search for result that has this parameter value less than specified. | [optional]
 **nameColonContains** | **kotlin.String**| Object name. Search for result that contains specified characters in this parameter. | [optional]
 **expire** | **kotlin.String**| Object modified date | [optional]
 **userId** | **kotlin.String**| Unique identifier of Object creator | [optional]
 **userIdColonIn** | [**kotlin.collections.List&lt;kotlin.String&gt;**](kotlin.String.md)| Unique identifier of Object creator recommended request size &lt;&#x3D; 100 | [optional]
 **modifiedColonLt** | **kotlin.String**| Object modified date. Search for result that has this parameter value less than specified. | [optional]
 **orderBy** | **kotlin.String**| Sorting options. Accepts id, name, modified, created, size. Sample format is id:asc | [optional]
 **createdColonGt** | **kotlin.String**| Object creation date. Search for result that has this parameter value greater than specified. | [optional]
 **returnEntity** | **kotlin.Boolean**|  | [optional]
 **createdColonLte** | **kotlin.String**| Email creation date. Search for result that has this parameter value less or equal to the specified. | [optional]
 **with** | **kotlin.String**|  | [optional]
 **limit** | **kotlin.Int**|  | [optional]
 **isPushed** | **kotlin.Boolean**| Whether the file is pushed | [optional]
 **deleted** | **kotlin.Boolean**| Don&#39;t show deleted, true - show only deleted, none - show both | [optional]
 **name** | **kotlin.String**| Object name | [optional]
 **createdColonGte** | **kotlin.String**| Object creation date. Search for result that has this parameter value greater or equal to the specified. | [optional]
 **modified** | **kotlin.String**| Object modified date | [optional]
 **offset** | **kotlin.Int**|  | [optional]

### Return type

[**FolderChildrenFiles**](FolderChildrenFiles.md)

### Authorization

No authorization required

### HTTP request headers

 - **Content-Type**: Not defined
 - **Accept**: */*

<a id="restFoldersSharedGet"></a>
# **restFoldersSharedGet**
> kotlin.collections.List&lt;Folder&gt; restFoldersSharedGet(name, nameColonContains, userId, userIdColonIn, created, createdColonGt, createdColonGte, createdColonLt, createdColonLte, modified, modifiedColonGt, modifiedColonGte, modifiedColonLt, modifiedColonLte, deleted, expire, expireColonGt, expireColonGte, expireColonLt, expireColonLte, fileLifetime, fileLifetimeColonGt, fileLifetimeColonGte, fileLifetimeColonLt, fileLifetimeColonLte, secure, descriptionColonContains, sharedByMe, orderBy, offset, limit, with, mode)

List top level shared folders

Return the list of top level shared folders.

### Example
```kotlin
// Import classes:
//import org.openapitools.client.infrastructure.*
//import org.openapitools.client.models.*

val apiInstance = FoldersApi()
val name : kotlin.String = name_example // kotlin.String | Folder name
val nameColonContains : kotlin.String = nameColonContains_example // kotlin.String | Folder name. Search for result that contains specified characters in this parameter.
val userId : kotlin.String = userId_example // kotlin.String | Unique identifier of Object creator
val userIdColonIn : kotlin.String = userIdColonIn_example // kotlin.String | Unique identifier of Object creator. Search for results that contain any of specified values of this parameter.
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
val expire : kotlin.Int = 56 // kotlin.Int | Expiration date
val expireColonGt : kotlin.Int = 56 // kotlin.Int | Expiration date. Search for result that has this parameter value greater than specified.
val expireColonGte : kotlin.Int = 56 // kotlin.Int | Expiration date. Search for result that has this parameter value greater or equal to the specified.
val expireColonLt : kotlin.Int = 56 // kotlin.Int | Expiration date. Search for result that has this parameter value less than specified.
val expireColonLte : kotlin.Int = 56 // kotlin.Int | Expiration date. Search for result that has this parameter value less or equal to the specified.
val fileLifetime : kotlin.Int = 56 // kotlin.Int | Folder lifetime
val fileLifetimeColonGt : kotlin.Int = 56 // kotlin.Int | Folder lifetime. Search for result that has this parameter value greater than specified.
val fileLifetimeColonGte : kotlin.Int = 56 // kotlin.Int | Folder lifetime. Search for result that has this parameter value greater or equal to the specified.
val fileLifetimeColonLt : kotlin.Int = 56 // kotlin.Int | Folder lifetime. Search for result that has this parameter value less than specified.
val fileLifetimeColonLte : kotlin.Int = 56 // kotlin.Int | Folder lifetime. Search for result that has this parameter value less or equal to the specified.
val secure : kotlin.Boolean = true // kotlin.Boolean | Folder secure flag
val descriptionColonContains : kotlin.String = descriptionColonContains_example // kotlin.String | Folder description. Search for result that contains specified characters in this parameter.
val sharedByMe : kotlin.Boolean = true // kotlin.Boolean | true - return only folders shared by me;                               false - return only folders shared with me;                               empty - return both
val orderBy : kotlin.collections.List<kotlin.String> =  // kotlin.collections.List<kotlin.String> | Sorting options
val offset : kotlin.Int = 56 // kotlin.Int | Offset
val limit : kotlin.Int = 56 // kotlin.Int | Limit
val with : kotlin.String = with_example // kotlin.String | With parameters
val mode : kotlin.String = mode_example // kotlin.String | Response mode
try {
    val result : kotlin.collections.List<Folder> = apiInstance.restFoldersSharedGet(name, nameColonContains, userId, userIdColonIn, created, createdColonGt, createdColonGte, createdColonLt, createdColonLte, modified, modifiedColonGt, modifiedColonGte, modifiedColonLt, modifiedColonLte, deleted, expire, expireColonGt, expireColonGte, expireColonLt, expireColonLte, fileLifetime, fileLifetimeColonGt, fileLifetimeColonGte, fileLifetimeColonLt, fileLifetimeColonLte, secure, descriptionColonContains, sharedByMe, orderBy, offset, limit, with, mode)
    println(result)
} catch (e: ClientException) {
    println("4xx response calling FoldersApi#restFoldersSharedGet")
    e.printStackTrace()
} catch (e: ServerException) {
    println("5xx response calling FoldersApi#restFoldersSharedGet")
    e.printStackTrace()
}
```

### Parameters

Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **name** | **kotlin.String**| Folder name | [optional]
 **nameColonContains** | **kotlin.String**| Folder name. Search for result that contains specified characters in this parameter. | [optional]
 **userId** | **kotlin.String**| Unique identifier of Object creator | [optional]
 **userIdColonIn** | **kotlin.String**| Unique identifier of Object creator. Search for results that contain any of specified values of this parameter. | [optional]
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
 **expire** | **kotlin.Int**| Expiration date | [optional]
 **expireColonGt** | **kotlin.Int**| Expiration date. Search for result that has this parameter value greater than specified. | [optional]
 **expireColonGte** | **kotlin.Int**| Expiration date. Search for result that has this parameter value greater or equal to the specified. | [optional]
 **expireColonLt** | **kotlin.Int**| Expiration date. Search for result that has this parameter value less than specified. | [optional]
 **expireColonLte** | **kotlin.Int**| Expiration date. Search for result that has this parameter value less or equal to the specified. | [optional]
 **fileLifetime** | **kotlin.Int**| Folder lifetime | [optional]
 **fileLifetimeColonGt** | **kotlin.Int**| Folder lifetime. Search for result that has this parameter value greater than specified. | [optional]
 **fileLifetimeColonGte** | **kotlin.Int**| Folder lifetime. Search for result that has this parameter value greater or equal to the specified. | [optional]
 **fileLifetimeColonLt** | **kotlin.Int**| Folder lifetime. Search for result that has this parameter value less than specified. | [optional]
 **fileLifetimeColonLte** | **kotlin.Int**| Folder lifetime. Search for result that has this parameter value less or equal to the specified. | [optional]
 **secure** | **kotlin.Boolean**| Folder secure flag | [optional]
 **descriptionColonContains** | **kotlin.String**| Folder description. Search for result that contains specified characters in this parameter. | [optional]
 **sharedByMe** | **kotlin.Boolean**| true - return only folders shared by me;                               false - return only folders shared with me;                               empty - return both | [optional]
 **orderBy** | [**kotlin.collections.List&lt;kotlin.String&gt;**](kotlin.String.md)| Sorting options | [optional]
 **offset** | **kotlin.Int**| Offset | [optional]
 **limit** | **kotlin.Int**| Limit | [optional]
 **with** | **kotlin.String**| With parameters | [optional]
 **mode** | **kotlin.String**| Response mode | [optional]

### Return type

[**kotlin.collections.List&lt;Folder&gt;**](Folder.md)

### Authorization

No authorization required

### HTTP request headers

 - **Content-Type**: Not defined
 - **Accept**: */*

<a id="restFoldersTopGet"></a>
# **restFoldersTopGet**
> Folders restFoldersTopGet(deleted, with, limit, mode, orderBy, offset, returnEntity)

Return the list of top level and shared folders.

Return the list of top level and shared folders.

### Example
```kotlin
// Import classes:
//import org.openapitools.client.infrastructure.*
//import org.openapitools.client.models.*

val apiInstance = FoldersApi()
val deleted : kotlin.Boolean = true // kotlin.Boolean | don't show deleted, true - show only deleted, none - show both
val with : kotlin.String = with_example // kotlin.String | 
val limit : kotlin.Int = 56 // kotlin.Int | limit
val mode : kotlin.String = mode_example // kotlin.String | 
val orderBy : kotlin.String = orderBy_example // kotlin.String | Sorting options. Accepts id, name, modified, created, size. Sample format is id:asc
val offset : kotlin.Int = 56 // kotlin.Int | offset
val returnEntity : kotlin.Boolean = true // kotlin.Boolean | 
try {
    val result : Folders = apiInstance.restFoldersTopGet(deleted, with, limit, mode, orderBy, offset, returnEntity)
    println(result)
} catch (e: ClientException) {
    println("4xx response calling FoldersApi#restFoldersTopGet")
    e.printStackTrace()
} catch (e: ServerException) {
    println("5xx response calling FoldersApi#restFoldersTopGet")
    e.printStackTrace()
}
```

### Parameters

Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **deleted** | **kotlin.Boolean**| don&#39;t show deleted, true - show only deleted, none - show both | [optional]
 **with** | **kotlin.String**|  | [optional]
 **limit** | **kotlin.Int**| limit | [optional]
 **mode** | **kotlin.String**|  | [optional]
 **orderBy** | **kotlin.String**| Sorting options. Accepts id, name, modified, created, size. Sample format is id:asc | [optional]
 **offset** | **kotlin.Int**| offset | [optional]
 **returnEntity** | **kotlin.Boolean**|  | [optional]

### Return type

[**Folders**](Folders.md)

### Authorization

No authorization required

### HTTP request headers

 - **Content-Type**: Not defined
 - **Accept**: */*

<a id="restPermissionsFolderFolderIdGet"></a>
# **restPermissionsFolderFolderIdGet**
> kotlin.collections.List&lt;Permission&gt; restPermissionsFolderFolderIdGet(folderId, id, idColonIn, name, nameColonContains, allowed, enabled, with, mode)

Return the list of permissions available on a folder

Return available permissions

### Example
```kotlin
// Import classes:
//import org.openapitools.client.infrastructure.*
//import org.openapitools.client.models.*

val apiInstance = FoldersApi()
val folderId : kotlin.String = folderId_example // kotlin.String | ID of the folder
val id : kotlin.Int = 56 // kotlin.Int | Unique action identifier
val idColonIn : kotlin.Int = 56 // kotlin.Int | Unique action identifier. Search for results that contain any of specified values of this parameter.
val name : kotlin.String = name_example // kotlin.String | Action name
val nameColonContains : kotlin.String = nameColonContains_example // kotlin.String | Action name. Search for result that contains specified characters in this parameter.
val allowed : kotlin.Boolean = true // kotlin.Boolean | Determines if one has permissions to perform action
val enabled : kotlin.Boolean = true // kotlin.Boolean | Determines if given action is available considering current object state (locked, deleted, etc)
val with : kotlin.String = with_example // kotlin.String | With parameters
val mode : kotlin.String = mode_example // kotlin.String | Response mode
try {
    val result : kotlin.collections.List<Permission> = apiInstance.restPermissionsFolderFolderIdGet(folderId, id, idColonIn, name, nameColonContains, allowed, enabled, with, mode)
    println(result)
} catch (e: ClientException) {
    println("4xx response calling FoldersApi#restPermissionsFolderFolderIdGet")
    e.printStackTrace()
} catch (e: ServerException) {
    println("5xx response calling FoldersApi#restPermissionsFolderFolderIdGet")
    e.printStackTrace()
}
```

### Parameters

Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **folderId** | **kotlin.String**| ID of the folder |
 **id** | **kotlin.Int**| Unique action identifier | [optional]
 **idColonIn** | **kotlin.Int**| Unique action identifier. Search for results that contain any of specified values of this parameter. | [optional]
 **name** | **kotlin.String**| Action name | [optional]
 **nameColonContains** | **kotlin.String**| Action name. Search for result that contains specified characters in this parameter. | [optional]
 **allowed** | **kotlin.Boolean**| Determines if one has permissions to perform action | [optional]
 **enabled** | **kotlin.Boolean**| Determines if given action is available considering current object state (locked, deleted, etc) | [optional]
 **with** | **kotlin.String**| With parameters | [optional]
 **mode** | **kotlin.String**| Response mode | [optional]

### Return type

[**kotlin.collections.List&lt;Permission&gt;**](Permission.md)

### Authorization

No authorization required

### HTTP request headers

 - **Content-Type**: Not defined
 - **Accept**: */*

