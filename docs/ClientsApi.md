# ClientsApi

All URIs are relative to *http://localhost*

Method | HTTP request | Description
------------- | ------------- | -------------
[**restClientsGet**](ClientsApi.md#restClientsGet) | **GET** /rest/clients | List clients
[**restClientsIdDelete**](ClientsApi.md#restClientsIdDelete) | **DELETE** /rest/clients/{id} | Delete a client
[**restClientsIdGet**](ClientsApi.md#restClientsIdGet) | **GET** /rest/clients/{id} | Get a client
[**restClientsIdPut**](ClientsApi.md#restClientsIdPut) | **PUT** /rest/clients/{id} | Update a client
[**restClientsIdScopesGet**](ClientsApi.md#restClientsIdScopesGet) | **GET** /rest/clients/{id}/scopes | List scopes of a client
[**restClientsMeGet**](ClientsApi.md#restClientsMeGet) | **GET** /rest/clients/me | Get current client
[**restClientsPost**](ClientsApi.md#restClientsPost) | **POST** /rest/clients | Create a client


<a id="restClientsGet"></a>
# **restClientsGet**
> kotlin.collections.List&lt;Client&gt; restClientsGet(name, nameColonContains, descriptionColonContains, orderBy, offset, limit, with, mode)

List clients

Return a list of clients

### Example
```kotlin
// Import classes:
//import org.openapitools.client.infrastructure.*
//import org.openapitools.client.models.*

val apiInstance = ClientsApi()
val name : kotlin.String = name_example // kotlin.String | Client name
val nameColonContains : kotlin.String = nameColonContains_example // kotlin.String | Client name. Search for result that contains specified characters in this parameter.
val descriptionColonContains : kotlin.String = descriptionColonContains_example // kotlin.String | Client description. Search for result that contains specified characters in this parameter.
val orderBy : kotlin.collections.List<kotlin.String> =  // kotlin.collections.List<kotlin.String> | Sorting options
val offset : kotlin.Int = 56 // kotlin.Int | Offset
val limit : kotlin.Int = 56 // kotlin.Int | Limit
val with : kotlin.String = with_example // kotlin.String | With parameters
val mode : kotlin.String = mode_example // kotlin.String | Response mode
try {
    val result : kotlin.collections.List<Client> = apiInstance.restClientsGet(name, nameColonContains, descriptionColonContains, orderBy, offset, limit, with, mode)
    println(result)
} catch (e: ClientException) {
    println("4xx response calling ClientsApi#restClientsGet")
    e.printStackTrace()
} catch (e: ServerException) {
    println("5xx response calling ClientsApi#restClientsGet")
    e.printStackTrace()
}
```

### Parameters

Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **name** | **kotlin.String**| Client name | [optional]
 **nameColonContains** | **kotlin.String**| Client name. Search for result that contains specified characters in this parameter. | [optional]
 **descriptionColonContains** | **kotlin.String**| Client description. Search for result that contains specified characters in this parameter. | [optional]
 **orderBy** | [**kotlin.collections.List&lt;kotlin.String&gt;**](kotlin.String.md)| Sorting options | [optional]
 **offset** | **kotlin.Int**| Offset | [optional]
 **limit** | **kotlin.Int**| Limit | [optional]
 **with** | **kotlin.String**| With parameters | [optional]
 **mode** | **kotlin.String**| Response mode | [optional]

### Return type

[**kotlin.collections.List&lt;Client&gt;**](Client.md)

### Authorization

No authorization required

### HTTP request headers

 - **Content-Type**: Not defined
 - **Accept**: */*

<a id="restClientsIdDelete"></a>
# **restClientsIdDelete**
> restClientsIdDelete(id)

Delete a client

Delete a client from the client list.

### Example
```kotlin
// Import classes:
//import org.openapitools.client.infrastructure.*
//import org.openapitools.client.models.*

val apiInstance = ClientsApi()
val id : kotlin.String = id_example // kotlin.String | ID of the client to be deleted
try {
    apiInstance.restClientsIdDelete(id)
} catch (e: ClientException) {
    println("4xx response calling ClientsApi#restClientsIdDelete")
    e.printStackTrace()
} catch (e: ServerException) {
    println("5xx response calling ClientsApi#restClientsIdDelete")
    e.printStackTrace()
}
```

### Parameters

Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **id** | **kotlin.String**| ID of the client to be deleted |

### Return type

null (empty response body)

### Authorization

No authorization required

### HTTP request headers

 - **Content-Type**: Not defined
 - **Accept**: Not defined

<a id="restClientsIdGet"></a>
# **restClientsIdGet**
> Client restClientsIdGet(id)

Get a client

Return the admin settings of a specified client.                e.g.: I want the admin settings for my iOS client; pin timeout, token lifetime, etc., 

### Example
```kotlin
// Import classes:
//import org.openapitools.client.infrastructure.*
//import org.openapitools.client.models.*

val apiInstance = ClientsApi()
val id : kotlin.String = id_example // kotlin.String | ID of the client to be retrieved
try {
    val result : Client = apiInstance.restClientsIdGet(id)
    println(result)
} catch (e: ClientException) {
    println("4xx response calling ClientsApi#restClientsIdGet")
    e.printStackTrace()
} catch (e: ServerException) {
    println("5xx response calling ClientsApi#restClientsIdGet")
    e.printStackTrace()
}
```

### Parameters

Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **id** | **kotlin.String**| ID of the client to be retrieved |

### Return type

[**Client**](Client.md)

### Authorization

No authorization required

### HTTP request headers

 - **Content-Type**: Not defined
 - **Accept**: */*

<a id="restClientsIdPut"></a>
# **restClientsIdPut**
> restClientsIdPut(id, body)

Update a client

Update the admin settings for the specified client

### Example
```kotlin
// Import classes:
//import org.openapitools.client.infrastructure.*
//import org.openapitools.client.models.*

val apiInstance = ClientsApi()
val id : kotlin.String = id_example // kotlin.String | ID of the client to be updated
val body : ClientPut =  // ClientPut | Details of the client
try {
    apiInstance.restClientsIdPut(id, body)
} catch (e: ClientException) {
    println("4xx response calling ClientsApi#restClientsIdPut")
    e.printStackTrace()
} catch (e: ServerException) {
    println("5xx response calling ClientsApi#restClientsIdPut")
    e.printStackTrace()
}
```

### Parameters

Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **id** | **kotlin.String**| ID of the client to be updated |
 **body** | [**ClientPut**](ClientPut.md)| Details of the client |

### Return type

null (empty response body)

### Authorization

No authorization required

### HTTP request headers

 - **Content-Type**: Not defined
 - **Accept**: Not defined

<a id="restClientsIdScopesGet"></a>
# **restClientsIdScopesGet**
> restClientsIdScopesGet(id, mode)

List scopes of a client

Return a list of scopes for a specific client.     This returns the methods that this client is allowed to use     such as folders, files, members, comments, etc.

### Example
```kotlin
// Import classes:
//import org.openapitools.client.infrastructure.*
//import org.openapitools.client.models.*

val apiInstance = ClientsApi()
val id : kotlin.String = id_example // kotlin.String | ID of the client whose scopes to be retrieved
val mode : kotlin.String = mode_example // kotlin.String | Response mode
try {
    apiInstance.restClientsIdScopesGet(id, mode)
} catch (e: ClientException) {
    println("4xx response calling ClientsApi#restClientsIdScopesGet")
    e.printStackTrace()
} catch (e: ServerException) {
    println("5xx response calling ClientsApi#restClientsIdScopesGet")
    e.printStackTrace()
}
```

### Parameters

Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **id** | **kotlin.String**| ID of the client whose scopes to be retrieved |
 **mode** | **kotlin.String**| Response mode | [optional]

### Return type

null (empty response body)

### Authorization

No authorization required

### HTTP request headers

 - **Content-Type**: Not defined
 - **Accept**: Not defined

<a id="restClientsMeGet"></a>
# **restClientsMeGet**
> Client restClientsMeGet()

Get current client

Return the settings of the current client.                e.g.: I want the admin settings for my client; pin timeout, token lifetime, etc., 

### Example
```kotlin
// Import classes:
//import org.openapitools.client.infrastructure.*
//import org.openapitools.client.models.*

val apiInstance = ClientsApi()
try {
    val result : Client = apiInstance.restClientsMeGet()
    println(result)
} catch (e: ClientException) {
    println("4xx response calling ClientsApi#restClientsMeGet")
    e.printStackTrace()
} catch (e: ServerException) {
    println("5xx response calling ClientsApi#restClientsMeGet")
    e.printStackTrace()
}
```

### Parameters
This endpoint does not need any parameter.

### Return type

[**Client**](Client.md)

### Authorization

No authorization required

### HTTP request headers

 - **Content-Type**: Not defined
 - **Accept**: */*

<a id="restClientsPost"></a>
# **restClientsPost**
> restClientsPost(body, returnEntity, mode)

Create a client

Create a new client that will be able to access the kiteworks system.                e.g.: A new mobile app that is customized for your company.

### Example
```kotlin
// Import classes:
//import org.openapitools.client.infrastructure.*
//import org.openapitools.client.models.*

val apiInstance = ClientsApi()
val body : ClientPost =  // ClientPost | Details of the client
val returnEntity : kotlin.Boolean = true // kotlin.Boolean | Return information about newly created entity
val mode : kotlin.String = mode_example // kotlin.String | Response mode
try {
    apiInstance.restClientsPost(body, returnEntity, mode)
} catch (e: ClientException) {
    println("4xx response calling ClientsApi#restClientsPost")
    e.printStackTrace()
} catch (e: ServerException) {
    println("5xx response calling ClientsApi#restClientsPost")
    e.printStackTrace()
}
```

### Parameters

Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **body** | [**ClientPost**](ClientPost.md)| Details of the client |
 **returnEntity** | **kotlin.Boolean**| Return information about newly created entity | [optional]
 **mode** | **kotlin.String**| Response mode | [optional]

### Return type

null (empty response body)

### Authorization

No authorization required

### HTTP request headers

 - **Content-Type**: Not defined
 - **Accept**: Not defined

