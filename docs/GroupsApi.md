# GroupsApi

All URIs are relative to *http://localhost*

Method | HTTP request | Description
------------- | ------------- | -------------
[**restGroupsGet**](GroupsApi.md#restGroupsGet) | **GET** /rest/groups | List kiteworks groups
[**restGroupsIdDelete**](GroupsApi.md#restGroupsIdDelete) | **DELETE** /rest/groups/{id} | Deletes a group entry
[**restGroupsIdGet**](GroupsApi.md#restGroupsIdGet) | **GET** /rest/groups/{id} | Return users for the specified group
[**restGroupsIdPut**](GroupsApi.md#restGroupsIdPut) | **PUT** /rest/groups/{id} | Update a group entry
[**restGroupsPost**](GroupsApi.md#restGroupsPost) | **POST** /rest/groups | Create a group entry


<a id="restGroupsGet"></a>
# **restGroupsGet**
> ContactList restGroupsGet(nameColonContains, name, limit, orderBy, offset)

List kiteworks groups

Returns the list of kiteworks groups for this user, including the email address of each member in the group.

### Example
```kotlin
// Import classes:
//import org.openapitools.client.infrastructure.*
//import org.openapitools.client.models.*

val apiInstance = GroupsApi()
val nameColonContains : kotlin.String = nameColonContains_example // kotlin.String | 
val name : kotlin.String = name_example // kotlin.String | 
val limit : kotlin.Int = 56 // kotlin.Int | limit
val orderBy : kotlin.String = orderBy_example // kotlin.String | Sorting options. Accepts id, name. Sample format is id:asc
val offset : kotlin.Int = 56 // kotlin.Int | offset
try {
    val result : ContactList = apiInstance.restGroupsGet(nameColonContains, name, limit, orderBy, offset)
    println(result)
} catch (e: ClientException) {
    println("4xx response calling GroupsApi#restGroupsGet")
    e.printStackTrace()
} catch (e: ServerException) {
    println("5xx response calling GroupsApi#restGroupsGet")
    e.printStackTrace()
}
```

### Parameters

Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **nameColonContains** | **kotlin.String**|  | [optional]
 **name** | **kotlin.String**|  | [optional]
 **limit** | **kotlin.Int**| limit | [optional]
 **orderBy** | **kotlin.String**| Sorting options. Accepts id, name. Sample format is id:asc | [optional]
 **offset** | **kotlin.Int**| offset | [optional]

### Return type

[**ContactList**](ContactList.md)

### Authorization

No authorization required

### HTTP request headers

 - **Content-Type**: Not defined
 - **Accept**: */*

<a id="restGroupsIdDelete"></a>
# **restGroupsIdDelete**
> restGroupsIdDelete(id)

Deletes a group entry

Delete a group

### Example
```kotlin
// Import classes:
//import org.openapitools.client.infrastructure.*
//import org.openapitools.client.models.*

val apiInstance = GroupsApi()
val id : kotlin.Int = 56 // kotlin.Int | The ID of the entity
try {
    apiInstance.restGroupsIdDelete(id)
} catch (e: ClientException) {
    println("4xx response calling GroupsApi#restGroupsIdDelete")
    e.printStackTrace()
} catch (e: ServerException) {
    println("5xx response calling GroupsApi#restGroupsIdDelete")
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

<a id="restGroupsIdGet"></a>
# **restGroupsIdGet**
> Contact restGroupsIdGet(id)

Return users for the specified group

Returns the list of users for the specified group.

### Example
```kotlin
// Import classes:
//import org.openapitools.client.infrastructure.*
//import org.openapitools.client.models.*

val apiInstance = GroupsApi()
val id : kotlin.Int = 56 // kotlin.Int | The ID of the entity
try {
    val result : Contact = apiInstance.restGroupsIdGet(id)
    println(result)
} catch (e: ClientException) {
    println("4xx response calling GroupsApi#restGroupsIdGet")
    e.printStackTrace()
} catch (e: ServerException) {
    println("5xx response calling GroupsApi#restGroupsIdGet")
    e.printStackTrace()
}
```

### Parameters

Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **id** | **kotlin.Int**| The ID of the entity |

### Return type

[**Contact**](Contact.md)

### Authorization

No authorization required

### HTTP request headers

 - **Content-Type**: Not defined
 - **Accept**: */*

<a id="restGroupsIdPut"></a>
# **restGroupsIdPut**
> restGroupsIdPut(id)

Update a group entry

Update a group

### Example
```kotlin
// Import classes:
//import org.openapitools.client.infrastructure.*
//import org.openapitools.client.models.*

val apiInstance = GroupsApi()
val id : kotlin.Int = 56 // kotlin.Int | The ID of the entity
try {
    apiInstance.restGroupsIdPut(id)
} catch (e: ClientException) {
    println("4xx response calling GroupsApi#restGroupsIdPut")
    e.printStackTrace()
} catch (e: ServerException) {
    println("5xx response calling GroupsApi#restGroupsIdPut")
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

<a id="restGroupsPost"></a>
# **restGroupsPost**
> Contact restGroupsPost(body)

Create a group entry

Create a group of users

### Example
```kotlin
// Import classes:
//import org.openapitools.client.infrastructure.*
//import org.openapitools.client.models.*

val apiInstance = GroupsApi()
val body : GroupCreate =  // GroupCreate | 
try {
    val result : Contact = apiInstance.restGroupsPost(body)
    println(result)
} catch (e: ClientException) {
    println("4xx response calling GroupsApi#restGroupsPost")
    e.printStackTrace()
} catch (e: ServerException) {
    println("5xx response calling GroupsApi#restGroupsPost")
    e.printStackTrace()
}
```

### Parameters

Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **body** | [**GroupCreate**](GroupCreate.md)|  |

### Return type

[**Contact**](Contact.md)

### Authorization

No authorization required

### HTTP request headers

 - **Content-Type**: Not defined
 - **Accept**: */*

