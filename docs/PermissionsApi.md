# PermissionsApi

All URIs are relative to *http://localhost*

Method | HTTP request | Description
------------- | ------------- | -------------
[**restPermissionsCommentCommentIdGet**](PermissionsApi.md#restPermissionsCommentCommentIdGet) | **GET** /rest/permissions/comment/{comment_id} | Return the list of permissions available on a comment
[**restPermissionsFileFileIdGet**](PermissionsApi.md#restPermissionsFileFileIdGet) | **GET** /rest/permissions/file/{file_id} | Return the list of permissions available on a file
[**restPermissionsFilesGet**](PermissionsApi.md#restPermissionsFilesGet) | **GET** /rest/permissions/files | Return the list of permissions available on a list of files
[**restPermissionsFolderFolderIdGet**](PermissionsApi.md#restPermissionsFolderFolderIdGet) | **GET** /rest/permissions/folder/{folder_id} | Return the list of permissions available on a folder
[**restPermissionsTaskTaskIdGet**](PermissionsApi.md#restPermissionsTaskTaskIdGet) | **GET** /rest/permissions/task/{task_id} | Return the list of permissions available on a task


<a id="restPermissionsCommentCommentIdGet"></a>
# **restPermissionsCommentCommentIdGet**
> kotlin.collections.List&lt;Permission&gt; restPermissionsCommentCommentIdGet(commentId, id, idColonIn, name, nameColonContains, allowed, enabled, with, mode)

Return the list of permissions available on a comment

Return available permissions

### Example
```kotlin
// Import classes:
//import org.openapitools.client.infrastructure.*
//import org.openapitools.client.models.*

val apiInstance = PermissionsApi()
val commentId : kotlin.Int = 56 // kotlin.Int | Id of the comment
val id : kotlin.Int = 56 // kotlin.Int | Unique action identifier
val idColonIn : kotlin.Int = 56 // kotlin.Int | Unique action identifier. Search for results that contain any of specified values of this parameter.
val name : kotlin.String = name_example // kotlin.String | Action name
val nameColonContains : kotlin.String = nameColonContains_example // kotlin.String | Action name. Search for result that contains specified characters in this parameter.
val allowed : kotlin.Boolean = true // kotlin.Boolean | Determines if one has permissions to perform action
val enabled : kotlin.Boolean = true // kotlin.Boolean | Determines if given action is available considering current object state (locked, deleted, etc)
val with : kotlin.String = with_example // kotlin.String | With parameters
val mode : kotlin.String = mode_example // kotlin.String | Response mode
try {
    val result : kotlin.collections.List<Permission> = apiInstance.restPermissionsCommentCommentIdGet(commentId, id, idColonIn, name, nameColonContains, allowed, enabled, with, mode)
    println(result)
} catch (e: ClientException) {
    println("4xx response calling PermissionsApi#restPermissionsCommentCommentIdGet")
    e.printStackTrace()
} catch (e: ServerException) {
    println("5xx response calling PermissionsApi#restPermissionsCommentCommentIdGet")
    e.printStackTrace()
}
```

### Parameters

Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **commentId** | **kotlin.Int**| Id of the comment |
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

val apiInstance = PermissionsApi()
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
    println("4xx response calling PermissionsApi#restPermissionsFileFileIdGet")
    e.printStackTrace()
} catch (e: ServerException) {
    println("5xx response calling PermissionsApi#restPermissionsFileFileIdGet")
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

val apiInstance = PermissionsApi()
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
    println("4xx response calling PermissionsApi#restPermissionsFilesGet")
    e.printStackTrace()
} catch (e: ServerException) {
    println("5xx response calling PermissionsApi#restPermissionsFilesGet")
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

val apiInstance = PermissionsApi()
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
    println("4xx response calling PermissionsApi#restPermissionsFolderFolderIdGet")
    e.printStackTrace()
} catch (e: ServerException) {
    println("5xx response calling PermissionsApi#restPermissionsFolderFolderIdGet")
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

<a id="restPermissionsTaskTaskIdGet"></a>
# **restPermissionsTaskTaskIdGet**
> kotlin.collections.List&lt;Permission&gt; restPermissionsTaskTaskIdGet(taskId, id, idColonIn, name, nameColonContains, allowed, enabled, with, mode)

Return the list of permissions available on a task

Return available permissions

### Example
```kotlin
// Import classes:
//import org.openapitools.client.infrastructure.*
//import org.openapitools.client.models.*

val apiInstance = PermissionsApi()
val taskId : kotlin.Int = 56 // kotlin.Int | Comment Id of the task
val id : kotlin.Int = 56 // kotlin.Int | Unique action identifier
val idColonIn : kotlin.Int = 56 // kotlin.Int | Unique action identifier. Search for results that contain any of specified values of this parameter.
val name : kotlin.String = name_example // kotlin.String | Action name
val nameColonContains : kotlin.String = nameColonContains_example // kotlin.String | Action name. Search for result that contains specified characters in this parameter.
val allowed : kotlin.Boolean = true // kotlin.Boolean | Determines if one has permissions to perform action
val enabled : kotlin.Boolean = true // kotlin.Boolean | Determines if given action is available considering current object state (locked, deleted, etc)
val with : kotlin.String = with_example // kotlin.String | With parameters
val mode : kotlin.String = mode_example // kotlin.String | Response mode
try {
    val result : kotlin.collections.List<Permission> = apiInstance.restPermissionsTaskTaskIdGet(taskId, id, idColonIn, name, nameColonContains, allowed, enabled, with, mode)
    println(result)
} catch (e: ClientException) {
    println("4xx response calling PermissionsApi#restPermissionsTaskTaskIdGet")
    e.printStackTrace()
} catch (e: ServerException) {
    println("5xx response calling PermissionsApi#restPermissionsTaskTaskIdGet")
    e.printStackTrace()
}
```

### Parameters

Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **taskId** | **kotlin.Int**| Comment Id of the task |
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

