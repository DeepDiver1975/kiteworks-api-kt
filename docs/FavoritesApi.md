# FavoritesApi

All URIs are relative to *http://localhost*

Method | HTTP request | Description
------------- | ------------- | -------------
[**restFavoritesGet**](FavoritesApi.md#restFavoritesGet) | **GET** /rest/favorites | List favorites
[**restFavoritesIdDelete**](FavoritesApi.md#restFavoritesIdDelete) | **DELETE** /rest/favorites/{id} | Remove a favorite
[**restFavoritesPost**](FavoritesApi.md#restFavoritesPost) | **POST** /rest/favorites | Add a favorite
[**restFoldersActionsFavoriteDelete**](FavoritesApi.md#restFoldersActionsFavoriteDelete) | **DELETE** /rest/folders/actions/favorite | Removes specified folders from favorites
[**restFoldersActionsFavoritePost**](FavoritesApi.md#restFoldersActionsFavoritePost) | **POST** /rest/folders/actions/favorite | Set multiple folders as favorite


<a id="restFavoritesGet"></a>
# **restFavoritesGet**
> FavoriteListOpenAPI2 restFavoritesGet(with, excludeEc, limit, mode, orderBy, parentId, parentIdColonIn, offset, returnEntity)

List favorites

List favorites

### Example
```kotlin
// Import classes:
//import org.openapitools.client.infrastructure.*
//import org.openapitools.client.models.*

val apiInstance = FavoritesApi()
val with : kotlin.String = with_example // kotlin.String | 
val excludeEc : kotlin.Boolean = true // kotlin.Boolean | Do not return EC folder if set to true
val limit : kotlin.Int = 56 // kotlin.Int | 
val mode : kotlin.String = mode_example // kotlin.String | 
val orderBy : kotlin.String = orderBy_example // kotlin.String | 
val parentId : kotlin.String = parentId_example // kotlin.String | Parent folder
val parentIdColonIn : kotlin.collections.List<kotlin.String> =  // kotlin.collections.List<kotlin.String> | Parent folder. Search for results that contain any of specified values of this parameter.
val offset : kotlin.Int = 56 // kotlin.Int | 
val returnEntity : kotlin.Boolean = true // kotlin.Boolean | 
try {
    val result : FavoriteListOpenAPI2 = apiInstance.restFavoritesGet(with, excludeEc, limit, mode, orderBy, parentId, parentIdColonIn, offset, returnEntity)
    println(result)
} catch (e: ClientException) {
    println("4xx response calling FavoritesApi#restFavoritesGet")
    e.printStackTrace()
} catch (e: ServerException) {
    println("5xx response calling FavoritesApi#restFavoritesGet")
    e.printStackTrace()
}
```

### Parameters

Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **with** | **kotlin.String**|  | [optional]
 **excludeEc** | **kotlin.Boolean**| Do not return EC folder if set to true | [optional]
 **limit** | **kotlin.Int**|  | [optional]
 **mode** | **kotlin.String**|  | [optional]
 **orderBy** | **kotlin.String**|  | [optional]
 **parentId** | **kotlin.String**| Parent folder | [optional]
 **parentIdColonIn** | [**kotlin.collections.List&lt;kotlin.String&gt;**](kotlin.String.md)| Parent folder. Search for results that contain any of specified values of this parameter. | [optional]
 **offset** | **kotlin.Int**|  | [optional]
 **returnEntity** | **kotlin.Boolean**|  | [optional]

### Return type

[**FavoriteListOpenAPI2**](FavoriteListOpenAPI2.md)

### Authorization

No authorization required

### HTTP request headers

 - **Content-Type**: Not defined
 - **Accept**: */*

<a id="restFavoritesIdDelete"></a>
# **restFavoritesIdDelete**
> restFavoritesIdDelete(id)

Remove a favorite

Deleting a favorite

### Example
```kotlin
// Import classes:
//import org.openapitools.client.infrastructure.*
//import org.openapitools.client.models.*

val apiInstance = FavoritesApi()
val id : kotlin.Int = 56 // kotlin.Int | ID of the favorite to be removed
try {
    apiInstance.restFavoritesIdDelete(id)
} catch (e: ClientException) {
    println("4xx response calling FavoritesApi#restFavoritesIdDelete")
    e.printStackTrace()
} catch (e: ServerException) {
    println("5xx response calling FavoritesApi#restFavoritesIdDelete")
    e.printStackTrace()
}
```

### Parameters

Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **id** | **kotlin.Int**| ID of the favorite to be removed |

### Return type

null (empty response body)

### Authorization

No authorization required

### HTTP request headers

 - **Content-Type**: Not defined
 - **Accept**: Not defined

<a id="restFavoritesPost"></a>
# **restFavoritesPost**
> restFavoritesPost(body, returnEntity, mode)

Add a favorite

Adding a favorite

### Example
```kotlin
// Import classes:
//import org.openapitools.client.infrastructure.*
//import org.openapitools.client.models.*

val apiInstance = FavoritesApi()
val body : FavoritePost =  // FavoritePost | Object ID of the folder being added to favorites
val returnEntity : kotlin.Boolean = true // kotlin.Boolean | Return information about newly created entity
val mode : kotlin.String = mode_example // kotlin.String | Response mode
try {
    apiInstance.restFavoritesPost(body, returnEntity, mode)
} catch (e: ClientException) {
    println("4xx response calling FavoritesApi#restFavoritesPost")
    e.printStackTrace()
} catch (e: ServerException) {
    println("5xx response calling FavoritesApi#restFavoritesPost")
    e.printStackTrace()
}
```

### Parameters

Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **body** | [**FavoritePost**](FavoritePost.md)| Object ID of the folder being added to favorites |
 **returnEntity** | **kotlin.Boolean**| Return information about newly created entity | [optional]
 **mode** | **kotlin.String**| Response mode | [optional]

### Return type

null (empty response body)

### Authorization

No authorization required

### HTTP request headers

 - **Content-Type**: Not defined
 - **Accept**: Not defined

<a id="restFoldersActionsFavoriteDelete"></a>
# **restFoldersActionsFavoriteDelete**
> restFoldersActionsFavoriteDelete(idColonIn, partialSuccess, mode)

Removes specified folders from favorites

Removes specified folders from favorites

### Example
```kotlin
// Import classes:
//import org.openapitools.client.infrastructure.*
//import org.openapitools.client.models.*

val apiInstance = FavoritesApi()
val idColonIn : kotlin.String = idColonIn_example // kotlin.String | Array of values which are going to be changed.
val partialSuccess : kotlin.Boolean = true // kotlin.Boolean | Whether to perform action on valid items even if some ones fail
val mode : kotlin.String = mode_example // kotlin.String | Response mode
try {
    apiInstance.restFoldersActionsFavoriteDelete(idColonIn, partialSuccess, mode)
} catch (e: ClientException) {
    println("4xx response calling FavoritesApi#restFoldersActionsFavoriteDelete")
    e.printStackTrace()
} catch (e: ServerException) {
    println("5xx response calling FavoritesApi#restFoldersActionsFavoriteDelete")
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

<a id="restFoldersActionsFavoritePost"></a>
# **restFoldersActionsFavoritePost**
> restFoldersActionsFavoritePost(idColonIn, partialSuccess, returnEntity, mode)

Set multiple folders as favorite

Set multiple folders as favorite

### Example
```kotlin
// Import classes:
//import org.openapitools.client.infrastructure.*
//import org.openapitools.client.models.*

val apiInstance = FavoritesApi()
val idColonIn : kotlin.String = idColonIn_example // kotlin.String | Array of values which are going to be changed.
val partialSuccess : kotlin.Boolean = true // kotlin.Boolean | Whether to perform action on valid items even if some ones fail
val returnEntity : kotlin.Boolean = true // kotlin.Boolean | Return information about newly created entity
val mode : kotlin.String = mode_example // kotlin.String | Response mode
try {
    apiInstance.restFoldersActionsFavoritePost(idColonIn, partialSuccess, returnEntity, mode)
} catch (e: ClientException) {
    println("4xx response calling FavoritesApi#restFoldersActionsFavoritePost")
    e.printStackTrace()
} catch (e: ServerException) {
    println("5xx response calling FavoritesApi#restFoldersActionsFavoritePost")
    e.printStackTrace()
}
```

### Parameters

Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **idColonIn** | **kotlin.String**| Array of values which are going to be changed. |
 **partialSuccess** | **kotlin.Boolean**| Whether to perform action on valid items even if some ones fail | [optional]
 **returnEntity** | **kotlin.Boolean**| Return information about newly created entity | [optional]
 **mode** | **kotlin.String**| Response mode | [optional]

### Return type

null (empty response body)

### Authorization

No authorization required

### HTTP request headers

 - **Content-Type**: Not defined
 - **Accept**: Not defined

