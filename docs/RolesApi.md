# RolesApi

All URIs are relative to *http://localhost*

Method | HTTP request | Description
------------- | ------------- | -------------
[**restRolesGet**](RolesApi.md#restRolesGet) | **GET** /rest/roles | List user roles
[**restRolesIdGet**](RolesApi.md#restRolesIdGet) | **GET** /rest/roles/{id} | Get a role


<a id="restRolesGet"></a>
# **restRolesGet**
> kotlin.collections.List&lt;Role&gt; restRolesGet(name, nameColonContains, disabled, type, orderBy, with, mode)

List user roles

Returns a list of available user roles. e.g.:                    kiteworks default roles are Manager, Collaborator, Downloader, Viewer, Uploader.

### Example
```kotlin
// Import classes:
//import org.openapitools.client.infrastructure.*
//import org.openapitools.client.models.*

val apiInstance = RolesApi()
val name : kotlin.String = name_example // kotlin.String | Role name
val nameColonContains : kotlin.String = nameColonContains_example // kotlin.String | Role name. Search for result that contains specified characters in this parameter.
val disabled : kotlin.Boolean = true // kotlin.Boolean | Whether Role is disabled
val type : kotlin.String = type_example // kotlin.String | Type of role
val orderBy : kotlin.collections.List<kotlin.String> =  // kotlin.collections.List<kotlin.String> | Sorting options
val with : kotlin.String = with_example // kotlin.String | With parameters
val mode : kotlin.String = mode_example // kotlin.String | Response mode
try {
    val result : kotlin.collections.List<Role> = apiInstance.restRolesGet(name, nameColonContains, disabled, type, orderBy, with, mode)
    println(result)
} catch (e: ClientException) {
    println("4xx response calling RolesApi#restRolesGet")
    e.printStackTrace()
} catch (e: ServerException) {
    println("5xx response calling RolesApi#restRolesGet")
    e.printStackTrace()
}
```

### Parameters

Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **name** | **kotlin.String**| Role name | [optional]
 **nameColonContains** | **kotlin.String**| Role name. Search for result that contains specified characters in this parameter. | [optional]
 **disabled** | **kotlin.Boolean**| Whether Role is disabled | [optional]
 **type** | **kotlin.String**| Type of role | [optional]
 **orderBy** | [**kotlin.collections.List&lt;kotlin.String&gt;**](kotlin.String.md)| Sorting options | [optional]
 **with** | **kotlin.String**| With parameters | [optional]
 **mode** | **kotlin.String**| Response mode | [optional]

### Return type

[**kotlin.collections.List&lt;Role&gt;**](Role.md)

### Authorization

No authorization required

### HTTP request headers

 - **Content-Type**: Not defined
 - **Accept**: */*

<a id="restRolesIdGet"></a>
# **restRolesIdGet**
> Role restRolesIdGet(id)

Get a role

Returns the details of a specified role including the mask that indicates                   what functionality this role is allowed to do.

### Example
```kotlin
// Import classes:
//import org.openapitools.client.infrastructure.*
//import org.openapitools.client.models.*

val apiInstance = RolesApi()
val id : kotlin.Int = 56 // kotlin.Int | ID of the role to be retrieved
try {
    val result : Role = apiInstance.restRolesIdGet(id)
    println(result)
} catch (e: ClientException) {
    println("4xx response calling RolesApi#restRolesIdGet")
    e.printStackTrace()
} catch (e: ServerException) {
    println("5xx response calling RolesApi#restRolesIdGet")
    e.printStackTrace()
}
```

### Parameters

Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **id** | **kotlin.Int**| ID of the role to be retrieved |

### Return type

[**Role**](Role.md)

### Authorization

No authorization required

### HTTP request headers

 - **Content-Type**: Not defined
 - **Accept**: */*

