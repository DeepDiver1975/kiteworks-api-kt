# ActivitiesApi

All URIs are relative to *http://localhost*

Method | HTTP request | Description
------------- | ------------- | -------------
[**restActivitiesGet**](ActivitiesApi.md#restActivitiesGet) | **GET** /rest/activities | Return the list of all Activities
[**restFilesFileIdActivitiesGet**](ActivitiesApi.md#restFilesFileIdActivitiesGet) | **GET** /rest/files/{file_id}/activities | Return the list of Activities for this file


<a id="restActivitiesGet"></a>
# **restActivitiesGet**
> kotlin.collections.List&lt;Activity&gt; restActivitiesGet(noDayBack, startDate, endDate, filter, search, type, transactionId, orderBy, offset, limit, with, mode)

Return the list of all Activities

Return the list of all Activities.

### Example
```kotlin
// Import classes:
//import org.openapitools.client.infrastructure.*
//import org.openapitools.client.models.*

val apiInstance = ActivitiesApi()
val noDayBack : kotlin.Int = 56 // kotlin.Int | Number of days back to search
val startDate : java.time.LocalDate = 2013-10-20 // java.time.LocalDate | Start date
val endDate : java.time.LocalDate = 2013-10-20 // java.time.LocalDate | End date
val filter : kotlin.String = filter_example // kotlin.String | All or my activities
val search : kotlin.String = search_example // kotlin.String | Search by mail body, subject and sender/recipients
val type : kotlin.String = type_example // kotlin.String | Activity type
val transactionId : kotlin.String = transactionId_example // kotlin.String | Transaction ID associated with the activities
val orderBy : kotlin.collections.List<kotlin.String> =  // kotlin.collections.List<kotlin.String> | Sorting options
val offset : kotlin.Int = 56 // kotlin.Int | Offset
val limit : kotlin.Int = 56 // kotlin.Int | Limit
val with : kotlin.String = with_example // kotlin.String | With parameters
val mode : kotlin.String = mode_example // kotlin.String | Response mode
try {
    val result : kotlin.collections.List<Activity> = apiInstance.restActivitiesGet(noDayBack, startDate, endDate, filter, search, type, transactionId, orderBy, offset, limit, with, mode)
    println(result)
} catch (e: ClientException) {
    println("4xx response calling ActivitiesApi#restActivitiesGet")
    e.printStackTrace()
} catch (e: ServerException) {
    println("5xx response calling ActivitiesApi#restActivitiesGet")
    e.printStackTrace()
}
```

### Parameters

Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **noDayBack** | **kotlin.Int**| Number of days back to search | [optional]
 **startDate** | **java.time.LocalDate**| Start date | [optional]
 **endDate** | **java.time.LocalDate**| End date | [optional]
 **filter** | **kotlin.String**| All or my activities | [optional]
 **search** | **kotlin.String**| Search by mail body, subject and sender/recipients | [optional]
 **type** | **kotlin.String**| Activity type | [optional]
 **transactionId** | **kotlin.String**| Transaction ID associated with the activities | [optional]
 **orderBy** | [**kotlin.collections.List&lt;kotlin.String&gt;**](kotlin.String.md)| Sorting options | [optional]
 **offset** | **kotlin.Int**| Offset | [optional]
 **limit** | **kotlin.Int**| Limit | [optional]
 **with** | **kotlin.String**| With parameters | [optional]
 **mode** | **kotlin.String**| Response mode | [optional]

### Return type

[**kotlin.collections.List&lt;Activity&gt;**](Activity.md)

### Authorization

No authorization required

### HTTP request headers

 - **Content-Type**: Not defined
 - **Accept**: */*

<a id="restFilesFileIdActivitiesGet"></a>
# **restFilesFileIdActivitiesGet**
> kotlin.collections.List&lt;Activity&gt; restFilesFileIdActivitiesGet(fileId, noDayBack, startDate, endDate, filter, search, type, transactionId, orderBy, offset, limit, with, mode)

Return the list of Activities for this file

Return the list of Activities for this file.

### Example
```kotlin
// Import classes:
//import org.openapitools.client.infrastructure.*
//import org.openapitools.client.models.*

val apiInstance = ActivitiesApi()
val fileId : kotlin.String = fileId_example // kotlin.String | ID of the file
val noDayBack : kotlin.Int = 56 // kotlin.Int | Number of days back to search
val startDate : java.time.LocalDate = 2013-10-20 // java.time.LocalDate | Start date
val endDate : java.time.LocalDate = 2013-10-20 // java.time.LocalDate | End date
val filter : kotlin.String = filter_example // kotlin.String | All or my activities
val search : kotlin.String = search_example // kotlin.String | Search by mail body, subject and sender/recipients
val type : kotlin.String = type_example // kotlin.String | Activity type
val transactionId : kotlin.String = transactionId_example // kotlin.String | Transaction ID associated with the activities
val orderBy : kotlin.collections.List<kotlin.String> =  // kotlin.collections.List<kotlin.String> | Sorting options
val offset : kotlin.Int = 56 // kotlin.Int | Offset
val limit : kotlin.Int = 56 // kotlin.Int | Limit
val with : kotlin.String = with_example // kotlin.String | With parameters
val mode : kotlin.String = mode_example // kotlin.String | Response mode
try {
    val result : kotlin.collections.List<Activity> = apiInstance.restFilesFileIdActivitiesGet(fileId, noDayBack, startDate, endDate, filter, search, type, transactionId, orderBy, offset, limit, with, mode)
    println(result)
} catch (e: ClientException) {
    println("4xx response calling ActivitiesApi#restFilesFileIdActivitiesGet")
    e.printStackTrace()
} catch (e: ServerException) {
    println("5xx response calling ActivitiesApi#restFilesFileIdActivitiesGet")
    e.printStackTrace()
}
```

### Parameters

Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **fileId** | **kotlin.String**| ID of the file |
 **noDayBack** | **kotlin.Int**| Number of days back to search | [optional]
 **startDate** | **java.time.LocalDate**| Start date | [optional]
 **endDate** | **java.time.LocalDate**| End date | [optional]
 **filter** | **kotlin.String**| All or my activities | [optional]
 **search** | **kotlin.String**| Search by mail body, subject and sender/recipients | [optional]
 **type** | **kotlin.String**| Activity type | [optional]
 **transactionId** | **kotlin.String**| Transaction ID associated with the activities | [optional]
 **orderBy** | [**kotlin.collections.List&lt;kotlin.String&gt;**](kotlin.String.md)| Sorting options | [optional]
 **offset** | **kotlin.Int**| Offset | [optional]
 **limit** | **kotlin.Int**| Limit | [optional]
 **with** | **kotlin.String**| With parameters | [optional]
 **mode** | **kotlin.String**| Response mode | [optional]

### Return type

[**kotlin.collections.List&lt;Activity&gt;**](Activity.md)

### Authorization

No authorization required

### HTTP request headers

 - **Content-Type**: Not defined
 - **Accept**: */*

