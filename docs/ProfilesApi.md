# ProfilesApi

All URIs are relative to *http://localhost*

Method | HTTP request | Description
------------- | ------------- | -------------
[**restProfilesGet**](ProfilesApi.md#restProfilesGet) | **GET** /rest/profiles | List user types
[**restProfilesIdGet**](ProfilesApi.md#restProfilesIdGet) | **GET** /rest/profiles/{id} | Return user type details
[**restProfilesIdPut**](ProfilesApi.md#restProfilesIdPut) | **PUT** /rest/profiles/{id} | Update profile
[**restProfilesIdReplaceNewProfileDelete**](ProfilesApi.md#restProfilesIdReplaceNewProfileDelete) | **DELETE** /rest/profiles/{id}/replace/{new_profile} | Delete custom profile and set new profile instead of deleted profile
[**restProfilesIdUsersGet**](ProfilesApi.md#restProfilesIdUsersGet) | **GET** /rest/profiles/{id}/users | Return list of users with the specified type
[**restProfilesIdUsersPut**](ProfilesApi.md#restProfilesIdUsersPut) | **PUT** /rest/profiles/{id}/users | Change user type
[**restProfilesPost**](ProfilesApi.md#restProfilesPost) | **POST** /rest/profiles | Add custom profile


<a id="restProfilesGet"></a>
# **restProfilesGet**
> RestProfilesGet200Response restProfilesGet(name, nameColonContains, orderBy, offset, limit, with, mode)

List user types

Returns a list of user types supported by kiteworks

### Example
```kotlin
// Import classes:
//import org.openapitools.client.infrastructure.*
//import org.openapitools.client.models.*

val apiInstance = ProfilesApi()
val name : kotlin.String = name_example // kotlin.String | Profile name
val nameColonContains : kotlin.String = nameColonContains_example // kotlin.String | Profile name. Search for result that contains specified characters in this parameter.
val orderBy : kotlin.collections.List<kotlin.String> =  // kotlin.collections.List<kotlin.String> | Sorting options
val offset : kotlin.Int = 56 // kotlin.Int | Offset
val limit : kotlin.Int = 56 // kotlin.Int | Limit
val with : kotlin.String = with_example // kotlin.String | With parameters
val mode : kotlin.String = mode_example // kotlin.String | Response mode
try {
    val result : RestProfilesGet200Response = apiInstance.restProfilesGet(name, nameColonContains, orderBy, offset, limit, with, mode)
    println(result)
} catch (e: ClientException) {
    println("4xx response calling ProfilesApi#restProfilesGet")
    e.printStackTrace()
} catch (e: ServerException) {
    println("5xx response calling ProfilesApi#restProfilesGet")
    e.printStackTrace()
}
```

### Parameters

Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **name** | **kotlin.String**| Profile name | [optional]
 **nameColonContains** | **kotlin.String**| Profile name. Search for result that contains specified characters in this parameter. | [optional]
 **orderBy** | [**kotlin.collections.List&lt;kotlin.String&gt;**](kotlin.String.md)| Sorting options | [optional]
 **offset** | **kotlin.Int**| Offset | [optional]
 **limit** | **kotlin.Int**| Limit | [optional]
 **with** | **kotlin.String**| With parameters | [optional]
 **mode** | **kotlin.String**| Response mode | [optional]

### Return type

[**RestProfilesGet200Response**](RestProfilesGet200Response.md)

### Authorization

No authorization required

### HTTP request headers

 - **Content-Type**: Not defined
 - **Accept**: */*

<a id="restProfilesIdGet"></a>
# **restProfilesIdGet**
> Profile restProfilesIdGet(id)

Return user type details

Returns the details of a specified user type. e.g.: Returns user type id and name.

### Example
```kotlin
// Import classes:
//import org.openapitools.client.infrastructure.*
//import org.openapitools.client.models.*

val apiInstance = ProfilesApi()
val id : kotlin.Int = 56 // kotlin.Int | ID of the user type to be retrieved
try {
    val result : Profile = apiInstance.restProfilesIdGet(id)
    println(result)
} catch (e: ClientException) {
    println("4xx response calling ProfilesApi#restProfilesIdGet")
    e.printStackTrace()
} catch (e: ServerException) {
    println("5xx response calling ProfilesApi#restProfilesIdGet")
    e.printStackTrace()
}
```

### Parameters

Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **id** | **kotlin.Int**| ID of the user type to be retrieved |

### Return type

[**Profile**](Profile.md)

### Authorization

No authorization required

### HTTP request headers

 - **Content-Type**: Not defined
 - **Accept**: */*

<a id="restProfilesIdPut"></a>
# **restProfilesIdPut**
> restProfilesIdPut(id, body)

Update profile

Update existing profile, Remove/Retain users data if Profile has no Collaboration Access

### Example
```kotlin
// Import classes:
//import org.openapitools.client.infrastructure.*
//import org.openapitools.client.models.*

val apiInstance = ProfilesApi()
val id : kotlin.Int = 56 // kotlin.Int | Id of the profile to be modified
val body : FeaturesListPut =  // FeaturesListPut | Features of the profile
try {
    apiInstance.restProfilesIdPut(id, body)
} catch (e: ClientException) {
    println("4xx response calling ProfilesApi#restProfilesIdPut")
    e.printStackTrace()
} catch (e: ServerException) {
    println("5xx response calling ProfilesApi#restProfilesIdPut")
    e.printStackTrace()
}
```

### Parameters

Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **id** | **kotlin.Int**| Id of the profile to be modified |
 **body** | [**FeaturesListPut**](FeaturesListPut.md)| Features of the profile |

### Return type

null (empty response body)

### Authorization

No authorization required

### HTTP request headers

 - **Content-Type**: Not defined
 - **Accept**: Not defined

<a id="restProfilesIdReplaceNewProfileDelete"></a>
# **restProfilesIdReplaceNewProfileDelete**
> restProfilesIdReplaceNewProfileDelete(id, newProfile, body)

Delete custom profile and set new profile instead of deleted profile

Delete custom profile and set new profile instead of deleted profile

### Example
```kotlin
// Import classes:
//import org.openapitools.client.infrastructure.*
//import org.openapitools.client.models.*

val apiInstance = ProfilesApi()
val id : kotlin.Int = 56 // kotlin.Int | Id of the custom profile to be deleted
val newProfile : kotlin.Int = 56 // kotlin.Int | Id of the new profile to be assigned for affected users
val body : UserDemoteOptionsPost =  // UserDemoteOptionsPost | The demotion options
try {
    apiInstance.restProfilesIdReplaceNewProfileDelete(id, newProfile, body)
} catch (e: ClientException) {
    println("4xx response calling ProfilesApi#restProfilesIdReplaceNewProfileDelete")
    e.printStackTrace()
} catch (e: ServerException) {
    println("5xx response calling ProfilesApi#restProfilesIdReplaceNewProfileDelete")
    e.printStackTrace()
}
```

### Parameters

Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **id** | **kotlin.Int**| Id of the custom profile to be deleted |
 **newProfile** | **kotlin.Int**| Id of the new profile to be assigned for affected users |
 **body** | [**UserDemoteOptionsPost**](UserDemoteOptionsPost.md)| The demotion options | [optional]

### Return type

null (empty response body)

### Authorization

No authorization required

### HTTP request headers

 - **Content-Type**: Not defined
 - **Accept**: Not defined

<a id="restProfilesIdUsersGet"></a>
# **restProfilesIdUsersGet**
> kotlin.collections.List&lt;User&gt; restProfilesIdUsersGet(id, email, emailColonContains, name, nameColonContains, metadata, metadataContains, deleted, active, verified, suspended, isRecipient, allowsCollaboration, created, createdColonGt, createdColonGte, createdColonLt, createdColonLte, orderBy, offset, limit, locateId, with, mode)

Return list of users with the specified type

Returns the list of users who have the specified type. e.g.:                   Return me the user names and email addresses of all the Restricted Users.

### Example
```kotlin
// Import classes:
//import org.openapitools.client.infrastructure.*
//import org.openapitools.client.models.*

val apiInstance = ProfilesApi()
val id : kotlin.Int = 56 // kotlin.Int | ID of the user type to retrieve users for
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
    val result : kotlin.collections.List<User> = apiInstance.restProfilesIdUsersGet(id, email, emailColonContains, name, nameColonContains, metadata, metadataContains, deleted, active, verified, suspended, isRecipient, allowsCollaboration, created, createdColonGt, createdColonGte, createdColonLt, createdColonLte, orderBy, offset, limit, locateId, with, mode)
    println(result)
} catch (e: ClientException) {
    println("4xx response calling ProfilesApi#restProfilesIdUsersGet")
    e.printStackTrace()
} catch (e: ServerException) {
    println("5xx response calling ProfilesApi#restProfilesIdUsersGet")
    e.printStackTrace()
}
```

### Parameters

Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **id** | **kotlin.Int**| ID of the user type to retrieve users for |
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

<a id="restProfilesIdUsersPut"></a>
# **restProfilesIdUsersPut**
> restProfilesIdUsersPut(id, idColonIn, mode, body)

Change user type

Change user type for specified user

### Example
```kotlin
// Import classes:
//import org.openapitools.client.infrastructure.*
//import org.openapitools.client.models.*

val apiInstance = ProfilesApi()
val id : kotlin.Int = 56 // kotlin.Int | ID of the user type
val idColonIn : kotlin.String = idColonIn_example // kotlin.String | IDs of users, who are going to be assigned to the user type
val mode : kotlin.String = mode_example // kotlin.String | Response mode
val body : UserDemoteOptionsPost =  // UserDemoteOptionsPost | The users details
try {
    apiInstance.restProfilesIdUsersPut(id, idColonIn, mode, body)
} catch (e: ClientException) {
    println("4xx response calling ProfilesApi#restProfilesIdUsersPut")
    e.printStackTrace()
} catch (e: ServerException) {
    println("5xx response calling ProfilesApi#restProfilesIdUsersPut")
    e.printStackTrace()
}
```

### Parameters

Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **id** | **kotlin.Int**| ID of the user type |
 **idColonIn** | **kotlin.String**| IDs of users, who are going to be assigned to the user type |
 **mode** | **kotlin.String**| Response mode | [optional]
 **body** | [**UserDemoteOptionsPost**](UserDemoteOptionsPost.md)| The users details | [optional]

### Return type

null (empty response body)

### Authorization

No authorization required

### HTTP request headers

 - **Content-Type**: Not defined
 - **Accept**: Not defined

<a id="restProfilesPost"></a>
# **restProfilesPost**
> restProfilesPost(body, returnEntity, mode)

Add custom profile

Add new custom profile cloned from built in profile

### Example
```kotlin
// Import classes:
//import org.openapitools.client.infrastructure.*
//import org.openapitools.client.models.*

val apiInstance = ProfilesApi()
val body : ProfilePost =  // ProfilePost | Params for custom profile
val returnEntity : kotlin.Boolean = true // kotlin.Boolean | Return information about newly created entity
val mode : kotlin.String = mode_example // kotlin.String | Response mode
try {
    apiInstance.restProfilesPost(body, returnEntity, mode)
} catch (e: ClientException) {
    println("4xx response calling ProfilesApi#restProfilesPost")
    e.printStackTrace()
} catch (e: ServerException) {
    println("5xx response calling ProfilesApi#restProfilesPost")
    e.printStackTrace()
}
```

### Parameters

Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **body** | [**ProfilePost**](ProfilePost.md)| Params for custom profile |
 **returnEntity** | **kotlin.Boolean**| Return information about newly created entity | [optional]
 **mode** | **kotlin.String**| Response mode | [optional]

### Return type

null (empty response body)

### Authorization

No authorization required

### HTTP request headers

 - **Content-Type**: Not defined
 - **Accept**: Not defined

