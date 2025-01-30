# LdapGroupsApi

All URIs are relative to *http://localhost*

Method | HTTP request | Description
------------- | ------------- | -------------
[**restLdapGroupsGet**](LdapGroupsApi.md#restLdapGroupsGet) | **GET** /rest/ldapGroups | Returns a list of LDAP groups.
[**restLdapGroupsIdDelete**](LdapGroupsApi.md#restLdapGroupsIdDelete) | **DELETE** /rest/ldapGroups/{id} | Deletes an LDAP group
[**restLdapGroupsIdGet**](LdapGroupsApi.md#restLdapGroupsIdGet) | **GET** /rest/ldapGroups/{id} | Gets an LDAP group
[**restLdapGroupsIdPut**](LdapGroupsApi.md#restLdapGroupsIdPut) | **PUT** /rest/ldapGroups/{id} | Updates an LDAP group
[**restLdapGroupsPost**](LdapGroupsApi.md#restLdapGroupsPost) | **POST** /rest/ldapGroups | Create an LDAP group


<a id="restLdapGroupsGet"></a>
# **restLdapGroupsGet**
> kotlin.collections.List&lt;LdapGroup&gt; restLdapGroupsGet(name, nameColonContains, email, emailColonContains, orderBy, offset, limit, with, mode)

Returns a list of LDAP groups.

Returns a list of LDAP groups that have been enabled through the kiteworks admin.

### Example
```kotlin
// Import classes:
//import org.openapitools.client.infrastructure.*
//import org.openapitools.client.models.*

val apiInstance = LdapGroupsApi()
val name : kotlin.String = name_example // kotlin.String | LDAP group name
val nameColonContains : kotlin.String = nameColonContains_example // kotlin.String | LDAP group name. Search for result that contains specified characters in this parameter.
val email : kotlin.String = email_example // kotlin.String | LDAP group Email
val emailColonContains : kotlin.String = emailColonContains_example // kotlin.String | LDAP group Email. Search for result that contains specified characters in this parameter.
val orderBy : kotlin.collections.List<kotlin.String> =  // kotlin.collections.List<kotlin.String> | Sorting options
val offset : kotlin.Int = 56 // kotlin.Int | Offset
val limit : kotlin.Int = 56 // kotlin.Int | Limit
val with : kotlin.String = with_example // kotlin.String | With parameters
val mode : kotlin.String = mode_example // kotlin.String | Response mode
try {
    val result : kotlin.collections.List<LdapGroup> = apiInstance.restLdapGroupsGet(name, nameColonContains, email, emailColonContains, orderBy, offset, limit, with, mode)
    println(result)
} catch (e: ClientException) {
    println("4xx response calling LdapGroupsApi#restLdapGroupsGet")
    e.printStackTrace()
} catch (e: ServerException) {
    println("5xx response calling LdapGroupsApi#restLdapGroupsGet")
    e.printStackTrace()
}
```

### Parameters

Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **name** | **kotlin.String**| LDAP group name | [optional]
 **nameColonContains** | **kotlin.String**| LDAP group name. Search for result that contains specified characters in this parameter. | [optional]
 **email** | **kotlin.String**| LDAP group Email | [optional]
 **emailColonContains** | **kotlin.String**| LDAP group Email. Search for result that contains specified characters in this parameter. | [optional]
 **orderBy** | [**kotlin.collections.List&lt;kotlin.String&gt;**](kotlin.String.md)| Sorting options | [optional]
 **offset** | **kotlin.Int**| Offset | [optional]
 **limit** | **kotlin.Int**| Limit | [optional]
 **with** | **kotlin.String**| With parameters | [optional]
 **mode** | **kotlin.String**| Response mode | [optional]

### Return type

[**kotlin.collections.List&lt;LdapGroup&gt;**](LdapGroup.md)

### Authorization

No authorization required

### HTTP request headers

 - **Content-Type**: Not defined
 - **Accept**: */*

<a id="restLdapGroupsIdDelete"></a>
# **restLdapGroupsIdDelete**
> restLdapGroupsIdDelete(id)

Deletes an LDAP group

Deletes an LDAP group

### Example
```kotlin
// Import classes:
//import org.openapitools.client.infrastructure.*
//import org.openapitools.client.models.*

val apiInstance = LdapGroupsApi()
val id : kotlin.Int = 56 // kotlin.Int | ID of the LDAP group to delete
try {
    apiInstance.restLdapGroupsIdDelete(id)
} catch (e: ClientException) {
    println("4xx response calling LdapGroupsApi#restLdapGroupsIdDelete")
    e.printStackTrace()
} catch (e: ServerException) {
    println("5xx response calling LdapGroupsApi#restLdapGroupsIdDelete")
    e.printStackTrace()
}
```

### Parameters

Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **id** | **kotlin.Int**| ID of the LDAP group to delete |

### Return type

null (empty response body)

### Authorization

No authorization required

### HTTP request headers

 - **Content-Type**: Not defined
 - **Accept**: Not defined

<a id="restLdapGroupsIdGet"></a>
# **restLdapGroupsIdGet**
> LdapGroup restLdapGroupsIdGet(id)

Gets an LDAP group

Returns the details of a specified LDAP group.                   This includes the settings from the admin.

### Example
```kotlin
// Import classes:
//import org.openapitools.client.infrastructure.*
//import org.openapitools.client.models.*

val apiInstance = LdapGroupsApi()
val id : kotlin.Int = 56 // kotlin.Int | ID of the LDAP group to be retrieved
try {
    val result : LdapGroup = apiInstance.restLdapGroupsIdGet(id)
    println(result)
} catch (e: ClientException) {
    println("4xx response calling LdapGroupsApi#restLdapGroupsIdGet")
    e.printStackTrace()
} catch (e: ServerException) {
    println("5xx response calling LdapGroupsApi#restLdapGroupsIdGet")
    e.printStackTrace()
}
```

### Parameters

Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **id** | **kotlin.Int**| ID of the LDAP group to be retrieved |

### Return type

[**LdapGroup**](LdapGroup.md)

### Authorization

No authorization required

### HTTP request headers

 - **Content-Type**: Not defined
 - **Accept**: */*

<a id="restLdapGroupsIdPut"></a>
# **restLdapGroupsIdPut**
> restLdapGroupsIdPut(id, body)

Updates an LDAP group

Updates an LDAP group

### Example
```kotlin
// Import classes:
//import org.openapitools.client.infrastructure.*
//import org.openapitools.client.models.*

val apiInstance = LdapGroupsApi()
val id : kotlin.Int = 56 // kotlin.Int | ID of the LDAP to update
val body : LdapGroupPut =  // LdapGroupPut | The LDAP group details
try {
    apiInstance.restLdapGroupsIdPut(id, body)
} catch (e: ClientException) {
    println("4xx response calling LdapGroupsApi#restLdapGroupsIdPut")
    e.printStackTrace()
} catch (e: ServerException) {
    println("5xx response calling LdapGroupsApi#restLdapGroupsIdPut")
    e.printStackTrace()
}
```

### Parameters

Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **id** | **kotlin.Int**| ID of the LDAP to update |
 **body** | [**LdapGroupPut**](LdapGroupPut.md)| The LDAP group details |

### Return type

null (empty response body)

### Authorization

No authorization required

### HTTP request headers

 - **Content-Type**: Not defined
 - **Accept**: Not defined

<a id="restLdapGroupsPost"></a>
# **restLdapGroupsPost**
> restLdapGroupsPost(body, returnEntity, mode)

Create an LDAP group

Creates an LDAP group

### Example
```kotlin
// Import classes:
//import org.openapitools.client.infrastructure.*
//import org.openapitools.client.models.*

val apiInstance = LdapGroupsApi()
val body : LdapGroupPost =  // LdapGroupPost | The LDAP group details
val returnEntity : kotlin.Boolean = true // kotlin.Boolean | Return information about newly created entity
val mode : kotlin.String = mode_example // kotlin.String | Response mode
try {
    apiInstance.restLdapGroupsPost(body, returnEntity, mode)
} catch (e: ClientException) {
    println("4xx response calling LdapGroupsApi#restLdapGroupsPost")
    e.printStackTrace()
} catch (e: ServerException) {
    println("5xx response calling LdapGroupsApi#restLdapGroupsPost")
    e.printStackTrace()
}
```

### Parameters

Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **body** | [**LdapGroupPost**](LdapGroupPost.md)| The LDAP group details |
 **returnEntity** | **kotlin.Boolean**| Return information about newly created entity | [optional]
 **mode** | **kotlin.String**| Response mode | [optional]

### Return type

null (empty response body)

### Authorization

No authorization required

### HTTP request headers

 - **Content-Type**: Not defined
 - **Accept**: Not defined

