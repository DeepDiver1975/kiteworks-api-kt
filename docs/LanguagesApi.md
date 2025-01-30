# LanguagesApi

All URIs are relative to *http://localhost*

Method | HTTP request | Description
------------- | ------------- | -------------
[**restLanguagesGet**](LanguagesApi.md#restLanguagesGet) | **GET** /rest/languages | List languages
[**restLanguagesIdGet**](LanguagesApi.md#restLanguagesIdGet) | **GET** /rest/languages/{id} | Get a language


<a id="restLanguagesGet"></a>
# **restLanguagesGet**
> kotlin.collections.List&lt;Language&gt; restLanguagesGet(name, nameColonContains, symbol, orderBy, mode)

List languages

Returns a list of available languages.

### Example
```kotlin
// Import classes:
//import org.openapitools.client.infrastructure.*
//import org.openapitools.client.models.*

val apiInstance = LanguagesApi()
val name : kotlin.String = name_example // kotlin.String | Language name
val nameColonContains : kotlin.String = nameColonContains_example // kotlin.String | Language name. Search for result that contains specified characters in this parameter.
val symbol : kotlin.String = symbol_example // kotlin.String | Language symbol
val orderBy : kotlin.collections.List<kotlin.String> =  // kotlin.collections.List<kotlin.String> | Sorting options
val mode : kotlin.String = mode_example // kotlin.String | Response mode
try {
    val result : kotlin.collections.List<Language> = apiInstance.restLanguagesGet(name, nameColonContains, symbol, orderBy, mode)
    println(result)
} catch (e: ClientException) {
    println("4xx response calling LanguagesApi#restLanguagesGet")
    e.printStackTrace()
} catch (e: ServerException) {
    println("5xx response calling LanguagesApi#restLanguagesGet")
    e.printStackTrace()
}
```

### Parameters

Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **name** | **kotlin.String**| Language name | [optional]
 **nameColonContains** | **kotlin.String**| Language name. Search for result that contains specified characters in this parameter. | [optional]
 **symbol** | **kotlin.String**| Language symbol | [optional]
 **orderBy** | [**kotlin.collections.List&lt;kotlin.String&gt;**](kotlin.String.md)| Sorting options | [optional]
 **mode** | **kotlin.String**| Response mode | [optional]

### Return type

[**kotlin.collections.List&lt;Language&gt;**](Language.md)

### Authorization

No authorization required

### HTTP request headers

 - **Content-Type**: Not defined
 - **Accept**: */*

<a id="restLanguagesIdGet"></a>
# **restLanguagesIdGet**
> Language restLanguagesIdGet(id)

Get a language

Returns the details of a specified language including language symbol, name, and link.

### Example
```kotlin
// Import classes:
//import org.openapitools.client.infrastructure.*
//import org.openapitools.client.models.*

val apiInstance = LanguagesApi()
val id : kotlin.Int = 56 // kotlin.Int | ID of the language to be retrieved
try {
    val result : Language = apiInstance.restLanguagesIdGet(id)
    println(result)
} catch (e: ClientException) {
    println("4xx response calling LanguagesApi#restLanguagesIdGet")
    e.printStackTrace()
} catch (e: ServerException) {
    println("5xx response calling LanguagesApi#restLanguagesIdGet")
    e.printStackTrace()
}
```

### Parameters

Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **id** | **kotlin.Int**| ID of the language to be retrieved |

### Return type

[**Language**](Language.md)

### Authorization

No authorization required

### HTTP request headers

 - **Content-Type**: Not defined
 - **Accept**: */*

