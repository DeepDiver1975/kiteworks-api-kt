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
val due : java.time.LocalDate = 2013-10-20 // java.time.LocalDate | Task due date
val dueColonGt : java.time.LocalDate = 2013-10-20 // java.time.LocalDate | Task due date. Search for result that has this parameter value greater than specified.
val dueColonGte : java.time.LocalDate = 2013-10-20 // java.time.LocalDate | Task due date. Search for result that has this parameter value greater or equal to the specified.
val dueColonLt : java.time.LocalDate = 2013-10-20 // java.time.LocalDate | Task due date. Search for result that has this parameter value less than specified.
val dueColonLte : java.time.LocalDate = 2013-10-20 // java.time.LocalDate | Task due date. Search for result that has this parameter value less or equal to the specified.
val parentId : kotlin.Int = 56 // kotlin.Int | Parent Comment identifier
val parentIdColonIn : kotlin.Int = 56 // kotlin.Int | Parent Comment identifier. Search for results that contain any of specified values of this parameter.
val userId : kotlin.String = userId_example // kotlin.String | Identifier of User who created a Task
val userIdColonIn : kotlin.String = userIdColonIn_example // kotlin.String | Identifier of User who created a Task. Search for results that contain any of specified values of this parameter.
val created : java.time.LocalDate = 2013-10-20 // java.time.LocalDate | Task creation date
val createdColonGt : java.time.LocalDate = 2013-10-20 // java.time.LocalDate | Task creation date. Search for result that has this parameter value greater than specified.
val createdColonGte : java.time.LocalDate = 2013-10-20 // java.time.LocalDate | Task creation date. Search for result that has this parameter value greater or equal to the specified.
val createdColonLt : java.time.LocalDate = 2013-10-20 // java.time.LocalDate | Task creation date. Search for result that has this parameter value less than specified.
val createdColonLte : java.time.LocalDate = 2013-10-20 // java.time.LocalDate | Task creation date. Search for result that has this parameter value less or equal to the specified.
val modified : java.time.LocalDate = 2013-10-20 // java.time.LocalDate | Task modification date
val modifiedColonGt : java.time.LocalDate = 2013-10-20 // java.time.LocalDate | Task modification date. Search for result that has this parameter value greater than specified.
val modifiedColonGte : java.time.LocalDate = 2013-10-20 // java.time.LocalDate | Task modification date. Search for result that has this parameter value greater or equal to the specified.
val modifiedColonLt : java.time.LocalDate = 2013-10-20 // java.time.LocalDate | Task modification date. Search for result that has this parameter value less than specified.
val modifiedColonLte : java.time.LocalDate = 2013-10-20 // java.time.LocalDate | Task modification date. Search for result that has this parameter value less or equal to the specified.
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
 **due** | **java.time.LocalDate**| Task due date | [optional]
 **dueColonGt** | **java.time.LocalDate**| Task due date. Search for result that has this parameter value greater than specified. | [optional]
 **dueColonGte** | **java.time.LocalDate**| Task due date. Search for result that has this parameter value greater or equal to the specified. | [optional]
 **dueColonLt** | **java.time.LocalDate**| Task due date. Search for result that has this parameter value less than specified. | [optional]
 **dueColonLte** | **java.time.LocalDate**| Task due date. Search for result that has this parameter value less or equal to the specified. | [optional]
 **parentId** | **kotlin.Int**| Parent Comment identifier | [optional]
 **parentIdColonIn** | **kotlin.Int**| Parent Comment identifier. Search for results that contain any of specified values of this parameter. | [optional]
 **userId** | **kotlin.String**| Identifier of User who created a Task | [optional]
 **userIdColonIn** | **kotlin.String**| Identifier of User who created a Task. Search for results that contain any of specified values of this parameter. | [optional]
 **created** | **java.time.LocalDate**| Task creation date | [optional]
 **createdColonGt** | **java.time.LocalDate**| Task creation date. Search for result that has this parameter value greater than specified. | [optional]
 **createdColonGte** | **java.time.LocalDate**| Task creation date. Search for result that has this parameter value greater or equal to the specified. | [optional]
 **createdColonLt** | **java.time.LocalDate**| Task creation date. Search for result that has this parameter value less than specified. | [optional]
 **createdColonLte** | **java.time.LocalDate**| Task creation date. Search for result that has this parameter value less or equal to the specified. | [optional]
 **modified** | **java.time.LocalDate**| Task modification date | [optional]
 **modifiedColonGt** | **java.time.LocalDate**| Task modification date. Search for result that has this parameter value greater than specified. | [optional]
 **modifiedColonGte** | **java.time.LocalDate**| Task modification date. Search for result that has this parameter value greater or equal to the specified. | [optional]
 **modifiedColonLt** | **java.time.LocalDate**| Task modification date. Search for result that has this parameter value less than specified. | [optional]
 **modifiedColonLte** | **java.time.LocalDate**| Task modification date. Search for result that has this parameter value less or equal to the specified. | [optional]
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
val due : java.time.LocalDate = 2013-10-20 // java.time.LocalDate | Task due date
val dueColonGt : java.time.LocalDate = 2013-10-20 // java.time.LocalDate | Task due date. Search for result that has this parameter value greater than specified.
val dueColonGte : java.time.LocalDate = 2013-10-20 // java.time.LocalDate | Task due date. Search for result that has this parameter value greater or equal to the specified.
val dueColonLt : java.time.LocalDate = 2013-10-20 // java.time.LocalDate | Task due date. Search for result that has this parameter value less than specified.
val dueColonLte : java.time.LocalDate = 2013-10-20 // java.time.LocalDate | Task due date. Search for result that has this parameter value less or equal to the specified.
val parentId : kotlin.Int = 56 // kotlin.Int | Parent Comment identifier
val parentIdColonIn : kotlin.Int = 56 // kotlin.Int | Parent Comment identifier. Search for results that contain any of specified values of this parameter.
val userId : kotlin.String = userId_example // kotlin.String | Identifier of User who created a Task
val userIdColonIn : kotlin.String = userIdColonIn_example // kotlin.String | Identifier of User who created a Task. Search for results that contain any of specified values of this parameter.
val created : java.time.LocalDate = 2013-10-20 // java.time.LocalDate | Task creation date
val createdColonGt : java.time.LocalDate = 2013-10-20 // java.time.LocalDate | Task creation date. Search for result that has this parameter value greater than specified.
val createdColonGte : java.time.LocalDate = 2013-10-20 // java.time.LocalDate | Task creation date. Search for result that has this parameter value greater or equal to the specified.
val createdColonLt : java.time.LocalDate = 2013-10-20 // java.time.LocalDate | Task creation date. Search for result that has this parameter value less than specified.
val createdColonLte : java.time.LocalDate = 2013-10-20 // java.time.LocalDate | Task creation date. Search for result that has this parameter value less or equal to the specified.
val modified : java.time.LocalDate = 2013-10-20 // java.time.LocalDate | Task modification date
val modifiedColonGt : java.time.LocalDate = 2013-10-20 // java.time.LocalDate | Task modification date. Search for result that has this parameter value greater than specified.
val modifiedColonGte : java.time.LocalDate = 2013-10-20 // java.time.LocalDate | Task modification date. Search for result that has this parameter value greater or equal to the specified.
val modifiedColonLt : java.time.LocalDate = 2013-10-20 // java.time.LocalDate | Task modification date. Search for result that has this parameter value less than specified.
val modifiedColonLte : java.time.LocalDate = 2013-10-20 // java.time.LocalDate | Task modification date. Search for result that has this parameter value less or equal to the specified.
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
 **due** | **java.time.LocalDate**| Task due date | [optional]
 **dueColonGt** | **java.time.LocalDate**| Task due date. Search for result that has this parameter value greater than specified. | [optional]
 **dueColonGte** | **java.time.LocalDate**| Task due date. Search for result that has this parameter value greater or equal to the specified. | [optional]
 **dueColonLt** | **java.time.LocalDate**| Task due date. Search for result that has this parameter value less than specified. | [optional]
 **dueColonLte** | **java.time.LocalDate**| Task due date. Search for result that has this parameter value less or equal to the specified. | [optional]
 **parentId** | **kotlin.Int**| Parent Comment identifier | [optional]
 **parentIdColonIn** | **kotlin.Int**| Parent Comment identifier. Search for results that contain any of specified values of this parameter. | [optional]
 **userId** | **kotlin.String**| Identifier of User who created a Task | [optional]
 **userIdColonIn** | **kotlin.String**| Identifier of User who created a Task. Search for results that contain any of specified values of this parameter. | [optional]
 **created** | **java.time.LocalDate**| Task creation date | [optional]
 **createdColonGt** | **java.time.LocalDate**| Task creation date. Search for result that has this parameter value greater than specified. | [optional]
 **createdColonGte** | **java.time.LocalDate**| Task creation date. Search for result that has this parameter value greater or equal to the specified. | [optional]
 **createdColonLt** | **java.time.LocalDate**| Task creation date. Search for result that has this parameter value less than specified. | [optional]
 **createdColonLte** | **java.time.LocalDate**| Task creation date. Search for result that has this parameter value less or equal to the specified. | [optional]
 **modified** | **java.time.LocalDate**| Task modification date | [optional]
 **modifiedColonGt** | **java.time.LocalDate**| Task modification date. Search for result that has this parameter value greater than specified. | [optional]
 **modifiedColonGte** | **java.time.LocalDate**| Task modification date. Search for result that has this parameter value greater or equal to the specified. | [optional]
 **modifiedColonLt** | **java.time.LocalDate**| Task modification date. Search for result that has this parameter value less than specified. | [optional]
 **modifiedColonLte** | **java.time.LocalDate**| Task modification date. Search for result that has this parameter value less or equal to the specified. | [optional]
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
val due : java.time.LocalDate = 2013-10-20 // java.time.LocalDate | Task due date
val dueColonGt : java.time.LocalDate = 2013-10-20 // java.time.LocalDate | Task due date. Search for result that has this parameter value greater than specified.
val dueColonGte : java.time.LocalDate = 2013-10-20 // java.time.LocalDate | Task due date. Search for result that has this parameter value greater or equal to the specified.
val dueColonLt : java.time.LocalDate = 2013-10-20 // java.time.LocalDate | Task due date. Search for result that has this parameter value less than specified.
val dueColonLte : java.time.LocalDate = 2013-10-20 // java.time.LocalDate | Task due date. Search for result that has this parameter value less or equal to the specified.
val parentId : kotlin.Int = 56 // kotlin.Int | Parent Comment identifier
val parentIdColonIn : kotlin.Int = 56 // kotlin.Int | Parent Comment identifier. Search for results that contain any of specified values of this parameter.
val created : java.time.LocalDate = 2013-10-20 // java.time.LocalDate | Task creation date
val createdColonGt : java.time.LocalDate = 2013-10-20 // java.time.LocalDate | Task creation date. Search for result that has this parameter value greater than specified.
val createdColonGte : java.time.LocalDate = 2013-10-20 // java.time.LocalDate | Task creation date. Search for result that has this parameter value greater or equal to the specified.
val createdColonLt : java.time.LocalDate = 2013-10-20 // java.time.LocalDate | Task creation date. Search for result that has this parameter value less than specified.
val createdColonLte : java.time.LocalDate = 2013-10-20 // java.time.LocalDate | Task creation date. Search for result that has this parameter value less or equal to the specified.
val modified : java.time.LocalDate = 2013-10-20 // java.time.LocalDate | Task modification date
val modifiedColonGt : java.time.LocalDate = 2013-10-20 // java.time.LocalDate | Task modification date. Search for result that has this parameter value greater than specified.
val modifiedColonGte : java.time.LocalDate = 2013-10-20 // java.time.LocalDate | Task modification date. Search for result that has this parameter value greater or equal to the specified.
val modifiedColonLt : java.time.LocalDate = 2013-10-20 // java.time.LocalDate | Task modification date. Search for result that has this parameter value less than specified.
val modifiedColonLte : java.time.LocalDate = 2013-10-20 // java.time.LocalDate | Task modification date. Search for result that has this parameter value less or equal to the specified.
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
 **due** | **java.time.LocalDate**| Task due date | [optional]
 **dueColonGt** | **java.time.LocalDate**| Task due date. Search for result that has this parameter value greater than specified. | [optional]
 **dueColonGte** | **java.time.LocalDate**| Task due date. Search for result that has this parameter value greater or equal to the specified. | [optional]
 **dueColonLt** | **java.time.LocalDate**| Task due date. Search for result that has this parameter value less than specified. | [optional]
 **dueColonLte** | **java.time.LocalDate**| Task due date. Search for result that has this parameter value less or equal to the specified. | [optional]
 **parentId** | **kotlin.Int**| Parent Comment identifier | [optional]
 **parentIdColonIn** | **kotlin.Int**| Parent Comment identifier. Search for results that contain any of specified values of this parameter. | [optional]
 **created** | **java.time.LocalDate**| Task creation date | [optional]
 **createdColonGt** | **java.time.LocalDate**| Task creation date. Search for result that has this parameter value greater than specified. | [optional]
 **createdColonGte** | **java.time.LocalDate**| Task creation date. Search for result that has this parameter value greater or equal to the specified. | [optional]
 **createdColonLt** | **java.time.LocalDate**| Task creation date. Search for result that has this parameter value less than specified. | [optional]
 **createdColonLte** | **java.time.LocalDate**| Task creation date. Search for result that has this parameter value less or equal to the specified. | [optional]
 **modified** | **java.time.LocalDate**| Task modification date | [optional]
 **modifiedColonGt** | **java.time.LocalDate**| Task modification date. Search for result that has this parameter value greater than specified. | [optional]
 **modifiedColonGte** | **java.time.LocalDate**| Task modification date. Search for result that has this parameter value greater or equal to the specified. | [optional]
 **modifiedColonLt** | **java.time.LocalDate**| Task modification date. Search for result that has this parameter value less than specified. | [optional]
 **modifiedColonLte** | **java.time.LocalDate**| Task modification date. Search for result that has this parameter value less or equal to the specified. | [optional]
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

