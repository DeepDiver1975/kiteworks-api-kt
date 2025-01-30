# NotificationsApi

All URIs are relative to *http://localhost*

Method | HTTP request | Description
------------- | ------------- | -------------
[**restFoldersIdActionsSetNotificationsPut**](NotificationsApi.md#restFoldersIdActionsSetNotificationsPut) | **PUT** /rest/folders/{id}/actions/setNotifications | Set/Update notifications
[**restNotificationsGet**](NotificationsApi.md#restNotificationsGet) | **GET** /rest/notifications | List notifications
[**restNotificationsObjectIdDelete**](NotificationsApi.md#restNotificationsObjectIdDelete) | **DELETE** /rest/notifications/{object_id} | Remove notification options


<a id="restFoldersIdActionsSetNotificationsPut"></a>
# **restFoldersIdActionsSetNotificationsPut**
> restFoldersIdActionsSetNotificationsPut(id, body, includeNested, offset, limit, mode)

Set/Update notifications

Set/Update notifications

### Example
```kotlin
// Import classes:
//import org.openapitools.client.infrastructure.*
//import org.openapitools.client.models.*

val apiInstance = NotificationsApi()
val id : kotlin.String = id_example // kotlin.String | ID of the folder
val body : UserNotificationPost =  // UserNotificationPost | Notification options
val includeNested : kotlin.Boolean = true // kotlin.Boolean | Set notification for nested folders as well
val offset : kotlin.Int = 56 // kotlin.Int | Offset
val limit : kotlin.Int = 56 // kotlin.Int | Limit
val mode : kotlin.String = mode_example // kotlin.String | Response mode
try {
    apiInstance.restFoldersIdActionsSetNotificationsPut(id, body, includeNested, offset, limit, mode)
} catch (e: ClientException) {
    println("4xx response calling NotificationsApi#restFoldersIdActionsSetNotificationsPut")
    e.printStackTrace()
} catch (e: ServerException) {
    println("5xx response calling NotificationsApi#restFoldersIdActionsSetNotificationsPut")
    e.printStackTrace()
}
```

### Parameters

Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **id** | **kotlin.String**| ID of the folder |
 **body** | [**UserNotificationPost**](UserNotificationPost.md)| Notification options |
 **includeNested** | **kotlin.Boolean**| Set notification for nested folders as well | [optional]
 **offset** | **kotlin.Int**| Offset | [optional]
 **limit** | **kotlin.Int**| Limit | [optional]
 **mode** | **kotlin.String**| Response mode | [optional]

### Return type

null (empty response body)

### Authorization

No authorization required

### HTTP request headers

 - **Content-Type**: Not defined
 - **Accept**: Not defined

<a id="restNotificationsGet"></a>
# **restNotificationsGet**
> kotlin.collections.List&lt;UserNotification&gt; restNotificationsGet(userId, userIdColonIn, objectId, objectIdColonIn, fileAdded, commentAdded, orderBy, offset, limit, with, mode)

List notifications

Returns list of notifications

### Example
```kotlin
// Import classes:
//import org.openapitools.client.infrastructure.*
//import org.openapitools.client.models.*

val apiInstance = NotificationsApi()
val userId : kotlin.String = userId_example // kotlin.String | ID of user who will send email notifications to end users
val userIdColonIn : kotlin.String = userIdColonIn_example // kotlin.String | ID of user who will send email notifications to end users. Search for results that contain any of specified values of this parameter.
val objectId : kotlin.String = objectId_example // kotlin.String | Id of folder included in Notification
val objectIdColonIn : kotlin.String = objectIdColonIn_example // kotlin.String | Id of folder included in Notification. Search for results that contain any of specified values of this parameter.
val fileAdded : kotlin.Boolean = true // kotlin.Boolean | Whether the notification is about the file added
val commentAdded : kotlin.Boolean = true // kotlin.Boolean | Whether the notification is about the comment added
val orderBy : kotlin.collections.List<kotlin.String> =  // kotlin.collections.List<kotlin.String> | Sorting options
val offset : kotlin.Int = 56 // kotlin.Int | Offset
val limit : kotlin.Int = 56 // kotlin.Int | Limit
val with : kotlin.String = with_example // kotlin.String | With parameters
val mode : kotlin.String = mode_example // kotlin.String | Response mode
try {
    val result : kotlin.collections.List<UserNotification> = apiInstance.restNotificationsGet(userId, userIdColonIn, objectId, objectIdColonIn, fileAdded, commentAdded, orderBy, offset, limit, with, mode)
    println(result)
} catch (e: ClientException) {
    println("4xx response calling NotificationsApi#restNotificationsGet")
    e.printStackTrace()
} catch (e: ServerException) {
    println("5xx response calling NotificationsApi#restNotificationsGet")
    e.printStackTrace()
}
```

### Parameters

Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **userId** | **kotlin.String**| ID of user who will send email notifications to end users | [optional]
 **userIdColonIn** | **kotlin.String**| ID of user who will send email notifications to end users. Search for results that contain any of specified values of this parameter. | [optional]
 **objectId** | **kotlin.String**| Id of folder included in Notification | [optional]
 **objectIdColonIn** | **kotlin.String**| Id of folder included in Notification. Search for results that contain any of specified values of this parameter. | [optional]
 **fileAdded** | **kotlin.Boolean**| Whether the notification is about the file added | [optional]
 **commentAdded** | **kotlin.Boolean**| Whether the notification is about the comment added | [optional]
 **orderBy** | [**kotlin.collections.List&lt;kotlin.String&gt;**](kotlin.String.md)| Sorting options | [optional]
 **offset** | **kotlin.Int**| Offset | [optional]
 **limit** | **kotlin.Int**| Limit | [optional]
 **with** | **kotlin.String**| With parameters | [optional]
 **mode** | **kotlin.String**| Response mode | [optional]

### Return type

[**kotlin.collections.List&lt;UserNotification&gt;**](UserNotification.md)

### Authorization

No authorization required

### HTTP request headers

 - **Content-Type**: Not defined
 - **Accept**: */*

<a id="restNotificationsObjectIdDelete"></a>
# **restNotificationsObjectIdDelete**
> restNotificationsObjectIdDelete(objectId)

Remove notification options

Remove notification option

### Example
```kotlin
// Import classes:
//import org.openapitools.client.infrastructure.*
//import org.openapitools.client.models.*

val apiInstance = NotificationsApi()
val objectId : kotlin.Int = 56 // kotlin.Int | Object ID of the folder to remove notification options
try {
    apiInstance.restNotificationsObjectIdDelete(objectId)
} catch (e: ClientException) {
    println("4xx response calling NotificationsApi#restNotificationsObjectIdDelete")
    e.printStackTrace()
} catch (e: ServerException) {
    println("5xx response calling NotificationsApi#restNotificationsObjectIdDelete")
    e.printStackTrace()
}
```

### Parameters

Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **objectId** | **kotlin.Int**| Object ID of the folder to remove notification options |

### Return type

null (empty response body)

### Authorization

No authorization required

### HTTP request headers

 - **Content-Type**: Not defined
 - **Accept**: Not defined

