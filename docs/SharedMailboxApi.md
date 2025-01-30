# SharedMailboxApi

All URIs are relative to *http://localhost*

Method | HTTP request | Description
------------- | ------------- | -------------
[**restAdminSharedMailboxesDelete**](SharedMailboxApi.md#restAdminSharedMailboxesDelete) | **DELETE** /rest/admin/sharedMailboxes | Delete shared mailboxes
[**restAdminSharedMailboxesGet**](SharedMailboxApi.md#restAdminSharedMailboxesGet) | **GET** /rest/admin/sharedMailboxes | Get shared mailbox list by user id list
[**restAdminSharedMailboxesIdPatch**](SharedMailboxApi.md#restAdminSharedMailboxesIdPatch) | **PATCH** /rest/admin/sharedMailboxes/{id} | Update shared mailbox members
[**restAdminSharedMailboxesPost**](SharedMailboxApi.md#restAdminSharedMailboxesPost) | **POST** /rest/admin/sharedMailboxes | Add shared mailbox record
[**restSharedMailboxesGet**](SharedMailboxApi.md#restSharedMailboxesGet) | **GET** /rest/sharedMailboxes | Get current user&#39;s shared mailboxes
[**restSharedMailboxesIdSettingsGet**](SharedMailboxApi.md#restSharedMailboxesIdSettingsGet) | **GET** /rest/sharedMailboxes/{id}/settings | Get current user&#39;s shared mailboxes setting
[**restSharedMailboxesIdWebFormsGet**](SharedMailboxApi.md#restSharedMailboxesIdWebFormsGet) | **GET** /rest/sharedMailboxes/{id}/webForms | List web forms available to shared mailboxes
[**restSharedMailboxesMailActionsCountersGet**](SharedMailboxApi.md#restSharedMailboxesMailActionsCountersGet) | **GET** /rest/sharedMailboxes/mail/actions/counters | Get current user&#39;s shared mailboxes counters
[**restSharedMailboxesPatch**](SharedMailboxApi.md#restSharedMailboxesPatch) | **PATCH** /rest/sharedMailboxes | Update current user&#39;s shared mailbox active status


<a id="restAdminSharedMailboxesDelete"></a>
# **restAdminSharedMailboxesDelete**
> restAdminSharedMailboxesDelete(idColonIn)

Delete shared mailboxes

Delete shared mailboxes

### Example
```kotlin
// Import classes:
//import org.openapitools.client.infrastructure.*
//import org.openapitools.client.models.*

val apiInstance = SharedMailboxApi()
val idColonIn : kotlin.collections.List<kotlin.String> =  // kotlin.collections.List<kotlin.String> | Shared mailbox user id list recommended request size <= 100
try {
    apiInstance.restAdminSharedMailboxesDelete(idColonIn)
} catch (e: ClientException) {
    println("4xx response calling SharedMailboxApi#restAdminSharedMailboxesDelete")
    e.printStackTrace()
} catch (e: ServerException) {
    println("5xx response calling SharedMailboxApi#restAdminSharedMailboxesDelete")
    e.printStackTrace()
}
```

### Parameters

Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **idColonIn** | [**kotlin.collections.List&lt;kotlin.String&gt;**](kotlin.String.md)| Shared mailbox user id list recommended request size &lt;&#x3D; 100 | [optional]

### Return type

null (empty response body)

### Authorization

No authorization required

### HTTP request headers

 - **Content-Type**: Not defined
 - **Accept**: Not defined

<a id="restAdminSharedMailboxesGet"></a>
# **restAdminSharedMailboxesGet**
> SharedMailboxList restAdminSharedMailboxesGet(active, limit, idColonIn, orderBy, offset)

Get shared mailbox list by user id list

Get shared mailbox list by user id list

### Example
```kotlin
// Import classes:
//import org.openapitools.client.infrastructure.*
//import org.openapitools.client.models.*

val apiInstance = SharedMailboxApi()
val active : kotlin.Boolean = true // kotlin.Boolean | 
val limit : kotlin.Int = 56 // kotlin.Int | 
val idColonIn : kotlin.collections.List<kotlin.String> =  // kotlin.collections.List<kotlin.String> | Shared mailbox user id list recommended request size <= 100
val orderBy : kotlin.String = orderBy_example // kotlin.String | 
val offset : kotlin.Int = 56 // kotlin.Int | 
try {
    val result : SharedMailboxList = apiInstance.restAdminSharedMailboxesGet(active, limit, idColonIn, orderBy, offset)
    println(result)
} catch (e: ClientException) {
    println("4xx response calling SharedMailboxApi#restAdminSharedMailboxesGet")
    e.printStackTrace()
} catch (e: ServerException) {
    println("5xx response calling SharedMailboxApi#restAdminSharedMailboxesGet")
    e.printStackTrace()
}
```

### Parameters

Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **active** | **kotlin.Boolean**|  | [optional]
 **limit** | **kotlin.Int**|  | [optional]
 **idColonIn** | [**kotlin.collections.List&lt;kotlin.String&gt;**](kotlin.String.md)| Shared mailbox user id list recommended request size &lt;&#x3D; 100 | [optional]
 **orderBy** | **kotlin.String**|  | [optional]
 **offset** | **kotlin.Int**|  | [optional]

### Return type

[**SharedMailboxList**](SharedMailboxList.md)

### Authorization

No authorization required

### HTTP request headers

 - **Content-Type**: Not defined
 - **Accept**: */*

<a id="restAdminSharedMailboxesIdPatch"></a>
# **restAdminSharedMailboxesIdPatch**
> SharedMailbox restAdminSharedMailboxesIdPatch(id, body)

Update shared mailbox members

Update shared mailbox members

### Example
```kotlin
// Import classes:
//import org.openapitools.client.infrastructure.*
//import org.openapitools.client.models.*

val apiInstance = SharedMailboxApi()
val id : kotlin.String = id_example // kotlin.String | User ID
val body : SharedMailboxPatchRequest =  // SharedMailboxPatchRequest | 
try {
    val result : SharedMailbox = apiInstance.restAdminSharedMailboxesIdPatch(id, body)
    println(result)
} catch (e: ClientException) {
    println("4xx response calling SharedMailboxApi#restAdminSharedMailboxesIdPatch")
    e.printStackTrace()
} catch (e: ServerException) {
    println("5xx response calling SharedMailboxApi#restAdminSharedMailboxesIdPatch")
    e.printStackTrace()
}
```

### Parameters

Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **id** | **kotlin.String**| User ID |
 **body** | [**SharedMailboxPatchRequest**](SharedMailboxPatchRequest.md)|  |

### Return type

[**SharedMailbox**](SharedMailbox.md)

### Authorization

No authorization required

### HTTP request headers

 - **Content-Type**: Not defined
 - **Accept**: */*

<a id="restAdminSharedMailboxesPost"></a>
# **restAdminSharedMailboxesPost**
> SharedMailbox restAdminSharedMailboxesPost(body)

Add shared mailbox record

Add shared mailbox

### Example
```kotlin
// Import classes:
//import org.openapitools.client.infrastructure.*
//import org.openapitools.client.models.*

val apiInstance = SharedMailboxApi()
val body : SharedMailboxPostRequest =  // SharedMailboxPostRequest | 
try {
    val result : SharedMailbox = apiInstance.restAdminSharedMailboxesPost(body)
    println(result)
} catch (e: ClientException) {
    println("4xx response calling SharedMailboxApi#restAdminSharedMailboxesPost")
    e.printStackTrace()
} catch (e: ServerException) {
    println("5xx response calling SharedMailboxApi#restAdminSharedMailboxesPost")
    e.printStackTrace()
}
```

### Parameters

Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **body** | [**SharedMailboxPostRequest**](SharedMailboxPostRequest.md)|  |

### Return type

[**SharedMailbox**](SharedMailbox.md)

### Authorization

No authorization required

### HTTP request headers

 - **Content-Type**: Not defined
 - **Accept**: */*

<a id="restSharedMailboxesGet"></a>
# **restSharedMailboxesGet**
> SharedMailboxList restSharedMailboxesGet(active, limit, idColonIn, orderBy, offset)

Get current user&#39;s shared mailboxes

Get current user&#39;s shared mailboxes

### Example
```kotlin
// Import classes:
//import org.openapitools.client.infrastructure.*
//import org.openapitools.client.models.*

val apiInstance = SharedMailboxApi()
val active : kotlin.Boolean = true // kotlin.Boolean | 
val limit : kotlin.Int = 56 // kotlin.Int | 
val idColonIn : kotlin.collections.List<kotlin.String> =  // kotlin.collections.List<kotlin.String> | Shared mailbox user id list recommended request size <= 100
val orderBy : kotlin.String = orderBy_example // kotlin.String | 
val offset : kotlin.Int = 56 // kotlin.Int | 
try {
    val result : SharedMailboxList = apiInstance.restSharedMailboxesGet(active, limit, idColonIn, orderBy, offset)
    println(result)
} catch (e: ClientException) {
    println("4xx response calling SharedMailboxApi#restSharedMailboxesGet")
    e.printStackTrace()
} catch (e: ServerException) {
    println("5xx response calling SharedMailboxApi#restSharedMailboxesGet")
    e.printStackTrace()
}
```

### Parameters

Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **active** | **kotlin.Boolean**|  | [optional]
 **limit** | **kotlin.Int**|  | [optional]
 **idColonIn** | [**kotlin.collections.List&lt;kotlin.String&gt;**](kotlin.String.md)| Shared mailbox user id list recommended request size &lt;&#x3D; 100 | [optional]
 **orderBy** | **kotlin.String**|  | [optional]
 **offset** | **kotlin.Int**|  | [optional]

### Return type

[**SharedMailboxList**](SharedMailboxList.md)

### Authorization

No authorization required

### HTTP request headers

 - **Content-Type**: Not defined
 - **Accept**: */*

<a id="restSharedMailboxesIdSettingsGet"></a>
# **restSharedMailboxesIdSettingsGet**
> SharedMailboxSetting restSharedMailboxesIdSettingsGet(id)

Get current user&#39;s shared mailboxes setting

Get current user&#39;s shared mailboxes setting

### Example
```kotlin
// Import classes:
//import org.openapitools.client.infrastructure.*
//import org.openapitools.client.models.*

val apiInstance = SharedMailboxApi()
val id : kotlin.String = id_example // kotlin.String | User ID
try {
    val result : SharedMailboxSetting = apiInstance.restSharedMailboxesIdSettingsGet(id)
    println(result)
} catch (e: ClientException) {
    println("4xx response calling SharedMailboxApi#restSharedMailboxesIdSettingsGet")
    e.printStackTrace()
} catch (e: ServerException) {
    println("5xx response calling SharedMailboxApi#restSharedMailboxesIdSettingsGet")
    e.printStackTrace()
}
```

### Parameters

Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **id** | **kotlin.String**| User ID |

### Return type

[**SharedMailboxSetting**](SharedMailboxSetting.md)

### Authorization

No authorization required

### HTTP request headers

 - **Content-Type**: Not defined
 - **Accept**: */*

<a id="restSharedMailboxesIdWebFormsGet"></a>
# **restSharedMailboxesIdWebFormsGet**
> WebFormList restSharedMailboxesIdWebFormsGet(id, mode, with, returnEntity)

List web forms available to shared mailboxes

Returns a list of web forms available to shared mailboxes

### Example
```kotlin
// Import classes:
//import org.openapitools.client.infrastructure.*
//import org.openapitools.client.models.*

val apiInstance = SharedMailboxApi()
val id : kotlin.String = id_example // kotlin.String | User ID
val mode : kotlin.String = mode_example // kotlin.String | 
val with : kotlin.String = with_example // kotlin.String | 
val returnEntity : kotlin.Boolean = true // kotlin.Boolean | 
try {
    val result : WebFormList = apiInstance.restSharedMailboxesIdWebFormsGet(id, mode, with, returnEntity)
    println(result)
} catch (e: ClientException) {
    println("4xx response calling SharedMailboxApi#restSharedMailboxesIdWebFormsGet")
    e.printStackTrace()
} catch (e: ServerException) {
    println("5xx response calling SharedMailboxApi#restSharedMailboxesIdWebFormsGet")
    e.printStackTrace()
}
```

### Parameters

Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **id** | **kotlin.String**| User ID |
 **mode** | **kotlin.String**|  | [optional]
 **with** | **kotlin.String**|  | [optional]
 **returnEntity** | **kotlin.Boolean**|  | [optional]

### Return type

[**WebFormList**](WebFormList.md)

### Authorization

No authorization required

### HTTP request headers

 - **Content-Type**: Not defined
 - **Accept**: */*

<a id="restSharedMailboxesMailActionsCountersGet"></a>
# **restSharedMailboxesMailActionsCountersGet**
> MailCountersList restSharedMailboxesMailActionsCountersGet(idColonIn)

Get current user&#39;s shared mailboxes counters

Get current user&#39;s shared mailboxes counters

### Example
```kotlin
// Import classes:
//import org.openapitools.client.infrastructure.*
//import org.openapitools.client.models.*

val apiInstance = SharedMailboxApi()
val idColonIn : kotlin.collections.List<kotlin.String> =  // kotlin.collections.List<kotlin.String> | Shared mailbox user id list recommended request size <= 100
try {
    val result : MailCountersList = apiInstance.restSharedMailboxesMailActionsCountersGet(idColonIn)
    println(result)
} catch (e: ClientException) {
    println("4xx response calling SharedMailboxApi#restSharedMailboxesMailActionsCountersGet")
    e.printStackTrace()
} catch (e: ServerException) {
    println("5xx response calling SharedMailboxApi#restSharedMailboxesMailActionsCountersGet")
    e.printStackTrace()
}
```

### Parameters

Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **idColonIn** | [**kotlin.collections.List&lt;kotlin.String&gt;**](kotlin.String.md)| Shared mailbox user id list recommended request size &lt;&#x3D; 100 | [optional]

### Return type

[**MailCountersList**](MailCountersList.md)

### Authorization

No authorization required

### HTTP request headers

 - **Content-Type**: Not defined
 - **Accept**: */*

<a id="restSharedMailboxesPatch"></a>
# **restSharedMailboxesPatch**
> SharedMailboxList restSharedMailboxesPatch(body)

Update current user&#39;s shared mailbox active status

Update current user&#39;s shared mailbox active status

### Example
```kotlin
// Import classes:
//import org.openapitools.client.infrastructure.*
//import org.openapitools.client.models.*

val apiInstance = SharedMailboxApi()
val body : SharedMailboxStatusPatchRequest =  // SharedMailboxStatusPatchRequest | 
try {
    val result : SharedMailboxList = apiInstance.restSharedMailboxesPatch(body)
    println(result)
} catch (e: ClientException) {
    println("4xx response calling SharedMailboxApi#restSharedMailboxesPatch")
    e.printStackTrace()
} catch (e: ServerException) {
    println("5xx response calling SharedMailboxApi#restSharedMailboxesPatch")
    e.printStackTrace()
}
```

### Parameters

Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **body** | [**SharedMailboxStatusPatchRequest**](SharedMailboxStatusPatchRequest.md)|  |

### Return type

[**SharedMailboxList**](SharedMailboxList.md)

### Authorization

No authorization required

### HTTP request headers

 - **Content-Type**: Not defined
 - **Accept**: */*

