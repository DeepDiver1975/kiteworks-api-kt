# UsersApi

All URIs are relative to *http://localhost*

Method | HTTP request | Description
------------- | ------------- | -------------
[**restAdminUsersActionsImportPost**](UsersApi.md#restAdminUsersActionsImportPost) | **POST** /rest/admin/users/actions/import | imports users endpoint
[**restUsersActionsGetDistributionListGet**](UsersApi.md#restUsersActionsGetDistributionListGet) | **GET** /rest/users/actions/getDistributionList | Return user which is LDAP distribution list
[**restUsersActionsLoginPost**](UsersApi.md#restUsersActionsLoginPost) | **POST** /rest/users/actions/login | User login
[**restUsersAliveTokenPut**](UsersApi.md#restUsersAliveTokenPut) | **PUT** /rest/users/aliveToken | Updates token state
[**restUsersDelete**](UsersApi.md#restUsersDelete) | **DELETE** /rest/users | Deletes Users
[**restUsersGet**](UsersApi.md#restUsersGet) | **GET** /rest/users | Get a list of Users
[**restUsersIdAdminRolesGet**](UsersApi.md#restUsersIdAdminRolesGet) | **GET** /rest/users/{id}/adminRoles | Return admin roles of the specified user id.
[**restUsersIdDelete**](UsersApi.md#restUsersIdDelete) | **DELETE** /rest/users/{id} | Deletes a User
[**restUsersIdGet**](UsersApi.md#restUsersIdGet) | **GET** /rest/users/{id} | Get User
[**restUsersIdProfileImageDelete**](UsersApi.md#restUsersIdProfileImageDelete) | **DELETE** /rest/users/{id}/profileImage | Deletes a profile image
[**restUsersIdProfileImagePost**](UsersApi.md#restUsersIdProfileImagePost) | **POST** /rest/users/{id}/profileImage | Uploads a profile image
[**restUsersIdSettingsGet**](UsersApi.md#restUsersIdSettingsGet) | **GET** /rest/users/{id}/settings | Get User Settings
[**restUsersIdSettingsPut**](UsersApi.md#restUsersIdSettingsPut) | **PUT** /rest/users/{id}/settings | Update User Settings
[**restUsersLdapSearchGet**](UsersApi.md#restUsersLdapSearchGet) | **GET** /rest/users/ldapSearch | Find users in LDAP by input supplied
[**restUsersMeForcedPasswordChangePost**](UsersApi.md#restUsersMeForcedPasswordChangePost) | **POST** /rest/users/me/forcedPasswordChange | Change the password for current user after expired
[**restUsersMeGet**](UsersApi.md#restUsersMeGet) | **GET** /rest/users/me | Get current logged in User
[**restUsersMeMobileNumberPut**](UsersApi.md#restUsersMeMobileNumberPut) | **PUT** /rest/users/me/mobileNumber | Update mobile number of the current user
[**restUsersMePinsDelete**](UsersApi.md#restUsersMePinsDelete) | **DELETE** /rest/users/me/pins | Delete user pin
[**restUsersMePinsPost**](UsersApi.md#restUsersMePinsPost) | **POST** /rest/users/me/pins | Add item to user pin
[**restUsersMePut**](UsersApi.md#restUsersMePut) | **PUT** /rest/users/me | Update current user
[**restUsersMeQuotaGet**](UsersApi.md#restUsersMeQuotaGet) | **GET** /rest/users/me/quota | Return user&#39;s quota
[**restUsersMeRecentGet**](UsersApi.md#restUsersMeRecentGet) | **GET** /rest/users/me/recent | Return user&#39;s recent items
[**restUsersMeRecentIdDelete**](UsersApi.md#restUsersMeRecentIdDelete) | **DELETE** /rest/users/me/recent/{id} | Delete user&#39;s recent item
[**restUsersMeRecentPost**](UsersApi.md#restUsersMeRecentPost) | **POST** /rest/users/me/recent | Adding objects to user&#39;s recent items
[**restUsersMeTfaAuthPost**](UsersApi.md#restUsersMeTfaAuthPost) | **POST** /rest/users/me/tfa/auth | Two Factor Authentication
[**restUsersMeTfaChallengePost**](UsersApi.md#restUsersMeTfaChallengePost) | **POST** /rest/users/me/tfa/challenge | Two Factor Authentication
[**restUsersMeTfaConfigGet**](UsersApi.md#restUsersMeTfaConfigGet) | **GET** /rest/users/me/tfa/config | Two Factor Authentication
[**restUsersMeTfaResetTotpSecretPost**](UsersApi.md#restUsersMeTfaResetTotpSecretPost) | **POST** /rest/users/me/tfa/resetTotpSecret | Reset secret key for time-based OTP of the current user
[**restUsersMeTfaSetupPut**](UsersApi.md#restUsersMeTfaSetupPut) | **PUT** /rest/users/me/tfaSetup | Setup 2FA settings
[**restUsersMeTfaSetupTotpSecretGet**](UsersApi.md#restUsersMeTfaSetupTotpSecretGet) | **GET** /rest/users/me/tfa/setupTotpSecret | Setup secret key for Time-based OTP of the current user
[**restUsersMeTfaVerifyTotpSecretPost**](UsersApi.md#restUsersMeTfaVerifyTotpSecretPost) | **POST** /rest/users/me/tfa/verifyTotpSecret | Verify code for finalising secret key for timed-based OTP
[**restUsersMeTosGet**](UsersApi.md#restUsersMeTosGet) | **GET** /rest/users/me/tos | Terms of Service
[**restUsersMeTosPost**](UsersApi.md#restUsersMeTosPost) | **POST** /rest/users/me/tos | Terms of Service
[**restUsersPost**](UsersApi.md#restUsersPost) | **POST** /rest/users | Create a User
[**restUsersPreauthPost**](UsersApi.md#restUsersPreauthPost) | **POST** /rest/users/preauth | User login preauth
[**restUsersRegisterPost**](UsersApi.md#restUsersRegisterPost) | **POST** /rest/users/register | Register a User
[**restUsersRequestPasswordResetPost**](UsersApi.md#restUsersRequestPasswordResetPost) | **POST** /rest/users/requestPasswordReset | Request for password reset
[**restUsersResetPasswordPost**](UsersApi.md#restUsersResetPasswordPost) | **POST** /rest/users/resetPassword | Reset password


<a id="restAdminUsersActionsImportPost"></a>
# **restAdminUsersActionsImportPost**
> AdminUserImport restAdminUsersActionsImportPost(content, updateIfExists, sendNotification, partialSuccess)

imports users endpoint

bulk imports users and optionally update existing users

### Example
```kotlin
// Import classes:
//import org.openapitools.client.infrastructure.*
//import org.openapitools.client.models.*

val apiInstance = UsersApi()
val content : io.ktor.client.request.forms.InputProvider = BINARY_DATA_HERE // io.ktor.client.request.forms.InputProvider | The file containing the users to be imported.
val updateIfExists : kotlin.Boolean = true // kotlin.Boolean | If user exists, update user's settings
val sendNotification : kotlin.Boolean = true // kotlin.Boolean | If true, a notification email will be sent to each newly created users
val partialSuccess : kotlin.Boolean = true // kotlin.Boolean | If true, partial processing will be performed, i.e., only validated users are imported, while others are rejected
try {
    val result : AdminUserImport = apiInstance.restAdminUsersActionsImportPost(content, updateIfExists, sendNotification, partialSuccess)
    println(result)
} catch (e: ClientException) {
    println("4xx response calling UsersApi#restAdminUsersActionsImportPost")
    e.printStackTrace()
} catch (e: ServerException) {
    println("5xx response calling UsersApi#restAdminUsersActionsImportPost")
    e.printStackTrace()
}
```

### Parameters

Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **content** | **io.ktor.client.request.forms.InputProvider**| The file containing the users to be imported. |
 **updateIfExists** | **kotlin.Boolean**| If user exists, update user&#39;s settings | [optional]
 **sendNotification** | **kotlin.Boolean**| If true, a notification email will be sent to each newly created users | [optional]
 **partialSuccess** | **kotlin.Boolean**| If true, partial processing will be performed, i.e., only validated users are imported, while others are rejected | [optional]

### Return type

[**AdminUserImport**](AdminUserImport.md)

### Authorization

No authorization required

### HTTP request headers

 - **Content-Type**: multipart/form-data
 - **Accept**: */*

<a id="restUsersActionsGetDistributionListGet"></a>
# **restUsersActionsGetDistributionListGet**
> UserDistributionList restUsersActionsGetDistributionListGet(emailColonIn)

Return user which is LDAP distribution list

Return user which is LDAP distribution list

### Example
```kotlin
// Import classes:
//import org.openapitools.client.infrastructure.*
//import org.openapitools.client.models.*

val apiInstance = UsersApi()
val emailColonIn : kotlin.collections.List<kotlin.String> =  // kotlin.collections.List<kotlin.String> | 
try {
    val result : UserDistributionList = apiInstance.restUsersActionsGetDistributionListGet(emailColonIn)
    println(result)
} catch (e: ClientException) {
    println("4xx response calling UsersApi#restUsersActionsGetDistributionListGet")
    e.printStackTrace()
} catch (e: ServerException) {
    println("5xx response calling UsersApi#restUsersActionsGetDistributionListGet")
    e.printStackTrace()
}
```

### Parameters

Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **emailColonIn** | [**kotlin.collections.List&lt;kotlin.String&gt;**](kotlin.String.md)|  |

### Return type

[**UserDistributionList**](UserDistributionList.md)

### Authorization

No authorization required

### HTTP request headers

 - **Content-Type**: Not defined
 - **Accept**: */*

<a id="restUsersActionsLoginPost"></a>
# **restUsersActionsLoginPost**
> restUsersActionsLoginPost(body)

User login

User login.

### Example
```kotlin
// Import classes:
//import org.openapitools.client.infrastructure.*
//import org.openapitools.client.models.*

val apiInstance = UsersApi()
val body : UserLoginPost =  // UserLoginPost | User Login
try {
    apiInstance.restUsersActionsLoginPost(body)
} catch (e: ClientException) {
    println("4xx response calling UsersApi#restUsersActionsLoginPost")
    e.printStackTrace()
} catch (e: ServerException) {
    println("5xx response calling UsersApi#restUsersActionsLoginPost")
    e.printStackTrace()
}
```

### Parameters

Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **body** | [**UserLoginPost**](UserLoginPost.md)| User Login |

### Return type

null (empty response body)

### Authorization

No authorization required

### HTTP request headers

 - **Content-Type**: Not defined
 - **Accept**: Not defined

<a id="restUsersAliveTokenPut"></a>
# **restUsersAliveTokenPut**
> restUsersAliveTokenPut()

Updates token state

Updates current session state to be not outdated any more

### Example
```kotlin
// Import classes:
//import org.openapitools.client.infrastructure.*
//import org.openapitools.client.models.*

val apiInstance = UsersApi()
try {
    apiInstance.restUsersAliveTokenPut()
} catch (e: ClientException) {
    println("4xx response calling UsersApi#restUsersAliveTokenPut")
    e.printStackTrace()
} catch (e: ServerException) {
    println("5xx response calling UsersApi#restUsersAliveTokenPut")
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

<a id="restUsersDelete"></a>
# **restUsersDelete**
> restUsersDelete(idColonIn, retainToUser, remoteWipe, deleteUnsharedData, retainData, retainPermissionToSharedData, withdrawFileLinks, withdrawRequestFiles, partialSuccess, mode)

Deletes Users

Mark the specified users as deleted. The size of request User UUID is limited (recommend &lt;&#x3D; 100)

### Example
```kotlin
// Import classes:
//import org.openapitools.client.infrastructure.*
//import org.openapitools.client.models.*

val apiInstance = UsersApi()
val idColonIn : kotlin.String = idColonIn_example // kotlin.String | List of the users id which will be deleted
val retainToUser : kotlin.String = retainToUser_example // kotlin.String | New owner id to re-assign data to (required if retainData or retainPermissionToSharedData is True)
val remoteWipe : kotlin.Boolean = true // kotlin.Boolean | Remote wipe data on desktop and mobile devices
val deleteUnsharedData : kotlin.Boolean = true // kotlin.Boolean | Delete all data owned by the user (required and must be True if retainData is False and vice versa)
val retainData : kotlin.Boolean = true // kotlin.Boolean | Retain users data (required and must be True if deleteUnsharedData is False and vice versa)
val retainPermissionToSharedData : kotlin.Boolean = true // kotlin.Boolean | Retain permissions to shared data
val withdrawFileLinks : kotlin.Boolean = true // kotlin.Boolean | Delete attached files in emails sent by deleted/demoted users
val withdrawRequestFiles : kotlin.Boolean = true // kotlin.Boolean | Delete request files emails sent by deleted/demoted users
val partialSuccess : kotlin.Boolean = true // kotlin.Boolean | Whether to perform action on valid items even if some ones fail
val mode : kotlin.String = mode_example // kotlin.String | Response mode
try {
    apiInstance.restUsersDelete(idColonIn, retainToUser, remoteWipe, deleteUnsharedData, retainData, retainPermissionToSharedData, withdrawFileLinks, withdrawRequestFiles, partialSuccess, mode)
} catch (e: ClientException) {
    println("4xx response calling UsersApi#restUsersDelete")
    e.printStackTrace()
} catch (e: ServerException) {
    println("5xx response calling UsersApi#restUsersDelete")
    e.printStackTrace()
}
```

### Parameters

Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **idColonIn** | **kotlin.String**| List of the users id which will be deleted |
 **retainToUser** | **kotlin.String**| New owner id to re-assign data to (required if retainData or retainPermissionToSharedData is True) | [optional]
 **remoteWipe** | **kotlin.Boolean**| Remote wipe data on desktop and mobile devices | [optional]
 **deleteUnsharedData** | **kotlin.Boolean**| Delete all data owned by the user (required and must be True if retainData is False and vice versa) | [optional]
 **retainData** | **kotlin.Boolean**| Retain users data (required and must be True if deleteUnsharedData is False and vice versa) | [optional]
 **retainPermissionToSharedData** | **kotlin.Boolean**| Retain permissions to shared data | [optional]
 **withdrawFileLinks** | **kotlin.Boolean**| Delete attached files in emails sent by deleted/demoted users | [optional]
 **withdrawRequestFiles** | **kotlin.Boolean**| Delete request files emails sent by deleted/demoted users | [optional]
 **partialSuccess** | **kotlin.Boolean**| Whether to perform action on valid items even if some ones fail | [optional]
 **mode** | **kotlin.String**| Response mode | [optional]

### Return type

null (empty response body)

### Authorization

No authorization required

### HTTP request headers

 - **Content-Type**: Not defined
 - **Accept**: Not defined

<a id="restUsersGet"></a>
# **restUsersGet**
> kotlin.collections.List&lt;User&gt; restUsersGet(email, emailColonContains, name, nameColonContains, metadata, metadataContains, deleted, active, verified, suspended, isRecipient, allowsCollaboration, created, createdColonGt, createdColonGte, createdColonLt, createdColonLte, orderBy, offset, limit, locateId, with, mode)

Get a list of Users

Returns a list of Users in the system.                   This call will only work for users with admin access.

### Example
```kotlin
// Import classes:
//import org.openapitools.client.infrastructure.*
//import org.openapitools.client.models.*

val apiInstance = UsersApi()
val email : kotlin.String = email_example // kotlin.String | The user's email
val emailColonContains : kotlin.String = emailColonContains_example // kotlin.String | The user's email. Search for result that contains specified characters in this parameter.
val name : kotlin.String = name_example // kotlin.String | The name of the user
val nameColonContains : kotlin.String = nameColonContains_example // kotlin.String | The name of the user. Search for result that contains specified characters in this parameter.
val metadata : kotlin.String = metadata_example // kotlin.String | The metadata of the user
val metadataContains : kotlin.String = metadataContains_example // kotlin.String | The metadata of the user. Search for result that contains specified characters in this parameter.
val deleted : kotlin.Boolean = true // kotlin.Boolean | Whether the user has been deleted
val active : kotlin.Boolean = true // kotlin.Boolean | Whether the user is an actual kitework user
val verified : kotlin.Boolean = true // kotlin.Boolean | Whether the user is verified
val suspended : kotlin.Boolean = true // kotlin.Boolean | Whether the user is suspended
val isRecipient : kotlin.Boolean = true // kotlin.Boolean | Whether user is recipient
val allowsCollaboration : kotlin.Boolean = true // kotlin.Boolean | Whether user's profile allows collaboration access
val created : java.time.LocalDate = 2013-10-20 // java.time.LocalDate | User creation date
val createdColonGt : java.time.LocalDate = 2013-10-20 // java.time.LocalDate | User creation date. Search for result that has this parameter value greater than specified.
val createdColonGte : java.time.LocalDate = 2013-10-20 // java.time.LocalDate | User creation date. Search for result that has this parameter value greater or equal to the specified.
val createdColonLt : java.time.LocalDate = 2013-10-20 // java.time.LocalDate | User creation date. Search for result that has this parameter value less than specified.
val createdColonLte : java.time.LocalDate = 2013-10-20 // java.time.LocalDate | User creation date. Search for result that has this parameter value less or equal to the specified.
val orderBy : kotlin.collections.List<kotlin.String> =  // kotlin.collections.List<kotlin.String> | Sorting options
val offset : kotlin.Int = 56 // kotlin.Int | Offset
val limit : kotlin.Int = 56 // kotlin.Int | Limit
val locateId : kotlin.Int = 56 // kotlin.Int | If specified, \"offset\" parameter will be ignored                                             and the page containing entity with this Id will be returned.
val with : kotlin.String = with_example // kotlin.String | With parameters
val mode : kotlin.String = mode_example // kotlin.String | Response mode
try {
    val result : kotlin.collections.List<User> = apiInstance.restUsersGet(email, emailColonContains, name, nameColonContains, metadata, metadataContains, deleted, active, verified, suspended, isRecipient, allowsCollaboration, created, createdColonGt, createdColonGte, createdColonLt, createdColonLte, orderBy, offset, limit, locateId, with, mode)
    println(result)
} catch (e: ClientException) {
    println("4xx response calling UsersApi#restUsersGet")
    e.printStackTrace()
} catch (e: ServerException) {
    println("5xx response calling UsersApi#restUsersGet")
    e.printStackTrace()
}
```

### Parameters

Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **email** | **kotlin.String**| The user&#39;s email | [optional]
 **emailColonContains** | **kotlin.String**| The user&#39;s email. Search for result that contains specified characters in this parameter. | [optional]
 **name** | **kotlin.String**| The name of the user | [optional]
 **nameColonContains** | **kotlin.String**| The name of the user. Search for result that contains specified characters in this parameter. | [optional]
 **metadata** | **kotlin.String**| The metadata of the user | [optional]
 **metadataContains** | **kotlin.String**| The metadata of the user. Search for result that contains specified characters in this parameter. | [optional]
 **deleted** | **kotlin.Boolean**| Whether the user has been deleted | [optional]
 **active** | **kotlin.Boolean**| Whether the user is an actual kitework user | [optional]
 **verified** | **kotlin.Boolean**| Whether the user is verified | [optional]
 **suspended** | **kotlin.Boolean**| Whether the user is suspended | [optional]
 **isRecipient** | **kotlin.Boolean**| Whether user is recipient | [optional]
 **allowsCollaboration** | **kotlin.Boolean**| Whether user&#39;s profile allows collaboration access | [optional]
 **created** | **java.time.LocalDate**| User creation date | [optional]
 **createdColonGt** | **java.time.LocalDate**| User creation date. Search for result that has this parameter value greater than specified. | [optional]
 **createdColonGte** | **java.time.LocalDate**| User creation date. Search for result that has this parameter value greater or equal to the specified. | [optional]
 **createdColonLt** | **java.time.LocalDate**| User creation date. Search for result that has this parameter value less than specified. | [optional]
 **createdColonLte** | **java.time.LocalDate**| User creation date. Search for result that has this parameter value less or equal to the specified. | [optional]
 **orderBy** | [**kotlin.collections.List&lt;kotlin.String&gt;**](kotlin.String.md)| Sorting options | [optional]
 **offset** | **kotlin.Int**| Offset | [optional]
 **limit** | **kotlin.Int**| Limit | [optional]
 **locateId** | **kotlin.Int**| If specified, \&quot;offset\&quot; parameter will be ignored                                             and the page containing entity with this Id will be returned. | [optional]
 **with** | **kotlin.String**| With parameters | [optional]
 **mode** | **kotlin.String**| Response mode | [optional]

### Return type

[**kotlin.collections.List&lt;User&gt;**](User.md)

### Authorization

No authorization required

### HTTP request headers

 - **Content-Type**: Not defined
 - **Accept**: */*

<a id="restUsersIdAdminRolesGet"></a>
# **restUsersIdAdminRolesGet**
> kotlin.collections.List&lt;AdminRole&gt; restUsersIdAdminRolesGet(id, orderBy, with, mode)

Return admin roles of the specified user id.

Returns the details of all adminroles                   (active and deleted users) with the specified user id.

### Example
```kotlin
// Import classes:
//import org.openapitools.client.infrastructure.*
//import org.openapitools.client.models.*

val apiInstance = UsersApi()
val id : kotlin.String = id_example // kotlin.String | ID of the user to retrieve admin role
val orderBy : kotlin.collections.List<kotlin.String> =  // kotlin.collections.List<kotlin.String> | Sorting options
val with : kotlin.String = with_example // kotlin.String | With parameters
val mode : kotlin.String = mode_example // kotlin.String | Response mode
try {
    val result : kotlin.collections.List<AdminRole> = apiInstance.restUsersIdAdminRolesGet(id, orderBy, with, mode)
    println(result)
} catch (e: ClientException) {
    println("4xx response calling UsersApi#restUsersIdAdminRolesGet")
    e.printStackTrace()
} catch (e: ServerException) {
    println("5xx response calling UsersApi#restUsersIdAdminRolesGet")
    e.printStackTrace()
}
```

### Parameters

Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **id** | **kotlin.String**| ID of the user to retrieve admin role |
 **orderBy** | [**kotlin.collections.List&lt;kotlin.String&gt;**](kotlin.String.md)| Sorting options | [optional]
 **with** | **kotlin.String**| With parameters | [optional]
 **mode** | **kotlin.String**| Response mode | [optional]

### Return type

[**kotlin.collections.List&lt;AdminRole&gt;**](AdminRole.md)

### Authorization

No authorization required

### HTTP request headers

 - **Content-Type**: Not defined
 - **Accept**: */*

<a id="restUsersIdDelete"></a>
# **restUsersIdDelete**
> restUsersIdDelete(id, retainToUser, remoteWipe, deleteUnsharedData, retainData, retainPermissionToSharedData, withdrawFileLinks, withdrawRequestFiles, partialSuccess, mode)

Deletes a User

Mark the specified user as deleted. This user will still be returned in the GET Users query.

### Example
```kotlin
// Import classes:
//import org.openapitools.client.infrastructure.*
//import org.openapitools.client.models.*

val apiInstance = UsersApi()
val id : kotlin.String = id_example // kotlin.String | ID of the user to delete
val retainToUser : kotlin.String = retainToUser_example // kotlin.String | New owner id to re-assign data to (required if retainData or retainPermissionToSharedData is True)
val remoteWipe : kotlin.Boolean = true // kotlin.Boolean | Remote wipe data on desktop and mobile devices
val deleteUnsharedData : kotlin.Boolean = true // kotlin.Boolean | Delete all data owned by the user (required and must be True if retainData is False and vice versa)
val retainData : kotlin.Boolean = true // kotlin.Boolean | Retain users data (required and must be True if deleteUnsharedData is False and vice versa)
val retainPermissionToSharedData : kotlin.Boolean = true // kotlin.Boolean | Retain permissions to shared data
val withdrawFileLinks : kotlin.Boolean = true // kotlin.Boolean | Delete attached files in emails sent by deleted/demoted users
val withdrawRequestFiles : kotlin.Boolean = true // kotlin.Boolean | Delete request files emails sent by deleted/demoted users
val partialSuccess : kotlin.Boolean = true // kotlin.Boolean | Whether to perform action on valid items even if some ones fail
val mode : kotlin.String = mode_example // kotlin.String | Response mode
try {
    apiInstance.restUsersIdDelete(id, retainToUser, remoteWipe, deleteUnsharedData, retainData, retainPermissionToSharedData, withdrawFileLinks, withdrawRequestFiles, partialSuccess, mode)
} catch (e: ClientException) {
    println("4xx response calling UsersApi#restUsersIdDelete")
    e.printStackTrace()
} catch (e: ServerException) {
    println("5xx response calling UsersApi#restUsersIdDelete")
    e.printStackTrace()
}
```

### Parameters

Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **id** | **kotlin.String**| ID of the user to delete |
 **retainToUser** | **kotlin.String**| New owner id to re-assign data to (required if retainData or retainPermissionToSharedData is True) | [optional]
 **remoteWipe** | **kotlin.Boolean**| Remote wipe data on desktop and mobile devices | [optional]
 **deleteUnsharedData** | **kotlin.Boolean**| Delete all data owned by the user (required and must be True if retainData is False and vice versa) | [optional]
 **retainData** | **kotlin.Boolean**| Retain users data (required and must be True if deleteUnsharedData is False and vice versa) | [optional]
 **retainPermissionToSharedData** | **kotlin.Boolean**| Retain permissions to shared data | [optional]
 **withdrawFileLinks** | **kotlin.Boolean**| Delete attached files in emails sent by deleted/demoted users | [optional]
 **withdrawRequestFiles** | **kotlin.Boolean**| Delete request files emails sent by deleted/demoted users | [optional]
 **partialSuccess** | **kotlin.Boolean**| Whether to perform action on valid items even if some ones fail | [optional]
 **mode** | **kotlin.String**| Response mode | [optional]

### Return type

null (empty response body)

### Authorization

No authorization required

### HTTP request headers

 - **Content-Type**: Not defined
 - **Accept**: Not defined

<a id="restUsersIdGet"></a>
# **restUsersIdGet**
> User restUsersIdGet(id)

Get User

Returns the details of the specified user (this includes email address and name)

### Example
```kotlin
// Import classes:
//import org.openapitools.client.infrastructure.*
//import org.openapitools.client.models.*

val apiInstance = UsersApi()
val id : kotlin.String = id_example // kotlin.String | ID of the user to retrieve
try {
    val result : User = apiInstance.restUsersIdGet(id)
    println(result)
} catch (e: ClientException) {
    println("4xx response calling UsersApi#restUsersIdGet")
    e.printStackTrace()
} catch (e: ServerException) {
    println("5xx response calling UsersApi#restUsersIdGet")
    e.printStackTrace()
}
```

### Parameters

Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **id** | **kotlin.String**| ID of the user to retrieve |

### Return type

[**User**](User.md)

### Authorization

No authorization required

### HTTP request headers

 - **Content-Type**: Not defined
 - **Accept**: */*

<a id="restUsersIdProfileImageDelete"></a>
# **restUsersIdProfileImageDelete**
> restUsersIdProfileImageDelete(id)

Deletes a profile image

Deletes an image file to use as profile image

### Example
```kotlin
// Import classes:
//import org.openapitools.client.infrastructure.*
//import org.openapitools.client.models.*

val apiInstance = UsersApi()
val id : kotlin.String = id_example // kotlin.String | user id
try {
    apiInstance.restUsersIdProfileImageDelete(id)
} catch (e: ClientException) {
    println("4xx response calling UsersApi#restUsersIdProfileImageDelete")
    e.printStackTrace()
} catch (e: ServerException) {
    println("5xx response calling UsersApi#restUsersIdProfileImageDelete")
    e.printStackTrace()
}
```

### Parameters

Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **id** | **kotlin.String**| user id |

### Return type

null (empty response body)

### Authorization

No authorization required

### HTTP request headers

 - **Content-Type**: Not defined
 - **Accept**: Not defined

<a id="restUsersIdProfileImagePost"></a>
# **restUsersIdProfileImagePost**
> restUsersIdProfileImagePost(id, body)

Uploads a profile image

Uploads an image file to use as profile image

### Example
```kotlin
// Import classes:
//import org.openapitools.client.infrastructure.*
//import org.openapitools.client.models.*

val apiInstance = UsersApi()
val id : kotlin.String = id_example // kotlin.String | user id
val body : io.ktor.client.request.forms.InputProvider = BINARY_DATA_HERE // io.ktor.client.request.forms.InputProvider | file content
try {
    apiInstance.restUsersIdProfileImagePost(id, body)
} catch (e: ClientException) {
    println("4xx response calling UsersApi#restUsersIdProfileImagePost")
    e.printStackTrace()
} catch (e: ServerException) {
    println("5xx response calling UsersApi#restUsersIdProfileImagePost")
    e.printStackTrace()
}
```

### Parameters

Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **id** | **kotlin.String**| user id |
 **body** | **io.ktor.client.request.forms.InputProvider**| file content |

### Return type

null (empty response body)

### Authorization

No authorization required

### HTTP request headers

 - **Content-Type**: multipart/form-data
 - **Accept**: Not defined

<a id="restUsersIdSettingsGet"></a>
# **restUsersIdSettingsGet**
> Settings restUsersIdSettingsGet(id)

Get User Settings

Returns the user settings

### Example
```kotlin
// Import classes:
//import org.openapitools.client.infrastructure.*
//import org.openapitools.client.models.*

val apiInstance = UsersApi()
val id : kotlin.String = id_example // kotlin.String | ID of the user to retrieve settings for
try {
    val result : Settings = apiInstance.restUsersIdSettingsGet(id)
    println(result)
} catch (e: ClientException) {
    println("4xx response calling UsersApi#restUsersIdSettingsGet")
    e.printStackTrace()
} catch (e: ServerException) {
    println("5xx response calling UsersApi#restUsersIdSettingsGet")
    e.printStackTrace()
}
```

### Parameters

Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **id** | **kotlin.String**| ID of the user to retrieve settings for |

### Return type

[**Settings**](Settings.md)

### Authorization

No authorization required

### HTTP request headers

 - **Content-Type**: Not defined
 - **Accept**: */*

<a id="restUsersIdSettingsPut"></a>
# **restUsersIdSettingsPut**
> restUsersIdSettingsPut(id, body)

Update User Settings

Updates the settings for the specified user

### Example
```kotlin
// Import classes:
//import org.openapitools.client.infrastructure.*
//import org.openapitools.client.models.*

val apiInstance = UsersApi()
val id : kotlin.String = id_example // kotlin.String | ID of the user to update settings for
val body : SettingsPut =  // SettingsPut | The Settings details
try {
    apiInstance.restUsersIdSettingsPut(id, body)
} catch (e: ClientException) {
    println("4xx response calling UsersApi#restUsersIdSettingsPut")
    e.printStackTrace()
} catch (e: ServerException) {
    println("5xx response calling UsersApi#restUsersIdSettingsPut")
    e.printStackTrace()
}
```

### Parameters

Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **id** | **kotlin.String**| ID of the user to update settings for |
 **body** | [**SettingsPut**](SettingsPut.md)| The Settings details |

### Return type

null (empty response body)

### Authorization

No authorization required

### HTTP request headers

 - **Content-Type**: Not defined
 - **Accept**: Not defined

<a id="restUsersLdapSearchGet"></a>
# **restUsersLdapSearchGet**
> LdapSearchResults restUsersLdapSearchGet(`value`, with, mode)

Find users in LDAP by input supplied

Returns a list of Users in LDAP by the input supplied.

### Example
```kotlin
// Import classes:
//import org.openapitools.client.infrastructure.*
//import org.openapitools.client.models.*

val apiInstance = UsersApi()
val `value` : kotlin.String = `value`_example // kotlin.String | The user's email or name
val with : kotlin.String = with_example // kotlin.String | With parameters
val mode : kotlin.String = mode_example // kotlin.String | Response mode
try {
    val result : LdapSearchResults = apiInstance.restUsersLdapSearchGet(`value`, with, mode)
    println(result)
} catch (e: ClientException) {
    println("4xx response calling UsersApi#restUsersLdapSearchGet")
    e.printStackTrace()
} catch (e: ServerException) {
    println("5xx response calling UsersApi#restUsersLdapSearchGet")
    e.printStackTrace()
}
```

### Parameters

Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **&#x60;value&#x60;** | **kotlin.String**| The user&#39;s email or name |
 **with** | **kotlin.String**| With parameters | [optional]
 **mode** | **kotlin.String**| Response mode | [optional]

### Return type

[**LdapSearchResults**](LdapSearchResults.md)

### Authorization

No authorization required

### HTTP request headers

 - **Content-Type**: Not defined
 - **Accept**: */*

<a id="restUsersMeForcedPasswordChangePost"></a>
# **restUsersMeForcedPasswordChangePost**
> restUsersMeForcedPasswordChangePost(body)

Change the password for current user after expired

Change the password for current user after password expired

### Example
```kotlin
// Import classes:
//import org.openapitools.client.infrastructure.*
//import org.openapitools.client.models.*

val apiInstance = UsersApi()
val body : UserForcedPasswordChangePut =  // UserForcedPasswordChangePut | Password and previous password
try {
    apiInstance.restUsersMeForcedPasswordChangePost(body)
} catch (e: ClientException) {
    println("4xx response calling UsersApi#restUsersMeForcedPasswordChangePost")
    e.printStackTrace()
} catch (e: ServerException) {
    println("5xx response calling UsersApi#restUsersMeForcedPasswordChangePost")
    e.printStackTrace()
}
```

### Parameters

Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **body** | [**UserForcedPasswordChangePut**](UserForcedPasswordChangePut.md)| Password and previous password |

### Return type

null (empty response body)

### Authorization

No authorization required

### HTTP request headers

 - **Content-Type**: Not defined
 - **Accept**: Not defined

<a id="restUsersMeGet"></a>
# **restUsersMeGet**
> UserMe restUsersMeGet()

Get current logged in User

Returns the details of the current user (this includes email address and name)

### Example
```kotlin
// Import classes:
//import org.openapitools.client.infrastructure.*
//import org.openapitools.client.models.*

val apiInstance = UsersApi()
try {
    val result : UserMe = apiInstance.restUsersMeGet()
    println(result)
} catch (e: ClientException) {
    println("4xx response calling UsersApi#restUsersMeGet")
    e.printStackTrace()
} catch (e: ServerException) {
    println("5xx response calling UsersApi#restUsersMeGet")
    e.printStackTrace()
}
```

### Parameters
This endpoint does not need any parameter.

### Return type

[**UserMe**](UserMe.md)

### Authorization

No authorization required

### HTTP request headers

 - **Content-Type**: Not defined
 - **Accept**: */*

<a id="restUsersMeMobileNumberPut"></a>
# **restUsersMeMobileNumberPut**
> restUsersMeMobileNumberPut(body)

Update mobile number of the current user

Update mobile number of the current user

### Example
```kotlin
// Import classes:
//import org.openapitools.client.infrastructure.*
//import org.openapitools.client.models.*

val apiInstance = UsersApi()
val body : UserMobileNumberPasswordPut =  // UserMobileNumberPasswordPut | The user's mobile number update details
try {
    apiInstance.restUsersMeMobileNumberPut(body)
} catch (e: ClientException) {
    println("4xx response calling UsersApi#restUsersMeMobileNumberPut")
    e.printStackTrace()
} catch (e: ServerException) {
    println("5xx response calling UsersApi#restUsersMeMobileNumberPut")
    e.printStackTrace()
}
```

### Parameters

Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **body** | [**UserMobileNumberPasswordPut**](UserMobileNumberPasswordPut.md)| The user&#39;s mobile number update details |

### Return type

null (empty response body)

### Authorization

No authorization required

### HTTP request headers

 - **Content-Type**: Not defined
 - **Accept**: Not defined

<a id="restUsersMePinsDelete"></a>
# **restUsersMePinsDelete**
> restUsersMePinsDelete(body)

Delete user pin

Delete user pin

### Example
```kotlin
// Import classes:
//import org.openapitools.client.infrastructure.*
//import org.openapitools.client.models.*

val apiInstance = UsersApi()
val body : UserMePinsPostRequest =  // UserMePinsPostRequest | 
try {
    apiInstance.restUsersMePinsDelete(body)
} catch (e: ClientException) {
    println("4xx response calling UsersApi#restUsersMePinsDelete")
    e.printStackTrace()
} catch (e: ServerException) {
    println("5xx response calling UsersApi#restUsersMePinsDelete")
    e.printStackTrace()
}
```

### Parameters

Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **body** | [**UserMePinsPostRequest**](UserMePinsPostRequest.md)|  |

### Return type

null (empty response body)

### Authorization

No authorization required

### HTTP request headers

 - **Content-Type**: Not defined
 - **Accept**: Not defined

<a id="restUsersMePinsPost"></a>
# **restUsersMePinsPost**
> restUsersMePinsPost(body)

Add item to user pin

Add item to user pin

### Example
```kotlin
// Import classes:
//import org.openapitools.client.infrastructure.*
//import org.openapitools.client.models.*

val apiInstance = UsersApi()
val body : UserMePinsPostRequest =  // UserMePinsPostRequest | 
try {
    apiInstance.restUsersMePinsPost(body)
} catch (e: ClientException) {
    println("4xx response calling UsersApi#restUsersMePinsPost")
    e.printStackTrace()
} catch (e: ServerException) {
    println("5xx response calling UsersApi#restUsersMePinsPost")
    e.printStackTrace()
}
```

### Parameters

Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **body** | [**UserMePinsPostRequest**](UserMePinsPostRequest.md)|  |

### Return type

null (empty response body)

### Authorization

No authorization required

### HTTP request headers

 - **Content-Type**: Not defined
 - **Accept**: Not defined

<a id="restUsersMePut"></a>
# **restUsersMePut**
> restUsersMePut(body)

Update current user

Updates the details of current user. e.g.: Change their name or password

### Example
```kotlin
// Import classes:
//import org.openapitools.client.infrastructure.*
//import org.openapitools.client.models.*

val apiInstance = UsersApi()
val body : UserNamePasswordPut =  // UserNamePasswordPut | The user details
try {
    apiInstance.restUsersMePut(body)
} catch (e: ClientException) {
    println("4xx response calling UsersApi#restUsersMePut")
    e.printStackTrace()
} catch (e: ServerException) {
    println("5xx response calling UsersApi#restUsersMePut")
    e.printStackTrace()
}
```

### Parameters

Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **body** | [**UserNamePasswordPut**](UserNamePasswordPut.md)| The user details |

### Return type

null (empty response body)

### Authorization

No authorization required

### HTTP request headers

 - **Content-Type**: Not defined
 - **Accept**: Not defined

<a id="restUsersMeQuotaGet"></a>
# **restUsersMeQuotaGet**
> UserQuota restUsersMeQuotaGet(filter)

Return user&#39;s quota

Return user&#39;s quota

### Example
```kotlin
// Import classes:
//import org.openapitools.client.infrastructure.*
//import org.openapitools.client.models.*

val apiInstance = UsersApi()
val filter : kotlin.String = filter_example // kotlin.String | 
try {
    val result : UserQuota = apiInstance.restUsersMeQuotaGet(filter)
    println(result)
} catch (e: ClientException) {
    println("4xx response calling UsersApi#restUsersMeQuotaGet")
    e.printStackTrace()
} catch (e: ServerException) {
    println("5xx response calling UsersApi#restUsersMeQuotaGet")
    e.printStackTrace()
}
```

### Parameters

Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **filter** | **kotlin.String**|  | [optional]

### Return type

[**UserQuota**](UserQuota.md)

### Authorization

No authorization required

### HTTP request headers

 - **Content-Type**: Not defined
 - **Accept**: */*

<a id="restUsersMeRecentGet"></a>
# **restUsersMeRecentGet**
> kotlin.collections.List&lt;Folder&gt; restUsersMeRecentGet(mode, with, type, returnEntity)

Return user&#39;s recent items

Return user&#39;s recent items

### Example
```kotlin
// Import classes:
//import org.openapitools.client.infrastructure.*
//import org.openapitools.client.models.*

val apiInstance = UsersApi()
val mode : kotlin.String = mode_example // kotlin.String | 
val with : kotlin.String = with_example // kotlin.String | 
val type : kotlin.collections.List<kotlin.String> =  // kotlin.collections.List<kotlin.String> | 
val returnEntity : kotlin.Boolean = true // kotlin.Boolean | 
try {
    val result : kotlin.collections.List<Folder> = apiInstance.restUsersMeRecentGet(mode, with, type, returnEntity)
    println(result)
} catch (e: ClientException) {
    println("4xx response calling UsersApi#restUsersMeRecentGet")
    e.printStackTrace()
} catch (e: ServerException) {
    println("5xx response calling UsersApi#restUsersMeRecentGet")
    e.printStackTrace()
}
```

### Parameters

Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **mode** | **kotlin.String**|  | [optional]
 **with** | **kotlin.String**|  | [optional]
 **type** | [**kotlin.collections.List&lt;kotlin.String&gt;**](kotlin.String.md)|  | [optional]
 **returnEntity** | **kotlin.Boolean**|  | [optional]

### Return type

[**kotlin.collections.List&lt;Folder&gt;**](Folder.md)

### Authorization

No authorization required

### HTTP request headers

 - **Content-Type**: Not defined
 - **Accept**: */*

<a id="restUsersMeRecentIdDelete"></a>
# **restUsersMeRecentIdDelete**
> restUsersMeRecentIdDelete(id)

Delete user&#39;s recent item

Delete user&#39;s recent item

### Example
```kotlin
// Import classes:
//import org.openapitools.client.infrastructure.*
//import org.openapitools.client.models.*

val apiInstance = UsersApi()
val id : kotlin.Int = 56 // kotlin.Int | The ID of the entity
try {
    apiInstance.restUsersMeRecentIdDelete(id)
} catch (e: ClientException) {
    println("4xx response calling UsersApi#restUsersMeRecentIdDelete")
    e.printStackTrace()
} catch (e: ServerException) {
    println("5xx response calling UsersApi#restUsersMeRecentIdDelete")
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

<a id="restUsersMeRecentPost"></a>
# **restUsersMeRecentPost**
> restUsersMeRecentPost(body)

Adding objects to user&#39;s recent items

Adding objects to user&#39;s recent items

### Example
```kotlin
// Import classes:
//import org.openapitools.client.infrastructure.*
//import org.openapitools.client.models.*

val apiInstance = UsersApi()
val body : RecentObjectsPostRequest =  // RecentObjectsPostRequest | 
try {
    apiInstance.restUsersMeRecentPost(body)
} catch (e: ClientException) {
    println("4xx response calling UsersApi#restUsersMeRecentPost")
    e.printStackTrace()
} catch (e: ServerException) {
    println("5xx response calling UsersApi#restUsersMeRecentPost")
    e.printStackTrace()
}
```

### Parameters

Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **body** | [**RecentObjectsPostRequest**](RecentObjectsPostRequest.md)|  |

### Return type

null (empty response body)

### Authorization

No authorization required

### HTTP request headers

 - **Content-Type**: Not defined
 - **Accept**: Not defined

<a id="restUsersMeTfaAuthPost"></a>
# **restUsersMeTfaAuthPost**
> restUsersMeTfaAuthPost(body)

Two Factor Authentication

Two Factor Authentication

### Example
```kotlin
// Import classes:
//import org.openapitools.client.infrastructure.*
//import org.openapitools.client.models.*

val apiInstance = UsersApi()
val body : UserTfaPost =  // UserTfaPost | TFA
try {
    apiInstance.restUsersMeTfaAuthPost(body)
} catch (e: ClientException) {
    println("4xx response calling UsersApi#restUsersMeTfaAuthPost")
    e.printStackTrace()
} catch (e: ServerException) {
    println("5xx response calling UsersApi#restUsersMeTfaAuthPost")
    e.printStackTrace()
}
```

### Parameters

Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **body** | [**UserTfaPost**](UserTfaPost.md)| TFA |

### Return type

null (empty response body)

### Authorization

No authorization required

### HTTP request headers

 - **Content-Type**: Not defined
 - **Accept**: Not defined

<a id="restUsersMeTfaChallengePost"></a>
# **restUsersMeTfaChallengePost**
> restUsersMeTfaChallengePost(referral)

Two Factor Authentication

Two Factor Authentication

### Example
```kotlin
// Import classes:
//import org.openapitools.client.infrastructure.*
//import org.openapitools.client.models.*

val apiInstance = UsersApi()
val referral : kotlin.String = referral_example // kotlin.String | Referral URL
try {
    apiInstance.restUsersMeTfaChallengePost(referral)
} catch (e: ClientException) {
    println("4xx response calling UsersApi#restUsersMeTfaChallengePost")
    e.printStackTrace()
} catch (e: ServerException) {
    println("5xx response calling UsersApi#restUsersMeTfaChallengePost")
    e.printStackTrace()
}
```

### Parameters

Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **referral** | **kotlin.String**| Referral URL | [optional]

### Return type

null (empty response body)

### Authorization

No authorization required

### HTTP request headers

 - **Content-Type**: Not defined
 - **Accept**: Not defined

<a id="restUsersMeTfaConfigGet"></a>
# **restUsersMeTfaConfigGet**
> restUsersMeTfaConfigGet()

Two Factor Authentication

Two Factor Authentication

### Example
```kotlin
// Import classes:
//import org.openapitools.client.infrastructure.*
//import org.openapitools.client.models.*

val apiInstance = UsersApi()
try {
    apiInstance.restUsersMeTfaConfigGet()
} catch (e: ClientException) {
    println("4xx response calling UsersApi#restUsersMeTfaConfigGet")
    e.printStackTrace()
} catch (e: ServerException) {
    println("5xx response calling UsersApi#restUsersMeTfaConfigGet")
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

<a id="restUsersMeTfaResetTotpSecretPost"></a>
# **restUsersMeTfaResetTotpSecretPost**
> restUsersMeTfaResetTotpSecretPost(body)

Reset secret key for time-based OTP of the current user

Reset secret key for time-based OTP of the current user

### Example
```kotlin
// Import classes:
//import org.openapitools.client.infrastructure.*
//import org.openapitools.client.models.*

val apiInstance = UsersApi()
val body : UserTfaTotpResetSecretPost =  // UserTfaTotpResetSecretPost | The user's credential to reset TOTP secret
try {
    apiInstance.restUsersMeTfaResetTotpSecretPost(body)
} catch (e: ClientException) {
    println("4xx response calling UsersApi#restUsersMeTfaResetTotpSecretPost")
    e.printStackTrace()
} catch (e: ServerException) {
    println("5xx response calling UsersApi#restUsersMeTfaResetTotpSecretPost")
    e.printStackTrace()
}
```

### Parameters

Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **body** | [**UserTfaTotpResetSecretPost**](UserTfaTotpResetSecretPost.md)| The user&#39;s credential to reset TOTP secret |

### Return type

null (empty response body)

### Authorization

No authorization required

### HTTP request headers

 - **Content-Type**: Not defined
 - **Accept**: Not defined

<a id="restUsersMeTfaSetupPut"></a>
# **restUsersMeTfaSetupPut**
> restUsersMeTfaSetupPut(body)

Setup 2FA settings

Updates the 2FA settings for the current user

### Example
```kotlin
// Import classes:
//import org.openapitools.client.infrastructure.*
//import org.openapitools.client.models.*

val apiInstance = UsersApi()
val body : UserTfaPut =  // UserTfaPut | The Settings details
try {
    apiInstance.restUsersMeTfaSetupPut(body)
} catch (e: ClientException) {
    println("4xx response calling UsersApi#restUsersMeTfaSetupPut")
    e.printStackTrace()
} catch (e: ServerException) {
    println("5xx response calling UsersApi#restUsersMeTfaSetupPut")
    e.printStackTrace()
}
```

### Parameters

Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **body** | [**UserTfaPut**](UserTfaPut.md)| The Settings details |

### Return type

null (empty response body)

### Authorization

No authorization required

### HTTP request headers

 - **Content-Type**: Not defined
 - **Accept**: Not defined

<a id="restUsersMeTfaSetupTotpSecretGet"></a>
# **restUsersMeTfaSetupTotpSecretGet**
> restUsersMeTfaSetupTotpSecretGet()

Setup secret key for Time-based OTP of the current user

Setup secret key for Time-based OTP of the current user

### Example
```kotlin
// Import classes:
//import org.openapitools.client.infrastructure.*
//import org.openapitools.client.models.*

val apiInstance = UsersApi()
try {
    apiInstance.restUsersMeTfaSetupTotpSecretGet()
} catch (e: ClientException) {
    println("4xx response calling UsersApi#restUsersMeTfaSetupTotpSecretGet")
    e.printStackTrace()
} catch (e: ServerException) {
    println("5xx response calling UsersApi#restUsersMeTfaSetupTotpSecretGet")
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

<a id="restUsersMeTfaVerifyTotpSecretPost"></a>
# **restUsersMeTfaVerifyTotpSecretPost**
> restUsersMeTfaVerifyTotpSecretPost(body)

Verify code for finalising secret key for timed-based OTP

Verify code for finalising secret key for timed-based OTP

### Example
```kotlin
// Import classes:
//import org.openapitools.client.infrastructure.*
//import org.openapitools.client.models.*

val apiInstance = UsersApi()
val body : UserTfaTotpVerifySecretPost =  // UserTfaTotpVerifySecretPost | OTP
try {
    apiInstance.restUsersMeTfaVerifyTotpSecretPost(body)
} catch (e: ClientException) {
    println("4xx response calling UsersApi#restUsersMeTfaVerifyTotpSecretPost")
    e.printStackTrace()
} catch (e: ServerException) {
    println("5xx response calling UsersApi#restUsersMeTfaVerifyTotpSecretPost")
    e.printStackTrace()
}
```

### Parameters

Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **body** | [**UserTfaTotpVerifySecretPost**](UserTfaTotpVerifySecretPost.md)| OTP |

### Return type

null (empty response body)

### Authorization

No authorization required

### HTTP request headers

 - **Content-Type**: Not defined
 - **Accept**: Not defined

<a id="restUsersMeTosGet"></a>
# **restUsersMeTosGet**
> restUsersMeTosGet()

Terms of Service

Terms of Service

### Example
```kotlin
// Import classes:
//import org.openapitools.client.infrastructure.*
//import org.openapitools.client.models.*

val apiInstance = UsersApi()
try {
    apiInstance.restUsersMeTosGet()
} catch (e: ClientException) {
    println("4xx response calling UsersApi#restUsersMeTosGet")
    e.printStackTrace()
} catch (e: ServerException) {
    println("5xx response calling UsersApi#restUsersMeTosGet")
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

<a id="restUsersMeTosPost"></a>
# **restUsersMeTosPost**
> restUsersMeTosPost(body)

Terms of Service

Terms of Service

### Example
```kotlin
// Import classes:
//import org.openapitools.client.infrastructure.*
//import org.openapitools.client.models.*

val apiInstance = UsersApi()
val body : UserTosPost =  // UserTosPost | TOS acceptance
try {
    apiInstance.restUsersMeTosPost(body)
} catch (e: ClientException) {
    println("4xx response calling UsersApi#restUsersMeTosPost")
    e.printStackTrace()
} catch (e: ServerException) {
    println("5xx response calling UsersApi#restUsersMeTosPost")
    e.printStackTrace()
}
```

### Parameters

Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **body** | [**UserTosPost**](UserTosPost.md)| TOS acceptance |

### Return type

null (empty response body)

### Authorization

No authorization required

### HTTP request headers

 - **Content-Type**: Not defined
 - **Accept**: Not defined

<a id="restUsersPost"></a>
# **restUsersPost**
> restUsersPost(body, returnEntity, mode)

Create a User

Creates a new User in the system by specifying an email address and name.

### Example
```kotlin
// Import classes:
//import org.openapitools.client.infrastructure.*
//import org.openapitools.client.models.*

val apiInstance = UsersApi()
val body : UserPost =  // UserPost | The user details
val returnEntity : kotlin.Boolean = true // kotlin.Boolean | Return information about newly created entity
val mode : kotlin.String = mode_example // kotlin.String | Response mode
try {
    apiInstance.restUsersPost(body, returnEntity, mode)
} catch (e: ClientException) {
    println("4xx response calling UsersApi#restUsersPost")
    e.printStackTrace()
} catch (e: ServerException) {
    println("5xx response calling UsersApi#restUsersPost")
    e.printStackTrace()
}
```

### Parameters

Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **body** | [**UserPost**](UserPost.md)| The user details |
 **returnEntity** | **kotlin.Boolean**| Return information about newly created entity | [optional]
 **mode** | **kotlin.String**| Response mode | [optional]

### Return type

null (empty response body)

### Authorization

No authorization required

### HTTP request headers

 - **Content-Type**: Not defined
 - **Accept**: Not defined

<a id="restUsersPreauthPost"></a>
# **restUsersPreauthPost**
> restUsersPreauthPost(body)

User login preauth

User login preauth.

### Example
```kotlin
// Import classes:
//import org.openapitools.client.infrastructure.*
//import org.openapitools.client.models.*

val apiInstance = UsersApi()
val body : UserPreauthPost =  // UserPreauthPost | User preauth
try {
    apiInstance.restUsersPreauthPost(body)
} catch (e: ClientException) {
    println("4xx response calling UsersApi#restUsersPreauthPost")
    e.printStackTrace()
} catch (e: ServerException) {
    println("5xx response calling UsersApi#restUsersPreauthPost")
    e.printStackTrace()
}
```

### Parameters

Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **body** | [**UserPreauthPost**](UserPreauthPost.md)| User preauth |

### Return type

null (empty response body)

### Authorization

No authorization required

### HTTP request headers

 - **Content-Type**: Not defined
 - **Accept**: Not defined

<a id="restUsersRegisterPost"></a>
# **restUsersRegisterPost**
> restUsersRegisterPost(body)

Register a User

Registers a new User in the system by specifying an email address and password.

### Example
```kotlin
// Import classes:
//import org.openapitools.client.infrastructure.*
//import org.openapitools.client.models.*

val apiInstance = UsersApi()
val body : UserRegisterPost =  // UserRegisterPost | The user details
try {
    apiInstance.restUsersRegisterPost(body)
} catch (e: ClientException) {
    println("4xx response calling UsersApi#restUsersRegisterPost")
    e.printStackTrace()
} catch (e: ServerException) {
    println("5xx response calling UsersApi#restUsersRegisterPost")
    e.printStackTrace()
}
```

### Parameters

Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **body** | [**UserRegisterPost**](UserRegisterPost.md)| The user details |

### Return type

null (empty response body)

### Authorization

No authorization required

### HTTP request headers

 - **Content-Type**: Not defined
 - **Accept**: Not defined

<a id="restUsersRequestPasswordResetPost"></a>
# **restUsersRequestPasswordResetPost**
> restUsersRequestPasswordResetPost(body)

Request for password reset

Request for password reset of existing user

### Example
```kotlin
// Import classes:
//import org.openapitools.client.infrastructure.*
//import org.openapitools.client.models.*

val apiInstance = UsersApi()
val body : UserRequestPasswordResetPost =  // UserRequestPasswordResetPost | The user email
try {
    apiInstance.restUsersRequestPasswordResetPost(body)
} catch (e: ClientException) {
    println("4xx response calling UsersApi#restUsersRequestPasswordResetPost")
    e.printStackTrace()
} catch (e: ServerException) {
    println("5xx response calling UsersApi#restUsersRequestPasswordResetPost")
    e.printStackTrace()
}
```

### Parameters

Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **body** | [**UserRequestPasswordResetPost**](UserRequestPasswordResetPost.md)| The user email |

### Return type

null (empty response body)

### Authorization

No authorization required

### HTTP request headers

 - **Content-Type**: Not defined
 - **Accept**: Not defined

<a id="restUsersResetPasswordPost"></a>
# **restUsersResetPasswordPost**
> restUsersResetPasswordPost(body)

Reset password

Reset password of an existing user

### Example
```kotlin
// Import classes:
//import org.openapitools.client.infrastructure.*
//import org.openapitools.client.models.*

val apiInstance = UsersApi()
val body : UserResetPasswordPost =  // UserResetPasswordPost | The password reset data
try {
    apiInstance.restUsersResetPasswordPost(body)
} catch (e: ClientException) {
    println("4xx response calling UsersApi#restUsersResetPasswordPost")
    e.printStackTrace()
} catch (e: ServerException) {
    println("5xx response calling UsersApi#restUsersResetPasswordPost")
    e.printStackTrace()
}
```

### Parameters

Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **body** | [**UserResetPasswordPost**](UserResetPasswordPost.md)| The password reset data |

### Return type

null (empty response body)

### Authorization

No authorization required

### HTTP request headers

 - **Content-Type**: Not defined
 - **Accept**: Not defined

