# AdminRolesApi

All URIs are relative to *http://localhost*

Method | HTTP request | Description
------------- | ------------- | -------------
[**restAdminRolesGet**](AdminRolesApi.md#restAdminRolesGet) | **GET** /rest/adminRoles | List admin roles
[**restAdminRolesIdGet**](AdminRolesApi.md#restAdminRolesIdGet) | **GET** /rest/adminRoles/{id} | Return an admin role
[**restAdminRolesIdUsersGet**](AdminRolesApi.md#restAdminRolesIdUsersGet) | **GET** /rest/adminRoles/{id}/users | Return list of users with the specified admin role
[**restAdminRolesIdUsersUserIdDelete**](AdminRolesApi.md#restAdminRolesIdUsersUserIdDelete) | **DELETE** /rest/adminRoles/{id}/users/{user_id} | Delete a user as admin role
[**restAdminRolesIdUsersUserIdPut**](AdminRolesApi.md#restAdminRolesIdUsersUserIdPut) | **PUT** /rest/adminRoles/{id}/users/{user_id} | Promote a user as admin role


<a id="restAdminRolesGet"></a>
# **restAdminRolesGet**
> kotlin.collections.List&lt;AdminRole&gt; restAdminRolesGet(orderBy, with, mode)

List admin roles

Returns a list of admin roles supported by kiteworks. e.g.:                   Today we return Application and System

### Example
```kotlin
// Import classes:
//import org.openapitools.client.infrastructure.*
//import org.openapitools.client.models.*

val apiInstance = AdminRolesApi()
val orderBy : kotlin.collections.List<kotlin.String> =  // kotlin.collections.List<kotlin.String> | Sorting options
val with : kotlin.String = with_example // kotlin.String | With parameters
val mode : kotlin.String = mode_example // kotlin.String | Response mode
try {
    val result : kotlin.collections.List<AdminRole> = apiInstance.restAdminRolesGet(orderBy, with, mode)
    println(result)
} catch (e: ClientException) {
    println("4xx response calling AdminRolesApi#restAdminRolesGet")
    e.printStackTrace()
} catch (e: ServerException) {
    println("5xx response calling AdminRolesApi#restAdminRolesGet")
    e.printStackTrace()
}
```

### Parameters

Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **orderBy** | [**kotlin.collections.List&lt;kotlin.String&gt;**](kotlin.String.md)| Sorting options | [optional]
 **with** | **kotlin.String**| With parameters | [optional]
 **mode** | **kotlin.String**| Response mode | [optional]

### Return type

[**kotlin.collections.List&lt;AdminRole&gt;**](AdminRole.md)

### Authorization

No authorization required

### HTTP request headers

 - **Content-Type**: Not defined
 - **Accept**: */*

<a id="restAdminRolesIdGet"></a>
# **restAdminRolesIdGet**
> AdminRole restAdminRolesIdGet(id)

Return an admin role

Returns the details of a specified admin role. e.g.: Returns id and admin role name.

### Example
```kotlin
// Import classes:
//import org.openapitools.client.infrastructure.*
//import org.openapitools.client.models.*

val apiInstance = AdminRolesApi()
val id : kotlin.Int = 56 // kotlin.Int | ID of the adminrole to be retrieved
try {
    val result : AdminRole = apiInstance.restAdminRolesIdGet(id)
    println(result)
} catch (e: ClientException) {
    println("4xx response calling AdminRolesApi#restAdminRolesIdGet")
    e.printStackTrace()
} catch (e: ServerException) {
    println("5xx response calling AdminRolesApi#restAdminRolesIdGet")
    e.printStackTrace()
}
```

### Parameters

Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **id** | **kotlin.Int**| ID of the adminrole to be retrieved |

### Return type

[**AdminRole**](AdminRole.md)

### Authorization

No authorization required

### HTTP request headers

 - **Content-Type**: Not defined
 - **Accept**: */*

<a id="restAdminRolesIdUsersGet"></a>
# **restAdminRolesIdUsersGet**
> kotlin.collections.List&lt;User&gt; restAdminRolesIdUsersGet(id, email, emailColonContains, name, nameColonContains, metadata, metadataContains, deleted, active, verified, suspended, isRecipient, allowsCollaboration, created, createdColonGt, createdColonGte, createdColonLt, createdColonLte, orderBy, offset, limit, locateId, with, mode)

Return list of users with the specified admin role

Returns the list of admins who have the specified role. e.g.:                   Return me the user names and email addresses of all the Application admins.

### Example
```kotlin
// Import classes:
//import org.openapitools.client.infrastructure.*
//import org.openapitools.client.models.*

val apiInstance = AdminRolesApi()
val id : kotlin.Int = 56 // kotlin.Int | ID of the admin role to retrieve users for
val email : kotlin.String = email_example // kotlin.String | The user's email
val emailColonContains : kotlin.String = emailColonContains_example // kotlin.String | The user's email. Search for result that contains specified characters in this parameter.
val name : kotlin.String = name_example // kotlin.String | The name of the user
val nameColonContains : kotlin.String = nameColonContains_example // kotlin.String | The name of the user. Search for result that contains specified characters in this parameter.
val metadata : kotlin.String = metadata_example // kotlin.String | The metadata of the user
val metadataContains : kotlin.String = metadataContains_example // kotlin.String | The metadata of the user. Search for result that contains specified characters in this parameter.
val deleted : kotlin.Boolean = true // kotlin.Boolean | Whether the user has been deleted
val active : kotlin.Boolean = true // kotlin.Boolean | Whether the user is an actual kitework user
val verified : kotlin.Boolean = true // kotlin.Boolean | Whether the user is verified
val suspended : kotlin.Boolean = true // kotlin.Boolean | Whether the user is suspended
val isRecipient : kotlin.Boolean = true // kotlin.Boolean | Whether user is recipient
val allowsCollaboration : kotlin.Boolean = true // kotlin.Boolean | Whether user's profile allows collaboration access
val created : kotlin.String = 2013-10-20 // kotlin.String | User creation date
val createdColonGt : kotlin.String = 2013-10-20 // kotlin.String | User creation date. Search for result that has this parameter value greater than specified.
val createdColonGte : kotlin.String = 2013-10-20 // kotlin.String | User creation date. Search for result that has this parameter value greater or equal to the specified.
val createdColonLt : kotlin.String = 2013-10-20 // kotlin.String | User creation date. Search for result that has this parameter value less than specified.
val createdColonLte : kotlin.String = 2013-10-20 // kotlin.String | User creation date. Search for result that has this parameter value less or equal to the specified.
val orderBy : kotlin.collections.List<kotlin.String> =  // kotlin.collections.List<kotlin.String> | Sorting options
val offset : kotlin.Int = 56 // kotlin.Int | Offset
val limit : kotlin.Int = 56 // kotlin.Int | Limit
val locateId : kotlin.Int = 56 // kotlin.Int | If specified, \"offset\" parameter will be ignored                                             and the page containing entity with this Id will be returned.
val with : kotlin.String = with_example // kotlin.String | With parameters
val mode : kotlin.String = mode_example // kotlin.String | Response mode
try {
    val result : kotlin.collections.List<User> = apiInstance.restAdminRolesIdUsersGet(id, email, emailColonContains, name, nameColonContains, metadata, metadataContains, deleted, active, verified, suspended, isRecipient, allowsCollaboration, created, createdColonGt, createdColonGte, createdColonLt, createdColonLte, orderBy, offset, limit, locateId, with, mode)
    println(result)
} catch (e: ClientException) {
    println("4xx response calling AdminRolesApi#restAdminRolesIdUsersGet")
    e.printStackTrace()
} catch (e: ServerException) {
    println("5xx response calling AdminRolesApi#restAdminRolesIdUsersGet")
    e.printStackTrace()
}
```

### Parameters

Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **id** | **kotlin.Int**| ID of the admin role to retrieve users for |
 **email** | **kotlin.String**| The user&#39;s email | [optional]
 **emailColonContains** | **kotlin.String**| The user&#39;s email. Search for result that contains specified characters in this parameter. | [optional]
 **name** | **kotlin.String**| The name of the user | [optional]
 **nameColonContains** | **kotlin.String**| The name of the user. Search for result that contains specified characters in this parameter. | [optional]
 **metadata** | **kotlin.String**| The metadata of the user | [optional]
 **metadataContains** | **kotlin.String**| The metadata of the user. Search for result that contains specified characters in this parameter. | [optional]
 **deleted** | **kotlin.Boolean**| Whether the user has been deleted | [optional]
 **active** | **kotlin.Boolean**| Whether the user is an actual kitework user | [optional]
 **verified** | **kotlin.Boolean**| Whether the user is verified | [optional]
 **suspended** | **kotlin.Boolean**| Whether the user is suspended | [optional]
 **isRecipient** | **kotlin.Boolean**| Whether user is recipient | [optional]
 **allowsCollaboration** | **kotlin.Boolean**| Whether user&#39;s profile allows collaboration access | [optional]
 **created** | **kotlin.String**| User creation date | [optional]
 **createdColonGt** | **kotlin.String**| User creation date. Search for result that has this parameter value greater than specified. | [optional]
 **createdColonGte** | **kotlin.String**| User creation date. Search for result that has this parameter value greater or equal to the specified. | [optional]
 **createdColonLt** | **kotlin.String**| User creation date. Search for result that has this parameter value less than specified. | [optional]
 **createdColonLte** | **kotlin.String**| User creation date. Search for result that has this parameter value less or equal to the specified. | [optional]
 **orderBy** | [**kotlin.collections.List&lt;kotlin.String&gt;**](kotlin.String.md)| Sorting options | [optional]
 **offset** | **kotlin.Int**| Offset | [optional]
 **limit** | **kotlin.Int**| Limit | [optional]
 **locateId** | **kotlin.Int**| If specified, \&quot;offset\&quot; parameter will be ignored                                             and the page containing entity with this Id will be returned. | [optional]
 **with** | **kotlin.String**| With parameters | [optional]
 **mode** | **kotlin.String**| Response mode | [optional]

### Return type

[**kotlin.collections.List&lt;User&gt;**](User.md)

### Authorization

No authorization required

### HTTP request headers

 - **Content-Type**: Not defined
 - **Accept**: */*

<a id="restAdminRolesIdUsersUserIdDelete"></a>
# **restAdminRolesIdUsersUserIdDelete**
> restAdminRolesIdUsersUserIdDelete(id, userId)

Delete a user as admin role

Delete a user as admin role.                   This method does not delete the user but only the role of admin for that user.

### Example
```kotlin
// Import classes:
//import org.openapitools.client.infrastructure.*
//import org.openapitools.client.models.*

val apiInstance = AdminRolesApi()
val id : kotlin.Int = 56 // kotlin.Int | ID of the admin role to remove from the specified user.
val userId : kotlin.String = userId_example // kotlin.String | ID of the user as admin role to be deleted
try {
    apiInstance.restAdminRolesIdUsersUserIdDelete(id, userId)
} catch (e: ClientException) {
    println("4xx response calling AdminRolesApi#restAdminRolesIdUsersUserIdDelete")
    e.printStackTrace()
} catch (e: ServerException) {
    println("5xx response calling AdminRolesApi#restAdminRolesIdUsersUserIdDelete")
    e.printStackTrace()
}
```

### Parameters

Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **id** | **kotlin.Int**| ID of the admin role to remove from the specified user. |
 **userId** | **kotlin.String**| ID of the user as admin role to be deleted |

### Return type

null (empty response body)

### Authorization

No authorization required

### HTTP request headers

 - **Content-Type**: Not defined
 - **Accept**: Not defined

<a id="restAdminRolesIdUsersUserIdPut"></a>
# **restAdminRolesIdUsersUserIdPut**
> restAdminRolesIdUsersUserIdPut(id, userId)

Promote a user as admin role

Promote a user to include an admin role. The user will become a system or application admin.

### Example
```kotlin
// Import classes:
//import org.openapitools.client.infrastructure.*
//import org.openapitools.client.models.*

val apiInstance = AdminRolesApi()
val id : kotlin.Int = 56 // kotlin.Int | ID of the Admin role
val userId : kotlin.String = userId_example // kotlin.String | ID of user to promote admin role
try {
    apiInstance.restAdminRolesIdUsersUserIdPut(id, userId)
} catch (e: ClientException) {
    println("4xx response calling AdminRolesApi#restAdminRolesIdUsersUserIdPut")
    e.printStackTrace()
} catch (e: ServerException) {
    println("5xx response calling AdminRolesApi#restAdminRolesIdUsersUserIdPut")
    e.printStackTrace()
}
```

### Parameters

Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **id** | **kotlin.Int**| ID of the Admin role |
 **userId** | **kotlin.String**| ID of user to promote admin role |

### Return type

null (empty response body)

### Authorization

No authorization required

### HTTP request headers

 - **Content-Type**: Not defined
 - **Accept**: Not defined

