# FilesApi

All URIs are relative to *http://localhost*

Method | HTTP request | Description
------------- | ------------- | -------------
[**previewFileIdGet**](FilesApi.md#previewFileIdGet) | **GET** /preview/file/{id} | Preview content of file from EC sources
[**restAdminFilesIdActionsRescanPost**](FilesApi.md#restAdminFilesIdActionsRescanPost) | **POST** /rest/admin/files/{id}/actions/rescan | Submit file for rescan
[**restAdminFilesPut**](FilesApi.md#restAdminFilesPut) | **PUT** /rest/admin/files | Bulk update files
[**restFilesActionsContentLinkRefGet**](FilesApi.md#restFilesActionsContentLinkRefGet) | **GET** /rest/files/actions/content/link/{ref} | Download a file by link
[**restFilesActionsCopyPost**](FilesApi.md#restFilesActionsCopyPost) | **POST** /rest/files/actions/copy | Copy multiple files to folder
[**restFilesActionsLockPatch**](FilesApi.md#restFilesActionsLockPatch) | **PATCH** /rest/files/actions/lock | Bulk lock files
[**restFilesActionsMobileSyncItemsDelete**](FilesApi.md#restFilesActionsMobileSyncItemsDelete) | **DELETE** /rest/files/actions/mobileSyncItems | Delete multiple files from user mobile sync list
[**restFilesActionsMobileSyncItemsPost**](FilesApi.md#restFilesActionsMobileSyncItemsPost) | **POST** /rest/files/actions/mobileSyncItems | Add multiple files to mobile sync list
[**restFilesActionsMovePost**](FilesApi.md#restFilesActionsMovePost) | **POST** /rest/files/actions/move | Move multiple files to folder
[**restFilesActionsPermanentDelete**](FilesApi.md#restFilesActionsPermanentDelete) | **DELETE** /rest/files/actions/permanent | Permanently delete list of files
[**restFilesActionsPushDelete**](FilesApi.md#restFilesActionsPushDelete) | **DELETE** /rest/files/actions/push | Un-Push collection of files
[**restFilesActionsPushPost**](FilesApi.md#restFilesActionsPushPost) | **POST** /rest/files/actions/push | Push files list to mobile sync list
[**restFilesActionsRecoverPatch**](FilesApi.md#restFilesActionsRecoverPatch) | **PATCH** /rest/files/actions/recover | Recover files
[**restFilesActionsScanPost**](FilesApi.md#restFilesActionsScanPost) | **POST** /rest/files/actions/scan | Triggers on demand AV/DLP scan on multiple files.
[**restFilesActionsUnlockPatch**](FilesApi.md#restFilesActionsUnlockPatch) | **PATCH** /rest/files/actions/unlock | Bulk unlock files
[**restFilesActionsZipGet**](FilesApi.md#restFilesActionsZipGet) | **GET** /rest/files/actions/zip | Download multiple files/folders as zip
[**restFilesActionsZipStatusGet**](FilesApi.md#restFilesActionsZipStatusGet) | **GET** /rest/files/actions/zipStatus | Check multiple files/folders AV/DLP status
[**restFilesDelete**](FilesApi.md#restFilesDelete) | **DELETE** /rest/files | Deletes list of files
[**restFilesIdActionsLockPatch**](FilesApi.md#restFilesIdActionsLockPatch) | **PATCH** /rest/files/{id}/actions/lock | Locks the file by its ID
[**restFilesIdActionsPermanentDelete**](FilesApi.md#restFilesIdActionsPermanentDelete) | **DELETE** /rest/files/{id}/actions/permanent | Permanently delete a file
[**restFilesIdActionsPushDelete**](FilesApi.md#restFilesIdActionsPushDelete) | **DELETE** /rest/files/{id}/actions/push | Un-Push file
[**restFilesIdActionsPushPost**](FilesApi.md#restFilesIdActionsPushPost) | **POST** /rest/files/{id}/actions/push | Push file to mobile sync list
[**restFilesIdActionsRecoverPatch**](FilesApi.md#restFilesIdActionsRecoverPatch) | **PATCH** /rest/files/{id}/actions/recover | Recovers deleted file.
[**restFilesIdActionsReturnPatch**](FilesApi.md#restFilesIdActionsReturnPatch) | **PATCH** /rest/files/{id}/actions/return | Returns file to EC source
[**restFilesIdActionsScanPost**](FilesApi.md#restFilesIdActionsScanPost) | **POST** /rest/files/{id}/actions/scan | Triggers on demand AV/DLP file scan.
[**restFilesIdActionsUnlockPatch**](FilesApi.md#restFilesIdActionsUnlockPatch) | **PATCH** /rest/files/{id}/actions/unlock | Unlocks the file by its ID
[**restFilesIdCommentsGet**](FilesApi.md#restFilesIdCommentsGet) | **GET** /rest/files/{id}/comments | Get Comments for a file
[**restFilesIdCommentsPost**](FilesApi.md#restFilesIdCommentsPost) | **POST** /rest/files/{id}/comments | Create a Comment on a file
[**restFilesIdContentGet**](FilesApi.md#restFilesIdContentGet) | **GET** /rest/files/{id}/content | Download a file
[**restFilesIdDelete**](FilesApi.md#restFilesIdDelete) | **DELETE** /rest/files/{id} | Mark file for deletion.
[**restFilesIdExternalEditGet**](FilesApi.md#restFilesIdExternalEditGet) | **GET** /rest/files/{id}/externalEdit | Get access token for external file edit.
[**restFilesIdGet**](FilesApi.md#restFilesIdGet) | **GET** /rest/files/{id} | Retrieve information about the file specified.
[**restFilesIdMembersDelete**](FilesApi.md#restFilesIdMembersDelete) | **DELETE** /rest/files/{id}/members | Delete all members in file
[**restFilesIdMembersGet**](FilesApi.md#restFilesIdMembersGet) | **GET** /rest/files/{id}/members | List of members in with access to the file
[**restFilesIdMembersLdapGroupGet**](FilesApi.md#restFilesIdMembersLdapGroupGet) | **GET** /rest/files/{id}/members/ldapGroup | List members
[**restFilesIdMembersLdapGroupLdapGroupIdGet**](FilesApi.md#restFilesIdMembersLdapGroupLdapGroupIdGet) | **GET** /rest/files/{id}/members/ldapGroup/{ldap_group_id} | display group member
[**restFilesIdMembersMeDelete**](FilesApi.md#restFilesIdMembersMeDelete) | **DELETE** /rest/files/{id}/members/me | Leave as the file member
[**restFilesIdMembersMemberUserIdDelete**](FilesApi.md#restFilesIdMembersMemberUserIdDelete) | **DELETE** /rest/files/{id}/members/{member_user_id} | Delete member from the file
[**restFilesIdMembersMemberUserIdGet**](FilesApi.md#restFilesIdMembersMemberUserIdGet) | **GET** /rest/files/{id}/members/{member_user_id} | display member
[**restFilesIdMembersMemberUserIdPut**](FilesApi.md#restFilesIdMembersMemberUserIdPut) | **PUT** /rest/files/{id}/members/{member_user_id} | Update members in the file
[**restFilesIdPathGet**](FilesApi.md#restFilesIdPathGet) | **GET** /rest/files/{id}/path | Gets the file path by its ID
[**restFilesIdPost**](FilesApi.md#restFilesIdPost) | **POST** /rest/files/{id} | upload new version
[**restFilesIdPreviewGet**](FilesApi.md#restFilesIdPreviewGet) | **GET** /rest/files/{id}/preview | Retrieve information about the file preview.
[**restFilesIdPut**](FilesApi.md#restFilesIdPut) | **PUT** /rest/files/{id} | Update the details of the file specified
[**restFilesIdTasksGet**](FilesApi.md#restFilesIdTasksGet) | **GET** /rest/files/{id}/tasks | Get Tasks for a file
[**restFilesIdTasksPost**](FilesApi.md#restFilesIdTasksPost) | **POST** /rest/files/{id}/tasks | Create a Task on a file
[**restFilesIdVersionsGet**](FilesApi.md#restFilesIdVersionsGet) | **GET** /rest/files/{id}/versions | List versions
[**restFilesIdVersionsPost**](FilesApi.md#restFilesIdVersionsPost) | **POST** /rest/files/{id}/versions | Uploads a new file version
[**restFilesIdVersionsVersionIdActionsPromotePost**](FilesApi.md#restFilesIdVersionsVersionIdActionsPromotePost) | **POST** /rest/files/{id}/versions/{version_id}/actions/promote | promote specified file version
[**restFilesIdVersionsVersionIdActionsScanPost**](FilesApi.md#restFilesIdVersionsVersionIdActionsScanPost) | **POST** /rest/files/{id}/versions/{version_id}/actions/scan | Triggers on demand AV/DLP file scan.
[**restFilesIdVersionsVersionIdContentGet**](FilesApi.md#restFilesIdVersionsVersionIdContentGet) | **GET** /rest/files/{id}/versions/{version_id}/content | download specified version
[**restFilesIdVersionsVersionIdDelete**](FilesApi.md#restFilesIdVersionsVersionIdDelete) | **DELETE** /rest/files/{id}/versions/{version_id} | Deletes the specified file version
[**restFilesIdVersionsVersionIdGet**](FilesApi.md#restFilesIdVersionsVersionIdGet) | **GET** /rest/files/{id}/versions/{version_id} | Get specified version
[**restFilesIdVersionsVersionIdPreviewGet**](FilesApi.md#restFilesIdVersionsVersionIdPreviewGet) | **GET** /rest/files/{id}/versions/{version_id}/preview | Retrieve information about the file preview.
[**restFilesMembersPost**](FilesApi.md#restFilesMembersPost) | **POST** /rest/files/members | Add multiple members
[**restFilesPreviewSupportGet**](FilesApi.md#restFilesPreviewSupportGet) | **GET** /rest/files/previewSupport | Check mime type before send
[**restFilesSharedGet**](FilesApi.md#restFilesSharedGet) | **GET** /rest/files/shared | Return user&#39;s all shared files and permissions
[**restFoldersIdActionsFileBase64EncodedPost**](FilesApi.md#restFoldersIdActionsFileBase64EncodedPost) | **POST** /rest/folders/{id}/actions/fileBase64Encoded | upload  base64 encoded content
[**restFoldersIdActionsFilePost**](FilesApi.md#restFoldersIdActionsFilePost) | **POST** /rest/folders/{id}/actions/file | upload content
[**restFoldersParentFilesPost**](FilesApi.md#restFoldersParentFilesPost) | **POST** /rest/folders/{parent}/files | Uploads a new file
[**restFoldersParentIdActionsFileFromTemplatePost**](FilesApi.md#restFoldersParentIdActionsFileFromTemplatePost) | **POST** /rest/folders/{parent_id}/actions/fileFromTemplate | Create a new empty file from template
[**restPermissionsFileFileIdGet**](FilesApi.md#restPermissionsFileFileIdGet) | **GET** /rest/permissions/file/{file_id} | Return the list of permissions available on a file
[**restPermissionsFilesGet**](FilesApi.md#restPermissionsFilesGet) | **GET** /rest/permissions/files | Return the list of permissions available on a list of files
[**restRequestFileRefActionsFilePost**](FilesApi.md#restRequestFileRefActionsFilePost) | **POST** /rest/requestFile/{ref}/actions/file | upload content
[**restRequestFileRefCommentObjectIdPost**](FilesApi.md#restRequestFileRefCommentObjectIdPost) | **POST** /rest/requestFile/{ref}/comment/{object_id} | Create a Comment on a file
[**restRequestFileRefSourcesObjectIdContentGet**](FilesApi.md#restRequestFileRefSourcesObjectIdContentGet) | **GET** /rest/requestFile/{ref}/sources/{object_id}/content | Read source file content
[**restRequestFileRefUploadsObjectIdContentGet**](FilesApi.md#restRequestFileRefUploadsObjectIdContentGet) | **GET** /rest/requestFile/{ref}/uploads/{object_id}/content | Read source file content
[**restSourcesActionsDownloadByTransactionGet**](FilesApi.md#restSourcesActionsDownloadByTransactionGet) | **GET** /rest/sources/actions/downloadByTransaction | Download EC file
[**restSourcesActionsFilesIdPost**](FilesApi.md#restSourcesActionsFilesIdPost) | **POST** /rest/sources/actions/files/{id} | upload new version of EC file
[**restSourcesIdActionsFilePost**](FilesApi.md#restSourcesIdActionsFilePost) | **POST** /rest/sources/{id}/actions/file | upload content
[**restSourcesIdActionsInitiateDownloadPost**](FilesApi.md#restSourcesIdActionsInitiateDownloadPost) | **POST** /rest/sources/{id}/actions/initiateDownload | Initiate EC file download
[**restSourcesIdContentGet**](FilesApi.md#restSourcesIdContentGet) | **GET** /rest/sources/{id}/content | Read EC file content
[**restSourcesIdPreviewGet**](FilesApi.md#restSourcesIdPreviewGet) | **GET** /rest/sources/{id}/preview | Retrieve information about the kitepoint file preview.


<a id="previewFileIdGet"></a>
# **previewFileIdGet**
> previewFileIdGet(id)

Preview content of file from EC sources

Preview content of file from EC sources

### Example
```kotlin
// Import classes:
//import org.openapitools.client.infrastructure.*
//import org.openapitools.client.models.*

val apiInstance = FilesApi()
val id : kotlin.Int = 56 // kotlin.Int | The ID of the entity
try {
    apiInstance.previewFileIdGet(id)
} catch (e: ClientException) {
    println("4xx response calling FilesApi#previewFileIdGet")
    e.printStackTrace()
} catch (e: ServerException) {
    println("5xx response calling FilesApi#previewFileIdGet")
    e.printStackTrace()
}
```

### Parameters

Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **id** | **kotlin.Int**| The ID of the entity |

### Return type

null (empty response body)

### Authorization

No authorization required

### HTTP request headers

 - **Content-Type**: Not defined
 - **Accept**: Not defined

<a id="restAdminFilesIdActionsRescanPost"></a>
# **restAdminFilesIdActionsRescanPost**
> AdminFileRescan restAdminFilesIdActionsRescanPost(id, mode, with, returnEntity)

Submit file for rescan

Submit file for rescan

### Example
```kotlin
// Import classes:
//import org.openapitools.client.infrastructure.*
//import org.openapitools.client.models.*

val apiInstance = FilesApi()
val id : kotlin.Int = 56 // kotlin.Int | The ID of the entity
val mode : kotlin.String = mode_example // kotlin.String | 
val with : kotlin.String = with_example // kotlin.String | 
val returnEntity : kotlin.Boolean = true // kotlin.Boolean | 
try {
    val result : AdminFileRescan = apiInstance.restAdminFilesIdActionsRescanPost(id, mode, with, returnEntity)
    println(result)
} catch (e: ClientException) {
    println("4xx response calling FilesApi#restAdminFilesIdActionsRescanPost")
    e.printStackTrace()
} catch (e: ServerException) {
    println("5xx response calling FilesApi#restAdminFilesIdActionsRescanPost")
    e.printStackTrace()
}
```

### Parameters

Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **id** | **kotlin.Int**| The ID of the entity |
 **mode** | **kotlin.String**|  | [optional]
 **with** | **kotlin.String**|  | [optional]
 **returnEntity** | **kotlin.Boolean**|  | [optional]

### Return type

[**AdminFileRescan**](AdminFileRescan.md)

### Authorization

No authorization required

### HTTP request headers

 - **Content-Type**: Not defined
 - **Accept**: */*

<a id="restAdminFilesPut"></a>
# **restAdminFilesPut**
> Files restAdminFilesPut(body, mode, with, returnEntity)

Bulk update files

Bulk update files

### Example
```kotlin
// Import classes:
//import org.openapitools.client.infrastructure.*
//import org.openapitools.client.models.*

val apiInstance = FilesApi()
val body : AdminFilePutRequest =  // AdminFilePutRequest | 
val mode : kotlin.String = mode_example // kotlin.String | 
val with : kotlin.String = with_example // kotlin.String | 
val returnEntity : kotlin.Boolean = true // kotlin.Boolean | 
try {
    val result : Files = apiInstance.restAdminFilesPut(body, mode, with, returnEntity)
    println(result)
} catch (e: ClientException) {
    println("4xx response calling FilesApi#restAdminFilesPut")
    e.printStackTrace()
} catch (e: ServerException) {
    println("5xx response calling FilesApi#restAdminFilesPut")
    e.printStackTrace()
}
```

### Parameters

Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **body** | [**AdminFilePutRequest**](AdminFilePutRequest.md)|  |
 **mode** | **kotlin.String**|  | [optional]
 **with** | **kotlin.String**|  | [optional]
 **returnEntity** | **kotlin.Boolean**|  | [optional]

### Return type

[**Files**](Files.md)

### Authorization

No authorization required

### HTTP request headers

 - **Content-Type**: Not defined
 - **Accept**: */*

<a id="restFilesActionsContentLinkRefGet"></a>
# **restFilesActionsContentLinkRefGet**
> org.openapitools.client.infrastructure.OctetByteArray restFilesActionsContentLinkRefGet(ref)

Download a file by link

Download a file by link

### Example
```kotlin
// Import classes:
//import org.openapitools.client.infrastructure.*
//import org.openapitools.client.models.*

val apiInstance = FilesApi()
val ref : kotlin.String = ref_example // kotlin.String | The ID of the download link
try {
    val result : org.openapitools.client.infrastructure.OctetByteArray = apiInstance.restFilesActionsContentLinkRefGet(ref)
    println(result)
} catch (e: ClientException) {
    println("4xx response calling FilesApi#restFilesActionsContentLinkRefGet")
    e.printStackTrace()
} catch (e: ServerException) {
    println("5xx response calling FilesApi#restFilesActionsContentLinkRefGet")
    e.printStackTrace()
}
```

### Parameters

Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **ref** | **kotlin.String**| The ID of the download link |

### Return type

[**org.openapitools.client.infrastructure.OctetByteArray**](org.openapitools.client.infrastructure.OctetByteArray.md)

### Authorization

No authorization required

### HTTP request headers

 - **Content-Type**: Not defined
 - **Accept**: */*

<a id="restFilesActionsCopyPost"></a>
# **restFilesActionsCopyPost**
> restFilesActionsCopyPost(idColonIn, body, partialSuccess, returnEntity, mode)

Copy multiple files to folder

Copy multiple files to folder

### Example
```kotlin
// Import classes:
//import org.openapitools.client.infrastructure.*
//import org.openapitools.client.models.*

val apiInstance = FilesApi()
val idColonIn : kotlin.String = idColonIn_example // kotlin.String | Array of values which are going to be changed.
val body : FileCopyMovePost =  // FileCopyMovePost | File copy move parameters
val partialSuccess : kotlin.Boolean = true // kotlin.Boolean | Whether to perform action on valid items even if some ones fail
val returnEntity : kotlin.Boolean = true // kotlin.Boolean | Return information about newly created entity
val mode : kotlin.String = mode_example // kotlin.String | Response mode
try {
    apiInstance.restFilesActionsCopyPost(idColonIn, body, partialSuccess, returnEntity, mode)
} catch (e: ClientException) {
    println("4xx response calling FilesApi#restFilesActionsCopyPost")
    e.printStackTrace()
} catch (e: ServerException) {
    println("5xx response calling FilesApi#restFilesActionsCopyPost")
    e.printStackTrace()
}
```

### Parameters

Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **idColonIn** | **kotlin.String**| Array of values which are going to be changed. |
 **body** | [**FileCopyMovePost**](FileCopyMovePost.md)| File copy move parameters |
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

<a id="restFilesActionsLockPatch"></a>
# **restFilesActionsLockPatch**
> BulkOperationLockFile restFilesActionsLockPatch(body, partialSuccess, with, mode, idColonIn, returnEntity)

Bulk lock files

Bulk lock files

### Example
```kotlin
// Import classes:
//import org.openapitools.client.infrastructure.*
//import org.openapitools.client.models.*

val apiInstance = FilesApi()
val body : FileLockPostRequest =  // FileLockPostRequest | 
val partialSuccess : kotlin.Boolean = true // kotlin.Boolean | 
val with : kotlin.String = with_example // kotlin.String | 
val mode : kotlin.String = mode_example // kotlin.String | 
val idColonIn : kotlin.collections.List<kotlin.String> =  // kotlin.collections.List<kotlin.String> | 
val returnEntity : kotlin.Boolean = true // kotlin.Boolean | 
try {
    val result : BulkOperationLockFile = apiInstance.restFilesActionsLockPatch(body, partialSuccess, with, mode, idColonIn, returnEntity)
    println(result)
} catch (e: ClientException) {
    println("4xx response calling FilesApi#restFilesActionsLockPatch")
    e.printStackTrace()
} catch (e: ServerException) {
    println("5xx response calling FilesApi#restFilesActionsLockPatch")
    e.printStackTrace()
}
```

### Parameters

Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **body** | [**FileLockPostRequest**](FileLockPostRequest.md)|  |
 **partialSuccess** | **kotlin.Boolean**|  | [optional]
 **with** | **kotlin.String**|  | [optional]
 **mode** | **kotlin.String**|  | [optional]
 **idColonIn** | [**kotlin.collections.List&lt;kotlin.String&gt;**](kotlin.String.md)|  | [optional]
 **returnEntity** | **kotlin.Boolean**|  | [optional]

### Return type

[**BulkOperationLockFile**](BulkOperationLockFile.md)

### Authorization

No authorization required

### HTTP request headers

 - **Content-Type**: Not defined
 - **Accept**: */*

<a id="restFilesActionsMobileSyncItemsDelete"></a>
# **restFilesActionsMobileSyncItemsDelete**
> restFilesActionsMobileSyncItemsDelete(idColonIn, partialSuccess, mode)

Delete multiple files from user mobile sync list

Delete multiple files from user mobile sync list

### Example
```kotlin
// Import classes:
//import org.openapitools.client.infrastructure.*
//import org.openapitools.client.models.*

val apiInstance = FilesApi()
val idColonIn : kotlin.String = idColonIn_example // kotlin.String | Array of values which are going to be changed.
val partialSuccess : kotlin.Boolean = true // kotlin.Boolean | Whether to perform action on valid items even if some ones fail
val mode : kotlin.String = mode_example // kotlin.String | Response mode
try {
    apiInstance.restFilesActionsMobileSyncItemsDelete(idColonIn, partialSuccess, mode)
} catch (e: ClientException) {
    println("4xx response calling FilesApi#restFilesActionsMobileSyncItemsDelete")
    e.printStackTrace()
} catch (e: ServerException) {
    println("5xx response calling FilesApi#restFilesActionsMobileSyncItemsDelete")
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

<a id="restFilesActionsMobileSyncItemsPost"></a>
# **restFilesActionsMobileSyncItemsPost**
> restFilesActionsMobileSyncItemsPost(idColonIn, partialSuccess, returnEntity, mode)

Add multiple files to mobile sync list

Add multiple files to mobile sync list This operation will not return location headers for each entity created, if the inserted records are         required, returnEntity should be set to true.

### Example
```kotlin
// Import classes:
//import org.openapitools.client.infrastructure.*
//import org.openapitools.client.models.*

val apiInstance = FilesApi()
val idColonIn : kotlin.String = idColonIn_example // kotlin.String | Array of values which are going to be changed.
val partialSuccess : kotlin.Boolean = true // kotlin.Boolean | Whether to perform action on valid items even if some ones fail
val returnEntity : kotlin.Boolean = true // kotlin.Boolean | Return information about newly created entity
val mode : kotlin.String = mode_example // kotlin.String | Response mode
try {
    apiInstance.restFilesActionsMobileSyncItemsPost(idColonIn, partialSuccess, returnEntity, mode)
} catch (e: ClientException) {
    println("4xx response calling FilesApi#restFilesActionsMobileSyncItemsPost")
    e.printStackTrace()
} catch (e: ServerException) {
    println("5xx response calling FilesApi#restFilesActionsMobileSyncItemsPost")
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

<a id="restFilesActionsMovePost"></a>
# **restFilesActionsMovePost**
> restFilesActionsMovePost(idColonIn, body, partialSuccess, returnEntity, mode)

Move multiple files to folder

Move multiple files to folder

### Example
```kotlin
// Import classes:
//import org.openapitools.client.infrastructure.*
//import org.openapitools.client.models.*

val apiInstance = FilesApi()
val idColonIn : kotlin.String = idColonIn_example // kotlin.String | Array of values which are going to be changed.
val body : FileCopyMovePost =  // FileCopyMovePost | File copy move parameters
val partialSuccess : kotlin.Boolean = true // kotlin.Boolean | Whether to perform action on valid items even if some ones fail
val returnEntity : kotlin.Boolean = true // kotlin.Boolean | Return information about newly created entity
val mode : kotlin.String = mode_example // kotlin.String | Response mode
try {
    apiInstance.restFilesActionsMovePost(idColonIn, body, partialSuccess, returnEntity, mode)
} catch (e: ClientException) {
    println("4xx response calling FilesApi#restFilesActionsMovePost")
    e.printStackTrace()
} catch (e: ServerException) {
    println("5xx response calling FilesApi#restFilesActionsMovePost")
    e.printStackTrace()
}
```

### Parameters

Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **idColonIn** | **kotlin.String**| Array of values which are going to be changed. |
 **body** | [**FileCopyMovePost**](FileCopyMovePost.md)| File copy move parameters |
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

<a id="restFilesActionsPermanentDelete"></a>
# **restFilesActionsPermanentDelete**
> restFilesActionsPermanentDelete(idColonIn, partialSuccess, mode)

Permanently delete list of files

Permanently delete list of files. These files will no longer be accessible.

### Example
```kotlin
// Import classes:
//import org.openapitools.client.infrastructure.*
//import org.openapitools.client.models.*

val apiInstance = FilesApi()
val idColonIn : kotlin.String = idColonIn_example // kotlin.String | Array of values which are going to be changed.
val partialSuccess : kotlin.Boolean = true // kotlin.Boolean | Whether to perform action on valid items even if some ones fail
val mode : kotlin.String = mode_example // kotlin.String | Response mode
try {
    apiInstance.restFilesActionsPermanentDelete(idColonIn, partialSuccess, mode)
} catch (e: ClientException) {
    println("4xx response calling FilesApi#restFilesActionsPermanentDelete")
    e.printStackTrace()
} catch (e: ServerException) {
    println("5xx response calling FilesApi#restFilesActionsPermanentDelete")
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

<a id="restFilesActionsPushDelete"></a>
# **restFilesActionsPushDelete**
> restFilesActionsPushDelete(idColonIn, partialSuccess, mode)

Un-Push collection of files

Un-Pushing files deletes these files from all folder members sync list.

### Example
```kotlin
// Import classes:
//import org.openapitools.client.infrastructure.*
//import org.openapitools.client.models.*

val apiInstance = FilesApi()
val idColonIn : kotlin.String = idColonIn_example // kotlin.String | Array of values which are going to be changed.
val partialSuccess : kotlin.Boolean = true // kotlin.Boolean | Whether to perform action on valid items even if some ones fail
val mode : kotlin.String = mode_example // kotlin.String | Response mode
try {
    apiInstance.restFilesActionsPushDelete(idColonIn, partialSuccess, mode)
} catch (e: ClientException) {
    println("4xx response calling FilesApi#restFilesActionsPushDelete")
    e.printStackTrace()
} catch (e: ServerException) {
    println("5xx response calling FilesApi#restFilesActionsPushDelete")
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

<a id="restFilesActionsPushPost"></a>
# **restFilesActionsPushPost**
> restFilesActionsPushPost(idColonIn, partialSuccess, returnEntity, mode)

Push files list to mobile sync list

Set list of files as mobile sync item for all folder members. This operation will not return location headers for each entity created, if the inserted records are         required, returnEntity should be set to true.

### Example
```kotlin
// Import classes:
//import org.openapitools.client.infrastructure.*
//import org.openapitools.client.models.*

val apiInstance = FilesApi()
val idColonIn : kotlin.String = idColonIn_example // kotlin.String | Array of values which are going to be changed.
val partialSuccess : kotlin.Boolean = true // kotlin.Boolean | Whether to perform action on valid items even if some ones fail
val returnEntity : kotlin.Boolean = true // kotlin.Boolean | Return information about newly created entity
val mode : kotlin.String = mode_example // kotlin.String | Response mode
try {
    apiInstance.restFilesActionsPushPost(idColonIn, partialSuccess, returnEntity, mode)
} catch (e: ClientException) {
    println("4xx response calling FilesApi#restFilesActionsPushPost")
    e.printStackTrace()
} catch (e: ServerException) {
    println("5xx response calling FilesApi#restFilesActionsPushPost")
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

<a id="restFilesActionsRecoverPatch"></a>
# **restFilesActionsRecoverPatch**
> restFilesActionsRecoverPatch(idColonIn, partialSuccess, returnEntity, mode)

Recover files

Recovers bulk list of files.

### Example
```kotlin
// Import classes:
//import org.openapitools.client.infrastructure.*
//import org.openapitools.client.models.*

val apiInstance = FilesApi()
val idColonIn : kotlin.String = idColonIn_example // kotlin.String | Array of values which are going to be changed.
val partialSuccess : kotlin.Boolean = true // kotlin.Boolean | Whether to perform action on valid items even if some ones fail
val returnEntity : kotlin.Boolean = true // kotlin.Boolean | Return information about newly created entity
val mode : kotlin.String = mode_example // kotlin.String | Response mode
try {
    apiInstance.restFilesActionsRecoverPatch(idColonIn, partialSuccess, returnEntity, mode)
} catch (e: ClientException) {
    println("4xx response calling FilesApi#restFilesActionsRecoverPatch")
    e.printStackTrace()
} catch (e: ServerException) {
    println("5xx response calling FilesApi#restFilesActionsRecoverPatch")
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

<a id="restFilesActionsScanPost"></a>
# **restFilesActionsScanPost**
> restFilesActionsScanPost(returnEntity, idColonIn, with, mode)

Triggers on demand AV/DLP scan on multiple files.

Attempts to trigger an AV/DLP scan on requested files.

### Example
```kotlin
// Import classes:
//import org.openapitools.client.infrastructure.*
//import org.openapitools.client.models.*

val apiInstance = FilesApi()
val returnEntity : kotlin.Boolean = true // kotlin.Boolean | Return information about newly created entity
val idColonIn : kotlin.String = idColonIn_example // kotlin.String | List of IDs of entities to scan. Search for results that contain any of specified values of this parameter.
val with : kotlin.String = with_example // kotlin.String | With parameters
val mode : kotlin.String = mode_example // kotlin.String | Response mode
try {
    apiInstance.restFilesActionsScanPost(returnEntity, idColonIn, with, mode)
} catch (e: ClientException) {
    println("4xx response calling FilesApi#restFilesActionsScanPost")
    e.printStackTrace()
} catch (e: ServerException) {
    println("5xx response calling FilesApi#restFilesActionsScanPost")
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

<a id="restFilesActionsUnlockPatch"></a>
# **restFilesActionsUnlockPatch**
> BulkOperationLockFile restFilesActionsUnlockPatch(body, partialSuccess, with, mode, idColonIn, returnEntity)

Bulk unlock files

Bulk unlock files

### Example
```kotlin
// Import classes:
//import org.openapitools.client.infrastructure.*
//import org.openapitools.client.models.*

val apiInstance = FilesApi()
val body : FileLockPostRequest =  // FileLockPostRequest | 
val partialSuccess : kotlin.Boolean = true // kotlin.Boolean | 
val with : kotlin.String = with_example // kotlin.String | 
val mode : kotlin.String = mode_example // kotlin.String | 
val idColonIn : kotlin.collections.List<kotlin.String> =  // kotlin.collections.List<kotlin.String> | 
val returnEntity : kotlin.Boolean = true // kotlin.Boolean | 
try {
    val result : BulkOperationLockFile = apiInstance.restFilesActionsUnlockPatch(body, partialSuccess, with, mode, idColonIn, returnEntity)
    println(result)
} catch (e: ClientException) {
    println("4xx response calling FilesApi#restFilesActionsUnlockPatch")
    e.printStackTrace()
} catch (e: ServerException) {
    println("5xx response calling FilesApi#restFilesActionsUnlockPatch")
    e.printStackTrace()
}
```

### Parameters

Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **body** | [**FileLockPostRequest**](FileLockPostRequest.md)|  |
 **partialSuccess** | **kotlin.Boolean**|  | [optional]
 **with** | **kotlin.String**|  | [optional]
 **mode** | **kotlin.String**|  | [optional]
 **idColonIn** | [**kotlin.collections.List&lt;kotlin.String&gt;**](kotlin.String.md)|  | [optional]
 **returnEntity** | **kotlin.Boolean**|  | [optional]

### Return type

[**BulkOperationLockFile**](BulkOperationLockFile.md)

### Authorization

No authorization required

### HTTP request headers

 - **Content-Type**: Not defined
 - **Accept**: */*

<a id="restFilesActionsZipGet"></a>
# **restFilesActionsZipGet**
> restFilesActionsZipGet(name, fileIdColonIn, folderIdColonIn, username, extensions, utcOffset, partialSuccess, mode)

Download multiple files/folders as zip

Download multiple files/folders as zip

### Example
```kotlin
// Import classes:
//import org.openapitools.client.infrastructure.*
//import org.openapitools.client.models.*

val apiInstance = FilesApi()
val name : kotlin.String = name_example // kotlin.String | The zip filename
val fileIdColonIn : kotlin.String = fileIdColonIn_example // kotlin.String | List of file ID. Search for results that contain any of specified values of this parameter.
val folderIdColonIn : kotlin.String = folderIdColonIn_example // kotlin.String | List of folder ID. Search for results that contain any of specified values of this parameter.
val username : kotlin.String = username_example // kotlin.String | User email of files' requestor
val extensions : kotlin.String = extensions_example // kotlin.String | Filter by files with these extensions
val utcOffset : kotlin.Int = 56 // kotlin.Int | The user timezone offset in (seconds). UTC+08:00 = 28800
val partialSuccess : kotlin.Boolean = true // kotlin.Boolean | Whether to perform action on valid items even if some ones fail
val mode : kotlin.String = mode_example // kotlin.String | Response mode
try {
    apiInstance.restFilesActionsZipGet(name, fileIdColonIn, folderIdColonIn, username, extensions, utcOffset, partialSuccess, mode)
} catch (e: ClientException) {
    println("4xx response calling FilesApi#restFilesActionsZipGet")
    e.printStackTrace()
} catch (e: ServerException) {
    println("5xx response calling FilesApi#restFilesActionsZipGet")
    e.printStackTrace()
}
```

### Parameters

Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **name** | **kotlin.String**| The zip filename | [optional]
 **fileIdColonIn** | **kotlin.String**| List of file ID. Search for results that contain any of specified values of this parameter. | [optional]
 **folderIdColonIn** | **kotlin.String**| List of folder ID. Search for results that contain any of specified values of this parameter. | [optional]
 **username** | **kotlin.String**| User email of files&#39; requestor | [optional]
 **extensions** | **kotlin.String**| Filter by files with these extensions | [optional]
 **utcOffset** | **kotlin.Int**| The user timezone offset in (seconds). UTC+08:00 &#x3D; 28800 | [optional]
 **partialSuccess** | **kotlin.Boolean**| Whether to perform action on valid items even if some ones fail | [optional]
 **mode** | **kotlin.String**| Response mode | [optional]

### Return type

null (empty response body)

### Authorization

No authorization required

### HTTP request headers

 - **Content-Type**: Not defined
 - **Accept**: Not defined

<a id="restFilesActionsZipStatusGet"></a>
# **restFilesActionsZipStatusGet**
> restFilesActionsZipStatusGet(fileIdColonIn, folderIdColonIn, partialSuccess, extensions)

Check multiple files/folders AV/DLP status

Check multiple files/folders AV/DLP status

### Example
```kotlin
// Import classes:
//import org.openapitools.client.infrastructure.*
//import org.openapitools.client.models.*

val apiInstance = FilesApi()
val fileIdColonIn : kotlin.collections.List<kotlin.String> =  // kotlin.collections.List<kotlin.String> | 
val folderIdColonIn : kotlin.collections.List<kotlin.String> =  // kotlin.collections.List<kotlin.String> | 
val partialSuccess : kotlin.Boolean = true // kotlin.Boolean | Controls whether to allow partial success
val extensions : kotlin.collections.List<kotlin.String> =  // kotlin.collections.List<kotlin.String> | Filter by files with these extensions
try {
    apiInstance.restFilesActionsZipStatusGet(fileIdColonIn, folderIdColonIn, partialSuccess, extensions)
} catch (e: ClientException) {
    println("4xx response calling FilesApi#restFilesActionsZipStatusGet")
    e.printStackTrace()
} catch (e: ServerException) {
    println("5xx response calling FilesApi#restFilesActionsZipStatusGet")
    e.printStackTrace()
}
```

### Parameters

Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **fileIdColonIn** | [**kotlin.collections.List&lt;kotlin.String&gt;**](kotlin.String.md)|  | [optional]
 **folderIdColonIn** | [**kotlin.collections.List&lt;kotlin.String&gt;**](kotlin.String.md)|  | [optional]
 **partialSuccess** | **kotlin.Boolean**| Controls whether to allow partial success | [optional]
 **extensions** | [**kotlin.collections.List&lt;kotlin.String&gt;**](kotlin.String.md)| Filter by files with these extensions | [optional]

### Return type

null (empty response body)

### Authorization

No authorization required

### HTTP request headers

 - **Content-Type**: Not defined
 - **Accept**: Not defined

<a id="restFilesDelete"></a>
# **restFilesDelete**
> restFilesDelete(idColonIn, partialSuccess, mode)

Deletes list of files

Deletes list of files.

### Example
```kotlin
// Import classes:
//import org.openapitools.client.infrastructure.*
//import org.openapitools.client.models.*

val apiInstance = FilesApi()
val idColonIn : kotlin.String = idColonIn_example // kotlin.String | Array of values which are going to be changed.
val partialSuccess : kotlin.Boolean = true // kotlin.Boolean | Whether to perform action on valid items even if some ones fail
val mode : kotlin.String = mode_example // kotlin.String | Response mode
try {
    apiInstance.restFilesDelete(idColonIn, partialSuccess, mode)
} catch (e: ClientException) {
    println("4xx response calling FilesApi#restFilesDelete")
    e.printStackTrace()
} catch (e: ServerException) {
    println("5xx response calling FilesApi#restFilesDelete")
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

<a id="restFilesIdActionsLockPatch"></a>
# **restFilesIdActionsLockPatch**
> restFilesIdActionsLockPatch(id, returnEntity, mode)

Locks the file by its ID

Lock the given file from access.                   Other users will not be able to add a new version of this file                   until it is unlocked by the owner.

### Example
```kotlin
// Import classes:
//import org.openapitools.client.infrastructure.*
//import org.openapitools.client.models.*

val apiInstance = FilesApi()
val id : kotlin.String = id_example // kotlin.String | ID of the file
val returnEntity : kotlin.Boolean = true // kotlin.Boolean | Return information about newly created entity
val mode : kotlin.String = mode_example // kotlin.String | Response mode
try {
    apiInstance.restFilesIdActionsLockPatch(id, returnEntity, mode)
} catch (e: ClientException) {
    println("4xx response calling FilesApi#restFilesIdActionsLockPatch")
    e.printStackTrace()
} catch (e: ServerException) {
    println("5xx response calling FilesApi#restFilesIdActionsLockPatch")
    e.printStackTrace()
}
```

### Parameters

Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **id** | **kotlin.String**| ID of the file |
 **returnEntity** | **kotlin.Boolean**| Return information about newly created entity | [optional]
 **mode** | **kotlin.String**| Response mode | [optional]

### Return type

null (empty response body)

### Authorization

No authorization required

### HTTP request headers

 - **Content-Type**: Not defined
 - **Accept**: Not defined

<a id="restFilesIdActionsPermanentDelete"></a>
# **restFilesIdActionsPermanentDelete**
> restFilesIdActionsPermanentDelete(id)

Permanently delete a file

Permanently delete the specified file. This file will no longer be accessible.

### Example
```kotlin
// Import classes:
//import org.openapitools.client.infrastructure.*
//import org.openapitools.client.models.*

val apiInstance = FilesApi()
val id : kotlin.String = id_example // kotlin.String | ID of the file
try {
    apiInstance.restFilesIdActionsPermanentDelete(id)
} catch (e: ClientException) {
    println("4xx response calling FilesApi#restFilesIdActionsPermanentDelete")
    e.printStackTrace()
} catch (e: ServerException) {
    println("5xx response calling FilesApi#restFilesIdActionsPermanentDelete")
    e.printStackTrace()
}
```

### Parameters

Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **id** | **kotlin.String**| ID of the file |

### Return type

null (empty response body)

### Authorization

No authorization required

### HTTP request headers

 - **Content-Type**: Not defined
 - **Accept**: Not defined

<a id="restFilesIdActionsPushDelete"></a>
# **restFilesIdActionsPushDelete**
> restFilesIdActionsPushDelete(id, returnEntity, mode)

Un-Push file

Un-Pushing file deletes this file from all folder members sync list.

### Example
```kotlin
// Import classes:
//import org.openapitools.client.infrastructure.*
//import org.openapitools.client.models.*

val apiInstance = FilesApi()
val id : kotlin.String = id_example // kotlin.String | File id
val returnEntity : kotlin.Boolean = true // kotlin.Boolean | Return information about newly created entity
val mode : kotlin.String = mode_example // kotlin.String | Response mode
try {
    apiInstance.restFilesIdActionsPushDelete(id, returnEntity, mode)
} catch (e: ClientException) {
    println("4xx response calling FilesApi#restFilesIdActionsPushDelete")
    e.printStackTrace()
} catch (e: ServerException) {
    println("5xx response calling FilesApi#restFilesIdActionsPushDelete")
    e.printStackTrace()
}
```

### Parameters

Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **id** | **kotlin.String**| File id |
 **returnEntity** | **kotlin.Boolean**| Return information about newly created entity | [optional]
 **mode** | **kotlin.String**| Response mode | [optional]

### Return type

null (empty response body)

### Authorization

No authorization required

### HTTP request headers

 - **Content-Type**: Not defined
 - **Accept**: Not defined

<a id="restFilesIdActionsPushPost"></a>
# **restFilesIdActionsPushPost**
> restFilesIdActionsPushPost(id, returnEntity, mode)

Push file to mobile sync list

Set file as mobile sync item for all folder members.

### Example
```kotlin
// Import classes:
//import org.openapitools.client.infrastructure.*
//import org.openapitools.client.models.*

val apiInstance = FilesApi()
val id : kotlin.String = id_example // kotlin.String | ID of the file
val returnEntity : kotlin.Boolean = true // kotlin.Boolean | Return information about newly created entity
val mode : kotlin.String = mode_example // kotlin.String | Response mode
try {
    apiInstance.restFilesIdActionsPushPost(id, returnEntity, mode)
} catch (e: ClientException) {
    println("4xx response calling FilesApi#restFilesIdActionsPushPost")
    e.printStackTrace()
} catch (e: ServerException) {
    println("5xx response calling FilesApi#restFilesIdActionsPushPost")
    e.printStackTrace()
}
```

### Parameters

Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **id** | **kotlin.String**| ID of the file |
 **returnEntity** | **kotlin.Boolean**| Return information about newly created entity | [optional]
 **mode** | **kotlin.String**| Response mode | [optional]

### Return type

null (empty response body)

### Authorization

No authorization required

### HTTP request headers

 - **Content-Type**: Not defined
 - **Accept**: Not defined

<a id="restFilesIdActionsRecoverPatch"></a>
# **restFilesIdActionsRecoverPatch**
> restFilesIdActionsRecoverPatch(id, returnEntity, mode)

Recovers deleted file.

Recover deleted file by its ID. This marks an already deleted file as not deleted.

### Example
```kotlin
// Import classes:
//import org.openapitools.client.infrastructure.*
//import org.openapitools.client.models.*

val apiInstance = FilesApi()
val id : kotlin.String = id_example // kotlin.String | ID of the file
val returnEntity : kotlin.Boolean = true // kotlin.Boolean | Return information about newly created entity
val mode : kotlin.String = mode_example // kotlin.String | Response mode
try {
    apiInstance.restFilesIdActionsRecoverPatch(id, returnEntity, mode)
} catch (e: ClientException) {
    println("4xx response calling FilesApi#restFilesIdActionsRecoverPatch")
    e.printStackTrace()
} catch (e: ServerException) {
    println("5xx response calling FilesApi#restFilesIdActionsRecoverPatch")
    e.printStackTrace()
}
```

### Parameters

Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **id** | **kotlin.String**| ID of the file |
 **returnEntity** | **kotlin.Boolean**| Return information about newly created entity | [optional]
 **mode** | **kotlin.String**| Response mode | [optional]

### Return type

null (empty response body)

### Authorization

No authorization required

### HTTP request headers

 - **Content-Type**: Not defined
 - **Accept**: Not defined

<a id="restFilesIdActionsReturnPatch"></a>
# **restFilesIdActionsReturnPatch**
> restFilesIdActionsReturnPatch(id, returnEntity, mode)

Returns file to EC source

Returns file to EC source

### Example
```kotlin
// Import classes:
//import org.openapitools.client.infrastructure.*
//import org.openapitools.client.models.*

val apiInstance = FilesApi()
val id : kotlin.String = id_example // kotlin.String | Object ID of the file
val returnEntity : kotlin.Boolean = true // kotlin.Boolean | Return information about newly created entity
val mode : kotlin.String = mode_example // kotlin.String | Response mode
try {
    apiInstance.restFilesIdActionsReturnPatch(id, returnEntity, mode)
} catch (e: ClientException) {
    println("4xx response calling FilesApi#restFilesIdActionsReturnPatch")
    e.printStackTrace()
} catch (e: ServerException) {
    println("5xx response calling FilesApi#restFilesIdActionsReturnPatch")
    e.printStackTrace()
}
```

### Parameters

Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **id** | **kotlin.String**| Object ID of the file |
 **returnEntity** | **kotlin.Boolean**| Return information about newly created entity | [optional]
 **mode** | **kotlin.String**| Response mode | [optional]

### Return type

null (empty response body)

### Authorization

No authorization required

### HTTP request headers

 - **Content-Type**: Not defined
 - **Accept**: Not defined

<a id="restFilesIdActionsScanPost"></a>
# **restFilesIdActionsScanPost**
> restFilesIdActionsScanPost(id, returnEntity, mode)

Triggers on demand AV/DLP file scan.

Attempts to trigger an AV/DLP scan on requested file.

### Example
```kotlin
// Import classes:
//import org.openapitools.client.infrastructure.*
//import org.openapitools.client.models.*

val apiInstance = FilesApi()
val id : kotlin.String = id_example // kotlin.String | ID of the file
val returnEntity : kotlin.Boolean = true // kotlin.Boolean | Return information about newly created entity
val mode : kotlin.String = mode_example // kotlin.String | Response mode
try {
    apiInstance.restFilesIdActionsScanPost(id, returnEntity, mode)
} catch (e: ClientException) {
    println("4xx response calling FilesApi#restFilesIdActionsScanPost")
    e.printStackTrace()
} catch (e: ServerException) {
    println("5xx response calling FilesApi#restFilesIdActionsScanPost")
    e.printStackTrace()
}
```

### Parameters

Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **id** | **kotlin.String**| ID of the file |
 **returnEntity** | **kotlin.Boolean**| Return information about newly created entity | [optional]
 **mode** | **kotlin.String**| Response mode | [optional]

### Return type

null (empty response body)

### Authorization

No authorization required

### HTTP request headers

 - **Content-Type**: Not defined
 - **Accept**: Not defined

<a id="restFilesIdActionsUnlockPatch"></a>
# **restFilesIdActionsUnlockPatch**
> restFilesIdActionsUnlockPatch(id, returnEntity, mode)

Unlocks the file by its ID

Unlock the given file.                   This will allow other users in the folder to upload a new version of the file.

### Example
```kotlin
// Import classes:
//import org.openapitools.client.infrastructure.*
//import org.openapitools.client.models.*

val apiInstance = FilesApi()
val id : kotlin.String = id_example // kotlin.String | ID of the file
val returnEntity : kotlin.Boolean = true // kotlin.Boolean | Return information about newly created entity
val mode : kotlin.String = mode_example // kotlin.String | Response mode
try {
    apiInstance.restFilesIdActionsUnlockPatch(id, returnEntity, mode)
} catch (e: ClientException) {
    println("4xx response calling FilesApi#restFilesIdActionsUnlockPatch")
    e.printStackTrace()
} catch (e: ServerException) {
    println("5xx response calling FilesApi#restFilesIdActionsUnlockPatch")
    e.printStackTrace()
}
```

### Parameters

Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **id** | **kotlin.String**| ID of the file |
 **returnEntity** | **kotlin.Boolean**| Return information about newly created entity | [optional]
 **mode** | **kotlin.String**| Response mode | [optional]

### Return type

null (empty response body)

### Authorization

No authorization required

### HTTP request headers

 - **Content-Type**: Not defined
 - **Accept**: Not defined

<a id="restFilesIdCommentsGet"></a>
# **restFilesIdCommentsGet**
> kotlin.collections.List&lt;Comment&gt; restFilesIdCommentsGet(id, parentId, parentIdColonIn, userId, userIdColonIn, created, createdColonGt, createdColonGte, createdColonLt, createdColonLte, modified, modifiedColonGt, modifiedColonGte, modifiedColonLt, modifiedColonLte, contentsColonContains, orderBy, offset, limit, with, mode)

Get Comments for a file

Returns all comments for a file

### Example
```kotlin
// Import classes:
//import org.openapitools.client.infrastructure.*
//import org.openapitools.client.models.*

val apiInstance = FilesApi()
val id : kotlin.String = id_example // kotlin.String | File object ID of the comments to retrieve
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
    val result : kotlin.collections.List<Comment> = apiInstance.restFilesIdCommentsGet(id, parentId, parentIdColonIn, userId, userIdColonIn, created, createdColonGt, createdColonGte, createdColonLt, createdColonLte, modified, modifiedColonGt, modifiedColonGte, modifiedColonLt, modifiedColonLte, contentsColonContains, orderBy, offset, limit, with, mode)
    println(result)
} catch (e: ClientException) {
    println("4xx response calling FilesApi#restFilesIdCommentsGet")
    e.printStackTrace()
} catch (e: ServerException) {
    println("5xx response calling FilesApi#restFilesIdCommentsGet")
    e.printStackTrace()
}
```

### Parameters

Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **id** | **kotlin.String**| File object ID of the comments to retrieve |
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

<a id="restFilesIdCommentsPost"></a>
# **restFilesIdCommentsPost**
> restFilesIdCommentsPost(id, body, returnEntity, mode)

Create a Comment on a file

Create a Comment on a file.

### Example
```kotlin
// Import classes:
//import org.openapitools.client.infrastructure.*
//import org.openapitools.client.models.*

val apiInstance = FilesApi()
val id : kotlin.String = id_example // kotlin.String | Object ID of the file being commented on
val body : CommentPost =  // CommentPost | The comment details
val returnEntity : kotlin.Boolean = true // kotlin.Boolean | Return information about newly created entity
val mode : kotlin.String = mode_example // kotlin.String | Response mode
try {
    apiInstance.restFilesIdCommentsPost(id, body, returnEntity, mode)
} catch (e: ClientException) {
    println("4xx response calling FilesApi#restFilesIdCommentsPost")
    e.printStackTrace()
} catch (e: ServerException) {
    println("5xx response calling FilesApi#restFilesIdCommentsPost")
    e.printStackTrace()
}
```

### Parameters

Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **id** | **kotlin.String**| Object ID of the file being commented on |
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

<a id="restFilesIdContentGet"></a>
# **restFilesIdContentGet**
> org.openapitools.client.infrastructure.OctetByteArray restFilesIdContentGet(id)

Download a file

Download a file

### Example
```kotlin
// Import classes:
//import org.openapitools.client.infrastructure.*
//import org.openapitools.client.models.*

val apiInstance = FilesApi()
val id : kotlin.String = id_example // kotlin.String | The ID of the entity
try {
    val result : org.openapitools.client.infrastructure.OctetByteArray = apiInstance.restFilesIdContentGet(id)
    println(result)
} catch (e: ClientException) {
    println("4xx response calling FilesApi#restFilesIdContentGet")
    e.printStackTrace()
} catch (e: ServerException) {
    println("5xx response calling FilesApi#restFilesIdContentGet")
    e.printStackTrace()
}
```

### Parameters

Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **id** | **kotlin.String**| The ID of the entity |

### Return type

[**org.openapitools.client.infrastructure.OctetByteArray**](org.openapitools.client.infrastructure.OctetByteArray.md)

### Authorization

No authorization required

### HTTP request headers

 - **Content-Type**: Not defined
 - **Accept**: */*

<a id="restFilesIdDelete"></a>
# **restFilesIdDelete**
> restFilesIdDelete(id)

Mark file for deletion.

Marks a file with the given ID as deleted. This file will be cleaned up                        after x days as set in the admin.

### Example
```kotlin
// Import classes:
//import org.openapitools.client.infrastructure.*
//import org.openapitools.client.models.*

val apiInstance = FilesApi()
val id : kotlin.String = id_example // kotlin.String | ID of the file
try {
    apiInstance.restFilesIdDelete(id)
} catch (e: ClientException) {
    println("4xx response calling FilesApi#restFilesIdDelete")
    e.printStackTrace()
} catch (e: ServerException) {
    println("5xx response calling FilesApi#restFilesIdDelete")
    e.printStackTrace()
}
```

### Parameters

Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **id** | **kotlin.String**| ID of the file |

### Return type

null (empty response body)

### Authorization

No authorization required

### HTTP request headers

 - **Content-Type**: Not defined
 - **Accept**: Not defined

<a id="restFilesIdExternalEditGet"></a>
# **restFilesIdExternalEditGet**
> RefreshToken restFilesIdExternalEditGet(id, with, mode)

Get access token for external file edit.

Retrieve refresh token for external file edit.

### Example
```kotlin
// Import classes:
//import org.openapitools.client.infrastructure.*
//import org.openapitools.client.models.*

val apiInstance = FilesApi()
val id : kotlin.String = id_example // kotlin.String | ID of the file
val with : kotlin.String = with_example // kotlin.String | With parameters
val mode : kotlin.String = mode_example // kotlin.String | Response mode
try {
    val result : RefreshToken = apiInstance.restFilesIdExternalEditGet(id, with, mode)
    println(result)
} catch (e: ClientException) {
    println("4xx response calling FilesApi#restFilesIdExternalEditGet")
    e.printStackTrace()
} catch (e: ServerException) {
    println("5xx response calling FilesApi#restFilesIdExternalEditGet")
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

[**RefreshToken**](RefreshToken.md)

### Authorization

No authorization required

### HTTP request headers

 - **Content-Type**: Not defined
 - **Accept**: */*

<a id="restFilesIdGet"></a>
# **restFilesIdGet**
> org.openapitools.client.infrastructure.OctetByteArray restFilesIdGet(id, mode, with, returnEntity)

Retrieve information about the file specified.

Retrieve information about the file specified.

### Example
```kotlin
// Import classes:
//import org.openapitools.client.infrastructure.*
//import org.openapitools.client.models.*

val apiInstance = FilesApi()
val id : kotlin.String = id_example // kotlin.String | The ID of the entity
val mode : kotlin.String = mode_example // kotlin.String | 
val with : kotlin.String = with_example // kotlin.String | 
val returnEntity : kotlin.Boolean = true // kotlin.Boolean | 
try {
    val result : org.openapitools.client.infrastructure.OctetByteArray = apiInstance.restFilesIdGet(id, mode, with, returnEntity)
    println(result)
} catch (e: ClientException) {
    println("4xx response calling FilesApi#restFilesIdGet")
    e.printStackTrace()
} catch (e: ServerException) {
    println("5xx response calling FilesApi#restFilesIdGet")
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

[**org.openapitools.client.infrastructure.OctetByteArray**](org.openapitools.client.infrastructure.OctetByteArray.md)

### Authorization

No authorization required

### HTTP request headers

 - **Content-Type**: Not defined
 - **Accept**: */*

<a id="restFilesIdMembersDelete"></a>
# **restFilesIdMembersDelete**
> restFilesIdMembersDelete(id)

Delete all members in file

Delete member from the file

### Example
```kotlin
// Import classes:
//import org.openapitools.client.infrastructure.*
//import org.openapitools.client.models.*

val apiInstance = FilesApi()
val id : kotlin.String = id_example // kotlin.String | The ID of the entity
try {
    apiInstance.restFilesIdMembersDelete(id)
} catch (e: ClientException) {
    println("4xx response calling FilesApi#restFilesIdMembersDelete")
    e.printStackTrace()
} catch (e: ServerException) {
    println("5xx response calling FilesApi#restFilesIdMembersDelete")
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

<a id="restFilesIdMembersGet"></a>
# **restFilesIdMembersGet**
> Members restFilesIdMembersGet(id, orderBy, groupIdColonIn, with, roleId, limit, mode, userId, userIdColonIn, roleIdColonIn, type, offset, groupId, returnEntity)

List of members in with access to the file

Returns a list of members in with access to the file

### Example
```kotlin
// Import classes:
//import org.openapitools.client.infrastructure.*
//import org.openapitools.client.models.*

val apiInstance = FilesApi()
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
    val result : Members = apiInstance.restFilesIdMembersGet(id, orderBy, groupIdColonIn, with, roleId, limit, mode, userId, userIdColonIn, roleIdColonIn, type, offset, groupId, returnEntity)
    println(result)
} catch (e: ClientException) {
    println("4xx response calling FilesApi#restFilesIdMembersGet")
    e.printStackTrace()
} catch (e: ServerException) {
    println("5xx response calling FilesApi#restFilesIdMembersGet")
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

<a id="restFilesIdMembersLdapGroupGet"></a>
# **restFilesIdMembersLdapGroupGet**
> kotlin.collections.List&lt;MemberGroup&gt; restFilesIdMembersLdapGroupGet(id, groupId, groupIdColonIn, roleId, roleIdColonIn, orderBy, offset, limit, with, mode)

List members

Returns a list of group members in with access to the file

### Example
```kotlin
// Import classes:
//import org.openapitools.client.infrastructure.*
//import org.openapitools.client.models.*

val apiInstance = FilesApi()
val id : kotlin.String = id_example // kotlin.String | ID of the file
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
    val result : kotlin.collections.List<MemberGroup> = apiInstance.restFilesIdMembersLdapGroupGet(id, groupId, groupIdColonIn, roleId, roleIdColonIn, orderBy, offset, limit, with, mode)
    println(result)
} catch (e: ClientException) {
    println("4xx response calling FilesApi#restFilesIdMembersLdapGroupGet")
    e.printStackTrace()
} catch (e: ServerException) {
    println("5xx response calling FilesApi#restFilesIdMembersLdapGroupGet")
    e.printStackTrace()
}
```

### Parameters

Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **id** | **kotlin.String**| ID of the file |
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

<a id="restFilesIdMembersLdapGroupLdapGroupIdGet"></a>
# **restFilesIdMembersLdapGroupLdapGroupIdGet**
> Member restFilesIdMembersLdapGroupLdapGroupIdGet(id, ldapGroupId, with, mode)

display group member

Display the specified group member in the file

### Example
```kotlin
// Import classes:
//import org.openapitools.client.infrastructure.*
//import org.openapitools.client.models.*

val apiInstance = FilesApi()
val id : kotlin.String = id_example // kotlin.String | ID of the file
val ldapGroupId : kotlin.Int = 56 // kotlin.Int | id of the member
val with : kotlin.String = with_example // kotlin.String | With parameters
val mode : kotlin.String = mode_example // kotlin.String | Response mode
try {
    val result : Member = apiInstance.restFilesIdMembersLdapGroupLdapGroupIdGet(id, ldapGroupId, with, mode)
    println(result)
} catch (e: ClientException) {
    println("4xx response calling FilesApi#restFilesIdMembersLdapGroupLdapGroupIdGet")
    e.printStackTrace()
} catch (e: ServerException) {
    println("5xx response calling FilesApi#restFilesIdMembersLdapGroupLdapGroupIdGet")
    e.printStackTrace()
}
```

### Parameters

Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **id** | **kotlin.String**| ID of the file |
 **ldapGroupId** | **kotlin.Int**| id of the member |
 **with** | **kotlin.String**| With parameters | [optional]
 **mode** | **kotlin.String**| Response mode | [optional]

### Return type

[**Member**](Member.md)

### Authorization

No authorization required

### HTTP request headers

 - **Content-Type**: Not defined
 - **Accept**: */*

<a id="restFilesIdMembersMeDelete"></a>
# **restFilesIdMembersMeDelete**
> restFilesIdMembersMeDelete(id)

Leave as the file member

Leave as the file member

### Example
```kotlin
// Import classes:
//import org.openapitools.client.infrastructure.*
//import org.openapitools.client.models.*

val apiInstance = FilesApi()
val id : kotlin.String = id_example // kotlin.String | The ID of the entity
try {
    apiInstance.restFilesIdMembersMeDelete(id)
} catch (e: ClientException) {
    println("4xx response calling FilesApi#restFilesIdMembersMeDelete")
    e.printStackTrace()
} catch (e: ServerException) {
    println("5xx response calling FilesApi#restFilesIdMembersMeDelete")
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

<a id="restFilesIdMembersMemberUserIdDelete"></a>
# **restFilesIdMembersMemberUserIdDelete**
> restFilesIdMembersMemberUserIdDelete(id, memberUserId)

Delete member from the file

Delete member from the file

### Example
```kotlin
// Import classes:
//import org.openapitools.client.infrastructure.*
//import org.openapitools.client.models.*

val apiInstance = FilesApi()
val id : kotlin.String = id_example // kotlin.String | The ID of the entity
val memberUserId : kotlin.String = memberUserId_example // kotlin.String | The member user ID
try {
    apiInstance.restFilesIdMembersMemberUserIdDelete(id, memberUserId)
} catch (e: ClientException) {
    println("4xx response calling FilesApi#restFilesIdMembersMemberUserIdDelete")
    e.printStackTrace()
} catch (e: ServerException) {
    println("5xx response calling FilesApi#restFilesIdMembersMemberUserIdDelete")
    e.printStackTrace()
}
```

### Parameters

Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **id** | **kotlin.String**| The ID of the entity |
 **memberUserId** | **kotlin.String**| The member user ID |

### Return type

null (empty response body)

### Authorization

No authorization required

### HTTP request headers

 - **Content-Type**: Not defined
 - **Accept**: Not defined

<a id="restFilesIdMembersMemberUserIdGet"></a>
# **restFilesIdMembersMemberUserIdGet**
> Member restFilesIdMembersMemberUserIdGet(id, memberUserId, with, mode)

display member

Display the specified member in the file

### Example
```kotlin
// Import classes:
//import org.openapitools.client.infrastructure.*
//import org.openapitools.client.models.*

val apiInstance = FilesApi()
val id : kotlin.String = id_example // kotlin.String | ID of the file
val memberUserId : kotlin.String = memberUserId_example // kotlin.String | ID of the member
val with : kotlin.String = with_example // kotlin.String | With parameters
val mode : kotlin.String = mode_example // kotlin.String | Response mode
try {
    val result : Member = apiInstance.restFilesIdMembersMemberUserIdGet(id, memberUserId, with, mode)
    println(result)
} catch (e: ClientException) {
    println("4xx response calling FilesApi#restFilesIdMembersMemberUserIdGet")
    e.printStackTrace()
} catch (e: ServerException) {
    println("5xx response calling FilesApi#restFilesIdMembersMemberUserIdGet")
    e.printStackTrace()
}
```

### Parameters

Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **id** | **kotlin.String**| ID of the file |
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

<a id="restFilesIdMembersMemberUserIdPut"></a>
# **restFilesIdMembersMemberUserIdPut**
> restFilesIdMembersMemberUserIdPut(id, memberUserId)

Update members in the file

Update members in the file

### Example
```kotlin
// Import classes:
//import org.openapitools.client.infrastructure.*
//import org.openapitools.client.models.*

val apiInstance = FilesApi()
val id : kotlin.String = id_example // kotlin.String | The ID of the entity
val memberUserId : kotlin.String = memberUserId_example // kotlin.String | The member user ID
try {
    apiInstance.restFilesIdMembersMemberUserIdPut(id, memberUserId)
} catch (e: ClientException) {
    println("4xx response calling FilesApi#restFilesIdMembersMemberUserIdPut")
    e.printStackTrace()
} catch (e: ServerException) {
    println("5xx response calling FilesApi#restFilesIdMembersMemberUserIdPut")
    e.printStackTrace()
}
```

### Parameters

Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **id** | **kotlin.String**| The ID of the entity |
 **memberUserId** | **kotlin.String**| The member user ID |

### Return type

null (empty response body)

### Authorization

No authorization required

### HTTP request headers

 - **Content-Type**: Not defined
 - **Accept**: Not defined

<a id="restFilesIdPathGet"></a>
# **restFilesIdPathGet**
> restFilesIdPathGet(id, mode)

Gets the file path by its ID

Gets the file path by its ID

### Example
```kotlin
// Import classes:
//import org.openapitools.client.infrastructure.*
//import org.openapitools.client.models.*

val apiInstance = FilesApi()
val id : kotlin.String = id_example // kotlin.String | ID of the file
val mode : kotlin.String = mode_example // kotlin.String | Response mode
try {
    apiInstance.restFilesIdPathGet(id, mode)
} catch (e: ClientException) {
    println("4xx response calling FilesApi#restFilesIdPathGet")
    e.printStackTrace()
} catch (e: ServerException) {
    println("5xx response calling FilesApi#restFilesIdPathGet")
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

<a id="restFilesIdPost"></a>
# **restFilesIdPost**
> restFilesIdPost(id, body, returnEntity, mode, clientCreated, clientModified)

upload new version

uploads new file version

### Example
```kotlin
// Import classes:
//import org.openapitools.client.infrastructure.*
//import org.openapitools.client.models.*

val apiInstance = FilesApi()
val id : kotlin.String = id_example // kotlin.String | ID of the file
val body : io.ktor.client.request.forms.InputProvider = BINARY_DATA_HERE // io.ktor.client.request.forms.InputProvider | file content
val returnEntity : kotlin.Boolean = true // kotlin.Boolean | Return information about newly created entity
val mode : kotlin.String = mode_example // kotlin.String | Response mode
val clientCreated : kotlin.String = 2013-10-20 // kotlin.String | Client created field for the file
val clientModified : kotlin.String = 2013-10-20 // kotlin.String | Client modified field for the file
try {
    apiInstance.restFilesIdPost(id, body, returnEntity, mode, clientCreated, clientModified)
} catch (e: ClientException) {
    println("4xx response calling FilesApi#restFilesIdPost")
    e.printStackTrace()
} catch (e: ServerException) {
    println("5xx response calling FilesApi#restFilesIdPost")
    e.printStackTrace()
}
```

### Parameters

Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **id** | **kotlin.String**| ID of the file |
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

<a id="restFilesIdPreviewGet"></a>
# **restFilesIdPreviewGet**
> restFilesIdPreviewGet(id)

Retrieve information about the file preview.

Retrieve information about the file preview.

### Example
```kotlin
// Import classes:
//import org.openapitools.client.infrastructure.*
//import org.openapitools.client.models.*

val apiInstance = FilesApi()
val id : kotlin.String = id_example // kotlin.String | The ID of the entity
try {
    apiInstance.restFilesIdPreviewGet(id)
} catch (e: ClientException) {
    println("4xx response calling FilesApi#restFilesIdPreviewGet")
    e.printStackTrace()
} catch (e: ServerException) {
    println("5xx response calling FilesApi#restFilesIdPreviewGet")
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

<a id="restFilesIdPut"></a>
# **restFilesIdPut**
> restFilesIdPut(id, body)

Update the details of the file specified

### Example
```kotlin
// Import classes:
//import org.openapitools.client.infrastructure.*
//import org.openapitools.client.models.*

val apiInstance = FilesApi()
val id : kotlin.String = id_example // kotlin.String | The ID of the entity
val body : FileUpdateRequest =  // FileUpdateRequest | 
try {
    apiInstance.restFilesIdPut(id, body)
} catch (e: ClientException) {
    println("4xx response calling FilesApi#restFilesIdPut")
    e.printStackTrace()
} catch (e: ServerException) {
    println("5xx response calling FilesApi#restFilesIdPut")
    e.printStackTrace()
}
```

### Parameters

Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **id** | **kotlin.String**| The ID of the entity |
 **body** | [**FileUpdateRequest**](FileUpdateRequest.md)|  |

### Return type

null (empty response body)

### Authorization

No authorization required

### HTTP request headers

 - **Content-Type**: Not defined
 - **Accept**: Not defined

<a id="restFilesIdTasksGet"></a>
# **restFilesIdTasksGet**
> kotlin.collections.List&lt;Task&gt; restFilesIdTasksGet(id, assigneeId, assigneeIdColonIn, due, dueColonGt, dueColonGte, dueColonLt, dueColonLte, parentId, parentIdColonIn, userId, userIdColonIn, created, createdColonGt, createdColonGte, createdColonLt, createdColonLte, modified, modifiedColonGt, modifiedColonGte, modifiedColonLt, modifiedColonLte, contentsColonContains, status, deleted, orderBy, offset, limit, with, mode)

Get Tasks for a file

Returns all tasks for a file

### Example
```kotlin
// Import classes:
//import org.openapitools.client.infrastructure.*
//import org.openapitools.client.models.*

val apiInstance = FilesApi()
val id : kotlin.String = id_example // kotlin.String | File object ID of the task to retrieve
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
    val result : kotlin.collections.List<Task> = apiInstance.restFilesIdTasksGet(id, assigneeId, assigneeIdColonIn, due, dueColonGt, dueColonGte, dueColonLt, dueColonLte, parentId, parentIdColonIn, userId, userIdColonIn, created, createdColonGt, createdColonGte, createdColonLt, createdColonLte, modified, modifiedColonGt, modifiedColonGte, modifiedColonLt, modifiedColonLte, contentsColonContains, status, deleted, orderBy, offset, limit, with, mode)
    println(result)
} catch (e: ClientException) {
    println("4xx response calling FilesApi#restFilesIdTasksGet")
    e.printStackTrace()
} catch (e: ServerException) {
    println("5xx response calling FilesApi#restFilesIdTasksGet")
    e.printStackTrace()
}
```

### Parameters

Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **id** | **kotlin.String**| File object ID of the task to retrieve |
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

<a id="restFilesIdTasksPost"></a>
# **restFilesIdTasksPost**
> restFilesIdTasksPost(id, body, returnEntity, mode)

Create a Task on a file

Creates a task on a file

### Example
```kotlin
// Import classes:
//import org.openapitools.client.infrastructure.*
//import org.openapitools.client.models.*

val apiInstance = FilesApi()
val id : kotlin.String = id_example // kotlin.String | Object ID of the file task is created on
val body : TaskPost =  // TaskPost | The task details
val returnEntity : kotlin.Boolean = true // kotlin.Boolean | Return information about newly created entity
val mode : kotlin.String = mode_example // kotlin.String | Response mode
try {
    apiInstance.restFilesIdTasksPost(id, body, returnEntity, mode)
} catch (e: ClientException) {
    println("4xx response calling FilesApi#restFilesIdTasksPost")
    e.printStackTrace()
} catch (e: ServerException) {
    println("5xx response calling FilesApi#restFilesIdTasksPost")
    e.printStackTrace()
}
```

### Parameters

Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **id** | **kotlin.String**| Object ID of the file task is created on |
 **body** | [**TaskPost**](TaskPost.md)| The task details |
 **returnEntity** | **kotlin.Boolean**| Return information about newly created entity | [optional]
 **mode** | **kotlin.String**| Response mode | [optional]

### Return type

null (empty response body)

### Authorization

No authorization required

### HTTP request headers

 - **Content-Type**: Not defined
 - **Accept**: Not defined

<a id="restFilesIdVersionsGet"></a>
# **restFilesIdVersionsGet**
> kotlin.collections.List&lt;Version&gt; restFilesIdVersionsGet(id, created, createdColonGt, createdColonGte, createdColonLt, createdColonLte, orderBy, offset, limit, locateId, with, mode)

List versions

Returns a list of versions for a given file

### Example
```kotlin
// Import classes:
//import org.openapitools.client.infrastructure.*
//import org.openapitools.client.models.*

val apiInstance = FilesApi()
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
    val result : kotlin.collections.List<Version> = apiInstance.restFilesIdVersionsGet(id, created, createdColonGt, createdColonGte, createdColonLt, createdColonLte, orderBy, offset, limit, locateId, with, mode)
    println(result)
} catch (e: ClientException) {
    println("4xx response calling FilesApi#restFilesIdVersionsGet")
    e.printStackTrace()
} catch (e: ServerException) {
    println("5xx response calling FilesApi#restFilesIdVersionsGet")
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

<a id="restFilesIdVersionsPost"></a>
# **restFilesIdVersionsPost**
> restFilesIdVersionsPost(id, body, returnEntity, mode)

Uploads a new file version

Uploads a new file version

### Example
```kotlin
// Import classes:
//import org.openapitools.client.infrastructure.*
//import org.openapitools.client.models.*

val apiInstance = FilesApi()
val id : kotlin.String = id_example // kotlin.String | ID of the file to replace
val body : io.ktor.client.request.forms.InputProvider = BINARY_DATA_HERE // io.ktor.client.request.forms.InputProvider | file content
val returnEntity : kotlin.Boolean = true // kotlin.Boolean | Return information about newly created entity
val mode : kotlin.String = mode_example // kotlin.String | Response mode
try {
    apiInstance.restFilesIdVersionsPost(id, body, returnEntity, mode)
} catch (e: ClientException) {
    println("4xx response calling FilesApi#restFilesIdVersionsPost")
    e.printStackTrace()
} catch (e: ServerException) {
    println("5xx response calling FilesApi#restFilesIdVersionsPost")
    e.printStackTrace()
}
```

### Parameters

Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **id** | **kotlin.String**| ID of the file to replace |
 **body** | **io.ktor.client.request.forms.InputProvider**| file content |
 **returnEntity** | **kotlin.Boolean**| Return information about newly created entity | [optional]
 **mode** | **kotlin.String**| Response mode | [optional]

### Return type

null (empty response body)

### Authorization

No authorization required

### HTTP request headers

 - **Content-Type**: multipart/form-data
 - **Accept**: Not defined

<a id="restFilesIdVersionsVersionIdActionsPromotePost"></a>
# **restFilesIdVersionsVersionIdActionsPromotePost**
> restFilesIdVersionsVersionIdActionsPromotePost(id, versionId, returnEntity, mode)

promote specified file version

promote version

### Example
```kotlin
// Import classes:
//import org.openapitools.client.infrastructure.*
//import org.openapitools.client.models.*

val apiInstance = FilesApi()
val id : kotlin.String = id_example // kotlin.String | Object id of file to promote version from
val versionId : kotlin.String = versionId_example // kotlin.String | version ID to promote to version 0
val returnEntity : kotlin.Boolean = true // kotlin.Boolean | Return information about newly created entity
val mode : kotlin.String = mode_example // kotlin.String | Response mode
try {
    apiInstance.restFilesIdVersionsVersionIdActionsPromotePost(id, versionId, returnEntity, mode)
} catch (e: ClientException) {
    println("4xx response calling FilesApi#restFilesIdVersionsVersionIdActionsPromotePost")
    e.printStackTrace()
} catch (e: ServerException) {
    println("5xx response calling FilesApi#restFilesIdVersionsVersionIdActionsPromotePost")
    e.printStackTrace()
}
```

### Parameters

Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **id** | **kotlin.String**| Object id of file to promote version from |
 **versionId** | **kotlin.String**| version ID to promote to version 0 |
 **returnEntity** | **kotlin.Boolean**| Return information about newly created entity | [optional]
 **mode** | **kotlin.String**| Response mode | [optional]

### Return type

null (empty response body)

### Authorization

No authorization required

### HTTP request headers

 - **Content-Type**: Not defined
 - **Accept**: Not defined

<a id="restFilesIdVersionsVersionIdActionsScanPost"></a>
# **restFilesIdVersionsVersionIdActionsScanPost**
> restFilesIdVersionsVersionIdActionsScanPost(id, versionId, returnEntity, mode)

Triggers on demand AV/DLP file scan.

Attempts to trigger an AV/DLP scan on requested file version.

### Example
```kotlin
// Import classes:
//import org.openapitools.client.infrastructure.*
//import org.openapitools.client.models.*

val apiInstance = FilesApi()
val id : kotlin.String = id_example // kotlin.String | Object ID of the file to scan
val versionId : kotlin.String = versionId_example // kotlin.String | Version ID of the file to scan
val returnEntity : kotlin.Boolean = true // kotlin.Boolean | Return information about newly created entity
val mode : kotlin.String = mode_example // kotlin.String | Response mode
try {
    apiInstance.restFilesIdVersionsVersionIdActionsScanPost(id, versionId, returnEntity, mode)
} catch (e: ClientException) {
    println("4xx response calling FilesApi#restFilesIdVersionsVersionIdActionsScanPost")
    e.printStackTrace()
} catch (e: ServerException) {
    println("5xx response calling FilesApi#restFilesIdVersionsVersionIdActionsScanPost")
    e.printStackTrace()
}
```

### Parameters

Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **id** | **kotlin.String**| Object ID of the file to scan |
 **versionId** | **kotlin.String**| Version ID of the file to scan |
 **returnEntity** | **kotlin.Boolean**| Return information about newly created entity | [optional]
 **mode** | **kotlin.String**| Response mode | [optional]

### Return type

null (empty response body)

### Authorization

No authorization required

### HTTP request headers

 - **Content-Type**: Not defined
 - **Accept**: Not defined

<a id="restFilesIdVersionsVersionIdContentGet"></a>
# **restFilesIdVersionsVersionIdContentGet**
> restFilesIdVersionsVersionIdContentGet(id, versionId, range)

download specified version

download specified version

### Example
```kotlin
// Import classes:
//import org.openapitools.client.infrastructure.*
//import org.openapitools.client.models.*

val apiInstance = FilesApi()
val id : kotlin.String = id_example // kotlin.String | ID of the file
val versionId : kotlin.String = versionId_example // kotlin.String | version ID for which to retrieve content
val range : kotlin.String = range_example // kotlin.String | Bytes range to retrieve. Example: bytes=0-1024
try {
    apiInstance.restFilesIdVersionsVersionIdContentGet(id, versionId, range)
} catch (e: ClientException) {
    println("4xx response calling FilesApi#restFilesIdVersionsVersionIdContentGet")
    e.printStackTrace()
} catch (e: ServerException) {
    println("5xx response calling FilesApi#restFilesIdVersionsVersionIdContentGet")
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

<a id="restFilesIdVersionsVersionIdDelete"></a>
# **restFilesIdVersionsVersionIdDelete**
> restFilesIdVersionsVersionIdDelete(id, versionId)

Deletes the specified file version

Delete version

### Example
```kotlin
// Import classes:
//import org.openapitools.client.infrastructure.*
//import org.openapitools.client.models.*

val apiInstance = FilesApi()
val id : kotlin.String = id_example // kotlin.String | Object id of file to delete version from
val versionId : kotlin.String = versionId_example // kotlin.String | version ID to delete
try {
    apiInstance.restFilesIdVersionsVersionIdDelete(id, versionId)
} catch (e: ClientException) {
    println("4xx response calling FilesApi#restFilesIdVersionsVersionIdDelete")
    e.printStackTrace()
} catch (e: ServerException) {
    println("5xx response calling FilesApi#restFilesIdVersionsVersionIdDelete")
    e.printStackTrace()
}
```

### Parameters

Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **id** | **kotlin.String**| Object id of file to delete version from |
 **versionId** | **kotlin.String**| version ID to delete |

### Return type

null (empty response body)

### Authorization

No authorization required

### HTTP request headers

 - **Content-Type**: Not defined
 - **Accept**: Not defined

<a id="restFilesIdVersionsVersionIdGet"></a>
# **restFilesIdVersionsVersionIdGet**
> Version restFilesIdVersionsVersionIdGet(id, versionId)

Get specified version

Returns the specified version of a file

### Example
```kotlin
// Import classes:
//import org.openapitools.client.infrastructure.*
//import org.openapitools.client.models.*

val apiInstance = FilesApi()
val id : kotlin.String = id_example // kotlin.String | Object id of file to retrieve versions for
val versionId : kotlin.String = versionId_example // kotlin.String | version ID
try {
    val result : Version = apiInstance.restFilesIdVersionsVersionIdGet(id, versionId)
    println(result)
} catch (e: ClientException) {
    println("4xx response calling FilesApi#restFilesIdVersionsVersionIdGet")
    e.printStackTrace()
} catch (e: ServerException) {
    println("5xx response calling FilesApi#restFilesIdVersionsVersionIdGet")
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

<a id="restFilesIdVersionsVersionIdPreviewGet"></a>
# **restFilesIdVersionsVersionIdPreviewGet**
> Preview restFilesIdVersionsVersionIdPreviewGet(id, versionId)

Retrieve information about the file preview.

Retrieve information about the file preview.

### Example
```kotlin
// Import classes:
//import org.openapitools.client.infrastructure.*
//import org.openapitools.client.models.*

val apiInstance = FilesApi()
val id : kotlin.String = id_example // kotlin.String | Object id of file to retrieve version preview for
val versionId : kotlin.String = versionId_example // kotlin.String | version ID
try {
    val result : Preview = apiInstance.restFilesIdVersionsVersionIdPreviewGet(id, versionId)
    println(result)
} catch (e: ClientException) {
    println("4xx response calling FilesApi#restFilesIdVersionsVersionIdPreviewGet")
    e.printStackTrace()
} catch (e: ServerException) {
    println("5xx response calling FilesApi#restFilesIdVersionsVersionIdPreviewGet")
    e.printStackTrace()
}
```

### Parameters

Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **id** | **kotlin.String**| Object id of file to retrieve version preview for |
 **versionId** | **kotlin.String**| version ID |

### Return type

[**Preview**](Preview.md)

### Authorization

No authorization required

### HTTP request headers

 - **Content-Type**: Not defined
 - **Accept**: */*

<a id="restFilesMembersPost"></a>
# **restFilesMembersPost**
> FileAddMembers restFilesMembersPost(body, partialSuccess, downgradeNested, with, mode, updateIfExists, returnEntity)

Add multiple members

Share files to multiple users

### Example
```kotlin
// Import classes:
//import org.openapitools.client.infrastructure.*
//import org.openapitools.client.models.*

val apiInstance = FilesApi()
val body : FileMembersPostRequest =  // FileMembersPostRequest | 
val partialSuccess : kotlin.Boolean = true // kotlin.Boolean | 
val downgradeNested : kotlin.Boolean = true // kotlin.Boolean | 
val with : kotlin.String = with_example // kotlin.String | 
val mode : kotlin.String = mode_example // kotlin.String | 
val updateIfExists : kotlin.Boolean = true // kotlin.Boolean | 
val returnEntity : kotlin.Boolean = true // kotlin.Boolean | 
try {
    val result : FileAddMembers = apiInstance.restFilesMembersPost(body, partialSuccess, downgradeNested, with, mode, updateIfExists, returnEntity)
    println(result)
} catch (e: ClientException) {
    println("4xx response calling FilesApi#restFilesMembersPost")
    e.printStackTrace()
} catch (e: ServerException) {
    println("5xx response calling FilesApi#restFilesMembersPost")
    e.printStackTrace()
}
```

### Parameters

Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **body** | [**FileMembersPostRequest**](FileMembersPostRequest.md)|  |
 **partialSuccess** | **kotlin.Boolean**|  | [optional]
 **downgradeNested** | **kotlin.Boolean**|  | [optional]
 **with** | **kotlin.String**|  | [optional]
 **mode** | **kotlin.String**|  | [optional]
 **updateIfExists** | **kotlin.Boolean**|  | [optional]
 **returnEntity** | **kotlin.Boolean**|  | [optional]

### Return type

[**FileAddMembers**](FileAddMembers.md)

### Authorization

No authorization required

### HTTP request headers

 - **Content-Type**: Not defined
 - **Accept**: */*

<a id="restFilesPreviewSupportGet"></a>
# **restFilesPreviewSupportGet**
> FilePreviewSupport restFilesPreviewSupportGet(idColonIn)

Check mime type before send

Check mime type before send

### Example
```kotlin
// Import classes:
//import org.openapitools.client.infrastructure.*
//import org.openapitools.client.models.*

val apiInstance = FilesApi()
val idColonIn : kotlin.collections.List<kotlin.String> =  // kotlin.collections.List<kotlin.String> | 
try {
    val result : FilePreviewSupport = apiInstance.restFilesPreviewSupportGet(idColonIn)
    println(result)
} catch (e: ClientException) {
    println("4xx response calling FilesApi#restFilesPreviewSupportGet")
    e.printStackTrace()
} catch (e: ServerException) {
    println("5xx response calling FilesApi#restFilesPreviewSupportGet")
    e.printStackTrace()
}
```

### Parameters

Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **idColonIn** | [**kotlin.collections.List&lt;kotlin.String&gt;**](kotlin.String.md)|  |

### Return type

[**FilePreviewSupport**](FilePreviewSupport.md)

### Authorization

No authorization required

### HTTP request headers

 - **Content-Type**: Not defined
 - **Accept**: */*

<a id="restFilesSharedGet"></a>
# **restFilesSharedGet**
> kotlin.collections.List&lt;org.openapitools.client.infrastructure.OctetByteArray&gt; restFilesSharedGet(orderType, with, limit, mode, orderBy, offset, returnEntity)

Return user&#39;s all shared files and permissions

Return user&#39;s all shared files and permissions

### Example
```kotlin
// Import classes:
//import org.openapitools.client.infrastructure.*
//import org.openapitools.client.models.*

val apiInstance = FilesApi()
val orderType : kotlin.String = orderType_example // kotlin.String | 
val with : kotlin.String = with_example // kotlin.String | 
val limit : kotlin.Int = 56 // kotlin.Int | 
val mode : kotlin.String = mode_example // kotlin.String | 
val orderBy : kotlin.String = orderBy_example // kotlin.String | 
val offset : kotlin.Int = 56 // kotlin.Int | 
val returnEntity : kotlin.Boolean = true // kotlin.Boolean | 
try {
    val result : kotlin.collections.List<org.openapitools.client.infrastructure.OctetByteArray> = apiInstance.restFilesSharedGet(orderType, with, limit, mode, orderBy, offset, returnEntity)
    println(result)
} catch (e: ClientException) {
    println("4xx response calling FilesApi#restFilesSharedGet")
    e.printStackTrace()
} catch (e: ServerException) {
    println("5xx response calling FilesApi#restFilesSharedGet")
    e.printStackTrace()
}
```

### Parameters

Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **orderType** | **kotlin.String**|  | [optional]
 **with** | **kotlin.String**|  | [optional]
 **limit** | **kotlin.Int**|  | [optional]
 **mode** | **kotlin.String**|  | [optional]
 **orderBy** | **kotlin.String**|  | [optional]
 **offset** | **kotlin.Int**|  | [optional]
 **returnEntity** | **kotlin.Boolean**|  | [optional]

### Return type

[**kotlin.collections.List&lt;org.openapitools.client.infrastructure.OctetByteArray&gt;**](org.openapitools.client.infrastructure.OctetByteArray.md)

### Authorization

No authorization required

### HTTP request headers

 - **Content-Type**: Not defined
 - **Accept**: */*

<a id="restFoldersIdActionsFileBase64EncodedPost"></a>
# **restFoldersIdActionsFileBase64EncodedPost**
> restFoldersIdActionsFileBase64EncodedPost(id, body, returnEntity, mode)

upload  base64 encoded content

uploads base64 encoded file content to a folder

### Example
```kotlin
// Import classes:
//import org.openapitools.client.infrastructure.*
//import org.openapitools.client.models.*

val apiInstance = FilesApi()
val id : kotlin.String = id_example // kotlin.String | ID of the folder
val body : ContentPost =  // ContentPost | File information
val returnEntity : kotlin.Boolean = true // kotlin.Boolean | Return information about newly created entity
val mode : kotlin.String = mode_example // kotlin.String | Response mode
try {
    apiInstance.restFoldersIdActionsFileBase64EncodedPost(id, body, returnEntity, mode)
} catch (e: ClientException) {
    println("4xx response calling FilesApi#restFoldersIdActionsFileBase64EncodedPost")
    e.printStackTrace()
} catch (e: ServerException) {
    println("5xx response calling FilesApi#restFoldersIdActionsFileBase64EncodedPost")
    e.printStackTrace()
}
```

### Parameters

Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **id** | **kotlin.String**| ID of the folder |
 **body** | [**ContentPost**](ContentPost.md)| File information |
 **returnEntity** | **kotlin.Boolean**| Return information about newly created entity | [optional]
 **mode** | **kotlin.String**| Response mode | [optional]

### Return type

null (empty response body)

### Authorization

No authorization required

### HTTP request headers

 - **Content-Type**: Not defined
 - **Accept**: Not defined

<a id="restFoldersIdActionsFilePost"></a>
# **restFoldersIdActionsFilePost**
> restFoldersIdActionsFilePost(id, body, returnEntity, mode, clientCreated, clientModified, disableAutoVersion, note)

upload content

uploads file content to a folder

### Example
```kotlin
// Import classes:
//import org.openapitools.client.infrastructure.*
//import org.openapitools.client.models.*

val apiInstance = FilesApi()
val id : kotlin.String = id_example // kotlin.String | ID of the folder
val body : io.ktor.client.request.forms.InputProvider = BINARY_DATA_HERE // io.ktor.client.request.forms.InputProvider | file content
val returnEntity : kotlin.Boolean = true // kotlin.Boolean | Return information about newly created entity
val mode : kotlin.String = mode_example // kotlin.String | Response mode
val clientCreated : kotlin.String = 2013-10-20 // kotlin.String | Client created field for the file
val clientModified : kotlin.String = 2013-10-20 // kotlin.String | Client modified field for the file
val disableAutoVersion : kotlin.Boolean = true // kotlin.Boolean | Indicates whether Client would like to save file as new version
val note : kotlin.Boolean = true // kotlin.Boolean | Indicates whether the file is note
try {
    apiInstance.restFoldersIdActionsFilePost(id, body, returnEntity, mode, clientCreated, clientModified, disableAutoVersion, note)
} catch (e: ClientException) {
    println("4xx response calling FilesApi#restFoldersIdActionsFilePost")
    e.printStackTrace()
} catch (e: ServerException) {
    println("5xx response calling FilesApi#restFoldersIdActionsFilePost")
    e.printStackTrace()
}
```

### Parameters

Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **id** | **kotlin.String**| ID of the folder |
 **body** | **io.ktor.client.request.forms.InputProvider**| file content |
 **returnEntity** | **kotlin.Boolean**| Return information about newly created entity | [optional]
 **mode** | **kotlin.String**| Response mode | [optional]
 **clientCreated** | **kotlin.String**| Client created field for the file | [optional]
 **clientModified** | **kotlin.String**| Client modified field for the file | [optional]
 **disableAutoVersion** | **kotlin.Boolean**| Indicates whether Client would like to save file as new version | [optional]
 **note** | **kotlin.Boolean**| Indicates whether the file is note | [optional]

### Return type

null (empty response body)

### Authorization

No authorization required

### HTTP request headers

 - **Content-Type**: multipart/form-data
 - **Accept**: Not defined

<a id="restFoldersParentFilesPost"></a>
# **restFoldersParentFilesPost**
> restFoldersParentFilesPost(parent, body, xKWNote, returnEntity, mode)

Uploads a new file

Uploads a new file

### Example
```kotlin
// Import classes:
//import org.openapitools.client.infrastructure.*
//import org.openapitools.client.models.*

val apiInstance = FilesApi()
val parent : kotlin.String = parent_example // kotlin.String | ID of the parent folder
val body : io.ktor.client.request.forms.InputProvider = BINARY_DATA_HERE // io.ktor.client.request.forms.InputProvider | file content
val xKWNote : kotlin.Boolean = true // kotlin.Boolean | Specifies that this file is a note
val returnEntity : kotlin.Boolean = true // kotlin.Boolean | Return information about newly created entity
val mode : kotlin.String = mode_example // kotlin.String | Response mode
try {
    apiInstance.restFoldersParentFilesPost(parent, body, xKWNote, returnEntity, mode)
} catch (e: ClientException) {
    println("4xx response calling FilesApi#restFoldersParentFilesPost")
    e.printStackTrace()
} catch (e: ServerException) {
    println("5xx response calling FilesApi#restFoldersParentFilesPost")
    e.printStackTrace()
}
```

### Parameters

Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **parent** | **kotlin.String**| ID of the parent folder |
 **body** | **io.ktor.client.request.forms.InputProvider**| file content |
 **xKWNote** | **kotlin.Boolean**| Specifies that this file is a note | [optional]
 **returnEntity** | **kotlin.Boolean**| Return information about newly created entity | [optional]
 **mode** | **kotlin.String**| Response mode | [optional]

### Return type

null (empty response body)

### Authorization

No authorization required

### HTTP request headers

 - **Content-Type**: multipart/form-data
 - **Accept**: Not defined

<a id="restFoldersParentIdActionsFileFromTemplatePost"></a>
# **restFoldersParentIdActionsFileFromTemplatePost**
> restFoldersParentIdActionsFileFromTemplatePost(parentId, body)

Create a new empty file from template

Create a new empty file from template

### Example
```kotlin
// Import classes:
//import org.openapitools.client.infrastructure.*
//import org.openapitools.client.models.*

val apiInstance = FilesApi()
val parentId : kotlin.String = parentId_example // kotlin.String | ID of the parent folder
val body : FileNameRequestPost =  // FileNameRequestPost | FIle from template parameters
try {
    apiInstance.restFoldersParentIdActionsFileFromTemplatePost(parentId, body)
} catch (e: ClientException) {
    println("4xx response calling FilesApi#restFoldersParentIdActionsFileFromTemplatePost")
    e.printStackTrace()
} catch (e: ServerException) {
    println("5xx response calling FilesApi#restFoldersParentIdActionsFileFromTemplatePost")
    e.printStackTrace()
}
```

### Parameters

Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **parentId** | **kotlin.String**| ID of the parent folder |
 **body** | [**FileNameRequestPost**](FileNameRequestPost.md)| FIle from template parameters |

### Return type

null (empty response body)

### Authorization

No authorization required

### HTTP request headers

 - **Content-Type**: Not defined
 - **Accept**: Not defined

<a id="restPermissionsFileFileIdGet"></a>
# **restPermissionsFileFileIdGet**
> kotlin.collections.List&lt;Permission&gt; restPermissionsFileFileIdGet(fileId, id, idColonIn, name, nameColonContains, allowed, enabled, with, mode)

Return the list of permissions available on a file

Return available permissions

### Example
```kotlin
// Import classes:
//import org.openapitools.client.infrastructure.*
//import org.openapitools.client.models.*

val apiInstance = FilesApi()
val fileId : kotlin.String = fileId_example // kotlin.String | ID of the file
val id : kotlin.Int = 56 // kotlin.Int | Unique action identifier
val idColonIn : kotlin.Int = 56 // kotlin.Int | Unique action identifier. Search for results that contain any of specified values of this parameter.
val name : kotlin.String = name_example // kotlin.String | Action name
val nameColonContains : kotlin.String = nameColonContains_example // kotlin.String | Action name. Search for result that contains specified characters in this parameter.
val allowed : kotlin.Boolean = true // kotlin.Boolean | Determines if one has permissions to perform action
val enabled : kotlin.Boolean = true // kotlin.Boolean | Determines if given action is available considering current object state (locked, deleted, etc)
val with : kotlin.String = with_example // kotlin.String | With parameters
val mode : kotlin.String = mode_example // kotlin.String | Response mode
try {
    val result : kotlin.collections.List<Permission> = apiInstance.restPermissionsFileFileIdGet(fileId, id, idColonIn, name, nameColonContains, allowed, enabled, with, mode)
    println(result)
} catch (e: ClientException) {
    println("4xx response calling FilesApi#restPermissionsFileFileIdGet")
    e.printStackTrace()
} catch (e: ServerException) {
    println("5xx response calling FilesApi#restPermissionsFileFileIdGet")
    e.printStackTrace()
}
```

### Parameters

Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **fileId** | **kotlin.String**| ID of the file |
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

<a id="restPermissionsFilesGet"></a>
# **restPermissionsFilesGet**
> kotlin.collections.List&lt;FilePermissions&gt; restPermissionsFilesGet(idColonIn, name, nameColonContains, allowed, enabled, actionId, actionIdColonIn, with, mode)

Return the list of permissions available on a list of files

Return available permissions

### Example
```kotlin
// Import classes:
//import org.openapitools.client.infrastructure.*
//import org.openapitools.client.models.*

val apiInstance = FilesApi()
val idColonIn : kotlin.String = idColonIn_example // kotlin.String | Search for results that contain any of specified values of this parameter.
val name : kotlin.String = name_example // kotlin.String | Action name
val nameColonContains : kotlin.String = nameColonContains_example // kotlin.String | Action name. Search for result that contains specified characters in this parameter.
val allowed : kotlin.Boolean = true // kotlin.Boolean | Determines if one has permissions to perform action
val enabled : kotlin.Boolean = true // kotlin.Boolean | Determines if given action is available considering current object state (locked, deleted, etc)
val actionId : kotlin.Int = 56 // kotlin.Int | Unique action identifier
val actionIdColonIn : kotlin.Int = 56 // kotlin.Int | Unique action identifier. Search for results that contain any of specified values of this parameter.
val with : kotlin.String = with_example // kotlin.String | With parameters
val mode : kotlin.String = mode_example // kotlin.String | Response mode
try {
    val result : kotlin.collections.List<FilePermissions> = apiInstance.restPermissionsFilesGet(idColonIn, name, nameColonContains, allowed, enabled, actionId, actionIdColonIn, with, mode)
    println(result)
} catch (e: ClientException) {
    println("4xx response calling FilesApi#restPermissionsFilesGet")
    e.printStackTrace()
} catch (e: ServerException) {
    println("5xx response calling FilesApi#restPermissionsFilesGet")
    e.printStackTrace()
}
```

### Parameters

Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **idColonIn** | **kotlin.String**| Search for results that contain any of specified values of this parameter. |
 **name** | **kotlin.String**| Action name | [optional]
 **nameColonContains** | **kotlin.String**| Action name. Search for result that contains specified characters in this parameter. | [optional]
 **allowed** | **kotlin.Boolean**| Determines if one has permissions to perform action | [optional]
 **enabled** | **kotlin.Boolean**| Determines if given action is available considering current object state (locked, deleted, etc) | [optional]
 **actionId** | **kotlin.Int**| Unique action identifier | [optional]
 **actionIdColonIn** | **kotlin.Int**| Unique action identifier. Search for results that contain any of specified values of this parameter. | [optional]
 **with** | **kotlin.String**| With parameters | [optional]
 **mode** | **kotlin.String**| Response mode | [optional]

### Return type

[**kotlin.collections.List&lt;FilePermissions&gt;**](FilePermissions.md)

### Authorization

No authorization required

### HTTP request headers

 - **Content-Type**: Not defined
 - **Accept**: */*

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

val apiInstance = FilesApi()
val ref : kotlin.String = ref_example // kotlin.String | Request file short link
val body : io.ktor.client.request.forms.InputProvider = BINARY_DATA_HERE // io.ktor.client.request.forms.InputProvider | file content
val returnEntity : kotlin.Boolean = true // kotlin.Boolean | Return information about newly created entity
val mode : kotlin.String = mode_example // kotlin.String | Response mode
val clientCreated : kotlin.String = 2013-10-20 // kotlin.String | Client created field for the file
val clientModified : kotlin.String = 2013-10-20 // kotlin.String | Client modified field for the file
try {
    apiInstance.restRequestFileRefActionsFilePost(ref, body, returnEntity, mode, clientCreated, clientModified)
} catch (e: ClientException) {
    println("4xx response calling FilesApi#restRequestFileRefActionsFilePost")
    e.printStackTrace()
} catch (e: ServerException) {
    println("5xx response calling FilesApi#restRequestFileRefActionsFilePost")
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

val apiInstance = FilesApi()
val ref : kotlin.String = ref_example // kotlin.String | The request file shortlink
val objectId : kotlin.String = objectId_example // kotlin.String | Object ID of the file being commented on
val body : CommentPost =  // CommentPost | The comment details
val returnEntity : kotlin.Boolean = true // kotlin.Boolean | Return information about newly created entity
val mode : kotlin.String = mode_example // kotlin.String | Response mode
try {
    apiInstance.restRequestFileRefCommentObjectIdPost(ref, objectId, body, returnEntity, mode)
} catch (e: ClientException) {
    println("4xx response calling FilesApi#restRequestFileRefCommentObjectIdPost")
    e.printStackTrace()
} catch (e: ServerException) {
    println("5xx response calling FilesApi#restRequestFileRefCommentObjectIdPost")
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

val apiInstance = FilesApi()
val ref : kotlin.String = ref_example // kotlin.String | Request file short link
val objectId : kotlin.String = objectId_example // kotlin.String | ID of the file
val range : kotlin.String = range_example // kotlin.String | Bytes range to retrieve. Example: bytes=0-1024
try {
    val result : Content = apiInstance.restRequestFileRefSourcesObjectIdContentGet(ref, objectId, range)
    println(result)
} catch (e: ClientException) {
    println("4xx response calling FilesApi#restRequestFileRefSourcesObjectIdContentGet")
    e.printStackTrace()
} catch (e: ServerException) {
    println("5xx response calling FilesApi#restRequestFileRefSourcesObjectIdContentGet")
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

val apiInstance = FilesApi()
val ref : kotlin.String = ref_example // kotlin.String | id
val objectId : kotlin.String = objectId_example // kotlin.String | ID of the file
val range : kotlin.String = range_example // kotlin.String | Bytes range to retrieve. Example: bytes=0-1024
try {
    val result : Content = apiInstance.restRequestFileRefUploadsObjectIdContentGet(ref, objectId, range)
    println(result)
} catch (e: ClientException) {
    println("4xx response calling FilesApi#restRequestFileRefUploadsObjectIdContentGet")
    e.printStackTrace()
} catch (e: ServerException) {
    println("5xx response calling FilesApi#restRequestFileRefUploadsObjectIdContentGet")
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

<a id="restSourcesActionsDownloadByTransactionGet"></a>
# **restSourcesActionsDownloadByTransactionGet**
> KPTransferStatus restSourcesActionsDownloadByTransactionGet(transactionId, mode)

Download EC file

Download EC file using the transaction ID

### Example
```kotlin
// Import classes:
//import org.openapitools.client.infrastructure.*
//import org.openapitools.client.models.*

val apiInstance = FilesApi()
val transactionId : kotlin.Int = 56 // kotlin.Int | Transaction ID of download
val mode : kotlin.String = mode_example // kotlin.String | Response mode
try {
    val result : KPTransferStatus = apiInstance.restSourcesActionsDownloadByTransactionGet(transactionId, mode)
    println(result)
} catch (e: ClientException) {
    println("4xx response calling FilesApi#restSourcesActionsDownloadByTransactionGet")
    e.printStackTrace()
} catch (e: ServerException) {
    println("5xx response calling FilesApi#restSourcesActionsDownloadByTransactionGet")
    e.printStackTrace()
}
```

### Parameters

Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **transactionId** | **kotlin.Int**| Transaction ID of download | [optional]
 **mode** | **kotlin.String**| Response mode | [optional]

### Return type

[**KPTransferStatus**](KPTransferStatus.md)

### Authorization

No authorization required

### HTTP request headers

 - **Content-Type**: Not defined
 - **Accept**: */*

<a id="restSourcesActionsFilesIdPost"></a>
# **restSourcesActionsFilesIdPost**
> KPTransferStatus restSourcesActionsFilesIdPost(id, body, returnEntity, mode)

upload new version of EC file

uploads new version of EC file

### Example
```kotlin
// Import classes:
//import org.openapitools.client.infrastructure.*
//import org.openapitools.client.models.*

val apiInstance = FilesApi()
val id : kotlin.Int = 56 // kotlin.Int | kp file id
val body : io.ktor.client.request.forms.InputProvider = BINARY_DATA_HERE // io.ktor.client.request.forms.InputProvider | file content
val returnEntity : kotlin.Boolean = true // kotlin.Boolean | Return information about newly created entity
val mode : kotlin.String = mode_example // kotlin.String | Response mode
try {
    val result : KPTransferStatus = apiInstance.restSourcesActionsFilesIdPost(id, body, returnEntity, mode)
    println(result)
} catch (e: ClientException) {
    println("4xx response calling FilesApi#restSourcesActionsFilesIdPost")
    e.printStackTrace()
} catch (e: ServerException) {
    println("5xx response calling FilesApi#restSourcesActionsFilesIdPost")
    e.printStackTrace()
}
```

### Parameters

Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **id** | **kotlin.Int**| kp file id |
 **body** | **io.ktor.client.request.forms.InputProvider**| file content |
 **returnEntity** | **kotlin.Boolean**| Return information about newly created entity | [optional]
 **mode** | **kotlin.String**| Response mode | [optional]

### Return type

[**KPTransferStatus**](KPTransferStatus.md)

### Authorization

No authorization required

### HTTP request headers

 - **Content-Type**: multipart/form-data
 - **Accept**: */*

<a id="restSourcesIdActionsFilePost"></a>
# **restSourcesIdActionsFilePost**
> KPTransferStatus restSourcesIdActionsFilePost(id, body, returnEntity, mode)

upload content

uploads file content to a kp folder

### Example
```kotlin
// Import classes:
//import org.openapitools.client.infrastructure.*
//import org.openapitools.client.models.*

val apiInstance = FilesApi()
val id : kotlin.Int = 56 // kotlin.Int | kp folder id
val body : io.ktor.client.request.forms.InputProvider = BINARY_DATA_HERE // io.ktor.client.request.forms.InputProvider | file content
val returnEntity : kotlin.Boolean = true // kotlin.Boolean | Return information about newly created entity
val mode : kotlin.String = mode_example // kotlin.String | Response mode
try {
    val result : KPTransferStatus = apiInstance.restSourcesIdActionsFilePost(id, body, returnEntity, mode)
    println(result)
} catch (e: ClientException) {
    println("4xx response calling FilesApi#restSourcesIdActionsFilePost")
    e.printStackTrace()
} catch (e: ServerException) {
    println("5xx response calling FilesApi#restSourcesIdActionsFilePost")
    e.printStackTrace()
}
```

### Parameters

Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **id** | **kotlin.Int**| kp folder id |
 **body** | **io.ktor.client.request.forms.InputProvider**| file content |
 **returnEntity** | **kotlin.Boolean**| Return information about newly created entity | [optional]
 **mode** | **kotlin.String**| Response mode | [optional]

### Return type

[**KPTransferStatus**](KPTransferStatus.md)

### Authorization

No authorization required

### HTTP request headers

 - **Content-Type**: multipart/form-data
 - **Accept**: */*

<a id="restSourcesIdActionsInitiateDownloadPost"></a>
# **restSourcesIdActionsInitiateDownloadPost**
> KPTransferStatus restSourcesIdActionsInitiateDownloadPost(id)

Initiate EC file download

Initiate Ec file download to kiteworks

### Example
```kotlin
// Import classes:
//import org.openapitools.client.infrastructure.*
//import org.openapitools.client.models.*

val apiInstance = FilesApi()
val id : kotlin.Int = 56 // kotlin.Int | EC file id
try {
    val result : KPTransferStatus = apiInstance.restSourcesIdActionsInitiateDownloadPost(id)
    println(result)
} catch (e: ClientException) {
    println("4xx response calling FilesApi#restSourcesIdActionsInitiateDownloadPost")
    e.printStackTrace()
} catch (e: ServerException) {
    println("5xx response calling FilesApi#restSourcesIdActionsInitiateDownloadPost")
    e.printStackTrace()
}
```

### Parameters

Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **id** | **kotlin.Int**| EC file id |

### Return type

[**KPTransferStatus**](KPTransferStatus.md)

### Authorization

No authorization required

### HTTP request headers

 - **Content-Type**: Not defined
 - **Accept**: */*

<a id="restSourcesIdContentGet"></a>
# **restSourcesIdContentGet**
> Content restSourcesIdContentGet(id)

Read EC file content

Read content of an EC file

### Example
```kotlin
// Import classes:
//import org.openapitools.client.infrastructure.*
//import org.openapitools.client.models.*

val apiInstance = FilesApi()
val id : kotlin.Int = 56 // kotlin.Int | EC file id
try {
    val result : Content = apiInstance.restSourcesIdContentGet(id)
    println(result)
} catch (e: ClientException) {
    println("4xx response calling FilesApi#restSourcesIdContentGet")
    e.printStackTrace()
} catch (e: ServerException) {
    println("5xx response calling FilesApi#restSourcesIdContentGet")
    e.printStackTrace()
}
```

### Parameters

Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **id** | **kotlin.Int**| EC file id |

### Return type

[**Content**](Content.md)

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

val apiInstance = FilesApi()
val id : kotlin.Int = 56 // kotlin.Int | ID of the kitepoint file
try {
    val result : KitepointPreview = apiInstance.restSourcesIdPreviewGet(id)
    println(result)
} catch (e: ClientException) {
    println("4xx response calling FilesApi#restSourcesIdPreviewGet")
    e.printStackTrace()
} catch (e: ServerException) {
    println("5xx response calling FilesApi#restSourcesIdPreviewGet")
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

