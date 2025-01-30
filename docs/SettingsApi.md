# SettingsApi

All URIs are relative to *http://localhost*

Method | HTTP request | Description
------------- | ------------- | -------------
[**restSettingsPasswordPolicyGet**](SettingsApi.md#restSettingsPasswordPolicyGet) | **GET** /rest/settings/passwordPolicy | Get Password Policy
[**restSettingsSystemGet**](SettingsApi.md#restSettingsSystemGet) | **GET** /rest/settings/system | Get system settings


<a id="restSettingsPasswordPolicyGet"></a>
# **restSettingsPasswordPolicyGet**
> PasswordPolicy restSettingsPasswordPolicyGet()

Get Password Policy

Returns the password policy settings

### Example
```kotlin
// Import classes:
//import org.openapitools.client.infrastructure.*
//import org.openapitools.client.models.*

val apiInstance = SettingsApi()
try {
    val result : PasswordPolicy = apiInstance.restSettingsPasswordPolicyGet()
    println(result)
} catch (e: ClientException) {
    println("4xx response calling SettingsApi#restSettingsPasswordPolicyGet")
    e.printStackTrace()
} catch (e: ServerException) {
    println("5xx response calling SettingsApi#restSettingsPasswordPolicyGet")
    e.printStackTrace()
}
```

### Parameters
This endpoint does not need any parameter.

### Return type

[**PasswordPolicy**](PasswordPolicy.md)

### Authorization

No authorization required

### HTTP request headers

 - **Content-Type**: Not defined
 - **Accept**: */*

<a id="restSettingsSystemGet"></a>
# **restSettingsSystemGet**
> Settings restSettingsSystemGet()

Get system settings

Returns system settings

### Example
```kotlin
// Import classes:
//import org.openapitools.client.infrastructure.*
//import org.openapitools.client.models.*

val apiInstance = SettingsApi()
try {
    val result : Settings = apiInstance.restSettingsSystemGet()
    println(result)
} catch (e: ClientException) {
    println("4xx response calling SettingsApi#restSettingsSystemGet")
    e.printStackTrace()
} catch (e: ServerException) {
    println("5xx response calling SettingsApi#restSettingsSystemGet")
    e.printStackTrace()
}
```

### Parameters
This endpoint does not need any parameter.

### Return type

[**Settings**](Settings.md)

### Authorization

No authorization required

### HTTP request headers

 - **Content-Type**: Not defined
 - **Accept**: */*

