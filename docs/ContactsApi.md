# ContactsApi

All URIs are relative to *http://localhost*

Method | HTTP request | Description
------------- | ------------- | -------------
[**restContactsGet**](ContactsApi.md#restContactsGet) | **GET** /rest/contacts | Get contacts list
[**restContactsIdDelete**](ContactsApi.md#restContactsIdDelete) | **DELETE** /rest/contacts/{id} | Deletes a contact entry
[**restContactsIdGet**](ContactsApi.md#restContactsIdGet) | **GET** /rest/contacts/{id} | Get a contact
[**restContactsIdPut**](ContactsApi.md#restContactsIdPut) | **PUT** /rest/contacts/{id} | Update a contact entry
[**restContactsPost**](ContactsApi.md#restContactsPost) | **POST** /rest/contacts | Create a contact entry


<a id="restContactsGet"></a>
# **restContactsGet**
> ContactList restContactsGet(nameColonContains, name, limit, orderBy, offset)

Get contacts list

Get contacts list

### Example
```kotlin
// Import classes:
//import org.openapitools.client.infrastructure.*
//import org.openapitools.client.models.*

val apiInstance = ContactsApi()
val nameColonContains : kotlin.String = nameColonContains_example // kotlin.String | 
val name : kotlin.String = name_example // kotlin.String | 
val limit : kotlin.Int = 56 // kotlin.Int | limit
val orderBy : kotlin.String = orderBy_example // kotlin.String | Sorting options. Accepts id, name. Sample format is id:asc
val offset : kotlin.Int = 56 // kotlin.Int | offset
try {
    val result : ContactList = apiInstance.restContactsGet(nameColonContains, name, limit, orderBy, offset)
    println(result)
} catch (e: ClientException) {
    println("4xx response calling ContactsApi#restContactsGet")
    e.printStackTrace()
} catch (e: ServerException) {
    println("5xx response calling ContactsApi#restContactsGet")
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

<a id="restContactsIdDelete"></a>
# **restContactsIdDelete**
> restContactsIdDelete(id)

Deletes a contact entry

Delete a contact entry from the kiteworks contact list for this user.

### Example
```kotlin
// Import classes:
//import org.openapitools.client.infrastructure.*
//import org.openapitools.client.models.*

val apiInstance = ContactsApi()
val id : kotlin.Int = 56 // kotlin.Int | The ID of the entity
try {
    apiInstance.restContactsIdDelete(id)
} catch (e: ClientException) {
    println("4xx response calling ContactsApi#restContactsIdDelete")
    e.printStackTrace()
} catch (e: ServerException) {
    println("5xx response calling ContactsApi#restContactsIdDelete")
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

<a id="restContactsIdGet"></a>
# **restContactsIdGet**
> Contact restContactsIdGet(id)

Get a contact

Returns the details of a specified kiteworks contact. e.g. I want the email address and name of this contact.

### Example
```kotlin
// Import classes:
//import org.openapitools.client.infrastructure.*
//import org.openapitools.client.models.*

val apiInstance = ContactsApi()
val id : kotlin.Int = 56 // kotlin.Int | The ID of the entity
try {
    val result : Contact = apiInstance.restContactsIdGet(id)
    println(result)
} catch (e: ClientException) {
    println("4xx response calling ContactsApi#restContactsIdGet")
    e.printStackTrace()
} catch (e: ServerException) {
    println("5xx response calling ContactsApi#restContactsIdGet")
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

<a id="restContactsIdPut"></a>
# **restContactsIdPut**
> restContactsIdPut(id)

Update a contact entry

Update a kiteworks contact. The email address and name can be changed.

### Example
```kotlin
// Import classes:
//import org.openapitools.client.infrastructure.*
//import org.openapitools.client.models.*

val apiInstance = ContactsApi()
val id : kotlin.Int = 56 // kotlin.Int | The ID of the entity
try {
    apiInstance.restContactsIdPut(id)
} catch (e: ClientException) {
    println("4xx response calling ContactsApi#restContactsIdPut")
    e.printStackTrace()
} catch (e: ServerException) {
    println("5xx response calling ContactsApi#restContactsIdPut")
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

<a id="restContactsPost"></a>
# **restContactsPost**
> Contact restContactsPost(body)

Create a contact entry

Creates a kiteworks contact entry that includes a contact name and email address.

### Example
```kotlin
// Import classes:
//import org.openapitools.client.infrastructure.*
//import org.openapitools.client.models.*

val apiInstance = ContactsApi()
val body : ContactCreate =  // ContactCreate | 
try {
    val result : Contact = apiInstance.restContactsPost(body)
    println(result)
} catch (e: ClientException) {
    println("4xx response calling ContactsApi#restContactsPost")
    e.printStackTrace()
} catch (e: ServerException) {
    println("5xx response calling ContactsApi#restContactsPost")
    e.printStackTrace()
}
```

### Parameters

Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **body** | [**ContactCreate**](ContactCreate.md)|  |

### Return type

[**Contact**](Contact.md)

### Authorization

No authorization required

### HTTP request headers

 - **Content-Type**: Not defined
 - **Accept**: */*

