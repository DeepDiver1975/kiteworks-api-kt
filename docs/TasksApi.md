# TasksApi

All URIs are relative to *http://localhost*

Method | HTTP request | Description
------------- | ------------- | -------------
[**restFilesIdTasksGet**](TasksApi.md#restFilesIdTasksGet) | **GET** /rest/files/{id}/tasks | Get Tasks for a file
[**restFilesIdTasksPost**](TasksApi.md#restFilesIdTasksPost) | **POST** /rest/files/{id}/tasks | Create a Task on a file
[**restFoldersIdTasksGet**](TasksApi.md#restFoldersIdTasksGet) | **GET** /rest/folders/{id}/tasks | Get Tasks for a folder
[**restPermissionsTaskTaskIdGet**](TasksApi.md#restPermissionsTaskTaskIdGet) | **GET** /rest/permissions/task/{task_id} | Return the list of permissions available on a task
[**restTasksGet**](TasksApi.md#restTasksGet) | **GET** /rest/tasks | Gets all tasks for current user
[**restTasksIdDelete**](TasksApi.md#restTasksIdDelete) | **DELETE** /rest/tasks/{id} | Delete a Task
[**restTasksIdGet**](TasksApi.md#restTasksIdGet) | **GET** /rest/tasks/{id} | Get Task by ID
[**restTasksIdPut**](TasksApi.md#restTasksIdPut) | **PUT** /rest/tasks/{id} | Update Task


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

val apiInstance = TasksApi()
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
    println("4xx response calling TasksApi#restFilesIdTasksGet")
    e.printStackTrace()
} catch (e: ServerException) {
    println("5xx response calling TasksApi#restFilesIdTasksGet")
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

val apiInstance = TasksApi()
val id : kotlin.String = id_example // kotlin.String | Object ID of the file task is created on
val body : TaskPost =  // TaskPost | The task details
val returnEntity : kotlin.Boolean = true // kotlin.Boolean | Return information about newly created entity
val mode : kotlin.String = mode_example // kotlin.String | Response mode
try {
    apiInstance.restFilesIdTasksPost(id, body, returnEntity, mode)
} catch (e: ClientException) {
    println("4xx response calling TasksApi#restFilesIdTasksPost")
    e.printStackTrace()
} catch (e: ServerException) {
    println("5xx response calling TasksApi#restFilesIdTasksPost")
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

val apiInstance = TasksApi()
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
    println("4xx response calling TasksApi#restFoldersIdTasksGet")
    e.printStackTrace()
} catch (e: ServerException) {
    println("5xx response calling TasksApi#restFoldersIdTasksGet")
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

val apiInstance = TasksApi()
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
    println("4xx response calling TasksApi#restPermissionsTaskTaskIdGet")
    e.printStackTrace()
} catch (e: ServerException) {
    println("5xx response calling TasksApi#restPermissionsTaskTaskIdGet")
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

<a id="restTasksGet"></a>
# **restTasksGet**
> kotlin.collections.List&lt;Task&gt; restTasksGet(assigneeId, assigneeIdColonIn, due, dueColonGt, dueColonGte, dueColonLt, dueColonLte, parentId, parentIdColonIn, created, createdColonGt, createdColonGte, createdColonLt, createdColonLte, modified, modifiedColonGt, modifiedColonGte, modifiedColonLt, modifiedColonLte, contentsColonContains, status, deleted, assigned, orderBy, offset, limit, with, mode)

Gets all tasks for current user

Gets all tasks for current user

### Example
```kotlin
// Import classes:
//import org.openapitools.client.infrastructure.*
//import org.openapitools.client.models.*

val apiInstance = TasksApi()
val assigneeId : kotlin.String = assigneeId_example // kotlin.String | Assigned User unique identifier
val assigneeIdColonIn : kotlin.String = assigneeIdColonIn_example // kotlin.String | Assigned User unique identifier. Search for results that contain any of specified values of this parameter.
val due : kotlin.String = 2013-10-20 // kotlin.String | Task due date
val dueColonGt : kotlin.String = 2013-10-20 // kotlin.String | Task due date. Search for result that has this parameter value greater than specified.
val dueColonGte : kotlin.String = 2013-10-20 // kotlin.String | Task due date. Search for result that has this parameter value greater or equal to the specified.
val dueColonLt : kotlin.String = 2013-10-20 // kotlin.String | Task due date. Search for result that has this parameter value less than specified.
val dueColonLte : kotlin.String = 2013-10-20 // kotlin.String | Task due date. Search for result that has this parameter value less or equal to the specified.
val parentId : kotlin.Int = 56 // kotlin.Int | Parent Comment identifier
val parentIdColonIn : kotlin.Int = 56 // kotlin.Int | Parent Comment identifier. Search for results that contain any of specified values of this parameter.
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
val assigned : kotlin.String = assigned_example // kotlin.String | Show assigned to
val orderBy : kotlin.collections.List<kotlin.String> =  // kotlin.collections.List<kotlin.String> | Sorting options
val offset : kotlin.Int = 56 // kotlin.Int | Offset
val limit : kotlin.Int = 56 // kotlin.Int | Limit
val with : kotlin.String = with_example // kotlin.String | With parameters
val mode : kotlin.String = mode_example // kotlin.String | Response mode
try {
    val result : kotlin.collections.List<Task> = apiInstance.restTasksGet(assigneeId, assigneeIdColonIn, due, dueColonGt, dueColonGte, dueColonLt, dueColonLte, parentId, parentIdColonIn, created, createdColonGt, createdColonGte, createdColonLt, createdColonLte, modified, modifiedColonGt, modifiedColonGte, modifiedColonLt, modifiedColonLte, contentsColonContains, status, deleted, assigned, orderBy, offset, limit, with, mode)
    println(result)
} catch (e: ClientException) {
    println("4xx response calling TasksApi#restTasksGet")
    e.printStackTrace()
} catch (e: ServerException) {
    println("5xx response calling TasksApi#restTasksGet")
    e.printStackTrace()
}
```

### Parameters

Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **assigneeId** | **kotlin.String**| Assigned User unique identifier | [optional]
 **assigneeIdColonIn** | **kotlin.String**| Assigned User unique identifier. Search for results that contain any of specified values of this parameter. | [optional]
 **due** | **kotlin.String**| Task due date | [optional]
 **dueColonGt** | **kotlin.String**| Task due date. Search for result that has this parameter value greater than specified. | [optional]
 **dueColonGte** | **kotlin.String**| Task due date. Search for result that has this parameter value greater or equal to the specified. | [optional]
 **dueColonLt** | **kotlin.String**| Task due date. Search for result that has this parameter value less than specified. | [optional]
 **dueColonLte** | **kotlin.String**| Task due date. Search for result that has this parameter value less or equal to the specified. | [optional]
 **parentId** | **kotlin.Int**| Parent Comment identifier | [optional]
 **parentIdColonIn** | **kotlin.Int**| Parent Comment identifier. Search for results that contain any of specified values of this parameter. | [optional]
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
 **assigned** | **kotlin.String**| Show assigned to | [optional]
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

<a id="restTasksIdDelete"></a>
# **restTasksIdDelete**
> restTasksIdDelete(id)

Delete a Task

Deletes a task

### Example
```kotlin
// Import classes:
//import org.openapitools.client.infrastructure.*
//import org.openapitools.client.models.*

val apiInstance = TasksApi()
val id : kotlin.Int = 56 // kotlin.Int | ID of the task to delete
try {
    apiInstance.restTasksIdDelete(id)
} catch (e: ClientException) {
    println("4xx response calling TasksApi#restTasksIdDelete")
    e.printStackTrace()
} catch (e: ServerException) {
    println("5xx response calling TasksApi#restTasksIdDelete")
    e.printStackTrace()
}
```

### Parameters

Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **id** | **kotlin.Int**| ID of the task to delete |

### Return type

null (empty response body)

### Authorization

No authorization required

### HTTP request headers

 - **Content-Type**: Not defined
 - **Accept**: Not defined

<a id="restTasksIdGet"></a>
# **restTasksIdGet**
> Task restTasksIdGet(id, with, mode)

Get Task by ID

Returns the details of a task based on ID

### Example
```kotlin
// Import classes:
//import org.openapitools.client.infrastructure.*
//import org.openapitools.client.models.*

val apiInstance = TasksApi()
val id : kotlin.String = id_example // kotlin.String | ID of the task to retrieve
val with : kotlin.String = with_example // kotlin.String | With parameters
val mode : kotlin.String = mode_example // kotlin.String | Response mode
try {
    val result : Task = apiInstance.restTasksIdGet(id, with, mode)
    println(result)
} catch (e: ClientException) {
    println("4xx response calling TasksApi#restTasksIdGet")
    e.printStackTrace()
} catch (e: ServerException) {
    println("5xx response calling TasksApi#restTasksIdGet")
    e.printStackTrace()
}
```

### Parameters

Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **id** | **kotlin.String**| ID of the task to retrieve |
 **with** | **kotlin.String**| With parameters | [optional]
 **mode** | **kotlin.String**| Response mode | [optional]

### Return type

[**Task**](Task.md)

### Authorization

No authorization required

### HTTP request headers

 - **Content-Type**: Not defined
 - **Accept**: */*

<a id="restTasksIdPut"></a>
# **restTasksIdPut**
> restTasksIdPut(id, body)

Update Task

Updates the details of a task

### Example
```kotlin
// Import classes:
//import org.openapitools.client.infrastructure.*
//import org.openapitools.client.models.*

val apiInstance = TasksApi()
val id : kotlin.Int = 56 // kotlin.Int | ID of the task to update
val body : TaskPut =  // TaskPut | The task details
try {
    apiInstance.restTasksIdPut(id, body)
} catch (e: ClientException) {
    println("4xx response calling TasksApi#restTasksIdPut")
    e.printStackTrace()
} catch (e: ServerException) {
    println("5xx response calling TasksApi#restTasksIdPut")
    e.printStackTrace()
}
```

### Parameters

Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **id** | **kotlin.Int**| ID of the task to update |
 **body** | [**TaskPut**](TaskPut.md)| The task details |

### Return type

null (empty response body)

### Authorization

No authorization required

### HTTP request headers

 - **Content-Type**: Not defined
 - **Accept**: Not defined

