# CardsApi

All URIs are relative to *http://localhost*

Method | HTTP request | Description
------------- | ------------- | -------------
[**restAdminCardsActionsPost**](CardsApi.md#restAdminCardsActionsPost) | **POST** /rest/admin/cards/actions | Post an action to take on a specific card
[**restAdminCardsDetailsGet**](CardsApi.md#restAdminCardsDetailsGet) | **GET** /rest/admin/cards/details | Get list of cards
[**restAdminCardsGet**](CardsApi.md#restAdminCardsGet) | **GET** /rest/admin/cards | Get list of cards


<a id="restAdminCardsActionsPost"></a>
# **restAdminCardsActionsPost**
> restAdminCardsActionsPost(body)

Post an action to take on a specific card

Post an action to take on a specific card

### Example
```kotlin
// Import classes:
//import org.openapitools.client.infrastructure.*
//import org.openapitools.client.models.*

val apiInstance = CardsApi()
val body : CardActionPostRequest =  // CardActionPostRequest | 
try {
    apiInstance.restAdminCardsActionsPost(body)
} catch (e: ClientException) {
    println("4xx response calling CardsApi#restAdminCardsActionsPost")
    e.printStackTrace()
} catch (e: ServerException) {
    println("5xx response calling CardsApi#restAdminCardsActionsPost")
    e.printStackTrace()
}
```

### Parameters

Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **body** | [**CardActionPostRequest**](CardActionPostRequest.md)|  |

### Return type

null (empty response body)

### Authorization

No authorization required

### HTTP request headers

 - **Content-Type**: Not defined
 - **Accept**: Not defined

<a id="restAdminCardsDetailsGet"></a>
# **restAdminCardsDetailsGet**
> Card restAdminCardsDetailsGet(typeColonIn)

Get list of cards

Get list of cards

### Example
```kotlin
// Import classes:
//import org.openapitools.client.infrastructure.*
//import org.openapitools.client.models.*

val apiInstance = CardsApi()
val typeColonIn : kotlin.collections.List<kotlin.String> =  // kotlin.collections.List<kotlin.String> | Type of cards to retrieve. Available card type(s): content_encryption,email_json_migration,event_log_partitioning_migration,system_security_scanning,events_table_monitor,appadmin_db,sysadmin_db,sysadmin_hosts
try {
    val result : Card = apiInstance.restAdminCardsDetailsGet(typeColonIn)
    println(result)
} catch (e: ClientException) {
    println("4xx response calling CardsApi#restAdminCardsDetailsGet")
    e.printStackTrace()
} catch (e: ServerException) {
    println("5xx response calling CardsApi#restAdminCardsDetailsGet")
    e.printStackTrace()
}
```

### Parameters

Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **typeColonIn** | [**kotlin.collections.List&lt;kotlin.String&gt;**](kotlin.String.md)| Type of cards to retrieve. Available card type(s): content_encryption,email_json_migration,event_log_partitioning_migration,system_security_scanning,events_table_monitor,appadmin_db,sysadmin_db,sysadmin_hosts |

### Return type

[**Card**](Card.md)

### Authorization

No authorization required

### HTTP request headers

 - **Content-Type**: Not defined
 - **Accept**: */*

<a id="restAdminCardsGet"></a>
# **restAdminCardsGet**
> Card restAdminCardsGet(typeColonIn)

Get list of cards

Get list of cards

### Example
```kotlin
// Import classes:
//import org.openapitools.client.infrastructure.*
//import org.openapitools.client.models.*

val apiInstance = CardsApi()
val typeColonIn : kotlin.collections.List<kotlin.String> =  // kotlin.collections.List<kotlin.String> | Type of cards to retrieve. Available card type(s): content_encryption,email_json_migration,event_log_partitioning_migration,system_security_scanning,events_table_monitor,appadmin_db,sysadmin_db,sysadmin_hosts
try {
    val result : Card = apiInstance.restAdminCardsGet(typeColonIn)
    println(result)
} catch (e: ClientException) {
    println("4xx response calling CardsApi#restAdminCardsGet")
    e.printStackTrace()
} catch (e: ServerException) {
    println("5xx response calling CardsApi#restAdminCardsGet")
    e.printStackTrace()
}
```

### Parameters

Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **typeColonIn** | [**kotlin.collections.List&lt;kotlin.String&gt;**](kotlin.String.md)| Type of cards to retrieve. Available card type(s): content_encryption,email_json_migration,event_log_partitioning_migration,system_security_scanning,events_table_monitor,appadmin_db,sysadmin_db,sysadmin_hosts |

### Return type

[**Card**](Card.md)

### Authorization

No authorization required

### HTTP request headers

 - **Content-Type**: Not defined
 - **Accept**: */*

