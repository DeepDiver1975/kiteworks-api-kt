# DevicesApi

All URIs are relative to *http://localhost*

Method | HTTP request | Description
------------- | ------------- | -------------
[**restDevicesGet**](DevicesApi.md#restDevicesGet) | **GET** /rest/devices | List devices
[**restDevicesIdDelete**](DevicesApi.md#restDevicesIdDelete) | **DELETE** /rest/devices/{id} | Delete a device
[**restDevicesIdGet**](DevicesApi.md#restDevicesIdGet) | **GET** /rest/devices/{id} | Get a device
[**restDevicesIdPut**](DevicesApi.md#restDevicesIdPut) | **PUT** /rest/devices/{id} | Update a device
[**restDevicesInstallTagIdWipeGet**](DevicesApi.md#restDevicesInstallTagIdWipeGet) | **GET** /rest/devices/{install_tag_id}/wipe | Get the wipe status
[**restDevicesMeActionsLogoutDelete**](DevicesApi.md#restDevicesMeActionsLogoutDelete) | **DELETE** /rest/devices/me/actions/logout | Logout current user
[**restDevicesMeActionsWipePatch**](DevicesApi.md#restDevicesMeActionsWipePatch) | **PATCH** /rest/devices/me/actions/wipe | Tell the server the device had completed the requested wipe
[**restDevicesMeGet**](DevicesApi.md#restDevicesMeGet) | **GET** /rest/devices/me | Get current device info
[**restDevicesMePut**](DevicesApi.md#restDevicesMePut) | **PUT** /rest/devices/me | Update the currently signed-in device
[**restDevicesPost**](DevicesApi.md#restDevicesPost) | **POST** /rest/devices | Add a device
[**restUsersIdDevicesGet**](DevicesApi.md#restUsersIdDevicesGet) | **GET** /rest/users/{id}/devices | List devices for a user


<a id="restDevicesGet"></a>
# **restDevicesGet**
> kotlin.collections.List&lt;Device&gt; restDevicesGet(installTagId, installTagIdColonContains, userId, userIdColonIn, clientId, clientIdColonContains, orderBy, offset, limit, with, mode)

List devices

Return a list of devices. e.g.: Returns a list of devices, per user,                   that have authenticated on this server.                   The list includes the name of the device (iPad, iPhone, etc),                   install tag id, client id, and remote wipe flag.

### Example
```kotlin
// Import classes:
//import org.openapitools.client.infrastructure.*
//import org.openapitools.client.models.*

val apiInstance = DevicesApi()
val installTagId : kotlin.String = installTagId_example // kotlin.String | Unique identifier of install tag for this Device
val installTagIdColonContains : kotlin.String = installTagIdColonContains_example // kotlin.String | Unique identifier of install tag for this Device. Search for result that contains specified characters in this parameter.
val userId : kotlin.String = userId_example // kotlin.String | Unique identifier of user for this Device
val userIdColonIn : kotlin.String = userIdColonIn_example // kotlin.String | Unique identifier of user for this Device. Search for results that contain any of specified values of this parameter.
val clientId : kotlin.String = clientId_example // kotlin.String | Unique identifier of client for this Device
val clientIdColonContains : kotlin.String = clientIdColonContains_example // kotlin.String | Unique identifier of client for this Device. Search for result that contains specified characters in this parameter.
val orderBy : kotlin.collections.List<kotlin.String> =  // kotlin.collections.List<kotlin.String> | Sorting options
val offset : kotlin.Int = 56 // kotlin.Int | Offset
val limit : kotlin.Int = 56 // kotlin.Int | Limit
val with : kotlin.String = with_example // kotlin.String | With parameters
val mode : kotlin.String = mode_example // kotlin.String | Response mode
try {
    val result : kotlin.collections.List<Device> = apiInstance.restDevicesGet(installTagId, installTagIdColonContains, userId, userIdColonIn, clientId, clientIdColonContains, orderBy, offset, limit, with, mode)
    println(result)
} catch (e: ClientException) {
    println("4xx response calling DevicesApi#restDevicesGet")
    e.printStackTrace()
} catch (e: ServerException) {
    println("5xx response calling DevicesApi#restDevicesGet")
    e.printStackTrace()
}
```

### Parameters

Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **installTagId** | **kotlin.String**| Unique identifier of install tag for this Device | [optional]
 **installTagIdColonContains** | **kotlin.String**| Unique identifier of install tag for this Device. Search for result that contains specified characters in this parameter. | [optional]
 **userId** | **kotlin.String**| Unique identifier of user for this Device | [optional]
 **userIdColonIn** | **kotlin.String**| Unique identifier of user for this Device. Search for results that contain any of specified values of this parameter. | [optional]
 **clientId** | **kotlin.String**| Unique identifier of client for this Device | [optional]
 **clientIdColonContains** | **kotlin.String**| Unique identifier of client for this Device. Search for result that contains specified characters in this parameter. | [optional]
 **orderBy** | [**kotlin.collections.List&lt;kotlin.String&gt;**](kotlin.String.md)| Sorting options | [optional]
 **offset** | **kotlin.Int**| Offset | [optional]
 **limit** | **kotlin.Int**| Limit | [optional]
 **with** | **kotlin.String**| With parameters | [optional]
 **mode** | **kotlin.String**| Response mode | [optional]

### Return type

[**kotlin.collections.List&lt;Device&gt;**](Device.md)

### Authorization

No authorization required

### HTTP request headers

 - **Content-Type**: Not defined
 - **Accept**: */*

<a id="restDevicesIdDelete"></a>
# **restDevicesIdDelete**
> restDevicesIdDelete(id)

Delete a device

Delete a device given the client id

### Example
```kotlin
// Import classes:
//import org.openapitools.client.infrastructure.*
//import org.openapitools.client.models.*

val apiInstance = DevicesApi()
val id : kotlin.String = id_example // kotlin.String | ID of the device to be deleted
try {
    apiInstance.restDevicesIdDelete(id)
} catch (e: ClientException) {
    println("4xx response calling DevicesApi#restDevicesIdDelete")
    e.printStackTrace()
} catch (e: ServerException) {
    println("5xx response calling DevicesApi#restDevicesIdDelete")
    e.printStackTrace()
}
```

### Parameters

Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **id** | **kotlin.String**| ID of the device to be deleted |

### Return type

null (empty response body)

### Authorization

No authorization required

### HTTP request headers

 - **Content-Type**: Not defined
 - **Accept**: Not defined

<a id="restDevicesIdGet"></a>
# **restDevicesIdGet**
> Device restDevicesIdGet(id)

Get a device

Return the details of a specified device. Given the device id,                   return the device name, install tag id, client id, and remote wipe flag.

### Example
```kotlin
// Import classes:
//import org.openapitools.client.infrastructure.*
//import org.openapitools.client.models.*

val apiInstance = DevicesApi()
val id : kotlin.Int = 56 // kotlin.Int | ID of the device to be retrieved
try {
    val result : Device = apiInstance.restDevicesIdGet(id)
    println(result)
} catch (e: ClientException) {
    println("4xx response calling DevicesApi#restDevicesIdGet")
    e.printStackTrace()
} catch (e: ServerException) {
    println("5xx response calling DevicesApi#restDevicesIdGet")
    e.printStackTrace()
}
```

### Parameters

Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **id** | **kotlin.Int**| ID of the device to be retrieved |

### Return type

[**Device**](Device.md)

### Authorization

No authorization required

### HTTP request headers

 - **Content-Type**: Not defined
 - **Accept**: */*

<a id="restDevicesIdPut"></a>
# **restDevicesIdPut**
> restDevicesIdPut(id, body)

Update a device

Update the details of a device. Can change the mobile key store and messaging registration token.

### Example
```kotlin
// Import classes:
//import org.openapitools.client.infrastructure.*
//import org.openapitools.client.models.*

val apiInstance = DevicesApi()
val id : kotlin.Int = 56 // kotlin.Int | ID of the device to be updated
val body : DevicePut =  // DevicePut | Details of the device
try {
    apiInstance.restDevicesIdPut(id, body)
} catch (e: ClientException) {
    println("4xx response calling DevicesApi#restDevicesIdPut")
    e.printStackTrace()
} catch (e: ServerException) {
    println("5xx response calling DevicesApi#restDevicesIdPut")
    e.printStackTrace()
}
```

### Parameters

Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **id** | **kotlin.Int**| ID of the device to be updated |
 **body** | [**DevicePut**](DevicePut.md)| Details of the device |

### Return type

null (empty response body)

### Authorization

No authorization required

### HTTP request headers

 - **Content-Type**: Not defined
 - **Accept**: Not defined

<a id="restDevicesInstallTagIdWipeGet"></a>
# **restDevicesInstallTagIdWipeGet**
> kotlin.Int restDevicesInstallTagIdWipeGet(installTagId)

Get the wipe status

Returns the remote wipe status of a specified device identified by install_tag_id

### Example
```kotlin
// Import classes:
//import org.openapitools.client.infrastructure.*
//import org.openapitools.client.models.*

val apiInstance = DevicesApi()
val installTagId : kotlin.String = installTagId_example // kotlin.String | Unique identifier of install tag for this device. Usually the serial number of device
try {
    val result : kotlin.Int = apiInstance.restDevicesInstallTagIdWipeGet(installTagId)
    println(result)
} catch (e: ClientException) {
    println("4xx response calling DevicesApi#restDevicesInstallTagIdWipeGet")
    e.printStackTrace()
} catch (e: ServerException) {
    println("5xx response calling DevicesApi#restDevicesInstallTagIdWipeGet")
    e.printStackTrace()
}
```

### Parameters

Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **installTagId** | **kotlin.String**| Unique identifier of install tag for this device. Usually the serial number of device |

### Return type

**kotlin.Int**

### Authorization

No authorization required

### HTTP request headers

 - **Content-Type**: Not defined
 - **Accept**: */*

<a id="restDevicesMeActionsLogoutDelete"></a>
# **restDevicesMeActionsLogoutDelete**
> Logout restDevicesMeActionsLogoutDelete()

Logout current user

Logout current user

### Example
```kotlin
// Import classes:
//import org.openapitools.client.infrastructure.*
//import org.openapitools.client.models.*

val apiInstance = DevicesApi()
try {
    val result : Logout = apiInstance.restDevicesMeActionsLogoutDelete()
    println(result)
} catch (e: ClientException) {
    println("4xx response calling DevicesApi#restDevicesMeActionsLogoutDelete")
    e.printStackTrace()
} catch (e: ServerException) {
    println("5xx response calling DevicesApi#restDevicesMeActionsLogoutDelete")
    e.printStackTrace()
}
```

### Parameters
This endpoint does not need any parameter.

### Return type

[**Logout**](Logout.md)

### Authorization

No authorization required

### HTTP request headers

 - **Content-Type**: Not defined
 - **Accept**: */*

<a id="restDevicesMeActionsWipePatch"></a>
# **restDevicesMeActionsWipePatch**
> restDevicesMeActionsWipePatch()

Tell the server the device had completed the requested wipe

Update the wipe flag to completed

### Example
```kotlin
// Import classes:
//import org.openapitools.client.infrastructure.*
//import org.openapitools.client.models.*

val apiInstance = DevicesApi()
try {
    apiInstance.restDevicesMeActionsWipePatch()
} catch (e: ClientException) {
    println("4xx response calling DevicesApi#restDevicesMeActionsWipePatch")
    e.printStackTrace()
} catch (e: ServerException) {
    println("5xx response calling DevicesApi#restDevicesMeActionsWipePatch")
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

<a id="restDevicesMeGet"></a>
# **restDevicesMeGet**
> Device restDevicesMeGet()

Get current device info

Return the details of the current device.

### Example
```kotlin
// Import classes:
//import org.openapitools.client.infrastructure.*
//import org.openapitools.client.models.*

val apiInstance = DevicesApi()
try {
    val result : Device = apiInstance.restDevicesMeGet()
    println(result)
} catch (e: ClientException) {
    println("4xx response calling DevicesApi#restDevicesMeGet")
    e.printStackTrace()
} catch (e: ServerException) {
    println("5xx response calling DevicesApi#restDevicesMeGet")
    e.printStackTrace()
}
```

### Parameters
This endpoint does not need any parameter.

### Return type

[**Device**](Device.md)

### Authorization

No authorization required

### HTTP request headers

 - **Content-Type**: Not defined
 - **Accept**: */*

<a id="restDevicesMePut"></a>
# **restDevicesMePut**
> restDevicesMePut(body)

Update the currently signed-in device

Update the details of the current device. Can change the mobile key store and messaging registration token.

### Example
```kotlin
// Import classes:
//import org.openapitools.client.infrastructure.*
//import org.openapitools.client.models.*

val apiInstance = DevicesApi()
val body : DevicePut =  // DevicePut | Details of the device
try {
    apiInstance.restDevicesMePut(body)
} catch (e: ClientException) {
    println("4xx response calling DevicesApi#restDevicesMePut")
    e.printStackTrace()
} catch (e: ServerException) {
    println("5xx response calling DevicesApi#restDevicesMePut")
    e.printStackTrace()
}
```

### Parameters

Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **body** | [**DevicePut**](DevicePut.md)| Details of the device |

### Return type

null (empty response body)

### Authorization

No authorization required

### HTTP request headers

 - **Content-Type**: Not defined
 - **Accept**: Not defined

<a id="restDevicesPost"></a>
# **restDevicesPost**
> restDevicesPost(body, returnEntity, mode)

Add a device

Add a device.                    This method is used when a user logs in to kiteworks to track the device they use.

### Example
```kotlin
// Import classes:
//import org.openapitools.client.infrastructure.*
//import org.openapitools.client.models.*

val apiInstance = DevicesApi()
val body : DevicePost =  // DevicePost | Details of the device
val returnEntity : kotlin.Boolean = true // kotlin.Boolean | Return information about newly created entity
val mode : kotlin.String = mode_example // kotlin.String | Response mode
try {
    apiInstance.restDevicesPost(body, returnEntity, mode)
} catch (e: ClientException) {
    println("4xx response calling DevicesApi#restDevicesPost")
    e.printStackTrace()
} catch (e: ServerException) {
    println("5xx response calling DevicesApi#restDevicesPost")
    e.printStackTrace()
}
```

### Parameters

Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **body** | [**DevicePost**](DevicePost.md)| Details of the device |
 **returnEntity** | **kotlin.Boolean**| Return information about newly created entity | [optional]
 **mode** | **kotlin.String**| Response mode | [optional]

### Return type

null (empty response body)

### Authorization

No authorization required

### HTTP request headers

 - **Content-Type**: Not defined
 - **Accept**: Not defined

<a id="restUsersIdDevicesGet"></a>
# **restUsersIdDevicesGet**
> kotlin.collections.List&lt;Device&gt; restUsersIdDevicesGet(id)

List devices for a user

Return a list of devices for a specific user

### Example
```kotlin
// Import classes:
//import org.openapitools.client.infrastructure.*
//import org.openapitools.client.models.*

val apiInstance = DevicesApi()
val id : kotlin.String = id_example // kotlin.String | ID of the user whose devices to be retrieved
try {
    val result : kotlin.collections.List<Device> = apiInstance.restUsersIdDevicesGet(id)
    println(result)
} catch (e: ClientException) {
    println("4xx response calling DevicesApi#restUsersIdDevicesGet")
    e.printStackTrace()
} catch (e: ServerException) {
    println("5xx response calling DevicesApi#restUsersIdDevicesGet")
    e.printStackTrace()
}
```

### Parameters

Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **id** | **kotlin.String**| ID of the user whose devices to be retrieved |

### Return type

[**kotlin.collections.List&lt;Device&gt;**](Device.md)

### Authorization

No authorization required

### HTTP request headers

 - **Content-Type**: Not defined
 - **Accept**: */*

