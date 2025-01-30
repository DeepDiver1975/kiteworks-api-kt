# JobsApi

All URIs are relative to *http://localhost*

Method | HTTP request | Description
------------- | ------------- | -------------
[**restJobsIdGet**](JobsApi.md#restJobsIdGet) | **GET** /rest/jobs/{id} | Retrieve information about scheduled job in queue.
[**restJobsIdPost**](JobsApi.md#restJobsIdPost) | **POST** /rest/jobs/{id} | Execute job


<a id="restJobsIdGet"></a>
# **restJobsIdGet**
> Job restJobsIdGet(id)

Retrieve information about scheduled job in queue.

Return job information for the specified job. e.g.:                   I want to check job status for copy EC file from tray

### Example
```kotlin
// Import classes:
//import org.openapitools.client.infrastructure.*
//import org.openapitools.client.models.*

val apiInstance = JobsApi()
val id : kotlin.Int = 56 // kotlin.Int | ID of the job
try {
    val result : Job = apiInstance.restJobsIdGet(id)
    println(result)
} catch (e: ClientException) {
    println("4xx response calling JobsApi#restJobsIdGet")
    e.printStackTrace()
} catch (e: ServerException) {
    println("5xx response calling JobsApi#restJobsIdGet")
    e.printStackTrace()
}
```

### Parameters

Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **id** | **kotlin.Int**| ID of the job |

### Return type

[**Job**](Job.md)

### Authorization

No authorization required

### HTTP request headers

 - **Content-Type**: Not defined
 - **Accept**: */*

<a id="restJobsIdPost"></a>
# **restJobsIdPost**
> restJobsIdPost(id)

Execute job

Execute job

### Example
```kotlin
// Import classes:
//import org.openapitools.client.infrastructure.*
//import org.openapitools.client.models.*

val apiInstance = JobsApi()
val id : kotlin.Int = 56 // kotlin.Int | ID of the job
try {
    apiInstance.restJobsIdPost(id)
} catch (e: ClientException) {
    println("4xx response calling JobsApi#restJobsIdPost")
    e.printStackTrace()
} catch (e: ServerException) {
    println("5xx response calling JobsApi#restJobsIdPost")
    e.printStackTrace()
}
```

### Parameters

Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **id** | **kotlin.Int**| ID of the job |

### Return type

null (empty response body)

### Authorization

No authorization required

### HTTP request headers

 - **Content-Type**: Not defined
 - **Accept**: Not defined

