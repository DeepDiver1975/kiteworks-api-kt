# LocationsApi

All URIs are relative to *http://localhost*

Method | HTTP request | Description
------------- | ------------- | -------------
[**restLocationsGet**](LocationsApi.md#restLocationsGet) | **GET** /rest/locations | List locations
[**restLocationsIdDelete**](LocationsApi.md#restLocationsIdDelete) | **DELETE** /rest/locations/{id} | Delete a location.
[**restLocationsIdGet**](LocationsApi.md#restLocationsIdGet) | **GET** /rest/locations/{id} | Return location name.
[**restLocationsPost**](LocationsApi.md#restLocationsPost) | **POST** /rest/locations | Create a location entry.


<a id="restLocationsGet"></a>
# **restLocationsGet**
> Location restLocationsGet(mode)

List locations

Returns a list of available kiteworks locations.                   Locations are logical collection of multiple kiteworks servers,                   usually with a common geography or particular purpose.

### Example
```kotlin
// Import classes:
//import org.openapitools.client.infrastructure.*
//import org.openapitools.client.models.*

val apiInstance = LocationsApi()
val mode : kotlin.String = mode_example // kotlin.String | Response mode
try {
    val result : Location = apiInstance.restLocationsGet(mode)
    println(result)
} catch (e: ClientException) {
    println("4xx response calling LocationsApi#restLocationsGet")
    e.printStackTrace()
} catch (e: ServerException) {
    println("5xx response calling LocationsApi#restLocationsGet")
    e.printStackTrace()
}
```

### Parameters

Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **mode** | **kotlin.String**| Response mode | [optional]

### Return type

[**Location**](Location.md)

### Authorization

No authorization required

### HTTP request headers

 - **Content-Type**: Not defined
 - **Accept**: */*

<a id="restLocationsIdDelete"></a>
# **restLocationsIdDelete**
> restLocationsIdDelete(id)

Delete a location.

Delete the specified location.

### Example
```kotlin
// Import classes:
//import org.openapitools.client.infrastructure.*
//import org.openapitools.client.models.*

val apiInstance = LocationsApi()
val id : kotlin.Int = 56 // kotlin.Int | ID of the location to remove from
try {
    apiInstance.restLocationsIdDelete(id)
} catch (e: ClientException) {
    println("4xx response calling LocationsApi#restLocationsIdDelete")
    e.printStackTrace()
} catch (e: ServerException) {
    println("5xx response calling LocationsApi#restLocationsIdDelete")
    e.printStackTrace()
}
```

### Parameters

Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **id** | **kotlin.Int**| ID of the location to remove from |

### Return type

null (empty response body)

### Authorization

No authorization required

### HTTP request headers

 - **Content-Type**: Not defined
 - **Accept**: Not defined

<a id="restLocationsIdGet"></a>
# **restLocationsIdGet**
> Location restLocationsIdGet(id)

Return location name.

Returns the name of a specified location.

### Example
```kotlin
// Import classes:
//import org.openapitools.client.infrastructure.*
//import org.openapitools.client.models.*

val apiInstance = LocationsApi()
val id : kotlin.Int = 56 // kotlin.Int | ID of the location to be retrieved
try {
    val result : Location = apiInstance.restLocationsIdGet(id)
    println(result)
} catch (e: ClientException) {
    println("4xx response calling LocationsApi#restLocationsIdGet")
    e.printStackTrace()
} catch (e: ServerException) {
    println("5xx response calling LocationsApi#restLocationsIdGet")
    e.printStackTrace()
}
```

### Parameters

Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **id** | **kotlin.Int**| ID of the location to be retrieved |

### Return type

[**Location**](Location.md)

### Authorization

No authorization required

### HTTP request headers

 - **Content-Type**: Not defined
 - **Accept**: */*

<a id="restLocationsPost"></a>
# **restLocationsPost**
> restLocationsPost(body, returnEntity, mode)

Create a location entry.

Creates a location entry by providing a name.

### Example
```kotlin
// Import classes:
//import org.openapitools.client.infrastructure.*
//import org.openapitools.client.models.*

val apiInstance = LocationsApi()
val body : LocationPost =  // LocationPost | The location details
val returnEntity : kotlin.Boolean = true // kotlin.Boolean | Return information about newly created entity
val mode : kotlin.String = mode_example // kotlin.String | Response mode
try {
    apiInstance.restLocationsPost(body, returnEntity, mode)
} catch (e: ClientException) {
    println("4xx response calling LocationsApi#restLocationsPost")
    e.printStackTrace()
} catch (e: ServerException) {
    println("5xx response calling LocationsApi#restLocationsPost")
    e.printStackTrace()
}
```

### Parameters

Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **body** | [**LocationPost**](LocationPost.md)| The location details |
 **returnEntity** | **kotlin.Boolean**| Return information about newly created entity | [optional]
 **mode** | **kotlin.String**| Response mode | [optional]

### Return type

null (empty response body)

### Authorization

No authorization required

### HTTP request headers

 - **Content-Type**: Not defined
 - **Accept**: Not defined

