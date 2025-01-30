# SubscribeApi

All URIs are relative to *http://localhost*

Method | HTTP request | Description
------------- | ------------- | -------------
[**restPubsubConfigGet**](SubscribeApi.md#restPubsubConfigGet) | **GET** /rest/pubsub/config | Return pub/sub configuration
[**restPubsubSubscribePost**](SubscribeApi.md#restPubsubSubscribePost) | **POST** /rest/pubsub/subscribe | Subscribe to entity events
[**restPubsubUnsubscribePost**](SubscribeApi.md#restPubsubUnsubscribePost) | **POST** /rest/pubsub/unsubscribe | Unsubscribe to entity events


<a id="restPubsubConfigGet"></a>
# **restPubsubConfigGet**
> PubSubConfig restPubsubConfigGet()

Return pub/sub configuration

Pub/sub configuration

### Example
```kotlin
// Import classes:
//import org.openapitools.client.infrastructure.*
//import org.openapitools.client.models.*

val apiInstance = SubscribeApi()
try {
    val result : PubSubConfig = apiInstance.restPubsubConfigGet()
    println(result)
} catch (e: ClientException) {
    println("4xx response calling SubscribeApi#restPubsubConfigGet")
    e.printStackTrace()
} catch (e: ServerException) {
    println("5xx response calling SubscribeApi#restPubsubConfigGet")
    e.printStackTrace()
}
```

### Parameters
This endpoint does not need any parameter.

### Return type

[**PubSubConfig**](PubSubConfig.md)

### Authorization

No authorization required

### HTTP request headers

 - **Content-Type**: Not defined
 - **Accept**: */*

<a id="restPubsubSubscribePost"></a>
# **restPubsubSubscribePost**
> restPubsubSubscribePost(body)

Subscribe to entity events

Subscribe to entity events

### Example
```kotlin
// Import classes:
//import org.openapitools.client.infrastructure.*
//import org.openapitools.client.models.*

val apiInstance = SubscribeApi()
val body : PubSubSubscribe =  // PubSubSubscribe | 
try {
    apiInstance.restPubsubSubscribePost(body)
} catch (e: ClientException) {
    println("4xx response calling SubscribeApi#restPubsubSubscribePost")
    e.printStackTrace()
} catch (e: ServerException) {
    println("5xx response calling SubscribeApi#restPubsubSubscribePost")
    e.printStackTrace()
}
```

### Parameters

Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **body** | [**PubSubSubscribe**](PubSubSubscribe.md)|  |

### Return type

null (empty response body)

### Authorization

No authorization required

### HTTP request headers

 - **Content-Type**: Not defined
 - **Accept**: Not defined

<a id="restPubsubUnsubscribePost"></a>
# **restPubsubUnsubscribePost**
> restPubsubUnsubscribePost(body)

Unsubscribe to entity events

Unsubscribe to entity events

### Example
```kotlin
// Import classes:
//import org.openapitools.client.infrastructure.*
//import org.openapitools.client.models.*

val apiInstance = SubscribeApi()
val body : PubSubUnsubscribe =  // PubSubUnsubscribe | 
try {
    apiInstance.restPubsubUnsubscribePost(body)
} catch (e: ClientException) {
    println("4xx response calling SubscribeApi#restPubsubUnsubscribePost")
    e.printStackTrace()
} catch (e: ServerException) {
    println("5xx response calling SubscribeApi#restPubsubUnsubscribePost")
    e.printStackTrace()
}
```

### Parameters

Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **body** | [**PubSubUnsubscribe**](PubSubUnsubscribe.md)|  |

### Return type

null (empty response body)

### Authorization

No authorization required

### HTTP request headers

 - **Content-Type**: Not defined
 - **Accept**: Not defined

