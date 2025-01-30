# SearchApi

All URIs are relative to *http://localhost*

Method | HTTP request | Description
------------- | ------------- | -------------
[**restQueryGet**](SearchApi.md#restQueryGet) | **GET** /rest/query | Search api
[**restSearchGet**](SearchApi.md#restSearchGet) | **GET** /rest/search | Return lists of files/folders/emails from search results
[**restSourcesIdQueryGet**](SearchApi.md#restSourcesIdQueryGet) | **GET** /rest/sources/{id}/query | SharePoint Sites Search api


<a id="restQueryGet"></a>
# **restQueryGet**
> SearchResult restQueryGet(includeContent, searchType, sharedMailboxId, createdColonGt, subject, fileSizeColonGte, fileSizeColonGt, createdColonLte, fileSizeColonLt, created, modified, modifiedColonGt, limit, recipientId, modifiedColonLt, createdColonGte, createdColonLt, path, flsOnly, objectId, spellCheck, fileSize, user, query, fileType, bucket, fileName, folderName, fileSizeColonLte, modifiedColonGte, orderType, senderId, offset, nameOnly, orderBy, modifiedColonLte)

Search api

search files/folders/emails

### Example
```kotlin
// Import classes:
//import org.openapitools.client.infrastructure.*
//import org.openapitools.client.models.*

val apiInstance = SearchApi()
val includeContent : kotlin.Boolean = true // kotlin.Boolean | indicate it is full_text_search or database search
val searchType : kotlin.collections.List<kotlin.String> =  // kotlin.collections.List<kotlin.String> | 
val sharedMailboxId : kotlin.String = sharedMailboxId_example // kotlin.String | 
val createdColonGt : kotlin.String = createdColonGt_example // kotlin.String | email/file/folder creation date > specified parameter
val subject : kotlin.String = subject_example // kotlin.String | 
val fileSizeColonGte : kotlin.String = fileSizeColonGte_example // kotlin.String | file size >= specified value
val fileSizeColonGt : kotlin.Int = 56 // kotlin.Int | file size > specified value
val createdColonLte : kotlin.String = createdColonLte_example // kotlin.String | email/file/folder <= specified parameter
val fileSizeColonLt : kotlin.String = fileSizeColonLt_example // kotlin.String | file size < specified value
val created : kotlin.String = created_example // kotlin.String | email/file/folder creation date = specified parameter
val modified : kotlin.String = modified_example // kotlin.String | email/file/folder modified date = specified value
val modifiedColonGt : kotlin.String = modifiedColonGt_example // kotlin.String | email/file/folder modified date > specified value
val limit : kotlin.Int = 56 // kotlin.Int | 
val recipientId : kotlin.String = recipientId_example // kotlin.String | recipient id or email
val modifiedColonLt : kotlin.String = modifiedColonLt_example // kotlin.String | email/file/folder modified date < specified value
val createdColonGte : kotlin.String = createdColonGte_example // kotlin.String | email/file/folder creation date >= specified parameter
val createdColonLt : kotlin.String = createdColonLt_example // kotlin.String | email/file/folder creation date < specified parameter
val path : kotlin.String = path_example // kotlin.String | 
val flsOnly : kotlin.Boolean = true // kotlin.Boolean | only include files/folders shared to me
val objectId : kotlin.String = objectId_example // kotlin.String | search within folder id
val spellCheck : kotlin.Boolean = true // kotlin.Boolean | To get suggestions of searching keyword
val fileSize : kotlin.Int = 56 // kotlin.Int | file size = specified parameter
val user : kotlin.String = user_example // kotlin.String | 
val query : kotlin.String = query_example // kotlin.String | 
val fileType : kotlin.collections.List<kotlin.String> =  // kotlin.collections.List<kotlin.String> | 
val bucket : kotlin.String = bucket_example // kotlin.String | 
val fileName : kotlin.String = fileName_example // kotlin.String | 
val folderName : kotlin.String = folderName_example // kotlin.String | 
val fileSizeColonLte : kotlin.String = fileSizeColonLte_example // kotlin.String | file size <= specified value
val modifiedColonGte : kotlin.String = modifiedColonGte_example // kotlin.String | email/file/folder modified date >= specified value
val orderType : kotlin.String = orderType_example // kotlin.String | 
val senderId : kotlin.String = senderId_example // kotlin.String | sender id or email
val offset : kotlin.Int = 56 // kotlin.Int | 
val nameOnly : kotlin.Boolean = true // kotlin.Boolean | indicate when searching file/only with name only option
val orderBy : kotlin.String = orderBy_example // kotlin.String | 
val modifiedColonLte : kotlin.String = modifiedColonLte_example // kotlin.String | email/file/folder modified date <= specified value
try {
    val result : SearchResult = apiInstance.restQueryGet(includeContent, searchType, sharedMailboxId, createdColonGt, subject, fileSizeColonGte, fileSizeColonGt, createdColonLte, fileSizeColonLt, created, modified, modifiedColonGt, limit, recipientId, modifiedColonLt, createdColonGte, createdColonLt, path, flsOnly, objectId, spellCheck, fileSize, user, query, fileType, bucket, fileName, folderName, fileSizeColonLte, modifiedColonGte, orderType, senderId, offset, nameOnly, orderBy, modifiedColonLte)
    println(result)
} catch (e: ClientException) {
    println("4xx response calling SearchApi#restQueryGet")
    e.printStackTrace()
} catch (e: ServerException) {
    println("5xx response calling SearchApi#restQueryGet")
    e.printStackTrace()
}
```

### Parameters

Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **includeContent** | **kotlin.Boolean**| indicate it is full_text_search or database search |
 **searchType** | [**kotlin.collections.List&lt;kotlin.String&gt;**](kotlin.String.md)|  |
 **sharedMailboxId** | **kotlin.String**|  | [optional]
 **createdColonGt** | **kotlin.String**| email/file/folder creation date &gt; specified parameter | [optional]
 **subject** | **kotlin.String**|  | [optional]
 **fileSizeColonGte** | **kotlin.String**| file size &gt;&#x3D; specified value | [optional]
 **fileSizeColonGt** | **kotlin.Int**| file size &gt; specified value | [optional]
 **createdColonLte** | **kotlin.String**| email/file/folder &lt;&#x3D; specified parameter | [optional]
 **fileSizeColonLt** | **kotlin.String**| file size &lt; specified value | [optional]
 **created** | **kotlin.String**| email/file/folder creation date &#x3D; specified parameter | [optional]
 **modified** | **kotlin.String**| email/file/folder modified date &#x3D; specified value | [optional]
 **modifiedColonGt** | **kotlin.String**| email/file/folder modified date &gt; specified value | [optional]
 **limit** | **kotlin.Int**|  | [optional]
 **recipientId** | **kotlin.String**| recipient id or email | [optional]
 **modifiedColonLt** | **kotlin.String**| email/file/folder modified date &lt; specified value | [optional]
 **createdColonGte** | **kotlin.String**| email/file/folder creation date &gt;&#x3D; specified parameter | [optional]
 **createdColonLt** | **kotlin.String**| email/file/folder creation date &lt; specified parameter | [optional]
 **path** | **kotlin.String**|  | [optional]
 **flsOnly** | **kotlin.Boolean**| only include files/folders shared to me | [optional]
 **objectId** | **kotlin.String**| search within folder id | [optional]
 **spellCheck** | **kotlin.Boolean**| To get suggestions of searching keyword | [optional]
 **fileSize** | **kotlin.Int**| file size &#x3D; specified parameter | [optional]
 **user** | **kotlin.String**|  | [optional]
 **query** | **kotlin.String**|  | [optional]
 **fileType** | [**kotlin.collections.List&lt;kotlin.String&gt;**](kotlin.String.md)|  | [optional]
 **bucket** | **kotlin.String**|  | [optional]
 **fileName** | **kotlin.String**|  | [optional]
 **folderName** | **kotlin.String**|  | [optional]
 **fileSizeColonLte** | **kotlin.String**| file size &lt;&#x3D; specified value | [optional]
 **modifiedColonGte** | **kotlin.String**| email/file/folder modified date &gt;&#x3D; specified value | [optional]
 **orderType** | **kotlin.String**|  | [optional]
 **senderId** | **kotlin.String**| sender id or email | [optional]
 **offset** | **kotlin.Int**|  | [optional]
 **nameOnly** | **kotlin.Boolean**| indicate when searching file/only with name only option | [optional]
 **orderBy** | **kotlin.String**|  | [optional]
 **modifiedColonLte** | **kotlin.String**| email/file/folder modified date &lt;&#x3D; specified value | [optional]

### Return type

[**SearchResult**](SearchResult.md)

### Authorization

No authorization required

### HTTP request headers

 - **Content-Type**: Not defined
 - **Accept**: */*

<a id="restSearchGet"></a>
# **restSearchGet**
> Search restSearchGet(objectId, content, contentColonContains, contentColonStartswith, description, descriptionColonContains, descriptionColonStartswith, user, modified, modifiedColonGt, modifiedColonGte, modifiedColonLt, modifiedColonLte, created, createdColonGt, createdColonGte, createdColonLt, createdColonLte, locked, lockedColonGt, lockedColonGte, lockedColonLt, lockedColonLte, filesize, filesizeColonGt, filesizeColonGte, filesizeColonLt, filesizeColonLte, fileType, emailType, path, pathColonContains, searchType, searchFilter, flsOnly, sharedMailboxId, orderBy, offset, limit, with, mode)

Return lists of files/folders/emails from search results

Return lists of files/folders/emails from search results

### Example
```kotlin
// Import classes:
//import org.openapitools.client.infrastructure.*
//import org.openapitools.client.models.*

val apiInstance = SearchApi()
val objectId : kotlin.String = objectId_example // kotlin.String | Id of folder to search
val content : kotlin.String = content_example // kotlin.String | Search by content
val contentColonContains : kotlin.String = contentColonContains_example // kotlin.String | Search by content. Search for result that contains specified characters in this parameter.
val contentColonStartswith : kotlin.String = contentColonStartswith_example // kotlin.String | 
val description : kotlin.String = description_example // kotlin.String | Search by description
val descriptionColonContains : kotlin.String = descriptionColonContains_example // kotlin.String | Search by description. Search for result that contains specified characters in this parameter.
val descriptionColonStartswith : kotlin.String = descriptionColonStartswith_example // kotlin.String | 
val user : kotlin.String = user_example // kotlin.String | Search by user
val modified : java.time.LocalDate = 2013-10-20 // java.time.LocalDate | Search by modified date
val modifiedColonGt : java.time.LocalDate = 2013-10-20 // java.time.LocalDate | Search by modified date. Search for result that has this parameter value greater than specified.
val modifiedColonGte : java.time.LocalDate = 2013-10-20 // java.time.LocalDate | Search by modified date. Search for result that has this parameter value greater or equal to the specified.
val modifiedColonLt : java.time.LocalDate = 2013-10-20 // java.time.LocalDate | Search by modified date. Search for result that has this parameter value less than specified.
val modifiedColonLte : java.time.LocalDate = 2013-10-20 // java.time.LocalDate | Search by modified date. Search for result that has this parameter value less or equal to the specified.
val created : java.time.LocalDate = 2013-10-20 // java.time.LocalDate | Search by created date
val createdColonGt : java.time.LocalDate = 2013-10-20 // java.time.LocalDate | Search by created date. Search for result that has this parameter value greater than specified.
val createdColonGte : java.time.LocalDate = 2013-10-20 // java.time.LocalDate | Search by created date. Search for result that has this parameter value greater or equal to the specified.
val createdColonLt : java.time.LocalDate = 2013-10-20 // java.time.LocalDate | Search by created date. Search for result that has this parameter value less than specified.
val createdColonLte : java.time.LocalDate = 2013-10-20 // java.time.LocalDate | Search by created date. Search for result that has this parameter value less or equal to the specified.
val locked : kotlin.Int = 56 // kotlin.Int | Search by lock status
val lockedColonGt : kotlin.Int = 56 // kotlin.Int | Search by lock status. Search for result that has this parameter value greater than specified.
val lockedColonGte : kotlin.Int = 56 // kotlin.Int | Search by lock status. Search for result that has this parameter value greater or equal to the specified.
val lockedColonLt : kotlin.Int = 56 // kotlin.Int | Search by lock status. Search for result that has this parameter value less than specified.
val lockedColonLte : kotlin.Int = 56 // kotlin.Int | Search by lock status. Search for result that has this parameter value less or equal to the specified.
val filesize : kotlin.Int = 56 // kotlin.Int | Search by file size
val filesizeColonGt : kotlin.Int = 56 // kotlin.Int | Search by file size. Search for result that has this parameter value greater than specified.
val filesizeColonGte : kotlin.Int = 56 // kotlin.Int | Search by file size. Search for result that has this parameter value greater or equal to the specified.
val filesizeColonLt : kotlin.Int = 56 // kotlin.Int | Search by file size. Search for result that has this parameter value less than specified.
val filesizeColonLte : kotlin.Int = 56 // kotlin.Int | Search by file size. Search for result that has this parameter value less or equal to the specified.
val fileType : kotlin.collections.List<kotlin.String> =  // kotlin.collections.List<kotlin.String> | Search by file type
val emailType : kotlin.collections.List<kotlin.String> =  // kotlin.collections.List<kotlin.String> | Search by email type
val path : kotlin.String = path_example // kotlin.String | Search files/folders by path. If this is specified, other search criteria is no longer valid.
val pathColonContains : kotlin.String = pathColonContains_example // kotlin.String | Search files/folders by path. If this is specified, other search criteria is no longer valid.. Search for result that contains specified characters in this parameter.
val searchType : kotlin.collections.List<kotlin.String> =  // kotlin.collections.List<kotlin.String> | Search type: f(files), d(directories), m(mails) or  k(kitepoint)
val searchFilter : kotlin.String = searchFilter_example // kotlin.String | Search all or only shared folders
val flsOnly : kotlin.Boolean = true // kotlin.Boolean | Search by file shared to me
val sharedMailboxId : kotlin.Int = 56 // kotlin.Int | Id of shared mailbox to search
val orderBy : kotlin.collections.List<kotlin.String> =  // kotlin.collections.List<kotlin.String> | Sorting options
val offset : kotlin.Int = 56 // kotlin.Int | Offset
val limit : kotlin.Int = 56 // kotlin.Int | Limit
val with : kotlin.String = with_example // kotlin.String | With parameters
val mode : kotlin.String = mode_example // kotlin.String | Response mode
try {
    val result : Search = apiInstance.restSearchGet(objectId, content, contentColonContains, contentColonStartswith, description, descriptionColonContains, descriptionColonStartswith, user, modified, modifiedColonGt, modifiedColonGte, modifiedColonLt, modifiedColonLte, created, createdColonGt, createdColonGte, createdColonLt, createdColonLte, locked, lockedColonGt, lockedColonGte, lockedColonLt, lockedColonLte, filesize, filesizeColonGt, filesizeColonGte, filesizeColonLt, filesizeColonLte, fileType, emailType, path, pathColonContains, searchType, searchFilter, flsOnly, sharedMailboxId, orderBy, offset, limit, with, mode)
    println(result)
} catch (e: ClientException) {
    println("4xx response calling SearchApi#restSearchGet")
    e.printStackTrace()
} catch (e: ServerException) {
    println("5xx response calling SearchApi#restSearchGet")
    e.printStackTrace()
}
```

### Parameters

Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **objectId** | **kotlin.String**| Id of folder to search | [optional]
 **content** | **kotlin.String**| Search by content | [optional]
 **contentColonContains** | **kotlin.String**| Search by content. Search for result that contains specified characters in this parameter. | [optional]
 **contentColonStartswith** | **kotlin.String**|  | [optional]
 **description** | **kotlin.String**| Search by description | [optional]
 **descriptionColonContains** | **kotlin.String**| Search by description. Search for result that contains specified characters in this parameter. | [optional]
 **descriptionColonStartswith** | **kotlin.String**|  | [optional]
 **user** | **kotlin.String**| Search by user | [optional]
 **modified** | **java.time.LocalDate**| Search by modified date | [optional]
 **modifiedColonGt** | **java.time.LocalDate**| Search by modified date. Search for result that has this parameter value greater than specified. | [optional]
 **modifiedColonGte** | **java.time.LocalDate**| Search by modified date. Search for result that has this parameter value greater or equal to the specified. | [optional]
 **modifiedColonLt** | **java.time.LocalDate**| Search by modified date. Search for result that has this parameter value less than specified. | [optional]
 **modifiedColonLte** | **java.time.LocalDate**| Search by modified date. Search for result that has this parameter value less or equal to the specified. | [optional]
 **created** | **java.time.LocalDate**| Search by created date | [optional]
 **createdColonGt** | **java.time.LocalDate**| Search by created date. Search for result that has this parameter value greater than specified. | [optional]
 **createdColonGte** | **java.time.LocalDate**| Search by created date. Search for result that has this parameter value greater or equal to the specified. | [optional]
 **createdColonLt** | **java.time.LocalDate**| Search by created date. Search for result that has this parameter value less than specified. | [optional]
 **createdColonLte** | **java.time.LocalDate**| Search by created date. Search for result that has this parameter value less or equal to the specified. | [optional]
 **locked** | **kotlin.Int**| Search by lock status | [optional]
 **lockedColonGt** | **kotlin.Int**| Search by lock status. Search for result that has this parameter value greater than specified. | [optional]
 **lockedColonGte** | **kotlin.Int**| Search by lock status. Search for result that has this parameter value greater or equal to the specified. | [optional]
 **lockedColonLt** | **kotlin.Int**| Search by lock status. Search for result that has this parameter value less than specified. | [optional]
 **lockedColonLte** | **kotlin.Int**| Search by lock status. Search for result that has this parameter value less or equal to the specified. | [optional]
 **filesize** | **kotlin.Int**| Search by file size | [optional]
 **filesizeColonGt** | **kotlin.Int**| Search by file size. Search for result that has this parameter value greater than specified. | [optional]
 **filesizeColonGte** | **kotlin.Int**| Search by file size. Search for result that has this parameter value greater or equal to the specified. | [optional]
 **filesizeColonLt** | **kotlin.Int**| Search by file size. Search for result that has this parameter value less than specified. | [optional]
 **filesizeColonLte** | **kotlin.Int**| Search by file size. Search for result that has this parameter value less or equal to the specified. | [optional]
 **fileType** | [**kotlin.collections.List&lt;kotlin.String&gt;**](kotlin.String.md)| Search by file type | [optional]
 **emailType** | [**kotlin.collections.List&lt;kotlin.String&gt;**](kotlin.String.md)| Search by email type | [optional]
 **path** | **kotlin.String**| Search files/folders by path. If this is specified, other search criteria is no longer valid. | [optional]
 **pathColonContains** | **kotlin.String**| Search files/folders by path. If this is specified, other search criteria is no longer valid.. Search for result that contains specified characters in this parameter. | [optional]
 **searchType** | [**kotlin.collections.List&lt;kotlin.String&gt;**](kotlin.String.md)| Search type: f(files), d(directories), m(mails) or  k(kitepoint) | [optional]
 **searchFilter** | **kotlin.String**| Search all or only shared folders | [optional]
 **flsOnly** | **kotlin.Boolean**| Search by file shared to me | [optional]
 **sharedMailboxId** | **kotlin.Int**| Id of shared mailbox to search | [optional]
 **orderBy** | [**kotlin.collections.List&lt;kotlin.String&gt;**](kotlin.String.md)| Sorting options | [optional]
 **offset** | **kotlin.Int**| Offset | [optional]
 **limit** | **kotlin.Int**| Limit | [optional]
 **with** | **kotlin.String**| With parameters | [optional]
 **mode** | **kotlin.String**| Response mode | [optional]

### Return type

[**Search**](Search.md)

### Authorization

No authorization required

### HTTP request headers

 - **Content-Type**: Not defined
 - **Accept**: */*

<a id="restSourcesIdQueryGet"></a>
# **restSourcesIdQueryGet**
> SearchSharePointSitesResult restSourcesIdQueryGet(id, includeKw, searchType, limit, query, includeContainer, offset)

SharePoint Sites Search api

search SharePoint sites

### Example
```kotlin
// Import classes:
//import org.openapitools.client.infrastructure.*
//import org.openapitools.client.models.*

val apiInstance = SearchApi()
val id : kotlin.Int = 56 // kotlin.Int | The ID of the entity
val includeKw : kotlin.Boolean = true // kotlin.Boolean | 
val searchType : kotlin.String = searchType_example // kotlin.String | 
val limit : kotlin.Int = 56 // kotlin.Int | 
val query : kotlin.String = query_example // kotlin.String | 
val includeContainer : kotlin.Boolean = true // kotlin.Boolean | 
val offset : kotlin.Int = 56 // kotlin.Int | 
try {
    val result : SearchSharePointSitesResult = apiInstance.restSourcesIdQueryGet(id, includeKw, searchType, limit, query, includeContainer, offset)
    println(result)
} catch (e: ClientException) {
    println("4xx response calling SearchApi#restSourcesIdQueryGet")
    e.printStackTrace()
} catch (e: ServerException) {
    println("5xx response calling SearchApi#restSourcesIdQueryGet")
    e.printStackTrace()
}
```

### Parameters

Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **id** | **kotlin.Int**| The ID of the entity |
 **includeKw** | **kotlin.Boolean**|  | [optional]
 **searchType** | **kotlin.String**|  | [optional]
 **limit** | **kotlin.Int**|  | [optional]
 **query** | **kotlin.String**|  | [optional]
 **includeContainer** | **kotlin.Boolean**|  | [optional]
 **offset** | **kotlin.Int**|  | [optional]

### Return type

[**SearchSharePointSitesResult**](SearchSharePointSitesResult.md)

### Authorization

No authorization required

### HTTP request headers

 - **Content-Type**: Not defined
 - **Accept**: */*

