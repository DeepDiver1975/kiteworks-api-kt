# MobileSyncApi

All URIs are relative to *http://localhost*

Method | HTTP request | Description
------------- | ------------- | -------------
[**restFilesActionsMobileSyncItemsDelete**](MobileSyncApi.md#restFilesActionsMobileSyncItemsDelete) | **DELETE** /rest/files/actions/mobileSyncItems | Delete multiple files from user mobile sync list
[**restFilesActionsMobileSyncItemsPost**](MobileSyncApi.md#restFilesActionsMobileSyncItemsPost) | **POST** /rest/files/actions/mobileSyncItems | Add multiple files to mobile sync list
[**restFilesActionsPushDelete**](MobileSyncApi.md#restFilesActionsPushDelete) | **DELETE** /rest/files/actions/push | Un-Push collection of files
[**restFilesActionsPushPost**](MobileSyncApi.md#restFilesActionsPushPost) | **POST** /rest/files/actions/push | Push files list to mobile sync list
[**restFilesIdActionsPushDelete**](MobileSyncApi.md#restFilesIdActionsPushDelete) | **DELETE** /rest/files/{id}/actions/push | Un-Push file
[**restFilesIdActionsPushPost**](MobileSyncApi.md#restFilesIdActionsPushPost) | **POST** /rest/files/{id}/actions/push | Push file to mobile sync list
[**restMobileSyncItemsGet**](MobileSyncApi.md#restMobileSyncItemsGet) | **GET** /rest/mobileSyncItems | Returns a list of mobile sync items for current user
[**restMobileSyncItemsIdDelete**](MobileSyncApi.md#restMobileSyncItemsIdDelete) | **DELETE** /rest/mobileSyncItems/{id} | Remove mobile sync item
[**restMobileSyncItemsIdGet**](MobileSyncApi.md#restMobileSyncItemsIdGet) | **GET** /rest/mobileSyncItems/{id} | Retrieve information about mobile sync item specified.
[**restMobileSyncItemsPost**](MobileSyncApi.md#restMobileSyncItemsPost) | **POST** /rest/mobileSyncItems | Set file as a mobile sync item


<a id="restFilesActionsMobileSyncItemsDelete"></a>
# **restFilesActionsMobileSyncItemsDelete**
> restFilesActionsMobileSyncItemsDelete(idColonIn, partialSuccess, mode)

Delete multiple files from user mobile sync list

Delete multiple files from user mobile sync list

### Example
```kotlin
// Import classes:
//import org.openapitools.client.infrastructure.*
//import org.openapitools.client.models.*

val apiInstance = MobileSyncApi()
val idColonIn : kotlin.String = idColonIn_example // kotlin.String | Array of values which are going to be changed.
val partialSuccess : kotlin.Boolean = true // kotlin.Boolean | Whether to perform action on valid items even if some ones fail
val mode : kotlin.String = mode_example // kotlin.String | Response mode
try {
    apiInstance.restFilesActionsMobileSyncItemsDelete(idColonIn, partialSuccess, mode)
} catch (e: ClientException) {
    println("4xx response calling MobileSyncApi#restFilesActionsMobileSyncItemsDelete")
    e.printStackTrace()
} catch (e: ServerException) {
    println("5xx response calling MobileSyncApi#restFilesActionsMobileSyncItemsDelete")
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

<a id="restFilesActionsMobileSyncItemsPost"></a>
# **restFilesActionsMobileSyncItemsPost**
> restFilesActionsMobileSyncItemsPost(idColonIn, partialSuccess, returnEntity, mode)

Add multiple files to mobile sync list

Add multiple files to mobile sync list This operation will not return location headers for each entity created, if the inserted records are         required, returnEntity should be set to true.

### Example
```kotlin
// Import classes:
//import org.openapitools.client.infrastructure.*
//import org.openapitools.client.models.*

val apiInstance = MobileSyncApi()
val idColonIn : kotlin.String = idColonIn_example // kotlin.String | Array of values which are going to be changed.
val partialSuccess : kotlin.Boolean = true // kotlin.Boolean | Whether to perform action on valid items even if some ones fail
val returnEntity : kotlin.Boolean = true // kotlin.Boolean | Return information about newly created entity
val mode : kotlin.String = mode_example // kotlin.String | Response mode
try {
    apiInstance.restFilesActionsMobileSyncItemsPost(idColonIn, partialSuccess, returnEntity, mode)
} catch (e: ClientException) {
    println("4xx response calling MobileSyncApi#restFilesActionsMobileSyncItemsPost")
    e.printStackTrace()
} catch (e: ServerException) {
    println("5xx response calling MobileSyncApi#restFilesActionsMobileSyncItemsPost")
    e.printStackTrace()
}
```

### Parameters

Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **idColonIn** | **kotlin.String**| Array of values which are going to be changed. |
 **partialSuccess** | **kotlin.Boolean**| Whether to perform action on valid items even if some ones fail | [optional]
 **returnEntity** | **kotlin.Boolean**| Return information about newly created entity | [optional]
 **mode** | **kotlin.String**| Response mode | [optional]

### Return type

null (empty response body)

### Authorization

No authorization required

### HTTP request headers

 - **Content-Type**: Not defined
 - **Accept**: Not defined

<a id="restFilesActionsPushDelete"></a>
# **restFilesActionsPushDelete**
> restFilesActionsPushDelete(idColonIn, partialSuccess, mode)

Un-Push collection of files

Un-Pushing files deletes these files from all folder members sync list.

### Example
```kotlin
// Import classes:
//import org.openapitools.client.infrastructure.*
//import org.openapitools.client.models.*

val apiInstance = MobileSyncApi()
val idColonIn : kotlin.String = idColonIn_example // kotlin.String | Array of values which are going to be changed.
val partialSuccess : kotlin.Boolean = true // kotlin.Boolean | Whether to perform action on valid items even if some ones fail
val mode : kotlin.String = mode_example // kotlin.String | Response mode
try {
    apiInstance.restFilesActionsPushDelete(idColonIn, partialSuccess, mode)
} catch (e: ClientException) {
    println("4xx response calling MobileSyncApi#restFilesActionsPushDelete")
    e.printStackTrace()
} catch (e: ServerException) {
    println("5xx response calling MobileSyncApi#restFilesActionsPushDelete")
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

<a id="restFilesActionsPushPost"></a>
# **restFilesActionsPushPost**
> restFilesActionsPushPost(idColonIn, partialSuccess, returnEntity, mode)

Push files list to mobile sync list

Set list of files as mobile sync item for all folder members. This operation will not return location headers for each entity created, if the inserted records are         required, returnEntity should be set to true.

### Example
```kotlin
// Import classes:
//import org.openapitools.client.infrastructure.*
//import org.openapitools.client.models.*

val apiInstance = MobileSyncApi()
val idColonIn : kotlin.String = idColonIn_example // kotlin.String | Array of values which are going to be changed.
val partialSuccess : kotlin.Boolean = true // kotlin.Boolean | Whether to perform action on valid items even if some ones fail
val returnEntity : kotlin.Boolean = true // kotlin.Boolean | Return information about newly created entity
val mode : kotlin.String = mode_example // kotlin.String | Response mode
try {
    apiInstance.restFilesActionsPushPost(idColonIn, partialSuccess, returnEntity, mode)
} catch (e: ClientException) {
    println("4xx response calling MobileSyncApi#restFilesActionsPushPost")
    e.printStackTrace()
} catch (e: ServerException) {
    println("5xx response calling MobileSyncApi#restFilesActionsPushPost")
    e.printStackTrace()
}
```

### Parameters

Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **idColonIn** | **kotlin.String**| Array of values which are going to be changed. |
 **partialSuccess** | **kotlin.Boolean**| Whether to perform action on valid items even if some ones fail | [optional]
 **returnEntity** | **kotlin.Boolean**| Return information about newly created entity | [optional]
 **mode** | **kotlin.String**| Response mode | [optional]

### Return type

null (empty response body)

### Authorization

No authorization required

### HTTP request headers

 - **Content-Type**: Not defined
 - **Accept**: Not defined

<a id="restFilesIdActionsPushDelete"></a>
# **restFilesIdActionsPushDelete**
> restFilesIdActionsPushDelete(id, returnEntity, mode)

Un-Push file

Un-Pushing file deletes this file from all folder members sync list.

### Example
```kotlin
// Import classes:
//import org.openapitools.client.infrastructure.*
//import org.openapitools.client.models.*

val apiInstance = MobileSyncApi()
val id : kotlin.String = id_example // kotlin.String | File id
val returnEntity : kotlin.Boolean = true // kotlin.Boolean | Return information about newly created entity
val mode : kotlin.String = mode_example // kotlin.String | Response mode
try {
    apiInstance.restFilesIdActionsPushDelete(id, returnEntity, mode)
} catch (e: ClientException) {
    println("4xx response calling MobileSyncApi#restFilesIdActionsPushDelete")
    e.printStackTrace()
} catch (e: ServerException) {
    println("5xx response calling MobileSyncApi#restFilesIdActionsPushDelete")
    e.printStackTrace()
}
```

### Parameters

Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **id** | **kotlin.String**| File id |
 **returnEntity** | **kotlin.Boolean**| Return information about newly created entity | [optional]
 **mode** | **kotlin.String**| Response mode | [optional]

### Return type

null (empty response body)

### Authorization

No authorization required

### HTTP request headers

 - **Content-Type**: Not defined
 - **Accept**: Not defined

<a id="restFilesIdActionsPushPost"></a>
# **restFilesIdActionsPushPost**
> restFilesIdActionsPushPost(id, returnEntity, mode)

Push file to mobile sync list

Set file as mobile sync item for all folder members.

### Example
```kotlin
// Import classes:
//import org.openapitools.client.infrastructure.*
//import org.openapitools.client.models.*

val apiInstance = MobileSyncApi()
val id : kotlin.String = id_example // kotlin.String | ID of the file
val returnEntity : kotlin.Boolean = true // kotlin.Boolean | Return information about newly created entity
val mode : kotlin.String = mode_example // kotlin.String | Response mode
try {
    apiInstance.restFilesIdActionsPushPost(id, returnEntity, mode)
} catch (e: ClientException) {
    println("4xx response calling MobileSyncApi#restFilesIdActionsPushPost")
    e.printStackTrace()
} catch (e: ServerException) {
    println("5xx response calling MobileSyncApi#restFilesIdActionsPushPost")
    e.printStackTrace()
}
```

### Parameters

Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **id** | **kotlin.String**| ID of the file |
 **returnEntity** | **kotlin.Boolean**| Return information about newly created entity | [optional]
 **mode** | **kotlin.String**| Response mode | [optional]

### Return type

null (empty response body)

### Authorization

No authorization required

### HTTP request headers

 - **Content-Type**: Not defined
 - **Accept**: Not defined

<a id="restMobileSyncItemsGet"></a>
# **restMobileSyncItemsGet**
> MobileSyncList restMobileSyncItemsGet(with, avStatus, limit, mode, dlpStatus, orderBy, offset, returnEntity)

Returns a list of mobile sync items for current user

Returns a list of mobile sync items for current user

### Example
```kotlin
// Import classes:
//import org.openapitools.client.infrastructure.*
//import org.openapitools.client.models.*

val apiInstance = MobileSyncApi()
val with : kotlin.String = with_example // kotlin.String | 
val avStatus : kotlin.String = avStatus_example // kotlin.String | Search by avStatus
val limit : kotlin.Int = 56 // kotlin.Int | 
val mode : kotlin.String = mode_example // kotlin.String | 
val dlpStatus : kotlin.String = dlpStatus_example // kotlin.String | Search by dlpStatus
val orderBy : kotlin.String = orderBy_example // kotlin.String | 
val offset : kotlin.Int = 56 // kotlin.Int | 
val returnEntity : kotlin.Boolean = true // kotlin.Boolean | 
try {
    val result : MobileSyncList = apiInstance.restMobileSyncItemsGet(with, avStatus, limit, mode, dlpStatus, orderBy, offset, returnEntity)
    println(result)
} catch (e: ClientException) {
    println("4xx response calling MobileSyncApi#restMobileSyncItemsGet")
    e.printStackTrace()
} catch (e: ServerException) {
    println("5xx response calling MobileSyncApi#restMobileSyncItemsGet")
    e.printStackTrace()
}
```

### Parameters

Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **with** | **kotlin.String**|  | [optional]
 **avStatus** | **kotlin.String**| Search by avStatus | [optional]
 **limit** | **kotlin.Int**|  | [optional]
 **mode** | **kotlin.String**|  | [optional]
 **dlpStatus** | **kotlin.String**| Search by dlpStatus | [optional]
 **orderBy** | **kotlin.String**|  | [optional]
 **offset** | **kotlin.Int**|  | [optional]
 **returnEntity** | **kotlin.Boolean**|  | [optional]

### Return type

[**MobileSyncList**](MobileSyncList.md)

### Authorization

No authorization required

### HTTP request headers

 - **Content-Type**: Not defined
 - **Accept**: */*

<a id="restMobileSyncItemsIdDelete"></a>
# **restMobileSyncItemsIdDelete**
> restMobileSyncItemsIdDelete(id)

Remove mobile sync item

Removing mobile sync item

### Example
```kotlin
// Import classes:
//import org.openapitools.client.infrastructure.*
//import org.openapitools.client.models.*

val apiInstance = MobileSyncApi()
val id : kotlin.Int = 56 // kotlin.Int | ID of the mobile sync item to be removed
try {
    apiInstance.restMobileSyncItemsIdDelete(id)
} catch (e: ClientException) {
    println("4xx response calling MobileSyncApi#restMobileSyncItemsIdDelete")
    e.printStackTrace()
} catch (e: ServerException) {
    println("5xx response calling MobileSyncApi#restMobileSyncItemsIdDelete")
    e.printStackTrace()
}
```

### Parameters

Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **id** | **kotlin.Int**| ID of the mobile sync item to be removed |

### Return type

null (empty response body)

### Authorization

No authorization required

### HTTP request headers

 - **Content-Type**: Not defined
 - **Accept**: Not defined

<a id="restMobileSyncItemsIdGet"></a>
# **restMobileSyncItemsIdGet**
> MobileSync restMobileSyncItemsIdGet(id, mode, with, returnEntity)

Retrieve information about mobile sync item specified.

Retrieve information about mobile sync item specified.

### Example
```kotlin
// Import classes:
//import org.openapitools.client.infrastructure.*
//import org.openapitools.client.models.*

val apiInstance = MobileSyncApi()
val id : kotlin.Int = 56 // kotlin.Int | The ID of the entity
val mode : kotlin.String = mode_example // kotlin.String | 
val with : kotlin.String = with_example // kotlin.String | 
val returnEntity : kotlin.Boolean = true // kotlin.Boolean | 
try {
    val result : MobileSync = apiInstance.restMobileSyncItemsIdGet(id, mode, with, returnEntity)
    println(result)
} catch (e: ClientException) {
    println("4xx response calling MobileSyncApi#restMobileSyncItemsIdGet")
    e.printStackTrace()
} catch (e: ServerException) {
    println("5xx response calling MobileSyncApi#restMobileSyncItemsIdGet")
    e.printStackTrace()
}
```

### Parameters

Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **id** | **kotlin.Int**| The ID of the entity |
 **mode** | **kotlin.String**|  | [optional]
 **with** | **kotlin.String**|  | [optional]
 **returnEntity** | **kotlin.Boolean**|  | [optional]

### Return type

[**MobileSync**](MobileSync.md)

### Authorization

No authorization required

### HTTP request headers

 - **Content-Type**: Not defined
 - **Accept**: */*

<a id="restMobileSyncItemsPost"></a>
# **restMobileSyncItemsPost**
> restMobileSyncItemsPost(body, returnEntity, mode)

Set file as a mobile sync item

Set file as a mobile sync item.

### Example
```kotlin
// Import classes:
//import org.openapitools.client.infrastructure.*
//import org.openapitools.client.models.*

val apiInstance = MobileSyncApi()
val body : MobileSyncPost =  // MobileSyncPost | The contact details
val returnEntity : kotlin.Boolean = true // kotlin.Boolean | Return information about newly created entity
val mode : kotlin.String = mode_example // kotlin.String | Response mode
try {
    apiInstance.restMobileSyncItemsPost(body, returnEntity, mode)
} catch (e: ClientException) {
    println("4xx response calling MobileSyncApi#restMobileSyncItemsPost")
    e.printStackTrace()
} catch (e: ServerException) {
    println("5xx response calling MobileSyncApi#restMobileSyncItemsPost")
    e.printStackTrace()
}
```

### Parameters

Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **body** | [**MobileSyncPost**](MobileSyncPost.md)| The contact details |
 **returnEntity** | **kotlin.Boolean**| Return information about newly created entity | [optional]
 **mode** | **kotlin.String**| Response mode | [optional]

### Return type

null (empty response body)

### Authorization

No authorization required

### HTTP request headers

 - **Content-Type**: Not defined
 - **Accept**: Not defined

