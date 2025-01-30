# UserSshPublicKeysApi

All URIs are relative to *http://localhost*

Method | HTTP request | Description
------------- | ------------- | -------------
[**restUserSshPublicKeysCreatePost**](UserSshPublicKeysApi.md#restUserSshPublicKeysCreatePost) | **POST** /rest/userSshPublicKeys/create | Create new SSH public key record for current login user
[**restUserSshPublicKeysGeneratePost**](UserSshPublicKeysApi.md#restUserSshPublicKeysGeneratePost) | **POST** /rest/userSshPublicKeys/generate | Generate a new ssh public/private key pair
[**restUserSshPublicKeysGet**](UserSshPublicKeysApi.md#restUserSshPublicKeysGet) | **GET** /rest/userSshPublicKeys | Get user&#39;s ssh public keys
[**restUserSshPublicKeysIdDelete**](UserSshPublicKeysApi.md#restUserSshPublicKeysIdDelete) | **DELETE** /rest/userSshPublicKeys/{id} | Delete current user&#39;s ssh public keys


<a id="restUserSshPublicKeysCreatePost"></a>
# **restUserSshPublicKeysCreatePost**
> restUserSshPublicKeysCreatePost(publicKey, name)

Create new SSH public key record for current login user

Create new SSH public key record for current login user

### Example
```kotlin
// Import classes:
//import org.openapitools.client.infrastructure.*
//import org.openapitools.client.models.*

val apiInstance = UserSshPublicKeysApi()
val publicKey : kotlin.String = publicKey_example // kotlin.String | SSH Public key
val name : kotlin.String = name_example // kotlin.String | The name of SSH Public key
try {
    apiInstance.restUserSshPublicKeysCreatePost(publicKey, name)
} catch (e: ClientException) {
    println("4xx response calling UserSshPublicKeysApi#restUserSshPublicKeysCreatePost")
    e.printStackTrace()
} catch (e: ServerException) {
    println("5xx response calling UserSshPublicKeysApi#restUserSshPublicKeysCreatePost")
    e.printStackTrace()
}
```

### Parameters

Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **publicKey** | **kotlin.String**| SSH Public key |
 **name** | **kotlin.String**| The name of SSH Public key |

### Return type

null (empty response body)

### Authorization

No authorization required

### HTTP request headers

 - **Content-Type**: Not defined
 - **Accept**: Not defined

<a id="restUserSshPublicKeysGeneratePost"></a>
# **restUserSshPublicKeysGeneratePost**
> UserGeneratedSshPublicKeyKey restUserSshPublicKeysGeneratePost(name, passphrase)

Generate a new ssh public/private key pair

Generate a new ssh public/private key pair

### Example
```kotlin
// Import classes:
//import org.openapitools.client.infrastructure.*
//import org.openapitools.client.models.*

val apiInstance = UserSshPublicKeysApi()
val name : kotlin.String = name_example // kotlin.String | The name of SSH Public key
val passphrase : kotlin.String = passphrase_example // kotlin.String | The passphrase of SSH Public key
try {
    val result : UserGeneratedSshPublicKeyKey = apiInstance.restUserSshPublicKeysGeneratePost(name, passphrase)
    println(result)
} catch (e: ClientException) {
    println("4xx response calling UserSshPublicKeysApi#restUserSshPublicKeysGeneratePost")
    e.printStackTrace()
} catch (e: ServerException) {
    println("5xx response calling UserSshPublicKeysApi#restUserSshPublicKeysGeneratePost")
    e.printStackTrace()
}
```

### Parameters

Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **name** | **kotlin.String**| The name of SSH Public key |
 **passphrase** | **kotlin.String**| The passphrase of SSH Public key | [optional]

### Return type

[**UserGeneratedSshPublicKeyKey**](UserGeneratedSshPublicKeyKey.md)

### Authorization

No authorization required

### HTTP request headers

 - **Content-Type**: Not defined
 - **Accept**: */*

<a id="restUserSshPublicKeysGet"></a>
# **restUserSshPublicKeysGet**
> UserSshPublicKeyList restUserSshPublicKeysGet()

Get user&#39;s ssh public keys

Get list of ssh public keys

### Example
```kotlin
// Import classes:
//import org.openapitools.client.infrastructure.*
//import org.openapitools.client.models.*

val apiInstance = UserSshPublicKeysApi()
try {
    val result : UserSshPublicKeyList = apiInstance.restUserSshPublicKeysGet()
    println(result)
} catch (e: ClientException) {
    println("4xx response calling UserSshPublicKeysApi#restUserSshPublicKeysGet")
    e.printStackTrace()
} catch (e: ServerException) {
    println("5xx response calling UserSshPublicKeysApi#restUserSshPublicKeysGet")
    e.printStackTrace()
}
```

### Parameters
This endpoint does not need any parameter.

### Return type

[**UserSshPublicKeyList**](UserSshPublicKeyList.md)

### Authorization

No authorization required

### HTTP request headers

 - **Content-Type**: Not defined
 - **Accept**: */*

<a id="restUserSshPublicKeysIdDelete"></a>
# **restUserSshPublicKeysIdDelete**
> restUserSshPublicKeysIdDelete(id)

Delete current user&#39;s ssh public keys

Delete current user&#39;s ssh public keys

### Example
```kotlin
// Import classes:
//import org.openapitools.client.infrastructure.*
//import org.openapitools.client.models.*

val apiInstance = UserSshPublicKeysApi()
val id : kotlin.Int = 56 // kotlin.Int | The ID of the entity
try {
    apiInstance.restUserSshPublicKeysIdDelete(id)
} catch (e: ClientException) {
    println("4xx response calling UserSshPublicKeysApi#restUserSshPublicKeysIdDelete")
    e.printStackTrace()
} catch (e: ServerException) {
    println("5xx response calling UserSshPublicKeysApi#restUserSshPublicKeysIdDelete")
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

