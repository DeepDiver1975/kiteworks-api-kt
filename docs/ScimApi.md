# ScimApi

All URIs are relative to *http://localhost*

Method | HTTP request | Description
------------- | ------------- | -------------
[**restScimResourceTypesGet**](ScimApi.md#restScimResourceTypesGet) | **GET** /rest/scim/ResourceTypes | 
[**restScimResourceTypesIdGet**](ScimApi.md#restScimResourceTypesIdGet) | **GET** /rest/scim/ResourceTypes/{id} | 
[**restScimSchemasGet**](ScimApi.md#restScimSchemasGet) | **GET** /rest/scim/Schemas | 
[**restScimSchemasIdGet**](ScimApi.md#restScimSchemasIdGet) | **GET** /rest/scim/Schemas/{id} | 
[**restScimServiceProviderConfigGet**](ScimApi.md#restScimServiceProviderConfigGet) | **GET** /rest/scim/ServiceProviderConfig | Get SCIM service provider config
[**restScimUsersGet**](ScimApi.md#restScimUsersGet) | **GET** /rest/scim/users | Retrieve users
[**restScimUsersIdDelete**](ScimApi.md#restScimUsersIdDelete) | **DELETE** /rest/scim/users/{id} | Delete single user
[**restScimUsersIdGet**](ScimApi.md#restScimUsersIdGet) | **GET** /rest/scim/users/{id} | Get a user specified by the id
[**restScimUsersIdPut**](ScimApi.md#restScimUsersIdPut) | **PUT** /rest/scim/users/{id} | 
[**restScimUsersPost**](ScimApi.md#restScimUsersPost) | **POST** /rest/scim/users | Create single user


<a id="restScimResourceTypesGet"></a>
# **restScimResourceTypesGet**
> restScimResourceTypesGet()



Get SCIM resource types

### Example
```kotlin
// Import classes:
//import org.openapitools.client.infrastructure.*
//import org.openapitools.client.models.*

val apiInstance = ScimApi()
try {
    apiInstance.restScimResourceTypesGet()
} catch (e: ClientException) {
    println("4xx response calling ScimApi#restScimResourceTypesGet")
    e.printStackTrace()
} catch (e: ServerException) {
    println("5xx response calling ScimApi#restScimResourceTypesGet")
    e.printStackTrace()
}
```

### Parameters
This endpoint does not need any parameter.

### Return type

null (empty response body)

### Authorization

No authorization required

### HTTP request headers

 - **Content-Type**: Not defined
 - **Accept**: Not defined

<a id="restScimResourceTypesIdGet"></a>
# **restScimResourceTypesIdGet**
> restScimResourceTypesIdGet(id)



Get a SCIM resource type

### Example
```kotlin
// Import classes:
//import org.openapitools.client.infrastructure.*
//import org.openapitools.client.models.*

val apiInstance = ScimApi()
val id : kotlin.String = id_example // kotlin.String | The ID/URN of the schema
try {
    apiInstance.restScimResourceTypesIdGet(id)
} catch (e: ClientException) {
    println("4xx response calling ScimApi#restScimResourceTypesIdGet")
    e.printStackTrace()
} catch (e: ServerException) {
    println("5xx response calling ScimApi#restScimResourceTypesIdGet")
    e.printStackTrace()
}
```

### Parameters

Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **id** | **kotlin.String**| The ID/URN of the schema |

### Return type

null (empty response body)

### Authorization

No authorization required

### HTTP request headers

 - **Content-Type**: Not defined
 - **Accept**: Not defined

<a id="restScimSchemasGet"></a>
# **restScimSchemasGet**
> restScimSchemasGet()



Get SCIM schemas

### Example
```kotlin
// Import classes:
//import org.openapitools.client.infrastructure.*
//import org.openapitools.client.models.*

val apiInstance = ScimApi()
try {
    apiInstance.restScimSchemasGet()
} catch (e: ClientException) {
    println("4xx response calling ScimApi#restScimSchemasGet")
    e.printStackTrace()
} catch (e: ServerException) {
    println("5xx response calling ScimApi#restScimSchemasGet")
    e.printStackTrace()
}
```

### Parameters
This endpoint does not need any parameter.

### Return type

null (empty response body)

### Authorization

No authorization required

### HTTP request headers

 - **Content-Type**: Not defined
 - **Accept**: Not defined

<a id="restScimSchemasIdGet"></a>
# **restScimSchemasIdGet**
> restScimSchemasIdGet(id)



Get a SCIM schema

### Example
```kotlin
// Import classes:
//import org.openapitools.client.infrastructure.*
//import org.openapitools.client.models.*

val apiInstance = ScimApi()
val id : kotlin.String = id_example // kotlin.String | The ID/URN of the schema
try {
    apiInstance.restScimSchemasIdGet(id)
} catch (e: ClientException) {
    println("4xx response calling ScimApi#restScimSchemasIdGet")
    e.printStackTrace()
} catch (e: ServerException) {
    println("5xx response calling ScimApi#restScimSchemasIdGet")
    e.printStackTrace()
}
```

### Parameters

Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **id** | **kotlin.String**| The ID/URN of the schema |

### Return type

null (empty response body)

### Authorization

No authorization required

### HTTP request headers

 - **Content-Type**: Not defined
 - **Accept**: Not defined

<a id="restScimServiceProviderConfigGet"></a>
# **restScimServiceProviderConfigGet**
> restScimServiceProviderConfigGet()

Get SCIM service provider config

Get SCIM service provider config

### Example
```kotlin
// Import classes:
//import org.openapitools.client.infrastructure.*
//import org.openapitools.client.models.*

val apiInstance = ScimApi()
try {
    apiInstance.restScimServiceProviderConfigGet()
} catch (e: ClientException) {
    println("4xx response calling ScimApi#restScimServiceProviderConfigGet")
    e.printStackTrace()
} catch (e: ServerException) {
    println("5xx response calling ScimApi#restScimServiceProviderConfigGet")
    e.printStackTrace()
}
```

### Parameters
This endpoint does not need any parameter.

### Return type

null (empty response body)

### Authorization

No authorization required

### HTTP request headers

 - **Content-Type**: Not defined
 - **Accept**: Not defined

<a id="restScimUsersGet"></a>
# **restScimUsersGet**
> ScimUsers restScimUsersGet(filter, sortOrder, count, startIndex, sortBy, excludedAttributes, attributes)

Retrieve users

Retrieve users

### Example
```kotlin
// Import classes:
//import org.openapitools.client.infrastructure.*
//import org.openapitools.client.models.*

val apiInstance = ScimApi()
val filter : kotlin.String = filter_example // kotlin.String | 
val sortOrder : kotlin.String = sortOrder_example // kotlin.String | 
val count : kotlin.Int = 56 // kotlin.Int | 
val startIndex : kotlin.Int = 56 // kotlin.Int | 
val sortBy : kotlin.String = sortBy_example // kotlin.String | 
val excludedAttributes : kotlin.collections.List<kotlin.String> =  // kotlin.collections.List<kotlin.String> | 
val attributes : kotlin.collections.List<kotlin.String> =  // kotlin.collections.List<kotlin.String> | 
try {
    val result : ScimUsers = apiInstance.restScimUsersGet(filter, sortOrder, count, startIndex, sortBy, excludedAttributes, attributes)
    println(result)
} catch (e: ClientException) {
    println("4xx response calling ScimApi#restScimUsersGet")
    e.printStackTrace()
} catch (e: ServerException) {
    println("5xx response calling ScimApi#restScimUsersGet")
    e.printStackTrace()
}
```

### Parameters

Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **filter** | **kotlin.String**|  | [optional]
 **sortOrder** | **kotlin.String**|  | [optional]
 **count** | **kotlin.Int**|  | [optional]
 **startIndex** | **kotlin.Int**|  | [optional]
 **sortBy** | **kotlin.String**|  | [optional]
 **excludedAttributes** | [**kotlin.collections.List&lt;kotlin.String&gt;**](kotlin.String.md)|  | [optional] [enum: meta, userName, displayName, userType, preferredLanguage, active, emails, phoneNumbers, photos, roles, meta.resourceType, meta.created, meta.location, urn:ietf:params:scim:schemas:core:2.0:User:meta, urn:ietf:params:scim:schemas:core:2.0:User:userName, urn:ietf:params:scim:schemas:core:2.0:User:displayName, urn:ietf:params:scim:schemas:core:2.0:User:userType, urn:ietf:params:scim:schemas:core:2.0:User:preferredLanguage, urn:ietf:params:scim:schemas:core:2.0:User:active, urn:ietf:params:scim:schemas:core:2.0:User:emails, urn:ietf:params:scim:schemas:core:2.0:User:phoneNumbers, urn:ietf:params:scim:schemas:core:2.0:User:photos, urn:ietf:params:scim:schemas:core:2.0:User:roles, urn:ietf:params:scim:schemas:core:2.0:User:meta.resourceType, urn:ietf:params:scim:schemas:core:2.0:User:meta.created, urn:ietf:params:scim:schemas:core:2.0:User:meta.location]
 **attributes** | [**kotlin.collections.List&lt;kotlin.String&gt;**](kotlin.String.md)|  | [optional] [enum: id, meta, userName, displayName, userType, preferredLanguage, active, emails, phoneNumbers, photos, roles, meta.resourceType, meta.created, meta.location, urn:ietf:params:scim:schemas:core:2.0:User:id, urn:ietf:params:scim:schemas:core:2.0:User:meta, urn:ietf:params:scim:schemas:core:2.0:User:userName, urn:ietf:params:scim:schemas:core:2.0:User:displayName, urn:ietf:params:scim:schemas:core:2.0:User:userType, urn:ietf:params:scim:schemas:core:2.0:User:preferredLanguage, urn:ietf:params:scim:schemas:core:2.0:User:active, urn:ietf:params:scim:schemas:core:2.0:User:emails, urn:ietf:params:scim:schemas:core:2.0:User:phoneNumbers, urn:ietf:params:scim:schemas:core:2.0:User:photos, urn:ietf:params:scim:schemas:core:2.0:User:roles, urn:ietf:params:scim:schemas:core:2.0:User:meta.resourceType, urn:ietf:params:scim:schemas:core:2.0:User:meta.created, urn:ietf:params:scim:schemas:core:2.0:User:meta.location]

### Return type

[**ScimUsers**](ScimUsers.md)

### Authorization

No authorization required

### HTTP request headers

 - **Content-Type**: Not defined
 - **Accept**: */*

<a id="restScimUsersIdDelete"></a>
# **restScimUsersIdDelete**
> restScimUsersIdDelete(id, remoteWipe, retainData, retainPermissionToSharedData, deleteUnsharedData, retainToUser)

Delete single user

Delete single user

### Example
```kotlin
// Import classes:
//import org.openapitools.client.infrastructure.*
//import org.openapitools.client.models.*

val apiInstance = ScimApi()
val id : kotlin.String = id_example // kotlin.String | The ID of the entity
val remoteWipe : kotlin.Boolean = true // kotlin.Boolean | 
val retainData : kotlin.Boolean = true // kotlin.Boolean | 
val retainPermissionToSharedData : kotlin.Boolean = true // kotlin.Boolean | 
val deleteUnsharedData : kotlin.Boolean = true // kotlin.Boolean | 
val retainToUser : kotlin.String = retainToUser_example // kotlin.String | 
try {
    apiInstance.restScimUsersIdDelete(id, remoteWipe, retainData, retainPermissionToSharedData, deleteUnsharedData, retainToUser)
} catch (e: ClientException) {
    println("4xx response calling ScimApi#restScimUsersIdDelete")
    e.printStackTrace()
} catch (e: ServerException) {
    println("5xx response calling ScimApi#restScimUsersIdDelete")
    e.printStackTrace()
}
```

### Parameters

Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **id** | **kotlin.String**| The ID of the entity |
 **remoteWipe** | **kotlin.Boolean**|  | [optional]
 **retainData** | **kotlin.Boolean**|  | [optional]
 **retainPermissionToSharedData** | **kotlin.Boolean**|  | [optional]
 **deleteUnsharedData** | **kotlin.Boolean**|  | [optional]
 **retainToUser** | **kotlin.String**|  | [optional]

### Return type

null (empty response body)

### Authorization

No authorization required

### HTTP request headers

 - **Content-Type**: Not defined
 - **Accept**: Not defined

<a id="restScimUsersIdGet"></a>
# **restScimUsersIdGet**
> ScimUser restScimUsersIdGet(id, attributes, excludedAttributes)

Get a user specified by the id

Get a user specified by the id

### Example
```kotlin
// Import classes:
//import org.openapitools.client.infrastructure.*
//import org.openapitools.client.models.*

val apiInstance = ScimApi()
val id : kotlin.String = id_example // kotlin.String | The ID of the entity
val attributes : kotlin.collections.List<kotlin.String> =  // kotlin.collections.List<kotlin.String> | 
val excludedAttributes : kotlin.collections.List<kotlin.String> =  // kotlin.collections.List<kotlin.String> | 
try {
    val result : ScimUser = apiInstance.restScimUsersIdGet(id, attributes, excludedAttributes)
    println(result)
} catch (e: ClientException) {
    println("4xx response calling ScimApi#restScimUsersIdGet")
    e.printStackTrace()
} catch (e: ServerException) {
    println("5xx response calling ScimApi#restScimUsersIdGet")
    e.printStackTrace()
}
```

### Parameters

Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **id** | **kotlin.String**| The ID of the entity |
 **attributes** | [**kotlin.collections.List&lt;kotlin.String&gt;**](kotlin.String.md)|  | [optional] [enum: id, meta, userName, displayName, userType, preferredLanguage, active, emails, phoneNumbers, photos, roles, meta.resourceType, meta.created, meta.location, urn:ietf:params:scim:schemas:core:2.0:User:id, urn:ietf:params:scim:schemas:core:2.0:User:meta, urn:ietf:params:scim:schemas:core:2.0:User:userName, urn:ietf:params:scim:schemas:core:2.0:User:displayName, urn:ietf:params:scim:schemas:core:2.0:User:userType, urn:ietf:params:scim:schemas:core:2.0:User:preferredLanguage, urn:ietf:params:scim:schemas:core:2.0:User:active, urn:ietf:params:scim:schemas:core:2.0:User:emails, urn:ietf:params:scim:schemas:core:2.0:User:phoneNumbers, urn:ietf:params:scim:schemas:core:2.0:User:photos, urn:ietf:params:scim:schemas:core:2.0:User:roles, urn:ietf:params:scim:schemas:core:2.0:User:meta.resourceType, urn:ietf:params:scim:schemas:core:2.0:User:meta.created, urn:ietf:params:scim:schemas:core:2.0:User:meta.location]
 **excludedAttributes** | [**kotlin.collections.List&lt;kotlin.String&gt;**](kotlin.String.md)|  | [optional] [enum: meta, userName, displayName, userType, preferredLanguage, active, emails, phoneNumbers, photos, roles, meta.resourceType, meta.created, meta.location, urn:ietf:params:scim:schemas:core:2.0:User:meta, urn:ietf:params:scim:schemas:core:2.0:User:userName, urn:ietf:params:scim:schemas:core:2.0:User:displayName, urn:ietf:params:scim:schemas:core:2.0:User:userType, urn:ietf:params:scim:schemas:core:2.0:User:preferredLanguage, urn:ietf:params:scim:schemas:core:2.0:User:active, urn:ietf:params:scim:schemas:core:2.0:User:emails, urn:ietf:params:scim:schemas:core:2.0:User:phoneNumbers, urn:ietf:params:scim:schemas:core:2.0:User:photos, urn:ietf:params:scim:schemas:core:2.0:User:roles, urn:ietf:params:scim:schemas:core:2.0:User:meta.resourceType, urn:ietf:params:scim:schemas:core:2.0:User:meta.created, urn:ietf:params:scim:schemas:core:2.0:User:meta.location]

### Return type

[**ScimUser**](ScimUser.md)

### Authorization

No authorization required

### HTTP request headers

 - **Content-Type**: Not defined
 - **Accept**: */*

<a id="restScimUsersIdPut"></a>
# **restScimUsersIdPut**
> ScimUser restScimUsersIdPut(id, body)



Update a user specified by the id

### Example
```kotlin
// Import classes:
//import org.openapitools.client.infrastructure.*
//import org.openapitools.client.models.*

val apiInstance = ScimApi()
val id : kotlin.String = id_example // kotlin.String | The ID of the entity
val body : ScimUsersPutRequest =  // ScimUsersPutRequest | 
try {
    val result : ScimUser = apiInstance.restScimUsersIdPut(id, body)
    println(result)
} catch (e: ClientException) {
    println("4xx response calling ScimApi#restScimUsersIdPut")
    e.printStackTrace()
} catch (e: ServerException) {
    println("5xx response calling ScimApi#restScimUsersIdPut")
    e.printStackTrace()
}
```

### Parameters

Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **id** | **kotlin.String**| The ID of the entity |
 **body** | [**ScimUsersPutRequest**](ScimUsersPutRequest.md)|  |

### Return type

[**ScimUser**](ScimUser.md)

### Authorization

No authorization required

### HTTP request headers

 - **Content-Type**: Not defined
 - **Accept**: */*

<a id="restScimUsersPost"></a>
# **restScimUsersPost**
> ScimUser restScimUsersPost(body, attributes, excludedAttributes)

Create single user

Create single user

### Example
```kotlin
// Import classes:
//import org.openapitools.client.infrastructure.*
//import org.openapitools.client.models.*

val apiInstance = ScimApi()
val body : ScimUsersPostRequest =  // ScimUsersPostRequest | 
val attributes : kotlin.collections.List<kotlin.String> =  // kotlin.collections.List<kotlin.String> | 
val excludedAttributes : kotlin.collections.List<kotlin.String> =  // kotlin.collections.List<kotlin.String> | 
try {
    val result : ScimUser = apiInstance.restScimUsersPost(body, attributes, excludedAttributes)
    println(result)
} catch (e: ClientException) {
    println("4xx response calling ScimApi#restScimUsersPost")
    e.printStackTrace()
} catch (e: ServerException) {
    println("5xx response calling ScimApi#restScimUsersPost")
    e.printStackTrace()
}
```

### Parameters

Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **body** | [**ScimUsersPostRequest**](ScimUsersPostRequest.md)|  |
 **attributes** | [**kotlin.collections.List&lt;kotlin.String&gt;**](kotlin.String.md)|  | [optional] [enum: id, meta, userName, displayName, userType, preferredLanguage, active, emails, phoneNumbers, photos, roles, meta.resourceType, meta.created, meta.location, urn:ietf:params:scim:schemas:core:2.0:User:id, urn:ietf:params:scim:schemas:core:2.0:User:meta, urn:ietf:params:scim:schemas:core:2.0:User:userName, urn:ietf:params:scim:schemas:core:2.0:User:displayName, urn:ietf:params:scim:schemas:core:2.0:User:userType, urn:ietf:params:scim:schemas:core:2.0:User:preferredLanguage, urn:ietf:params:scim:schemas:core:2.0:User:active, urn:ietf:params:scim:schemas:core:2.0:User:emails, urn:ietf:params:scim:schemas:core:2.0:User:phoneNumbers, urn:ietf:params:scim:schemas:core:2.0:User:photos, urn:ietf:params:scim:schemas:core:2.0:User:roles, urn:ietf:params:scim:schemas:core:2.0:User:meta.resourceType, urn:ietf:params:scim:schemas:core:2.0:User:meta.created, urn:ietf:params:scim:schemas:core:2.0:User:meta.location]
 **excludedAttributes** | [**kotlin.collections.List&lt;kotlin.String&gt;**](kotlin.String.md)|  | [optional] [enum: meta, userName, displayName, userType, preferredLanguage, active, emails, phoneNumbers, photos, roles, meta.resourceType, meta.created, meta.location, urn:ietf:params:scim:schemas:core:2.0:User:meta, urn:ietf:params:scim:schemas:core:2.0:User:userName, urn:ietf:params:scim:schemas:core:2.0:User:displayName, urn:ietf:params:scim:schemas:core:2.0:User:userType, urn:ietf:params:scim:schemas:core:2.0:User:preferredLanguage, urn:ietf:params:scim:schemas:core:2.0:User:active, urn:ietf:params:scim:schemas:core:2.0:User:emails, urn:ietf:params:scim:schemas:core:2.0:User:phoneNumbers, urn:ietf:params:scim:schemas:core:2.0:User:photos, urn:ietf:params:scim:schemas:core:2.0:User:roles, urn:ietf:params:scim:schemas:core:2.0:User:meta.resourceType, urn:ietf:params:scim:schemas:core:2.0:User:meta.created, urn:ietf:params:scim:schemas:core:2.0:User:meta.location]

### Return type

[**ScimUser**](ScimUser.md)

### Authorization

No authorization required

### HTTP request headers

 - **Content-Type**: Not defined
 - **Accept**: */*

