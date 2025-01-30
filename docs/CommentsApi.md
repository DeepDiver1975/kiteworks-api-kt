# CommentsApi

All URIs are relative to *http://localhost*

Method | HTTP request | Description
------------- | ------------- | -------------
[**restCommentsIdDelete**](CommentsApi.md#restCommentsIdDelete) | **DELETE** /rest/comments/{id} | Delete a Comment
[**restCommentsIdGet**](CommentsApi.md#restCommentsIdGet) | **GET** /rest/comments/{id} | Get Comment by ID
[**restCommentsIdPut**](CommentsApi.md#restCommentsIdPut) | **PUT** /rest/comments/{id} | Update Comment
[**restFilesIdCommentsGet**](CommentsApi.md#restFilesIdCommentsGet) | **GET** /rest/files/{id}/comments | Get Comments for a file
[**restFilesIdCommentsPost**](CommentsApi.md#restFilesIdCommentsPost) | **POST** /rest/files/{id}/comments | Create a Comment on a file
[**restFoldersIdCommentsGet**](CommentsApi.md#restFoldersIdCommentsGet) | **GET** /rest/folders/{id}/comments | Return the list of Comments for this folder
[**restPermissionsCommentCommentIdGet**](CommentsApi.md#restPermissionsCommentCommentIdGet) | **GET** /rest/permissions/comment/{comment_id} | Return the list of permissions available on a comment


<a id="restCommentsIdDelete"></a>
# **restCommentsIdDelete**
> restCommentsIdDelete(id)

Delete a Comment

Deletes the comment with the specified id.

### Example
```kotlin
// Import classes:
//import org.openapitools.client.infrastructure.*
//import org.openapitools.client.models.*

val apiInstance = CommentsApi()
val id : kotlin.Int = 56 // kotlin.Int | ID of the comment to delete
try {
    apiInstance.restCommentsIdDelete(id)
} catch (e: ClientException) {
    println("4xx response calling CommentsApi#restCommentsIdDelete")
    e.printStackTrace()
} catch (e: ServerException) {
    println("5xx response calling CommentsApi#restCommentsIdDelete")
    e.printStackTrace()
}
```

### Parameters

Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **id** | **kotlin.Int**| ID of the comment to delete |

### Return type

null (empty response body)

### Authorization

No authorization required

### HTTP request headers

 - **Content-Type**: Not defined
 - **Accept**: Not defined

<a id="restCommentsIdGet"></a>
# **restCommentsIdGet**
> Comment restCommentsIdGet(id, with, mode)

Get Comment by ID

Returns the details of a comment based on ID. e.g.:                I want to know the file or folder this comment is attached to and the comment itself.

### Example
```kotlin
// Import classes:
//import org.openapitools.client.infrastructure.*
//import org.openapitools.client.models.*

val apiInstance = CommentsApi()
val id : kotlin.Int = 56 // kotlin.Int | ID of the comment to retrieve
val with : kotlin.String = with_example // kotlin.String | With parameters
val mode : kotlin.String = mode_example // kotlin.String | Response mode
try {
    val result : Comment = apiInstance.restCommentsIdGet(id, with, mode)
    println(result)
} catch (e: ClientException) {
    println("4xx response calling CommentsApi#restCommentsIdGet")
    e.printStackTrace()
} catch (e: ServerException) {
    println("5xx response calling CommentsApi#restCommentsIdGet")
    e.printStackTrace()
}
```

### Parameters

Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **id** | **kotlin.Int**| ID of the comment to retrieve |
 **with** | **kotlin.String**| With parameters | [optional]
 **mode** | **kotlin.String**| Response mode | [optional]

### Return type

[**Comment**](Comment.md)

### Authorization

No authorization required

### HTTP request headers

 - **Content-Type**: Not defined
 - **Accept**: */*

<a id="restCommentsIdPut"></a>
# **restCommentsIdPut**
> restCommentsIdPut(id, body)

Update Comment

Updates the text of a previously entered comment.

### Example
```kotlin
// Import classes:
//import org.openapitools.client.infrastructure.*
//import org.openapitools.client.models.*

val apiInstance = CommentsApi()
val id : kotlin.Int = 56 // kotlin.Int | ID of the comment to update
val body : CommentPut =  // CommentPut | The comment details
try {
    apiInstance.restCommentsIdPut(id, body)
} catch (e: ClientException) {
    println("4xx response calling CommentsApi#restCommentsIdPut")
    e.printStackTrace()
} catch (e: ServerException) {
    println("5xx response calling CommentsApi#restCommentsIdPut")
    e.printStackTrace()
}
```

### Parameters

Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **id** | **kotlin.Int**| ID of the comment to update |
 **body** | [**CommentPut**](CommentPut.md)| The comment details |

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

val apiInstance = CommentsApi()
val id : kotlin.String = id_example // kotlin.String | File object ID of the comments to retrieve
val parentId : kotlin.Int = 56 // kotlin.Int | Parent Comment unique identifier
val parentIdColonIn : kotlin.Int = 56 // kotlin.Int | Parent Comment unique identifier. Search for results that contain any of specified values of this parameter.
val userId : kotlin.String = userId_example // kotlin.String | Unique identifier of comment author
val userIdColonIn : kotlin.String = userIdColonIn_example // kotlin.String | Unique identifier of comment author. Search for results that contain any of specified values of this parameter.
val created : java.time.LocalDate = 2013-10-20 // java.time.LocalDate | Comment creation date
val createdColonGt : java.time.LocalDate = 2013-10-20 // java.time.LocalDate | Comment creation date. Search for result that has this parameter value greater than specified.
val createdColonGte : java.time.LocalDate = 2013-10-20 // java.time.LocalDate | Comment creation date. Search for result that has this parameter value greater or equal to the specified.
val createdColonLt : java.time.LocalDate = 2013-10-20 // java.time.LocalDate | Comment creation date. Search for result that has this parameter value less than specified.
val createdColonLte : java.time.LocalDate = 2013-10-20 // java.time.LocalDate | Comment creation date. Search for result that has this parameter value less or equal to the specified.
val modified : java.time.LocalDate = 2013-10-20 // java.time.LocalDate | Comment modification date
val modifiedColonGt : java.time.LocalDate = 2013-10-20 // java.time.LocalDate | Comment modification date. Search for result that has this parameter value greater than specified.
val modifiedColonGte : java.time.LocalDate = 2013-10-20 // java.time.LocalDate | Comment modification date. Search for result that has this parameter value greater or equal to the specified.
val modifiedColonLt : java.time.LocalDate = 2013-10-20 // java.time.LocalDate | Comment modification date. Search for result that has this parameter value less than specified.
val modifiedColonLte : java.time.LocalDate = 2013-10-20 // java.time.LocalDate | Comment modification date. Search for result that has this parameter value less or equal to the specified.
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
    println("4xx response calling CommentsApi#restFilesIdCommentsGet")
    e.printStackTrace()
} catch (e: ServerException) {
    println("5xx response calling CommentsApi#restFilesIdCommentsGet")
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
 **created** | **java.time.LocalDate**| Comment creation date | [optional]
 **createdColonGt** | **java.time.LocalDate**| Comment creation date. Search for result that has this parameter value greater than specified. | [optional]
 **createdColonGte** | **java.time.LocalDate**| Comment creation date. Search for result that has this parameter value greater or equal to the specified. | [optional]
 **createdColonLt** | **java.time.LocalDate**| Comment creation date. Search for result that has this parameter value less than specified. | [optional]
 **createdColonLte** | **java.time.LocalDate**| Comment creation date. Search for result that has this parameter value less or equal to the specified. | [optional]
 **modified** | **java.time.LocalDate**| Comment modification date | [optional]
 **modifiedColonGt** | **java.time.LocalDate**| Comment modification date. Search for result that has this parameter value greater than specified. | [optional]
 **modifiedColonGte** | **java.time.LocalDate**| Comment modification date. Search for result that has this parameter value greater or equal to the specified. | [optional]
 **modifiedColonLt** | **java.time.LocalDate**| Comment modification date. Search for result that has this parameter value less than specified. | [optional]
 **modifiedColonLte** | **java.time.LocalDate**| Comment modification date. Search for result that has this parameter value less or equal to the specified. | [optional]
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

val apiInstance = CommentsApi()
val id : kotlin.String = id_example // kotlin.String | Object ID of the file being commented on
val body : CommentPost =  // CommentPost | The comment details
val returnEntity : kotlin.Boolean = true // kotlin.Boolean | Return information about newly created entity
val mode : kotlin.String = mode_example // kotlin.String | Response mode
try {
    apiInstance.restFilesIdCommentsPost(id, body, returnEntity, mode)
} catch (e: ClientException) {
    println("4xx response calling CommentsApi#restFilesIdCommentsPost")
    e.printStackTrace()
} catch (e: ServerException) {
    println("5xx response calling CommentsApi#restFilesIdCommentsPost")
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

val apiInstance = CommentsApi()
val id : kotlin.String = id_example // kotlin.String | ID of the parent folder
val parentId : kotlin.Int = 56 // kotlin.Int | Parent Comment unique identifier
val parentIdColonIn : kotlin.Int = 56 // kotlin.Int | Parent Comment unique identifier. Search for results that contain any of specified values of this parameter.
val userId : kotlin.String = userId_example // kotlin.String | Unique identifier of comment author
val userIdColonIn : kotlin.String = userIdColonIn_example // kotlin.String | Unique identifier of comment author. Search for results that contain any of specified values of this parameter.
val created : java.time.LocalDate = 2013-10-20 // java.time.LocalDate | Comment creation date
val createdColonGt : java.time.LocalDate = 2013-10-20 // java.time.LocalDate | Comment creation date. Search for result that has this parameter value greater than specified.
val createdColonGte : java.time.LocalDate = 2013-10-20 // java.time.LocalDate | Comment creation date. Search for result that has this parameter value greater or equal to the specified.
val createdColonLt : java.time.LocalDate = 2013-10-20 // java.time.LocalDate | Comment creation date. Search for result that has this parameter value less than specified.
val createdColonLte : java.time.LocalDate = 2013-10-20 // java.time.LocalDate | Comment creation date. Search for result that has this parameter value less or equal to the specified.
val modified : java.time.LocalDate = 2013-10-20 // java.time.LocalDate | Comment modification date
val modifiedColonGt : java.time.LocalDate = 2013-10-20 // java.time.LocalDate | Comment modification date. Search for result that has this parameter value greater than specified.
val modifiedColonGte : java.time.LocalDate = 2013-10-20 // java.time.LocalDate | Comment modification date. Search for result that has this parameter value greater or equal to the specified.
val modifiedColonLt : java.time.LocalDate = 2013-10-20 // java.time.LocalDate | Comment modification date. Search for result that has this parameter value less than specified.
val modifiedColonLte : java.time.LocalDate = 2013-10-20 // java.time.LocalDate | Comment modification date. Search for result that has this parameter value less or equal to the specified.
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
    println("4xx response calling CommentsApi#restFoldersIdCommentsGet")
    e.printStackTrace()
} catch (e: ServerException) {
    println("5xx response calling CommentsApi#restFoldersIdCommentsGet")
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
 **created** | **java.time.LocalDate**| Comment creation date | [optional]
 **createdColonGt** | **java.time.LocalDate**| Comment creation date. Search for result that has this parameter value greater than specified. | [optional]
 **createdColonGte** | **java.time.LocalDate**| Comment creation date. Search for result that has this parameter value greater or equal to the specified. | [optional]
 **createdColonLt** | **java.time.LocalDate**| Comment creation date. Search for result that has this parameter value less than specified. | [optional]
 **createdColonLte** | **java.time.LocalDate**| Comment creation date. Search for result that has this parameter value less or equal to the specified. | [optional]
 **modified** | **java.time.LocalDate**| Comment modification date | [optional]
 **modifiedColonGt** | **java.time.LocalDate**| Comment modification date. Search for result that has this parameter value greater than specified. | [optional]
 **modifiedColonGte** | **java.time.LocalDate**| Comment modification date. Search for result that has this parameter value greater or equal to the specified. | [optional]
 **modifiedColonLt** | **java.time.LocalDate**| Comment modification date. Search for result that has this parameter value less than specified. | [optional]
 **modifiedColonLte** | **java.time.LocalDate**| Comment modification date. Search for result that has this parameter value less or equal to the specified. | [optional]
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

val apiInstance = CommentsApi()
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
    println("4xx response calling CommentsApi#restPermissionsCommentCommentIdGet")
    e.printStackTrace()
} catch (e: ServerException) {
    println("5xx response calling CommentsApi#restPermissionsCommentCommentIdGet")
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

