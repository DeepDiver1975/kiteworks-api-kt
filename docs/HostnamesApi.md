# HostnamesApi

All URIs are relative to *http://localhost*

Method | HTTP request | Description
------------- | ------------- | -------------
[**restHostnamesDelete**](HostnamesApi.md#restHostnamesDelete) | **DELETE** /rest/hostnames | Deletes list of hostnames
[**restHostnamesGet**](HostnamesApi.md#restHostnamesGet) | **GET** /rest/hostnames | List hostnames
[**restHostnamesIdDelete**](HostnamesApi.md#restHostnamesIdDelete) | **DELETE** /rest/hostnames/{id} | Mark specified hostname as deleted.
[**restHostnamesIdGet**](HostnamesApi.md#restHostnamesIdGet) | **GET** /rest/hostnames/{id} | Get hostname info from the hostname ID
[**restHostnamesIdPut**](HostnamesApi.md#restHostnamesIdPut) | **PUT** /rest/hostnames/{id} | Disable alias hostname
[**restHostnamesPost**](HostnamesApi.md#restHostnamesPost) | **POST** /rest/hostnames | Create an alias hostname


<a id="restHostnamesDelete"></a>
# **restHostnamesDelete**
> restHostnamesDelete(idColonIn, partialSuccess, mode)

Deletes list of hostnames

Deletes list of hostnames.

### Example
```kotlin
// Import classes:
//import org.openapitools.client.infrastructure.*
//import org.openapitools.client.models.*

val apiInstance = HostnamesApi()
val idColonIn : kotlin.String = idColonIn_example // kotlin.String | Array of values which are going to be changed.
val partialSuccess : kotlin.Boolean = true // kotlin.Boolean | Whether to perform action on valid items even if some ones fail
val mode : kotlin.String = mode_example // kotlin.String | Response mode
try {
    apiInstance.restHostnamesDelete(idColonIn, partialSuccess, mode)
} catch (e: ClientException) {
    println("4xx response calling HostnamesApi#restHostnamesDelete")
    e.printStackTrace()
} catch (e: ServerException) {
    println("5xx response calling HostnamesApi#restHostnamesDelete")
    e.printStackTrace()
}
```

### Parameters

Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **idColonIn** | **kotlin.String**| Array of values which are going to be changed. |
 **partialSuccess** | **kotlin.Boolean**| Whether to perform action on valid items even if some ones fail | [optional]
 **mode** | **kotlin.String**| Response mode | [optional]

### Return type

null (empty response body)

### Authorization

No authorization required

### HTTP request headers

 - **Content-Type**: Not defined
 - **Accept**: Not defined

<a id="restHostnamesGet"></a>
# **restHostnamesGet**
> kotlin.collections.List&lt;Hostname&gt; restHostnamesGet(aliasName, aliasNameColonContains, tenantId, tenantIdColonGt, tenantIdColonGte, tenantIdColonLt, tenantIdColonLte, deleted, disabled, orderBy, offset, limit, with, mode)

List hostnames

Returns a list of hostnames

### Example
```kotlin
// Import classes:
//import org.openapitools.client.infrastructure.*
//import org.openapitools.client.models.*

val apiInstance = HostnamesApi()
val aliasName : kotlin.String = aliasName_example // kotlin.String | Alias name
val aliasNameColonContains : kotlin.String = aliasNameColonContains_example // kotlin.String | Alias name. Search for result that contains specified characters in this parameter.
val tenantId : kotlin.Int = 56 // kotlin.Int | Tenant ID
val tenantIdColonGt : kotlin.Int = 56 // kotlin.Int | Tenant ID. Search for result that has this parameter value greater than specified.
val tenantIdColonGte : kotlin.Int = 56 // kotlin.Int | Tenant ID. Search for result that has this parameter value greater or equal to the specified.
val tenantIdColonLt : kotlin.Int = 56 // kotlin.Int | Tenant ID. Search for result that has this parameter value less than specified.
val tenantIdColonLte : kotlin.Int = 56 // kotlin.Int | Tenant ID. Search for result that has this parameter value less or equal to the specified.
val deleted : kotlin.Boolean = true // kotlin.Boolean | Alias name deleted
val disabled : kotlin.Boolean = true // kotlin.Boolean | Alias name disabled
val orderBy : kotlin.collections.List<kotlin.String> =  // kotlin.collections.List<kotlin.String> | Sorting options
val offset : kotlin.Int = 56 // kotlin.Int | Offset
val limit : kotlin.Int = 56 // kotlin.Int | Limit
val with : kotlin.String = with_example // kotlin.String | With parameters
val mode : kotlin.String = mode_example // kotlin.String | Response mode
try {
    val result : kotlin.collections.List<Hostname> = apiInstance.restHostnamesGet(aliasName, aliasNameColonContains, tenantId, tenantIdColonGt, tenantIdColonGte, tenantIdColonLt, tenantIdColonLte, deleted, disabled, orderBy, offset, limit, with, mode)
    println(result)
} catch (e: ClientException) {
    println("4xx response calling HostnamesApi#restHostnamesGet")
    e.printStackTrace()
} catch (e: ServerException) {
    println("5xx response calling HostnamesApi#restHostnamesGet")
    e.printStackTrace()
}
```

### Parameters

Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **aliasName** | **kotlin.String**| Alias name | [optional]
 **aliasNameColonContains** | **kotlin.String**| Alias name. Search for result that contains specified characters in this parameter. | [optional]
 **tenantId** | **kotlin.Int**| Tenant ID | [optional]
 **tenantIdColonGt** | **kotlin.Int**| Tenant ID. Search for result that has this parameter value greater than specified. | [optional]
 **tenantIdColonGte** | **kotlin.Int**| Tenant ID. Search for result that has this parameter value greater or equal to the specified. | [optional]
 **tenantIdColonLt** | **kotlin.Int**| Tenant ID. Search for result that has this parameter value less than specified. | [optional]
 **tenantIdColonLte** | **kotlin.Int**| Tenant ID. Search for result that has this parameter value less or equal to the specified. | [optional]
 **deleted** | **kotlin.Boolean**| Alias name deleted | [optional]
 **disabled** | **kotlin.Boolean**| Alias name disabled | [optional]
 **orderBy** | [**kotlin.collections.List&lt;kotlin.String&gt;**](kotlin.String.md)| Sorting options | [optional]
 **offset** | **kotlin.Int**| Offset | [optional]
 **limit** | **kotlin.Int**| Limit | [optional]
 **with** | **kotlin.String**| With parameters | [optional]
 **mode** | **kotlin.String**| Response mode | [optional]

### Return type

[**kotlin.collections.List&lt;Hostname&gt;**](Hostname.md)

### Authorization

No authorization required

### HTTP request headers

 - **Content-Type**: Not defined
 - **Accept**: */*

<a id="restHostnamesIdDelete"></a>
# **restHostnamesIdDelete**
> restHostnamesIdDelete(id)

Mark specified hostname as deleted.

Marks the specified hostname as deleted.

### Example
```kotlin
// Import classes:
//import org.openapitools.client.infrastructure.*
//import org.openapitools.client.models.*

val apiInstance = HostnamesApi()
val id : kotlin.Int = 56 // kotlin.Int | ID of the hostname
try {
    apiInstance.restHostnamesIdDelete(id)
} catch (e: ClientException) {
    println("4xx response calling HostnamesApi#restHostnamesIdDelete")
    e.printStackTrace()
} catch (e: ServerException) {
    println("5xx response calling HostnamesApi#restHostnamesIdDelete")
    e.printStackTrace()
}
```

### Parameters

Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **id** | **kotlin.Int**| ID of the hostname |

### Return type

null (empty response body)

### Authorization

No authorization required

### HTTP request headers

 - **Content-Type**: Not defined
 - **Accept**: Not defined

<a id="restHostnamesIdGet"></a>
# **restHostnamesIdGet**
> Hostname restHostnamesIdGet(id)

Get hostname info from the hostname ID

Returns the details of the specified hostname.

### Example
```kotlin
// Import classes:
//import org.openapitools.client.infrastructure.*
//import org.openapitools.client.models.*

val apiInstance = HostnamesApi()
val id : kotlin.Int = 56 // kotlin.Int | ID of the hostname to be retrieved
try {
    val result : Hostname = apiInstance.restHostnamesIdGet(id)
    println(result)
} catch (e: ClientException) {
    println("4xx response calling HostnamesApi#restHostnamesIdGet")
    e.printStackTrace()
} catch (e: ServerException) {
    println("5xx response calling HostnamesApi#restHostnamesIdGet")
    e.printStackTrace()
}
```

### Parameters

Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **id** | **kotlin.Int**| ID of the hostname to be retrieved |

### Return type

[**Hostname**](Hostname.md)

### Authorization

No authorization required

### HTTP request headers

 - **Content-Type**: Not defined
 - **Accept**: */*

<a id="restHostnamesIdPut"></a>
# **restHostnamesIdPut**
> restHostnamesIdPut(id, body)

Disable alias hostname

Disable the specified hostname.

### Example
```kotlin
// Import classes:
//import org.openapitools.client.infrastructure.*
//import org.openapitools.client.models.*

val apiInstance = HostnamesApi()
val id : kotlin.Int = 56 // kotlin.Int | ID of the hostname to disable
val body : HostnamePut =  // HostnamePut | comment to activity
try {
    apiInstance.restHostnamesIdPut(id, body)
} catch (e: ClientException) {
    println("4xx response calling HostnamesApi#restHostnamesIdPut")
    e.printStackTrace()
} catch (e: ServerException) {
    println("5xx response calling HostnamesApi#restHostnamesIdPut")
    e.printStackTrace()
}
```

### Parameters

Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **id** | **kotlin.Int**| ID of the hostname to disable |
 **body** | [**HostnamePut**](HostnamePut.md)| comment to activity |

### Return type

null (empty response body)

### Authorization

No authorization required

### HTTP request headers

 - **Content-Type**: Not defined
 - **Accept**: Not defined

<a id="restHostnamesPost"></a>
# **restHostnamesPost**
> Hostname restHostnamesPost(body, returnEntity, mode)

Create an alias hostname

Create an alias hostname.

### Example
```kotlin
// Import classes:
//import org.openapitools.client.infrastructure.*
//import org.openapitools.client.models.*

val apiInstance = HostnamesApi()
val body : HostnamePost =  // HostnamePost | comment to activity
val returnEntity : kotlin.Boolean = true // kotlin.Boolean | Return information about newly created entity
val mode : kotlin.String = mode_example // kotlin.String | Response mode
try {
    val result : Hostname = apiInstance.restHostnamesPost(body, returnEntity, mode)
    println(result)
} catch (e: ClientException) {
    println("4xx response calling HostnamesApi#restHostnamesPost")
    e.printStackTrace()
} catch (e: ServerException) {
    println("5xx response calling HostnamesApi#restHostnamesPost")
    e.printStackTrace()
}
```

### Parameters

Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **body** | [**HostnamePost**](HostnamePost.md)| comment to activity |
 **returnEntity** | **kotlin.Boolean**| Return information about newly created entity | [optional]
 **mode** | **kotlin.String**| Response mode | [optional]

### Return type

[**Hostname**](Hostname.md)

### Authorization

No authorization required

### HTTP request headers

 - **Content-Type**: Not defined
 - **Accept**: */*

