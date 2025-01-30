# ClientEventLogsApi

All URIs are relative to *http://localhost*

Method | HTTP request | Description
------------- | ------------- | -------------
[**restClientsActionEventLogPost**](ClientEventLogsApi.md#restClientsActionEventLogPost) | **POST** /rest/clients/action/eventLog | Post event logs from client


<a id="restClientsActionEventLogPost"></a>
# **restClientsActionEventLogPost**
> ClientCustomEventLog restClientsActionEventLogPost(body)

Post event logs from client

Post event logs from client

### Example
```kotlin
// Import classes:
//import org.openapitools.client.infrastructure.*
//import org.openapitools.client.models.*

val apiInstance = ClientEventLogsApi()
val body : BulkClientEventLogsPostRequest =  // BulkClientEventLogsPostRequest | 
try {
    val result : ClientCustomEventLog = apiInstance.restClientsActionEventLogPost(body)
    println(result)
} catch (e: ClientException) {
    println("4xx response calling ClientEventLogsApi#restClientsActionEventLogPost")
    e.printStackTrace()
} catch (e: ServerException) {
    println("5xx response calling ClientEventLogsApi#restClientsActionEventLogPost")
    e.printStackTrace()
}
```

### Parameters

Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **body** | [**BulkClientEventLogsPostRequest**](BulkClientEventLogsPostRequest.md)|  |

### Return type

[**ClientCustomEventLog**](ClientCustomEventLog.md)

### Authorization

No authorization required

### HTTP request headers

 - **Content-Type**: Not defined
 - **Accept**: */*

