# AdminApi

All URIs are relative to *http://localhost*

Method | HTTP request | Description
------------- | ------------- | -------------
[**restAdminActivitiesGet**](AdminApi.md#restAdminActivitiesGet) | **GET** /rest/admin/activities | Get admin activities list
[**restAdminAvailableLdapGroupsGet**](AdminApi.md#restAdminAvailableLdapGroupsGet) | **GET** /rest/admin/availableLdapGroups | Returns a list of available LDAP groups.
[**restAdminClientsClientIdScopesGet**](AdminApi.md#restAdminClientsClientIdScopesGet) | **GET** /rest/admin/clients/{client_id}/scopes | List scopes of a client
[**restAdminClientsGet**](AdminApi.md#restAdminClientsGet) | **GET** /rest/admin/clients | List clients
[**restAdminClientsIdDelete**](AdminApi.md#restAdminClientsIdDelete) | **DELETE** /rest/admin/clients/{id} | Delete a client
[**restAdminClientsIdGet**](AdminApi.md#restAdminClientsIdGet) | **GET** /rest/admin/clients/{id} | Get a client
[**restAdminClientsIdPut**](AdminApi.md#restAdminClientsIdPut) | **PUT** /rest/admin/clients/{id} | Update a client
[**restAdminClientsPost**](AdminApi.md#restAdminClientsPost) | **POST** /rest/admin/clients | Create a client
[**restAdminDevicesActionsWipePost**](AdminApi.md#restAdminDevicesActionsWipePost) | **POST** /rest/admin/devices/actions/wipe | Remote wipe the specified device
[**restAdminDevicesGet**](AdminApi.md#restAdminDevicesGet) | **GET** /rest/admin/devices | List devices
[**restAdminDevicesIdDelete**](AdminApi.md#restAdminDevicesIdDelete) | **DELETE** /rest/admin/devices/{id} | Delete a device
[**restAdminDevicesIdGet**](AdminApi.md#restAdminDevicesIdGet) | **GET** /rest/admin/devices/{id} | Get a device
[**restAdminDevicesIdPut**](AdminApi.md#restAdminDevicesIdPut) | **PUT** /rest/admin/devices/{id} | Update a device
[**restAdminDevicesInstallTagIdWipeGet**](AdminApi.md#restAdminDevicesInstallTagIdWipeGet) | **GET** /rest/admin/devices/{install_tag_id}/wipe | Get the wipe status
[**restAdminDevicesPost**](AdminApi.md#restAdminDevicesPost) | **POST** /rest/admin/devices | Add a device
[**restAdminHostnamesDelete**](AdminApi.md#restAdminHostnamesDelete) | **DELETE** /rest/admin/hostnames | Deletes list of hostnames
[**restAdminHostnamesGet**](AdminApi.md#restAdminHostnamesGet) | **GET** /rest/admin/hostnames | List hostnames
[**restAdminHostnamesIdDelete**](AdminApi.md#restAdminHostnamesIdDelete) | **DELETE** /rest/admin/hostnames/{id} | Mark specified hostname as deleted.
[**restAdminHostnamesIdGet**](AdminApi.md#restAdminHostnamesIdGet) | **GET** /rest/admin/hostnames/{id} | Returns the details of hostname of the specified ID.
[**restAdminHostnamesIdPut**](AdminApi.md#restAdminHostnamesIdPut) | **PUT** /rest/admin/hostnames/{id} | Disable / enable alias hostname
[**restAdminHostnamesPost**](AdminApi.md#restAdminHostnamesPost) | **POST** /rest/admin/hostnames | Create an alias hostname
[**restAdminLdapGroupsGet**](AdminApi.md#restAdminLdapGroupsGet) | **GET** /rest/admin/ldapGroups | Returns a list of LDAP groups.
[**restAdminLdapGroupsIdDelete**](AdminApi.md#restAdminLdapGroupsIdDelete) | **DELETE** /rest/admin/ldapGroups/{id} | Deletes an LDAP group
[**restAdminLdapGroupsIdGet**](AdminApi.md#restAdminLdapGroupsIdGet) | **GET** /rest/admin/ldapGroups/{id} | Gets an LDAP group
[**restAdminLdapGroupsIdPut**](AdminApi.md#restAdminLdapGroupsIdPut) | **PUT** /rest/admin/ldapGroups/{id} | Updates an LDAP group
[**restAdminLdapGroupsPost**](AdminApi.md#restAdminLdapGroupsPost) | **POST** /rest/admin/ldapGroups | Create an LDAP group
[**restAdminLocationsGet**](AdminApi.md#restAdminLocationsGet) | **GET** /rest/admin/locations | List locations
[**restAdminLocationsIdDelete**](AdminApi.md#restAdminLocationsIdDelete) | **DELETE** /rest/admin/locations/{id} | Delete a location.
[**restAdminLocationsIdGet**](AdminApi.md#restAdminLocationsIdGet) | **GET** /rest/admin/locations/{id} | Return location name.
[**restAdminLocationsPost**](AdminApi.md#restAdminLocationsPost) | **POST** /rest/admin/locations | Create a location entry.
[**restAdminMailActionsWithdrawFilesUsersUserIdDelete**](AdminApi.md#restAdminMailActionsWithdrawFilesUsersUserIdDelete) | **DELETE** /rest/admin/mail/actions/withdrawFiles/users/{userId} | Withdraw all files from deleted/demoted users&#39; emails
[**restAdminMailGet**](AdminApi.md#restAdminMailGet) | **GET** /rest/admin/mail | List emails
[**restAdminProfilesGet**](AdminApi.md#restAdminProfilesGet) | **GET** /rest/admin/profiles | List user types
[**restAdminProfilesIdGet**](AdminApi.md#restAdminProfilesIdGet) | **GET** /rest/admin/profiles/{id} | Return an user type
[**restAdminProfilesIdMappingsGet**](AdminApi.md#restAdminProfilesIdMappingsGet) | **GET** /rest/admin/profiles/{id}/mappings | Get profile mapping details
[**restAdminProfilesIdMappingsPut**](AdminApi.md#restAdminProfilesIdMappingsPut) | **PUT** /rest/admin/profiles/{id}/mappings | Update profile mapping details
[**restAdminProfilesIdUsersGet**](AdminApi.md#restAdminProfilesIdUsersGet) | **GET** /rest/admin/profiles/{id}/users | Return list of users with the specified types
[**restAdminProfilesIdUsersPut**](AdminApi.md#restAdminProfilesIdUsersPut) | **PUT** /rest/admin/profiles/{id}/users | Change user type
[**restAdminProfilesMappingOrderGet**](AdminApi.md#restAdminProfilesMappingOrderGet) | **GET** /rest/admin/profiles/mappingOrder | Get profile mapping order
[**restAdminProfilesMappingOrderPut**](AdminApi.md#restAdminProfilesMappingOrderPut) | **PUT** /rest/admin/profiles/mappingOrder | Update profile mapping order
[**restAdminProfilesMappingsGet**](AdminApi.md#restAdminProfilesMappingsGet) | **GET** /rest/admin/profiles/mappings | Get profile mapping results for user
[**restAdminRequestFileUsersUserIdDelete**](AdminApi.md#restAdminRequestFileUsersUserIdDelete) | **DELETE** /rest/admin/requestFile/users/{userId} | Delete request files sent by the the specified user
[**restAdminSourcesGet**](AdminApi.md#restAdminSourcesGet) | **GET** /rest/admin/sources | List all added sources
[**restAdminSourcesIdDelete**](AdminApi.md#restAdminSourcesIdDelete) | **DELETE** /rest/admin/sources/{id} | Deletes specified assigned source
[**restAdminSourcesIdGet**](AdminApi.md#restAdminSourcesIdGet) | **GET** /rest/admin/sources/{id} | Returns requested assigned ECM source
[**restAdminSourcesIdPut**](AdminApi.md#restAdminSourcesIdPut) | **PUT** /rest/admin/sources/{id} | Updates details of the specified ECM source
[**restAdminSourcesPost**](AdminApi.md#restAdminSourcesPost) | **POST** /rest/admin/sources | Add assigned ECM source
[**restAdminUsersGet**](AdminApi.md#restAdminUsersGet) | **GET** /rest/admin/users | Get a list of Users
[**restAdminUsersIdAdminRolesGet**](AdminApi.md#restAdminUsersIdAdminRolesGet) | **GET** /rest/admin/users/{id}/adminRoles | Return admin roles of the specified user id.
[**restAdminUsersIdDelete**](AdminApi.md#restAdminUsersIdDelete) | **DELETE** /rest/admin/users/{id} | Deletes a User
[**restAdminUsersIdDevicesGet**](AdminApi.md#restAdminUsersIdDevicesGet) | **GET** /rest/admin/users/{id}/devices | List devices for a user
[**restAdminUsersIdGet**](AdminApi.md#restAdminUsersIdGet) | **GET** /rest/admin/users/{id} | Get User
[**restAdminUsersIdPut**](AdminApi.md#restAdminUsersIdPut) | **PUT** /rest/admin/users/{id} | Update User
[**restAdminUsersIdSettingsGet**](AdminApi.md#restAdminUsersIdSettingsGet) | **GET** /rest/admin/users/{id}/settings | Get User Settings
[**restAdminUsersMigrateEmailsCsvPost**](AdminApi.md#restAdminUsersMigrateEmailsCsvPost) | **POST** /rest/admin/users/migrateEmailsCsv | Endpoint to bulk update users emails
[**restAdminUsersMigrateEmailsPost**](AdminApi.md#restAdminUsersMigrateEmailsPost) | **POST** /rest/admin/users/migrateEmails | Endpoint to bulk update users emails
[**restAdminUsersPost**](AdminApi.md#restAdminUsersPost) | **POST** /rest/admin/users | Create a User


<a id="restAdminActivitiesGet"></a>
# **restAdminActivitiesGet**
> ActivityList restAdminActivitiesGet(endDateTime, startDateTime, objectIdsColonIn, maxPages, limit, userId, orderBy, compact, eventFiltersColonIn, offset)

Get admin activities list

Get admin activities list

### Example
```kotlin
// Import classes:
//import org.openapitools.client.infrastructure.*
//import org.openapitools.client.models.*

val apiInstance = AdminApi()
val endDateTime : kotlin.String = endDateTime_example // kotlin.String | End date time
val startDateTime : kotlin.String = startDateTime_example // kotlin.String | Start date time
val objectIdsColonIn : kotlin.collections.List<kotlin.String> =  // kotlin.collections.List<kotlin.String> | 
val maxPages : kotlin.Int = 56 // kotlin.Int | 
val limit : kotlin.Int = 56 // kotlin.Int | 
val userId : kotlin.String = userId_example // kotlin.String | 
val orderBy : kotlin.String = orderBy_example // kotlin.String | Order By (created, username, client, ip_address)
val compact : kotlin.Boolean = true // kotlin.Boolean | 
val eventFiltersColonIn : kotlin.collections.List<kotlin.String> =  // kotlin.collections.List<kotlin.String> | 
val offset : kotlin.Int = 56 // kotlin.Int | 
try {
    val result : ActivityList = apiInstance.restAdminActivitiesGet(endDateTime, startDateTime, objectIdsColonIn, maxPages, limit, userId, orderBy, compact, eventFiltersColonIn, offset)
    println(result)
} catch (e: ClientException) {
    println("4xx response calling AdminApi#restAdminActivitiesGet")
    e.printStackTrace()
} catch (e: ServerException) {
    println("5xx response calling AdminApi#restAdminActivitiesGet")
    e.printStackTrace()
}
```

### Parameters

Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **endDateTime** | **kotlin.String**| End date time |
 **startDateTime** | **kotlin.String**| Start date time |
 **objectIdsColonIn** | [**kotlin.collections.List&lt;kotlin.String&gt;**](kotlin.String.md)|  | [optional]
 **maxPages** | **kotlin.Int**|  | [optional]
 **limit** | **kotlin.Int**|  | [optional]
 **userId** | **kotlin.String**|  | [optional]
 **orderBy** | **kotlin.String**| Order By (created, username, client, ip_address) | [optional]
 **compact** | **kotlin.Boolean**|  | [optional]
 **eventFiltersColonIn** | [**kotlin.collections.List&lt;kotlin.String&gt;**](kotlin.String.md)|  | [optional]
 **offset** | **kotlin.Int**|  | [optional]

### Return type

[**ActivityList**](ActivityList.md)

### Authorization

No authorization required

### HTTP request headers

 - **Content-Type**: Not defined
 - **Accept**: */*

<a id="restAdminAvailableLdapGroupsGet"></a>
# **restAdminAvailableLdapGroupsGet**
> kotlin.collections.List&lt;AvailableLdapGroup&gt; restAdminAvailableLdapGroupsGet(filter, orderBy, mode)

Returns a list of available LDAP groups.

Returns a list of available LDAP groups.

### Example
```kotlin
// Import classes:
//import org.openapitools.client.infrastructure.*
//import org.openapitools.client.models.*

val apiInstance = AdminApi()
val filter : kotlin.String = filter_example // kotlin.String | Text to search for in cn, dn or description.
val orderBy : kotlin.collections.List<kotlin.String> =  // kotlin.collections.List<kotlin.String> | Sorting options
val mode : kotlin.String = mode_example // kotlin.String | Response mode
try {
    val result : kotlin.collections.List<AvailableLdapGroup> = apiInstance.restAdminAvailableLdapGroupsGet(filter, orderBy, mode)
    println(result)
} catch (e: ClientException) {
    println("4xx response calling AdminApi#restAdminAvailableLdapGroupsGet")
    e.printStackTrace()
} catch (e: ServerException) {
    println("5xx response calling AdminApi#restAdminAvailableLdapGroupsGet")
    e.printStackTrace()
}
```

### Parameters

Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **filter** | **kotlin.String**| Text to search for in cn, dn or description. |
 **orderBy** | [**kotlin.collections.List&lt;kotlin.String&gt;**](kotlin.String.md)| Sorting options | [optional]
 **mode** | **kotlin.String**| Response mode | [optional]

### Return type

[**kotlin.collections.List&lt;AvailableLdapGroup&gt;**](AvailableLdapGroup.md)

### Authorization

No authorization required

### HTTP request headers

 - **Content-Type**: Not defined
 - **Accept**: */*

<a id="restAdminClientsClientIdScopesGet"></a>
# **restAdminClientsClientIdScopesGet**
> restAdminClientsClientIdScopesGet(clientId)

List scopes of a client

Return a list of scopes for a specific client.     This returns the methods that this client is allowed to use     such as folders, files, members, comments, etc.

### Example
```kotlin
// Import classes:
//import org.openapitools.client.infrastructure.*
//import org.openapitools.client.models.*

val apiInstance = AdminApi()
val clientId : kotlin.String = clientId_example // kotlin.String | ID of the client whose scopes to be retrieved
try {
    apiInstance.restAdminClientsClientIdScopesGet(clientId)
} catch (e: ClientException) {
    println("4xx response calling AdminApi#restAdminClientsClientIdScopesGet")
    e.printStackTrace()
} catch (e: ServerException) {
    println("5xx response calling AdminApi#restAdminClientsClientIdScopesGet")
    e.printStackTrace()
}
```

### Parameters

Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **clientId** | **kotlin.String**| ID of the client whose scopes to be retrieved |

### Return type

null (empty response body)

### Authorization

No authorization required

### HTTP request headers

 - **Content-Type**: Not defined
 - **Accept**: Not defined

<a id="restAdminClientsGet"></a>
# **restAdminClientsGet**
> kotlin.collections.List&lt;Client&gt; restAdminClientsGet(name, nameColonContains, descriptionColonContains, orderBy, offset, limit, with, mode)

List clients

Return a list of clients

### Example
```kotlin
// Import classes:
//import org.openapitools.client.infrastructure.*
//import org.openapitools.client.models.*

val apiInstance = AdminApi()
val name : kotlin.String = name_example // kotlin.String | Client name
val nameColonContains : kotlin.String = nameColonContains_example // kotlin.String | Client name. Search for result that contains specified characters in this parameter.
val descriptionColonContains : kotlin.String = descriptionColonContains_example // kotlin.String | Client description. Search for result that contains specified characters in this parameter.
val orderBy : kotlin.collections.List<kotlin.String> =  // kotlin.collections.List<kotlin.String> | Sorting options
val offset : kotlin.Int = 56 // kotlin.Int | Offset
val limit : kotlin.Int = 56 // kotlin.Int | Limit
val with : kotlin.String = with_example // kotlin.String | With parameters
val mode : kotlin.String = mode_example // kotlin.String | Response mode
try {
    val result : kotlin.collections.List<Client> = apiInstance.restAdminClientsGet(name, nameColonContains, descriptionColonContains, orderBy, offset, limit, with, mode)
    println(result)
} catch (e: ClientException) {
    println("4xx response calling AdminApi#restAdminClientsGet")
    e.printStackTrace()
} catch (e: ServerException) {
    println("5xx response calling AdminApi#restAdminClientsGet")
    e.printStackTrace()
}
```

### Parameters

Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **name** | **kotlin.String**| Client name | [optional]
 **nameColonContains** | **kotlin.String**| Client name. Search for result that contains specified characters in this parameter. | [optional]
 **descriptionColonContains** | **kotlin.String**| Client description. Search for result that contains specified characters in this parameter. | [optional]
 **orderBy** | [**kotlin.collections.List&lt;kotlin.String&gt;**](kotlin.String.md)| Sorting options | [optional]
 **offset** | **kotlin.Int**| Offset | [optional]
 **limit** | **kotlin.Int**| Limit | [optional]
 **with** | **kotlin.String**| With parameters | [optional]
 **mode** | **kotlin.String**| Response mode | [optional]

### Return type

[**kotlin.collections.List&lt;Client&gt;**](Client.md)

### Authorization

No authorization required

### HTTP request headers

 - **Content-Type**: Not defined
 - **Accept**: */*

<a id="restAdminClientsIdDelete"></a>
# **restAdminClientsIdDelete**
> restAdminClientsIdDelete(id)

Delete a client

Delete a client from the client list.

### Example
```kotlin
// Import classes:
//import org.openapitools.client.infrastructure.*
//import org.openapitools.client.models.*

val apiInstance = AdminApi()
val id : kotlin.String = id_example // kotlin.String | ID of the client to be deleted
try {
    apiInstance.restAdminClientsIdDelete(id)
} catch (e: ClientException) {
    println("4xx response calling AdminApi#restAdminClientsIdDelete")
    e.printStackTrace()
} catch (e: ServerException) {
    println("5xx response calling AdminApi#restAdminClientsIdDelete")
    e.printStackTrace()
}
```

### Parameters

Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **id** | **kotlin.String**| ID of the client to be deleted |

### Return type

null (empty response body)

### Authorization

No authorization required

### HTTP request headers

 - **Content-Type**: Not defined
 - **Accept**: Not defined

<a id="restAdminClientsIdGet"></a>
# **restAdminClientsIdGet**
> Client restAdminClientsIdGet(id)

Get a client

Return the admin settings of a specified client.     e.g.: I want the admin settings for my iOS client; pin timeout, token lifetime, etc., 

### Example
```kotlin
// Import classes:
//import org.openapitools.client.infrastructure.*
//import org.openapitools.client.models.*

val apiInstance = AdminApi()
val id : kotlin.Int = 56 // kotlin.Int | ID of the client to be retrieved
try {
    val result : Client = apiInstance.restAdminClientsIdGet(id)
    println(result)
} catch (e: ClientException) {
    println("4xx response calling AdminApi#restAdminClientsIdGet")
    e.printStackTrace()
} catch (e: ServerException) {
    println("5xx response calling AdminApi#restAdminClientsIdGet")
    e.printStackTrace()
}
```

### Parameters

Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **id** | **kotlin.Int**| ID of the client to be retrieved |

### Return type

[**Client**](Client.md)

### Authorization

No authorization required

### HTTP request headers

 - **Content-Type**: Not defined
 - **Accept**: */*

<a id="restAdminClientsIdPut"></a>
# **restAdminClientsIdPut**
> restAdminClientsIdPut(id, body)

Update a client

Update the admin settings for the specified client

### Example
```kotlin
// Import classes:
//import org.openapitools.client.infrastructure.*
//import org.openapitools.client.models.*

val apiInstance = AdminApi()
val id : kotlin.Int = 56 // kotlin.Int | ID of the client to be updated
val body : ClientPut =  // ClientPut | Details of the client
try {
    apiInstance.restAdminClientsIdPut(id, body)
} catch (e: ClientException) {
    println("4xx response calling AdminApi#restAdminClientsIdPut")
    e.printStackTrace()
} catch (e: ServerException) {
    println("5xx response calling AdminApi#restAdminClientsIdPut")
    e.printStackTrace()
}
```

### Parameters

Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **id** | **kotlin.Int**| ID of the client to be updated |
 **body** | [**ClientPut**](ClientPut.md)| Details of the client |

### Return type

null (empty response body)

### Authorization

No authorization required

### HTTP request headers

 - **Content-Type**: Not defined
 - **Accept**: Not defined

<a id="restAdminClientsPost"></a>
# **restAdminClientsPost**
> restAdminClientsPost(body, returnEntity, mode)

Create a client

Create a new client that will be able to access the kiteworks system.     e.g.: A new mobile app that is customized for your company.

### Example
```kotlin
// Import classes:
//import org.openapitools.client.infrastructure.*
//import org.openapitools.client.models.*

val apiInstance = AdminApi()
val body : ClientPost =  // ClientPost | Details of the client
val returnEntity : kotlin.Boolean = true // kotlin.Boolean | Return information about newly created entity
val mode : kotlin.String = mode_example // kotlin.String | Response mode
try {
    apiInstance.restAdminClientsPost(body, returnEntity, mode)
} catch (e: ClientException) {
    println("4xx response calling AdminApi#restAdminClientsPost")
    e.printStackTrace()
} catch (e: ServerException) {
    println("5xx response calling AdminApi#restAdminClientsPost")
    e.printStackTrace()
}
```

### Parameters

Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **body** | [**ClientPost**](ClientPost.md)| Details of the client |
 **returnEntity** | **kotlin.Boolean**| Return information about newly created entity | [optional]
 **mode** | **kotlin.String**| Response mode | [optional]

### Return type

null (empty response body)

### Authorization

No authorization required

### HTTP request headers

 - **Content-Type**: Not defined
 - **Accept**: Not defined

<a id="restAdminDevicesActionsWipePost"></a>
# **restAdminDevicesActionsWipePost**
> restAdminDevicesActionsWipePost(body)

Remote wipe the specified device

Set the remote wipe flag for the specified install_tag_id

### Example
```kotlin
// Import classes:
//import org.openapitools.client.infrastructure.*
//import org.openapitools.client.models.*

val apiInstance = AdminApi()
val body : RemoteWipePost =  // RemoteWipePost | Details of device to wipe
try {
    apiInstance.restAdminDevicesActionsWipePost(body)
} catch (e: ClientException) {
    println("4xx response calling AdminApi#restAdminDevicesActionsWipePost")
    e.printStackTrace()
} catch (e: ServerException) {
    println("5xx response calling AdminApi#restAdminDevicesActionsWipePost")
    e.printStackTrace()
}
```

### Parameters

Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **body** | [**RemoteWipePost**](RemoteWipePost.md)| Details of device to wipe |

### Return type

null (empty response body)

### Authorization

No authorization required

### HTTP request headers

 - **Content-Type**: Not defined
 - **Accept**: Not defined

<a id="restAdminDevicesGet"></a>
# **restAdminDevicesGet**
> kotlin.collections.List&lt;Device&gt; restAdminDevicesGet(installTagId, installTagIdColonContains, userId, userIdColonIn, clientId, clientIdColonContains, orderBy, offset, limit, with, mode)

List devices

Return a list of devices. e.g.: Returns a list of devices, per user,     that have authenticated on this server.     The list includes the name of the device (iPad, iPhone, etc),     install tag id, client id, and remote wipe flag.

### Example
```kotlin
// Import classes:
//import org.openapitools.client.infrastructure.*
//import org.openapitools.client.models.*

val apiInstance = AdminApi()
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
    val result : kotlin.collections.List<Device> = apiInstance.restAdminDevicesGet(installTagId, installTagIdColonContains, userId, userIdColonIn, clientId, clientIdColonContains, orderBy, offset, limit, with, mode)
    println(result)
} catch (e: ClientException) {
    println("4xx response calling AdminApi#restAdminDevicesGet")
    e.printStackTrace()
} catch (e: ServerException) {
    println("5xx response calling AdminApi#restAdminDevicesGet")
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

<a id="restAdminDevicesIdDelete"></a>
# **restAdminDevicesIdDelete**
> restAdminDevicesIdDelete(id)

Delete a device

Delete a device given the client id

### Example
```kotlin
// Import classes:
//import org.openapitools.client.infrastructure.*
//import org.openapitools.client.models.*

val apiInstance = AdminApi()
val id : kotlin.String = id_example // kotlin.String | ID of the device to be deleted
try {
    apiInstance.restAdminDevicesIdDelete(id)
} catch (e: ClientException) {
    println("4xx response calling AdminApi#restAdminDevicesIdDelete")
    e.printStackTrace()
} catch (e: ServerException) {
    println("5xx response calling AdminApi#restAdminDevicesIdDelete")
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

<a id="restAdminDevicesIdGet"></a>
# **restAdminDevicesIdGet**
> Device restAdminDevicesIdGet(id)

Get a device

Return the details of a specified device. Given the device id,     return the device name, install tag id, client id, and remote wipe flag.

### Example
```kotlin
// Import classes:
//import org.openapitools.client.infrastructure.*
//import org.openapitools.client.models.*

val apiInstance = AdminApi()
val id : kotlin.Int = 56 // kotlin.Int | ID of the device to be retrieved
try {
    val result : Device = apiInstance.restAdminDevicesIdGet(id)
    println(result)
} catch (e: ClientException) {
    println("4xx response calling AdminApi#restAdminDevicesIdGet")
    e.printStackTrace()
} catch (e: ServerException) {
    println("5xx response calling AdminApi#restAdminDevicesIdGet")
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

<a id="restAdminDevicesIdPut"></a>
# **restAdminDevicesIdPut**
> restAdminDevicesIdPut(id, body)

Update a device

Update the details of a device. Can change the mobile key store and messaging registration token.

### Example
```kotlin
// Import classes:
//import org.openapitools.client.infrastructure.*
//import org.openapitools.client.models.*

val apiInstance = AdminApi()
val id : kotlin.Int = 56 // kotlin.Int | ID of the device to be updated
val body : DevicePut =  // DevicePut | Details of the device
try {
    apiInstance.restAdminDevicesIdPut(id, body)
} catch (e: ClientException) {
    println("4xx response calling AdminApi#restAdminDevicesIdPut")
    e.printStackTrace()
} catch (e: ServerException) {
    println("5xx response calling AdminApi#restAdminDevicesIdPut")
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

<a id="restAdminDevicesInstallTagIdWipeGet"></a>
# **restAdminDevicesInstallTagIdWipeGet**
> kotlin.Int restAdminDevicesInstallTagIdWipeGet(installTagId)

Get the wipe status

Returns the remote wipe status of a specified device identified by install_tag_id

### Example
```kotlin
// Import classes:
//import org.openapitools.client.infrastructure.*
//import org.openapitools.client.models.*

val apiInstance = AdminApi()
val installTagId : kotlin.String = installTagId_example // kotlin.String | ID of the device to be retrieved
try {
    val result : kotlin.Int = apiInstance.restAdminDevicesInstallTagIdWipeGet(installTagId)
    println(result)
} catch (e: ClientException) {
    println("4xx response calling AdminApi#restAdminDevicesInstallTagIdWipeGet")
    e.printStackTrace()
} catch (e: ServerException) {
    println("5xx response calling AdminApi#restAdminDevicesInstallTagIdWipeGet")
    e.printStackTrace()
}
```

### Parameters

Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **installTagId** | **kotlin.String**| ID of the device to be retrieved |

### Return type

**kotlin.Int**

### Authorization

No authorization required

### HTTP request headers

 - **Content-Type**: Not defined
 - **Accept**: */*

<a id="restAdminDevicesPost"></a>
# **restAdminDevicesPost**
> restAdminDevicesPost(body, returnEntity, mode)

Add a device

Add a device. This method is used when a user logs in to kiteworks     to track the device they use.

### Example
```kotlin
// Import classes:
//import org.openapitools.client.infrastructure.*
//import org.openapitools.client.models.*

val apiInstance = AdminApi()
val body : DevicePost =  // DevicePost | Details of the device
val returnEntity : kotlin.Boolean = true // kotlin.Boolean | Return information about newly created entity
val mode : kotlin.String = mode_example // kotlin.String | Response mode
try {
    apiInstance.restAdminDevicesPost(body, returnEntity, mode)
} catch (e: ClientException) {
    println("4xx response calling AdminApi#restAdminDevicesPost")
    e.printStackTrace()
} catch (e: ServerException) {
    println("5xx response calling AdminApi#restAdminDevicesPost")
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

<a id="restAdminHostnamesDelete"></a>
# **restAdminHostnamesDelete**
> restAdminHostnamesDelete(idColonIn, partialSuccess, mode)

Deletes list of hostnames

Deletes list of hostnames.

### Example
```kotlin
// Import classes:
//import org.openapitools.client.infrastructure.*
//import org.openapitools.client.models.*

val apiInstance = AdminApi()
val idColonIn : kotlin.String = idColonIn_example // kotlin.String | Array of values which are going to be changed.
val partialSuccess : kotlin.Boolean = true // kotlin.Boolean | Whether to perform action on valid items even if some ones fail
val mode : kotlin.String = mode_example // kotlin.String | Response mode
try {
    apiInstance.restAdminHostnamesDelete(idColonIn, partialSuccess, mode)
} catch (e: ClientException) {
    println("4xx response calling AdminApi#restAdminHostnamesDelete")
    e.printStackTrace()
} catch (e: ServerException) {
    println("5xx response calling AdminApi#restAdminHostnamesDelete")
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

<a id="restAdminHostnamesGet"></a>
# **restAdminHostnamesGet**
> Hostname restAdminHostnamesGet(with, mode)

List hostnames

Returns a list of hostnames

### Example
```kotlin
// Import classes:
//import org.openapitools.client.infrastructure.*
//import org.openapitools.client.models.*

val apiInstance = AdminApi()
val with : kotlin.String = with_example // kotlin.String | With parameters
val mode : kotlin.String = mode_example // kotlin.String | Response mode
try {
    val result : Hostname = apiInstance.restAdminHostnamesGet(with, mode)
    println(result)
} catch (e: ClientException) {
    println("4xx response calling AdminApi#restAdminHostnamesGet")
    e.printStackTrace()
} catch (e: ServerException) {
    println("5xx response calling AdminApi#restAdminHostnamesGet")
    e.printStackTrace()
}
```

### Parameters

Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **with** | **kotlin.String**| With parameters | [optional]
 **mode** | **kotlin.String**| Response mode | [optional]

### Return type

[**Hostname**](Hostname.md)

### Authorization

No authorization required

### HTTP request headers

 - **Content-Type**: Not defined
 - **Accept**: */*

<a id="restAdminHostnamesIdDelete"></a>
# **restAdminHostnamesIdDelete**
> restAdminHostnamesIdDelete(id)

Mark specified hostname as deleted.

Marks the specified hostname as deleted.

### Example
```kotlin
// Import classes:
//import org.openapitools.client.infrastructure.*
//import org.openapitools.client.models.*

val apiInstance = AdminApi()
val id : kotlin.Int = 56 // kotlin.Int | ID of the hostname
try {
    apiInstance.restAdminHostnamesIdDelete(id)
} catch (e: ClientException) {
    println("4xx response calling AdminApi#restAdminHostnamesIdDelete")
    e.printStackTrace()
} catch (e: ServerException) {
    println("5xx response calling AdminApi#restAdminHostnamesIdDelete")
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

<a id="restAdminHostnamesIdGet"></a>
# **restAdminHostnamesIdGet**
> Hostname restAdminHostnamesIdGet(id)

Returns the details of hostname of the specified ID.

Returns the details of hostname of the specified ID.

### Example
```kotlin
// Import classes:
//import org.openapitools.client.infrastructure.*
//import org.openapitools.client.models.*

val apiInstance = AdminApi()
val id : kotlin.Int = 56 // kotlin.Int | ID of the hostname to be retrieved
try {
    val result : Hostname = apiInstance.restAdminHostnamesIdGet(id)
    println(result)
} catch (e: ClientException) {
    println("4xx response calling AdminApi#restAdminHostnamesIdGet")
    e.printStackTrace()
} catch (e: ServerException) {
    println("5xx response calling AdminApi#restAdminHostnamesIdGet")
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

<a id="restAdminHostnamesIdPut"></a>
# **restAdminHostnamesIdPut**
> restAdminHostnamesIdPut(id, body)

Disable / enable alias hostname

Disable / enable the specified hostname.

### Example
```kotlin
// Import classes:
//import org.openapitools.client.infrastructure.*
//import org.openapitools.client.models.*

val apiInstance = AdminApi()
val id : kotlin.Int = 56 // kotlin.Int | ID of the hostname to disable
val body : HostnamePut =  // HostnamePut | comment to activity
try {
    apiInstance.restAdminHostnamesIdPut(id, body)
} catch (e: ClientException) {
    println("4xx response calling AdminApi#restAdminHostnamesIdPut")
    e.printStackTrace()
} catch (e: ServerException) {
    println("5xx response calling AdminApi#restAdminHostnamesIdPut")
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

<a id="restAdminHostnamesPost"></a>
# **restAdminHostnamesPost**
> restAdminHostnamesPost(body, returnEntity, mode)

Create an alias hostname

Create an alias hostname.

### Example
```kotlin
// Import classes:
//import org.openapitools.client.infrastructure.*
//import org.openapitools.client.models.*

val apiInstance = AdminApi()
val body : HostnamePost =  // HostnamePost | comment to activity
val returnEntity : kotlin.Boolean = true // kotlin.Boolean | Return information about newly created entity
val mode : kotlin.String = mode_example // kotlin.String | Response mode
try {
    apiInstance.restAdminHostnamesPost(body, returnEntity, mode)
} catch (e: ClientException) {
    println("4xx response calling AdminApi#restAdminHostnamesPost")
    e.printStackTrace()
} catch (e: ServerException) {
    println("5xx response calling AdminApi#restAdminHostnamesPost")
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

null (empty response body)

### Authorization

No authorization required

### HTTP request headers

 - **Content-Type**: Not defined
 - **Accept**: Not defined

<a id="restAdminLdapGroupsGet"></a>
# **restAdminLdapGroupsGet**
> kotlin.collections.List&lt;LdapGroup&gt; restAdminLdapGroupsGet(name, nameColonContains, email, emailColonContains, orderBy, offset, limit, with, mode)

Returns a list of LDAP groups.

Returns a list of LDAP groups that have been enabled through the kiteworks admin.

### Example
```kotlin
// Import classes:
//import org.openapitools.client.infrastructure.*
//import org.openapitools.client.models.*

val apiInstance = AdminApi()
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
    val result : kotlin.collections.List<LdapGroup> = apiInstance.restAdminLdapGroupsGet(name, nameColonContains, email, emailColonContains, orderBy, offset, limit, with, mode)
    println(result)
} catch (e: ClientException) {
    println("4xx response calling AdminApi#restAdminLdapGroupsGet")
    e.printStackTrace()
} catch (e: ServerException) {
    println("5xx response calling AdminApi#restAdminLdapGroupsGet")
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

<a id="restAdminLdapGroupsIdDelete"></a>
# **restAdminLdapGroupsIdDelete**
> restAdminLdapGroupsIdDelete(id)

Deletes an LDAP group

Deletes an LDAP group

### Example
```kotlin
// Import classes:
//import org.openapitools.client.infrastructure.*
//import org.openapitools.client.models.*

val apiInstance = AdminApi()
val id : kotlin.Int = 56 // kotlin.Int | ID of the LDAP group to delete
try {
    apiInstance.restAdminLdapGroupsIdDelete(id)
} catch (e: ClientException) {
    println("4xx response calling AdminApi#restAdminLdapGroupsIdDelete")
    e.printStackTrace()
} catch (e: ServerException) {
    println("5xx response calling AdminApi#restAdminLdapGroupsIdDelete")
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

<a id="restAdminLdapGroupsIdGet"></a>
# **restAdminLdapGroupsIdGet**
> LdapGroup restAdminLdapGroupsIdGet(id)

Gets an LDAP group

Returns the details of a specified LDAP group. This includes the settings from the admin.

### Example
```kotlin
// Import classes:
//import org.openapitools.client.infrastructure.*
//import org.openapitools.client.models.*

val apiInstance = AdminApi()
val id : kotlin.Int = 56 // kotlin.Int | ID of the LDAP group to be retrieved
try {
    val result : LdapGroup = apiInstance.restAdminLdapGroupsIdGet(id)
    println(result)
} catch (e: ClientException) {
    println("4xx response calling AdminApi#restAdminLdapGroupsIdGet")
    e.printStackTrace()
} catch (e: ServerException) {
    println("5xx response calling AdminApi#restAdminLdapGroupsIdGet")
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

<a id="restAdminLdapGroupsIdPut"></a>
# **restAdminLdapGroupsIdPut**
> restAdminLdapGroupsIdPut(id, body)

Updates an LDAP group

Updates an LDAP group

### Example
```kotlin
// Import classes:
//import org.openapitools.client.infrastructure.*
//import org.openapitools.client.models.*

val apiInstance = AdminApi()
val id : kotlin.Int = 56 // kotlin.Int | ID of the LDAP to update
val body : LdapGroupPut =  // LdapGroupPut | The LDAP group details
try {
    apiInstance.restAdminLdapGroupsIdPut(id, body)
} catch (e: ClientException) {
    println("4xx response calling AdminApi#restAdminLdapGroupsIdPut")
    e.printStackTrace()
} catch (e: ServerException) {
    println("5xx response calling AdminApi#restAdminLdapGroupsIdPut")
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

<a id="restAdminLdapGroupsPost"></a>
# **restAdminLdapGroupsPost**
> restAdminLdapGroupsPost(body, returnEntity, mode)

Create an LDAP group

Creates an LDAP group

### Example
```kotlin
// Import classes:
//import org.openapitools.client.infrastructure.*
//import org.openapitools.client.models.*

val apiInstance = AdminApi()
val body : LdapGroupPost =  // LdapGroupPost | The LDAP group details
val returnEntity : kotlin.Boolean = true // kotlin.Boolean | Return information about newly created entity
val mode : kotlin.String = mode_example // kotlin.String | Response mode
try {
    apiInstance.restAdminLdapGroupsPost(body, returnEntity, mode)
} catch (e: ClientException) {
    println("4xx response calling AdminApi#restAdminLdapGroupsPost")
    e.printStackTrace()
} catch (e: ServerException) {
    println("5xx response calling AdminApi#restAdminLdapGroupsPost")
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

<a id="restAdminLocationsGet"></a>
# **restAdminLocationsGet**
> Location restAdminLocationsGet(mode)

List locations

Returns a list of available kiteworks locations.     Locations are logical collection of multiple kiteworks servers,     usually with a common geography or particular purpose.

### Example
```kotlin
// Import classes:
//import org.openapitools.client.infrastructure.*
//import org.openapitools.client.models.*

val apiInstance = AdminApi()
val mode : kotlin.String = mode_example // kotlin.String | Response mode
try {
    val result : Location = apiInstance.restAdminLocationsGet(mode)
    println(result)
} catch (e: ClientException) {
    println("4xx response calling AdminApi#restAdminLocationsGet")
    e.printStackTrace()
} catch (e: ServerException) {
    println("5xx response calling AdminApi#restAdminLocationsGet")
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

<a id="restAdminLocationsIdDelete"></a>
# **restAdminLocationsIdDelete**
> restAdminLocationsIdDelete(id)

Delete a location.

Delete the specified location.

### Example
```kotlin
// Import classes:
//import org.openapitools.client.infrastructure.*
//import org.openapitools.client.models.*

val apiInstance = AdminApi()
val id : kotlin.Int = 56 // kotlin.Int | ID of the location to remove from
try {
    apiInstance.restAdminLocationsIdDelete(id)
} catch (e: ClientException) {
    println("4xx response calling AdminApi#restAdminLocationsIdDelete")
    e.printStackTrace()
} catch (e: ServerException) {
    println("5xx response calling AdminApi#restAdminLocationsIdDelete")
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

<a id="restAdminLocationsIdGet"></a>
# **restAdminLocationsIdGet**
> Location restAdminLocationsIdGet(id)

Return location name.

Returns the name of a specified location.

### Example
```kotlin
// Import classes:
//import org.openapitools.client.infrastructure.*
//import org.openapitools.client.models.*

val apiInstance = AdminApi()
val id : kotlin.Int = 56 // kotlin.Int | ID of the location to be retrieved
try {
    val result : Location = apiInstance.restAdminLocationsIdGet(id)
    println(result)
} catch (e: ClientException) {
    println("4xx response calling AdminApi#restAdminLocationsIdGet")
    e.printStackTrace()
} catch (e: ServerException) {
    println("5xx response calling AdminApi#restAdminLocationsIdGet")
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

<a id="restAdminLocationsPost"></a>
# **restAdminLocationsPost**
> restAdminLocationsPost(body, returnEntity, mode)

Create a location entry.

Creates a location entry by providing a name.

### Example
```kotlin
// Import classes:
//import org.openapitools.client.infrastructure.*
//import org.openapitools.client.models.*

val apiInstance = AdminApi()
val body : LocationPost =  // LocationPost | The location details
val returnEntity : kotlin.Boolean = true // kotlin.Boolean | Return information about newly created entity
val mode : kotlin.String = mode_example // kotlin.String | Response mode
try {
    apiInstance.restAdminLocationsPost(body, returnEntity, mode)
} catch (e: ClientException) {
    println("4xx response calling AdminApi#restAdminLocationsPost")
    e.printStackTrace()
} catch (e: ServerException) {
    println("5xx response calling AdminApi#restAdminLocationsPost")
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

<a id="restAdminMailActionsWithdrawFilesUsersUserIdDelete"></a>
# **restAdminMailActionsWithdrawFilesUsersUserIdDelete**
> restAdminMailActionsWithdrawFilesUsersUserIdDelete(userId, emailIdColonIn, partialSuccess, mode)

Withdraw all files from deleted/demoted users&#39; emails

Withdraw all files from deleted/demoted users&#39; emails

### Example
```kotlin
// Import classes:
//import org.openapitools.client.infrastructure.*
//import org.openapitools.client.models.*

val apiInstance = AdminApi()
val userId : kotlin.String = userId_example // kotlin.String | ID of the user to withdraw files
val emailIdColonIn : kotlin.String = emailIdColonIn_example // kotlin.String | A list of email ids which will be processed
val partialSuccess : kotlin.Boolean = true // kotlin.Boolean | Whether to perform action on valid items even if some ones fail
val mode : kotlin.String = mode_example // kotlin.String | Response mode
try {
    apiInstance.restAdminMailActionsWithdrawFilesUsersUserIdDelete(userId, emailIdColonIn, partialSuccess, mode)
} catch (e: ClientException) {
    println("4xx response calling AdminApi#restAdminMailActionsWithdrawFilesUsersUserIdDelete")
    e.printStackTrace()
} catch (e: ServerException) {
    println("5xx response calling AdminApi#restAdminMailActionsWithdrawFilesUsersUserIdDelete")
    e.printStackTrace()
}
```

### Parameters

Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **userId** | **kotlin.String**| ID of the user to withdraw files |
 **emailIdColonIn** | **kotlin.String**| A list of email ids which will be processed | [optional]
 **partialSuccess** | **kotlin.Boolean**| Whether to perform action on valid items even if some ones fail | [optional]
 **mode** | **kotlin.String**| Response mode | [optional]

### Return type

null (empty response body)

### Authorization

No authorization required

### HTTP request headers

 - **Content-Type**: Not defined
 - **Accept**: Not defined

<a id="restAdminMailGet"></a>
# **restAdminMailGet**
> kotlin.collections.List&lt;Email&gt; restAdminMailGet(senderId, senderIdColonIn, date, dateColonGt, dateColonGte, dateColonLt, dateColonLte, modifiedDate, modifiedDateColonGt, modifiedDateColonGte, modifiedDateColonLt, modifiedDateColonLte, deleted, emailPackageId, emailPackageIdColonIn, templateId, templateIdColonIn, status, isPreview, isUserSent, webFormId, webFormIdColonContains, orderBy, offset, limit)

List emails

Returns the list of all emails for this user.     This includes sent emails, received emails, draft emails, and request a file emails.

### Example
```kotlin
// Import classes:
//import org.openapitools.client.infrastructure.*
//import org.openapitools.client.models.*

val apiInstance = AdminApi()
val senderId : kotlin.String = senderId_example // kotlin.String | Unique identifier of User who sent Email
val senderIdColonIn : kotlin.String = senderIdColonIn_example // kotlin.String | Unique identifier of User who sent Email. Search for results that contain any of specified values of this parameter.
val date : java.time.LocalDate = 2013-10-20 // java.time.LocalDate | Email creation date
val dateColonGt : java.time.LocalDate = 2013-10-20 // java.time.LocalDate | Email creation date. Search for result that has this parameter value greater than specified.
val dateColonGte : java.time.LocalDate = 2013-10-20 // java.time.LocalDate | Email creation date. Search for result that has this parameter value greater or equal to the specified.
val dateColonLt : java.time.LocalDate = 2013-10-20 // java.time.LocalDate | Email creation date. Search for result that has this parameter value less than specified.
val dateColonLte : java.time.LocalDate = 2013-10-20 // java.time.LocalDate | Email creation date. Search for result that has this parameter value less or equal to the specified.
val modifiedDate : java.time.LocalDate = 2013-10-20 // java.time.LocalDate | Email modification date
val modifiedDateColonGt : java.time.LocalDate = 2013-10-20 // java.time.LocalDate | Email modification date. Search for result that has this parameter value greater than specified.
val modifiedDateColonGte : java.time.LocalDate = 2013-10-20 // java.time.LocalDate | Email modification date. Search for result that has this parameter value greater or equal to the specified.
val modifiedDateColonLt : java.time.LocalDate = 2013-10-20 // java.time.LocalDate | Email modification date. Search for result that has this parameter value less than specified.
val modifiedDateColonLte : java.time.LocalDate = 2013-10-20 // java.time.LocalDate | Email modification date. Search for result that has this parameter value less or equal to the specified.
val deleted : kotlin.Boolean = true // kotlin.Boolean | Indicates that Email is deleted
val emailPackageId : kotlin.String = emailPackageId_example // kotlin.String | Email Package unique identifier
val emailPackageIdColonIn : kotlin.String = emailPackageIdColonIn_example // kotlin.String | Email Package unique identifier. Search for results that contain any of specified values of this parameter.
val templateId : kotlin.Int = 56 // kotlin.Int | Email Template unique identifier
val templateIdColonIn : kotlin.Int = 56 // kotlin.Int | Email Template unique identifier. Search for results that contain any of specified values of this parameter.
val status : kotlin.collections.List<kotlin.String> =  // kotlin.collections.List<kotlin.String> | Email status
val isPreview : kotlin.Boolean = true // kotlin.Boolean | Whether the email is a preview email
val isUserSent : kotlin.Boolean = true // kotlin.Boolean | Whether the email was sent by some user
val webFormId : kotlin.String = webFormId_example // kotlin.String | Email web form ID
val webFormIdColonContains : kotlin.String = webFormIdColonContains_example // kotlin.String | Email web form ID. Search for result that contains specified characters in this parameter.
val orderBy : kotlin.collections.List<kotlin.String> =  // kotlin.collections.List<kotlin.String> | Sorting options
val offset : kotlin.Int = 56 // kotlin.Int | Offset
val limit : kotlin.Int = 56 // kotlin.Int | Limit
try {
    val result : kotlin.collections.List<Email> = apiInstance.restAdminMailGet(senderId, senderIdColonIn, date, dateColonGt, dateColonGte, dateColonLt, dateColonLte, modifiedDate, modifiedDateColonGt, modifiedDateColonGte, modifiedDateColonLt, modifiedDateColonLte, deleted, emailPackageId, emailPackageIdColonIn, templateId, templateIdColonIn, status, isPreview, isUserSent, webFormId, webFormIdColonContains, orderBy, offset, limit)
    println(result)
} catch (e: ClientException) {
    println("4xx response calling AdminApi#restAdminMailGet")
    e.printStackTrace()
} catch (e: ServerException) {
    println("5xx response calling AdminApi#restAdminMailGet")
    e.printStackTrace()
}
```

### Parameters

Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **senderId** | **kotlin.String**| Unique identifier of User who sent Email | [optional]
 **senderIdColonIn** | **kotlin.String**| Unique identifier of User who sent Email. Search for results that contain any of specified values of this parameter. | [optional]
 **date** | **java.time.LocalDate**| Email creation date | [optional]
 **dateColonGt** | **java.time.LocalDate**| Email creation date. Search for result that has this parameter value greater than specified. | [optional]
 **dateColonGte** | **java.time.LocalDate**| Email creation date. Search for result that has this parameter value greater or equal to the specified. | [optional]
 **dateColonLt** | **java.time.LocalDate**| Email creation date. Search for result that has this parameter value less than specified. | [optional]
 **dateColonLte** | **java.time.LocalDate**| Email creation date. Search for result that has this parameter value less or equal to the specified. | [optional]
 **modifiedDate** | **java.time.LocalDate**| Email modification date | [optional]
 **modifiedDateColonGt** | **java.time.LocalDate**| Email modification date. Search for result that has this parameter value greater than specified. | [optional]
 **modifiedDateColonGte** | **java.time.LocalDate**| Email modification date. Search for result that has this parameter value greater or equal to the specified. | [optional]
 **modifiedDateColonLt** | **java.time.LocalDate**| Email modification date. Search for result that has this parameter value less than specified. | [optional]
 **modifiedDateColonLte** | **java.time.LocalDate**| Email modification date. Search for result that has this parameter value less or equal to the specified. | [optional]
 **deleted** | **kotlin.Boolean**| Indicates that Email is deleted | [optional]
 **emailPackageId** | **kotlin.String**| Email Package unique identifier | [optional]
 **emailPackageIdColonIn** | **kotlin.String**| Email Package unique identifier. Search for results that contain any of specified values of this parameter. | [optional]
 **templateId** | **kotlin.Int**| Email Template unique identifier | [optional]
 **templateIdColonIn** | **kotlin.Int**| Email Template unique identifier. Search for results that contain any of specified values of this parameter. | [optional]
 **status** | [**kotlin.collections.List&lt;kotlin.String&gt;**](kotlin.String.md)| Email status | [optional]
 **isPreview** | **kotlin.Boolean**| Whether the email is a preview email | [optional]
 **isUserSent** | **kotlin.Boolean**| Whether the email was sent by some user | [optional]
 **webFormId** | **kotlin.String**| Email web form ID | [optional]
 **webFormIdColonContains** | **kotlin.String**| Email web form ID. Search for result that contains specified characters in this parameter. | [optional]
 **orderBy** | [**kotlin.collections.List&lt;kotlin.String&gt;**](kotlin.String.md)| Sorting options | [optional]
 **offset** | **kotlin.Int**| Offset | [optional]
 **limit** | **kotlin.Int**| Limit | [optional]

### Return type

[**kotlin.collections.List&lt;Email&gt;**](Email.md)

### Authorization

No authorization required

### HTTP request headers

 - **Content-Type**: Not defined
 - **Accept**: */*

<a id="restAdminProfilesGet"></a>
# **restAdminProfilesGet**
> kotlin.collections.List&lt;Profile&gt; restAdminProfilesGet(name, nameColonContains, orderBy, offset, limit, with, mode)

List user types

Returns a list of user types supported by kiteworks. e.g.:     Today we return Standard and Restricted

### Example
```kotlin
// Import classes:
//import org.openapitools.client.infrastructure.*
//import org.openapitools.client.models.*

val apiInstance = AdminApi()
val name : kotlin.String = name_example // kotlin.String | Profile name
val nameColonContains : kotlin.String = nameColonContains_example // kotlin.String | Profile name. Search for result that contains specified characters in this parameter.
val orderBy : kotlin.collections.List<kotlin.String> =  // kotlin.collections.List<kotlin.String> | Sorting options
val offset : kotlin.Int = 56 // kotlin.Int | Offset
val limit : kotlin.Int = 56 // kotlin.Int | Limit
val with : kotlin.String = with_example // kotlin.String | With parameters
val mode : kotlin.String = mode_example // kotlin.String | Response mode
try {
    val result : kotlin.collections.List<Profile> = apiInstance.restAdminProfilesGet(name, nameColonContains, orderBy, offset, limit, with, mode)
    println(result)
} catch (e: ClientException) {
    println("4xx response calling AdminApi#restAdminProfilesGet")
    e.printStackTrace()
} catch (e: ServerException) {
    println("5xx response calling AdminApi#restAdminProfilesGet")
    e.printStackTrace()
}
```

### Parameters

Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **name** | **kotlin.String**| Profile name | [optional]
 **nameColonContains** | **kotlin.String**| Profile name. Search for result that contains specified characters in this parameter. | [optional]
 **orderBy** | [**kotlin.collections.List&lt;kotlin.String&gt;**](kotlin.String.md)| Sorting options | [optional]
 **offset** | **kotlin.Int**| Offset | [optional]
 **limit** | **kotlin.Int**| Limit | [optional]
 **with** | **kotlin.String**| With parameters | [optional]
 **mode** | **kotlin.String**| Response mode | [optional]

### Return type

[**kotlin.collections.List&lt;Profile&gt;**](Profile.md)

### Authorization

No authorization required

### HTTP request headers

 - **Content-Type**: Not defined
 - **Accept**: */*

<a id="restAdminProfilesIdGet"></a>
# **restAdminProfilesIdGet**
> kotlin.collections.List&lt;Profile&gt; restAdminProfilesIdGet(id)

Return an user type

Returns the details of a specified user type. e.g.: Returns user type id and name.

### Example
```kotlin
// Import classes:
//import org.openapitools.client.infrastructure.*
//import org.openapitools.client.models.*

val apiInstance = AdminApi()
val id : kotlin.Int = 56 // kotlin.Int | ID of the user type to be retrieved
try {
    val result : kotlin.collections.List<Profile> = apiInstance.restAdminProfilesIdGet(id)
    println(result)
} catch (e: ClientException) {
    println("4xx response calling AdminApi#restAdminProfilesIdGet")
    e.printStackTrace()
} catch (e: ServerException) {
    println("5xx response calling AdminApi#restAdminProfilesIdGet")
    e.printStackTrace()
}
```

### Parameters

Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **id** | **kotlin.Int**| ID of the user type to be retrieved |

### Return type

[**kotlin.collections.List&lt;Profile&gt;**](Profile.md)

### Authorization

No authorization required

### HTTP request headers

 - **Content-Type**: Not defined
 - **Accept**: */*

<a id="restAdminProfilesIdMappingsGet"></a>
# **restAdminProfilesIdMappingsGet**
> ProfileMappings restAdminProfilesIdMappingsGet(id)

Get profile mapping details

Get profile mapping details for user profile

### Example
```kotlin
// Import classes:
//import org.openapitools.client.infrastructure.*
//import org.openapitools.client.models.*

val apiInstance = AdminApi()
val id : kotlin.Int = 56 // kotlin.Int | Id of the profile to get mapping details for
try {
    val result : ProfileMappings = apiInstance.restAdminProfilesIdMappingsGet(id)
    println(result)
} catch (e: ClientException) {
    println("4xx response calling AdminApi#restAdminProfilesIdMappingsGet")
    e.printStackTrace()
} catch (e: ServerException) {
    println("5xx response calling AdminApi#restAdminProfilesIdMappingsGet")
    e.printStackTrace()
}
```

### Parameters

Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **id** | **kotlin.Int**| Id of the profile to get mapping details for |

### Return type

[**ProfileMappings**](ProfileMappings.md)

### Authorization

No authorization required

### HTTP request headers

 - **Content-Type**: Not defined
 - **Accept**: */*

<a id="restAdminProfilesIdMappingsPut"></a>
# **restAdminProfilesIdMappingsPut**
> restAdminProfilesIdMappingsPut(id, body, with, mode)

Update profile mapping details

Update profile mapping details for user profile

### Example
```kotlin
// Import classes:
//import org.openapitools.client.infrastructure.*
//import org.openapitools.client.models.*

val apiInstance = AdminApi()
val id : kotlin.Int = 56 // kotlin.Int | Id of the profile to get mapping details for
val body : ProfileMappingChangesPut =  // ProfileMappingChangesPut | Profile mapping details
val with : kotlin.String = with_example // kotlin.String | With parameters
val mode : kotlin.String = mode_example // kotlin.String | Response mode
try {
    apiInstance.restAdminProfilesIdMappingsPut(id, body, with, mode)
} catch (e: ClientException) {
    println("4xx response calling AdminApi#restAdminProfilesIdMappingsPut")
    e.printStackTrace()
} catch (e: ServerException) {
    println("5xx response calling AdminApi#restAdminProfilesIdMappingsPut")
    e.printStackTrace()
}
```

### Parameters

Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **id** | **kotlin.Int**| Id of the profile to get mapping details for |
 **body** | [**ProfileMappingChangesPut**](ProfileMappingChangesPut.md)| Profile mapping details |
 **with** | **kotlin.String**| With parameters | [optional]
 **mode** | **kotlin.String**| Response mode | [optional]

### Return type

null (empty response body)

### Authorization

No authorization required

### HTTP request headers

 - **Content-Type**: Not defined
 - **Accept**: Not defined

<a id="restAdminProfilesIdUsersGet"></a>
# **restAdminProfilesIdUsersGet**
> kotlin.collections.List&lt;User&gt; restAdminProfilesIdUsersGet(id, email, emailColonContains, name, nameColonContains, metadata, metadataContains, deleted, active, verified, suspended, isRecipient, allowsCollaboration, created, createdColonGt, createdColonGte, createdColonLt, createdColonLte, orderBy, offset, limit, locateId, with, mode)

Return list of users with the specified types

Returns the list of users who have the specified type.     e.g.: Return me the user names and email addresses of all the Restricted Users.

### Example
```kotlin
// Import classes:
//import org.openapitools.client.infrastructure.*
//import org.openapitools.client.models.*

val apiInstance = AdminApi()
val id : kotlin.Int = 56 // kotlin.Int | ID of the user type to retrieve users for
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
    val result : kotlin.collections.List<User> = apiInstance.restAdminProfilesIdUsersGet(id, email, emailColonContains, name, nameColonContains, metadata, metadataContains, deleted, active, verified, suspended, isRecipient, allowsCollaboration, created, createdColonGt, createdColonGte, createdColonLt, createdColonLte, orderBy, offset, limit, locateId, with, mode)
    println(result)
} catch (e: ClientException) {
    println("4xx response calling AdminApi#restAdminProfilesIdUsersGet")
    e.printStackTrace()
} catch (e: ServerException) {
    println("5xx response calling AdminApi#restAdminProfilesIdUsersGet")
    e.printStackTrace()
}
```

### Parameters

Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **id** | **kotlin.Int**| ID of the user type to retrieve users for |
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

<a id="restAdminProfilesIdUsersPut"></a>
# **restAdminProfilesIdUsersPut**
> restAdminProfilesIdUsersPut(id, idColonIn, mode, body)

Change user type

Change user type for specified user

### Example
```kotlin
// Import classes:
//import org.openapitools.client.infrastructure.*
//import org.openapitools.client.models.*

val apiInstance = AdminApi()
val id : kotlin.Int = 56 // kotlin.Int | ID of the user type
val idColonIn : kotlin.String = idColonIn_example // kotlin.String | IDs of users, who are going to be assigned to the user type
val mode : kotlin.String = mode_example // kotlin.String | Response mode
val body : UserDemoteOptionsPost =  // UserDemoteOptionsPost | The users details
try {
    apiInstance.restAdminProfilesIdUsersPut(id, idColonIn, mode, body)
} catch (e: ClientException) {
    println("4xx response calling AdminApi#restAdminProfilesIdUsersPut")
    e.printStackTrace()
} catch (e: ServerException) {
    println("5xx response calling AdminApi#restAdminProfilesIdUsersPut")
    e.printStackTrace()
}
```

### Parameters

Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **id** | **kotlin.Int**| ID of the user type |
 **idColonIn** | **kotlin.String**| IDs of users, who are going to be assigned to the user type |
 **mode** | **kotlin.String**| Response mode | [optional]
 **body** | [**UserDemoteOptionsPost**](UserDemoteOptionsPost.md)| The users details | [optional]

### Return type

null (empty response body)

### Authorization

No authorization required

### HTTP request headers

 - **Content-Type**: Not defined
 - **Accept**: Not defined

<a id="restAdminProfilesMappingOrderGet"></a>
# **restAdminProfilesMappingOrderGet**
> ProfileMappingOrder restAdminProfilesMappingOrderGet()

Get profile mapping order

Get profile mapping order that determines application of filters on login

### Example
```kotlin
// Import classes:
//import org.openapitools.client.infrastructure.*
//import org.openapitools.client.models.*

val apiInstance = AdminApi()
try {
    val result : ProfileMappingOrder = apiInstance.restAdminProfilesMappingOrderGet()
    println(result)
} catch (e: ClientException) {
    println("4xx response calling AdminApi#restAdminProfilesMappingOrderGet")
    e.printStackTrace()
} catch (e: ServerException) {
    println("5xx response calling AdminApi#restAdminProfilesMappingOrderGet")
    e.printStackTrace()
}
```

### Parameters
This endpoint does not need any parameter.

### Return type

[**ProfileMappingOrder**](ProfileMappingOrder.md)

### Authorization

No authorization required

### HTTP request headers

 - **Content-Type**: Not defined
 - **Accept**: */*

<a id="restAdminProfilesMappingOrderPut"></a>
# **restAdminProfilesMappingOrderPut**
> restAdminProfilesMappingOrderPut(body, with, mode)

Update profile mapping order

Update profile mapping order that determines application of filters on login

### Example
```kotlin
// Import classes:
//import org.openapitools.client.infrastructure.*
//import org.openapitools.client.models.*

val apiInstance = AdminApi()
val body : ProfileMappingOrderPut =  // ProfileMappingOrderPut | profile ordering
val with : kotlin.String = with_example // kotlin.String | With parameters
val mode : kotlin.String = mode_example // kotlin.String | Response mode
try {
    apiInstance.restAdminProfilesMappingOrderPut(body, with, mode)
} catch (e: ClientException) {
    println("4xx response calling AdminApi#restAdminProfilesMappingOrderPut")
    e.printStackTrace()
} catch (e: ServerException) {
    println("5xx response calling AdminApi#restAdminProfilesMappingOrderPut")
    e.printStackTrace()
}
```

### Parameters

Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **body** | [**ProfileMappingOrderPut**](ProfileMappingOrderPut.md)| profile ordering |
 **with** | **kotlin.String**| With parameters | [optional]
 **mode** | **kotlin.String**| Response mode | [optional]

### Return type

null (empty response body)

### Authorization

No authorization required

### HTTP request headers

 - **Content-Type**: Not defined
 - **Accept**: Not defined

<a id="restAdminProfilesMappingsGet"></a>
# **restAdminProfilesMappingsGet**
> ProfileMappingsTest restAdminProfilesMappingsGet(user)

Get profile mapping results for user

Get profile mapping results for user

### Example
```kotlin
// Import classes:
//import org.openapitools.client.infrastructure.*
//import org.openapitools.client.models.*

val apiInstance = AdminApi()
val user : kotlin.String = user_example // kotlin.String | User to test mappings for
try {
    val result : ProfileMappingsTest = apiInstance.restAdminProfilesMappingsGet(user)
    println(result)
} catch (e: ClientException) {
    println("4xx response calling AdminApi#restAdminProfilesMappingsGet")
    e.printStackTrace()
} catch (e: ServerException) {
    println("5xx response calling AdminApi#restAdminProfilesMappingsGet")
    e.printStackTrace()
}
```

### Parameters

Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **user** | **kotlin.String**| User to test mappings for |

### Return type

[**ProfileMappingsTest**](ProfileMappingsTest.md)

### Authorization

No authorization required

### HTTP request headers

 - **Content-Type**: Not defined
 - **Accept**: */*

<a id="restAdminRequestFileUsersUserIdDelete"></a>
# **restAdminRequestFileUsersUserIdDelete**
> RequestFile restAdminRequestFileUsersUserIdDelete(userId, requestFileIdColonIn, mode)

Delete request files sent by the the specified user

Delete request files sent by the the specified user

### Example
```kotlin
// Import classes:
//import org.openapitools.client.infrastructure.*
//import org.openapitools.client.models.*

val apiInstance = AdminApi()
val userId : kotlin.String = userId_example // kotlin.String | The user ID of request file
val requestFileIdColonIn : kotlin.Int = 56 // kotlin.Int | Search for results that contain any of specified values of this parameter.
val mode : kotlin.String = mode_example // kotlin.String | Response mode
try {
    val result : RequestFile = apiInstance.restAdminRequestFileUsersUserIdDelete(userId, requestFileIdColonIn, mode)
    println(result)
} catch (e: ClientException) {
    println("4xx response calling AdminApi#restAdminRequestFileUsersUserIdDelete")
    e.printStackTrace()
} catch (e: ServerException) {
    println("5xx response calling AdminApi#restAdminRequestFileUsersUserIdDelete")
    e.printStackTrace()
}
```

### Parameters

Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **userId** | **kotlin.String**| The user ID of request file |
 **requestFileIdColonIn** | **kotlin.Int**| Search for results that contain any of specified values of this parameter. | [optional]
 **mode** | **kotlin.String**| Response mode | [optional]

### Return type

[**RequestFile**](RequestFile.md)

### Authorization

No authorization required

### HTTP request headers

 - **Content-Type**: Not defined
 - **Accept**: */*

<a id="restAdminSourcesGet"></a>
# **restAdminSourcesGet**
> kotlin.collections.List&lt;Source&gt; restAdminSourcesGet(includeKw, with, mode)

List all added sources

Returns a list of all available ECM sources.

### Example
```kotlin
// Import classes:
//import org.openapitools.client.infrastructure.*
//import org.openapitools.client.models.*

val apiInstance = AdminApi()
val includeKw : kotlin.Boolean = true // kotlin.Boolean | Include KW
val with : kotlin.String = with_example // kotlin.String | With parameters
val mode : kotlin.String = mode_example // kotlin.String | Response mode
try {
    val result : kotlin.collections.List<Source> = apiInstance.restAdminSourcesGet(includeKw, with, mode)
    println(result)
} catch (e: ClientException) {
    println("4xx response calling AdminApi#restAdminSourcesGet")
    e.printStackTrace()
} catch (e: ServerException) {
    println("5xx response calling AdminApi#restAdminSourcesGet")
    e.printStackTrace()
}
```

### Parameters

Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **includeKw** | **kotlin.Boolean**| Include KW | [optional]
 **with** | **kotlin.String**| With parameters | [optional]
 **mode** | **kotlin.String**| Response mode | [optional]

### Return type

[**kotlin.collections.List&lt;Source&gt;**](Source.md)

### Authorization

No authorization required

### HTTP request headers

 - **Content-Type**: Not defined
 - **Accept**: */*

<a id="restAdminSourcesIdDelete"></a>
# **restAdminSourcesIdDelete**
> restAdminSourcesIdDelete(id)

Deletes specified assigned source

Deletes specified assigned source.

### Example
```kotlin
// Import classes:
//import org.openapitools.client.infrastructure.*
//import org.openapitools.client.models.*

val apiInstance = AdminApi()
val id : kotlin.String = id_example // kotlin.String | ID of the assigned source to be deleted.
try {
    apiInstance.restAdminSourcesIdDelete(id)
} catch (e: ClientException) {
    println("4xx response calling AdminApi#restAdminSourcesIdDelete")
    e.printStackTrace()
} catch (e: ServerException) {
    println("5xx response calling AdminApi#restAdminSourcesIdDelete")
    e.printStackTrace()
}
```

### Parameters

Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **id** | **kotlin.String**| ID of the assigned source to be deleted. |

### Return type

null (empty response body)

### Authorization

No authorization required

### HTTP request headers

 - **Content-Type**: Not defined
 - **Accept**: Not defined

<a id="restAdminSourcesIdGet"></a>
# **restAdminSourcesIdGet**
> Source restAdminSourcesIdGet(id)

Returns requested assigned ECM source

Returns requested assigned source.

### Example
```kotlin
// Import classes:
//import org.openapitools.client.infrastructure.*
//import org.openapitools.client.models.*

val apiInstance = AdminApi()
val id : kotlin.String = id_example // kotlin.String | ID of the assigned source to be retrieved
try {
    val result : Source = apiInstance.restAdminSourcesIdGet(id)
    println(result)
} catch (e: ClientException) {
    println("4xx response calling AdminApi#restAdminSourcesIdGet")
    e.printStackTrace()
} catch (e: ServerException) {
    println("5xx response calling AdminApi#restAdminSourcesIdGet")
    e.printStackTrace()
}
```

### Parameters

Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **id** | **kotlin.String**| ID of the assigned source to be retrieved |

### Return type

[**Source**](Source.md)

### Authorization

No authorization required

### HTTP request headers

 - **Content-Type**: Not defined
 - **Accept**: */*

<a id="restAdminSourcesIdPut"></a>
# **restAdminSourcesIdPut**
> restAdminSourcesIdPut(id, body)

Updates details of the specified ECM source

Updates requested source.

### Example
```kotlin
// Import classes:
//import org.openapitools.client.infrastructure.*
//import org.openapitools.client.models.*

val apiInstance = AdminApi()
val id : kotlin.String = id_example // kotlin.String | ID of the source to update
val body : SourcePut =  // SourcePut | source details
try {
    apiInstance.restAdminSourcesIdPut(id, body)
} catch (e: ClientException) {
    println("4xx response calling AdminApi#restAdminSourcesIdPut")
    e.printStackTrace()
} catch (e: ServerException) {
    println("5xx response calling AdminApi#restAdminSourcesIdPut")
    e.printStackTrace()
}
```

### Parameters

Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **id** | **kotlin.String**| ID of the source to update |
 **body** | [**SourcePut**](SourcePut.md)| source details |

### Return type

null (empty response body)

### Authorization

No authorization required

### HTTP request headers

 - **Content-Type**: Not defined
 - **Accept**: Not defined

<a id="restAdminSourcesPost"></a>
# **restAdminSourcesPost**
> restAdminSourcesPost(body, returnEntity, mode)

Add assigned ECM source

Add assigned source.

### Example
```kotlin
// Import classes:
//import org.openapitools.client.infrastructure.*
//import org.openapitools.client.models.*

val apiInstance = AdminApi()
val body : SourcePost =  // SourcePost | source details
val returnEntity : kotlin.Boolean = true // kotlin.Boolean | Return information about newly created entity
val mode : kotlin.String = mode_example // kotlin.String | Response mode
try {
    apiInstance.restAdminSourcesPost(body, returnEntity, mode)
} catch (e: ClientException) {
    println("4xx response calling AdminApi#restAdminSourcesPost")
    e.printStackTrace()
} catch (e: ServerException) {
    println("5xx response calling AdminApi#restAdminSourcesPost")
    e.printStackTrace()
}
```

### Parameters

Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **body** | [**SourcePost**](SourcePost.md)| source details |
 **returnEntity** | **kotlin.Boolean**| Return information about newly created entity | [optional]
 **mode** | **kotlin.String**| Response mode | [optional]

### Return type

null (empty response body)

### Authorization

No authorization required

### HTTP request headers

 - **Content-Type**: Not defined
 - **Accept**: Not defined

<a id="restAdminUsersGet"></a>
# **restAdminUsersGet**
> RestAdminUsersGet200Response restAdminUsersGet(email, emailColonContains, name, nameColonContains, metadata, metadataContains, deleted, active, verified, suspended, isRecipient, allowsCollaboration, created, createdColonGt, createdColonGte, createdColonLt, createdColonLte, orderBy, offset, limit, locateId, with, mode)

Get a list of Users

Returns a list of Users in the system.     This call will only work for users with admin access.

### Example
```kotlin
// Import classes:
//import org.openapitools.client.infrastructure.*
//import org.openapitools.client.models.*

val apiInstance = AdminApi()
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
    val result : RestAdminUsersGet200Response = apiInstance.restAdminUsersGet(email, emailColonContains, name, nameColonContains, metadata, metadataContains, deleted, active, verified, suspended, isRecipient, allowsCollaboration, created, createdColonGt, createdColonGte, createdColonLt, createdColonLte, orderBy, offset, limit, locateId, with, mode)
    println(result)
} catch (e: ClientException) {
    println("4xx response calling AdminApi#restAdminUsersGet")
    e.printStackTrace()
} catch (e: ServerException) {
    println("5xx response calling AdminApi#restAdminUsersGet")
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

[**RestAdminUsersGet200Response**](RestAdminUsersGet200Response.md)

### Authorization

No authorization required

### HTTP request headers

 - **Content-Type**: Not defined
 - **Accept**: */*

<a id="restAdminUsersIdAdminRolesGet"></a>
# **restAdminUsersIdAdminRolesGet**
> kotlin.collections.List&lt;AdminRole&gt; restAdminUsersIdAdminRolesGet(id, orderBy, with, mode)

Return admin roles of the specified user id.

Returns the details of all adminroles (active and deleted users)     with the specified user id.

### Example
```kotlin
// Import classes:
//import org.openapitools.client.infrastructure.*
//import org.openapitools.client.models.*

val apiInstance = AdminApi()
val id : kotlin.String = id_example // kotlin.String | ID of the user to retrieve admin role
val orderBy : kotlin.collections.List<kotlin.String> =  // kotlin.collections.List<kotlin.String> | Sorting options
val with : kotlin.String = with_example // kotlin.String | With parameters
val mode : kotlin.String = mode_example // kotlin.String | Response mode
try {
    val result : kotlin.collections.List<AdminRole> = apiInstance.restAdminUsersIdAdminRolesGet(id, orderBy, with, mode)
    println(result)
} catch (e: ClientException) {
    println("4xx response calling AdminApi#restAdminUsersIdAdminRolesGet")
    e.printStackTrace()
} catch (e: ServerException) {
    println("5xx response calling AdminApi#restAdminUsersIdAdminRolesGet")
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

<a id="restAdminUsersIdDelete"></a>
# **restAdminUsersIdDelete**
> restAdminUsersIdDelete(id, retainToUser, remoteWipe, deleteUnsharedData, retainData, retainPermissionToSharedData, withdrawFileLinks, withdrawRequestFiles, partialSuccess, mode)

Deletes a User

Mark the specified user as deleted. This user will still be returned in the GET Users query.

### Example
```kotlin
// Import classes:
//import org.openapitools.client.infrastructure.*
//import org.openapitools.client.models.*

val apiInstance = AdminApi()
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
    apiInstance.restAdminUsersIdDelete(id, retainToUser, remoteWipe, deleteUnsharedData, retainData, retainPermissionToSharedData, withdrawFileLinks, withdrawRequestFiles, partialSuccess, mode)
} catch (e: ClientException) {
    println("4xx response calling AdminApi#restAdminUsersIdDelete")
    e.printStackTrace()
} catch (e: ServerException) {
    println("5xx response calling AdminApi#restAdminUsersIdDelete")
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

<a id="restAdminUsersIdDevicesGet"></a>
# **restAdminUsersIdDevicesGet**
> kotlin.collections.List&lt;Device&gt; restAdminUsersIdDevicesGet(id, installTagId, installTagIdColonContains, userId, userIdColonIn, clientId, clientIdColonContains, orderBy, offset, limit, with, mode)

List devices for a user

Return a list of devices for a specific user

### Example
```kotlin
// Import classes:
//import org.openapitools.client.infrastructure.*
//import org.openapitools.client.models.*

val apiInstance = AdminApi()
val id : kotlin.String = id_example // kotlin.String | ID of the user whose devices to be retrieved
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
    val result : kotlin.collections.List<Device> = apiInstance.restAdminUsersIdDevicesGet(id, installTagId, installTagIdColonContains, userId, userIdColonIn, clientId, clientIdColonContains, orderBy, offset, limit, with, mode)
    println(result)
} catch (e: ClientException) {
    println("4xx response calling AdminApi#restAdminUsersIdDevicesGet")
    e.printStackTrace()
} catch (e: ServerException) {
    println("5xx response calling AdminApi#restAdminUsersIdDevicesGet")
    e.printStackTrace()
}
```

### Parameters

Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **id** | **kotlin.String**| ID of the user whose devices to be retrieved |
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

<a id="restAdminUsersIdGet"></a>
# **restAdminUsersIdGet**
> User restAdminUsersIdGet(id)

Get User

Returns the details of the specified user (this includes email address and name)

### Example
```kotlin
// Import classes:
//import org.openapitools.client.infrastructure.*
//import org.openapitools.client.models.*

val apiInstance = AdminApi()
val id : kotlin.String = id_example // kotlin.String | ID of the user to retrieve
try {
    val result : User = apiInstance.restAdminUsersIdGet(id)
    println(result)
} catch (e: ClientException) {
    println("4xx response calling AdminApi#restAdminUsersIdGet")
    e.printStackTrace()
} catch (e: ServerException) {
    println("5xx response calling AdminApi#restAdminUsersIdGet")
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

<a id="restAdminUsersIdPut"></a>
# **restAdminUsersIdPut**
> restAdminUsersIdPut(id, body)

Update User

Updates the details of a user.     e.g.: Change their name, set as deleted, set as active or inactive, etc.

### Example
```kotlin
// Import classes:
//import org.openapitools.client.infrastructure.*
//import org.openapitools.client.models.*

val apiInstance = AdminApi()
val id : kotlin.String = id_example // kotlin.String | ID of the user to update
val body : UserPut =  // UserPut | The user details
try {
    apiInstance.restAdminUsersIdPut(id, body)
} catch (e: ClientException) {
    println("4xx response calling AdminApi#restAdminUsersIdPut")
    e.printStackTrace()
} catch (e: ServerException) {
    println("5xx response calling AdminApi#restAdminUsersIdPut")
    e.printStackTrace()
}
```

### Parameters

Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **id** | **kotlin.String**| ID of the user to update |
 **body** | [**UserPut**](UserPut.md)| The user details |

### Return type

null (empty response body)

### Authorization

No authorization required

### HTTP request headers

 - **Content-Type**: Not defined
 - **Accept**: Not defined

<a id="restAdminUsersIdSettingsGet"></a>
# **restAdminUsersIdSettingsGet**
> Settings restAdminUsersIdSettingsGet(id)

Get User Settings

Returns the user settings

### Example
```kotlin
// Import classes:
//import org.openapitools.client.infrastructure.*
//import org.openapitools.client.models.*

val apiInstance = AdminApi()
val id : kotlin.String = id_example // kotlin.String | ID of the user to retrieve settings for
try {
    val result : Settings = apiInstance.restAdminUsersIdSettingsGet(id)
    println(result)
} catch (e: ClientException) {
    println("4xx response calling AdminApi#restAdminUsersIdSettingsGet")
    e.printStackTrace()
} catch (e: ServerException) {
    println("5xx response calling AdminApi#restAdminUsersIdSettingsGet")
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

<a id="restAdminUsersMigrateEmailsCsvPost"></a>
# **restAdminUsersMigrateEmailsCsvPost**
> restAdminUsersMigrateEmailsCsvPost(body, returnEntity, mode, deleteIfExists)

Endpoint to bulk update users emails

Endpoint to bulk update users emails. Accepts CSV file. 

### Example
```kotlin
// Import classes:
//import org.openapitools.client.infrastructure.*
//import org.openapitools.client.models.*

val apiInstance = AdminApi()
val body : io.ktor.client.request.forms.InputProvider = BINARY_DATA_HERE // io.ktor.client.request.forms.InputProvider | CSV file
val returnEntity : kotlin.Boolean = true // kotlin.Boolean | Return information about newly created entity
val mode : kotlin.String = mode_example // kotlin.String | Response mode
val deleteIfExists : kotlin.Boolean = true // kotlin.Boolean | Delete users which have emails mentioned in any newEmail field
try {
    apiInstance.restAdminUsersMigrateEmailsCsvPost(body, returnEntity, mode, deleteIfExists)
} catch (e: ClientException) {
    println("4xx response calling AdminApi#restAdminUsersMigrateEmailsCsvPost")
    e.printStackTrace()
} catch (e: ServerException) {
    println("5xx response calling AdminApi#restAdminUsersMigrateEmailsCsvPost")
    e.printStackTrace()
}
```

### Parameters

Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **body** | **io.ktor.client.request.forms.InputProvider**| CSV file |
 **returnEntity** | **kotlin.Boolean**| Return information about newly created entity | [optional]
 **mode** | **kotlin.String**| Response mode | [optional]
 **deleteIfExists** | **kotlin.Boolean**| Delete users which have emails mentioned in any newEmail field | [optional]

### Return type

null (empty response body)

### Authorization

No authorization required

### HTTP request headers

 - **Content-Type**: multipart/form-data
 - **Accept**: Not defined

<a id="restAdminUsersMigrateEmailsPost"></a>
# **restAdminUsersMigrateEmailsPost**
> kotlin.collections.List&lt;User&gt; restAdminUsersMigrateEmailsPost(body, returnEntity, mode)

Endpoint to bulk update users emails

Endpoint to bulk update users emails. Accepts array of old and new user email pairs

### Example
```kotlin
// Import classes:
//import org.openapitools.client.infrastructure.*
//import org.openapitools.client.models.*

val apiInstance = AdminApi()
val body : UsersEmailMigrationPost =  // UsersEmailMigrationPost | The user details
val returnEntity : kotlin.Boolean = true // kotlin.Boolean | Return information about newly created entity
val mode : kotlin.String = mode_example // kotlin.String | Response mode
try {
    val result : kotlin.collections.List<User> = apiInstance.restAdminUsersMigrateEmailsPost(body, returnEntity, mode)
    println(result)
} catch (e: ClientException) {
    println("4xx response calling AdminApi#restAdminUsersMigrateEmailsPost")
    e.printStackTrace()
} catch (e: ServerException) {
    println("5xx response calling AdminApi#restAdminUsersMigrateEmailsPost")
    e.printStackTrace()
}
```

### Parameters

Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **body** | [**UsersEmailMigrationPost**](UsersEmailMigrationPost.md)| The user details |
 **returnEntity** | **kotlin.Boolean**| Return information about newly created entity | [optional]
 **mode** | **kotlin.String**| Response mode | [optional]

### Return type

[**kotlin.collections.List&lt;User&gt;**](User.md)

### Authorization

No authorization required

### HTTP request headers

 - **Content-Type**: Not defined
 - **Accept**: */*

<a id="restAdminUsersPost"></a>
# **restAdminUsersPost**
> restAdminUsersPost(body, returnEntity, mode)

Create a User

Creates a new User in the system by specifying an email address and name.

### Example
```kotlin
// Import classes:
//import org.openapitools.client.infrastructure.*
//import org.openapitools.client.models.*

val apiInstance = AdminApi()
val body : UserPost =  // UserPost | The user details
val returnEntity : kotlin.Boolean = true // kotlin.Boolean | Return information about newly created entity
val mode : kotlin.String = mode_example // kotlin.String | Response mode
try {
    apiInstance.restAdminUsersPost(body, returnEntity, mode)
} catch (e: ClientException) {
    println("4xx response calling AdminApi#restAdminUsersPost")
    e.printStackTrace()
} catch (e: ServerException) {
    println("5xx response calling AdminApi#restAdminUsersPost")
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

