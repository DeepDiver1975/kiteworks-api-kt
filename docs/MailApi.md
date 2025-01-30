# MailApi

All URIs are relative to *http://localhost*

Method | HTTP request | Description
------------- | ------------- | -------------
[**restFoldersIdActionsSendMessagePost**](MailApi.md#restFoldersIdActionsSendMessagePost) | **POST** /rest/folders/{id}/actions/sendMessage | Create a send message email entry
[**restMailActionsCountersGet**](MailApi.md#restMailActionsCountersGet) | **GET** /rest/mail/actions/counters | Returns number of emails in each bucket
[**restMailActionsDeletePermanentPatch**](MailApi.md#restMailActionsDeletePermanentPatch) | **PATCH** /rest/mail/actions/deletePermanent | Permanently deletes list of emails
[**restMailActionsDistributionListGet**](MailApi.md#restMailActionsDistributionListGet) | **GET** /rest/mail/actions/distributionList | Returns list of emails inside distribution list
[**restMailActionsReadPatch**](MailApi.md#restMailActionsReadPatch) | **PATCH** /rest/mail/actions/read | Mark the mail read status to true on the given email ids
[**restMailActionsRecoverPatch**](MailApi.md#restMailActionsRecoverPatch) | **PATCH** /rest/mail/actions/recover | Moves the list of emails back to original bucket from trash
[**restMailActionsSendFileExternalPost**](MailApi.md#restMailActionsSendFileExternalPost) | **POST** /rest/mail/actions/sendFileExternal | Create a mail
[**restMailActionsSendFilePost**](MailApi.md#restMailActionsSendFilePost) | **POST** /rest/mail/actions/sendFile | Create a mail
[**restMailActionsTrashPatch**](MailApi.md#restMailActionsTrashPatch) | **PATCH** /rest/mail/actions/trash | Moves the list of emails to trash for current user
[**restMailActionsUnreadPatch**](MailApi.md#restMailActionsUnreadPatch) | **PATCH** /rest/mail/actions/unread | Mark the mail read status to false on the given email ids
[**restMailActionsWithdrawFilesUsersUserIdDelete**](MailApi.md#restMailActionsWithdrawFilesUsersUserIdDelete) | **DELETE** /rest/mail/actions/withdrawFiles/users/{userId} | Withdraw all files from deleted/demoted users&#39; emails
[**restMailAttachmentsDelete**](MailApi.md#restMailAttachmentsDelete) | **DELETE** /rest/mail/attachments | Delete attachment(s)
[**restMailAttachmentsGet**](MailApi.md#restMailAttachmentsGet) | **GET** /rest/mail/attachments | Get email attachments
[**restMailDelete**](MailApi.md#restMailDelete) | **DELETE** /rest/mail | Delete a list of email drafts
[**restMailEmailIdAttachmentsActionsZipGet**](MailApi.md#restMailEmailIdAttachmentsActionsZipGet) | **GET** /rest/mail/{emailId}/attachments/actions/zip | Download multiple attachments as zip
[**restMailEmailIdAttachmentsActionsZipStatusGet**](MailApi.md#restMailEmailIdAttachmentsActionsZipStatusGet) | **GET** /rest/mail/{emailId}/attachments/actions/zipStatus | Get multiple attachments AV/DLP status
[**restMailEmailIdAttachmentsIdContentGet**](MailApi.md#restMailEmailIdAttachmentsIdContentGet) | **GET** /rest/mail/{emailId}/attachments/{id}/content | Return attachment content
[**restMailEmailIdAttachmentsIdPreviewGet**](MailApi.md#restMailEmailIdAttachmentsIdPreviewGet) | **GET** /rest/mail/{emailId}/attachments/{id}/preview | Retrieve information about the file preview of given email.
[**restMailEmailIdAttachmentsReportCsvGet**](MailApi.md#restMailEmailIdAttachmentsReportCsvGet) | **GET** /rest/mail/{emailId}/attachments/reportCsv | Get a report about downloaded attachments as a CSV file
[**restMailEmailIdAttachmentsReportGet**](MailApi.md#restMailEmailIdAttachmentsReportGet) | **GET** /rest/mail/{emailId}/attachments/report | Get a report about downloaded attachments
[**restMailGet**](MailApi.md#restMailGet) | **GET** /rest/mail | List emails
[**restMailIdActionsCopyPost**](MailApi.md#restMailIdActionsCopyPost) | **POST** /rest/mail/{id}/actions/copy | Copy attachments from mail to folder
[**restMailIdActionsSendFileExternalPut**](MailApi.md#restMailIdActionsSendFileExternalPut) | **PUT** /rest/mail/{id}/actions/sendFileExternal | Update a mail
[**restMailIdActionsSendFilePut**](MailApi.md#restMailIdActionsSendFilePut) | **PUT** /rest/mail/{id}/actions/sendFile | Update a mail
[**restMailIdActionsSendTrackingReportPost**](MailApi.md#restMailIdActionsSendTrackingReportPost) | **POST** /rest/mail/{id}/actions/sendTrackingReport | Send tracking report for email
[**restMailIdActionsWithdrawFilesPost**](MailApi.md#restMailIdActionsWithdrawFilesPost) | **POST** /rest/mail/{id}/actions/withdrawFiles | Withdraw attachments from mail
[**restMailIdAttachmentsAttachmentIdGet**](MailApi.md#restMailIdAttachmentsAttachmentIdGet) | **GET** /rest/mail/{id}/attachments/{attachment_id} | Returns a list of attachments for a given mail.
[**restMailIdAttachmentsGet**](MailApi.md#restMailIdAttachmentsGet) | **GET** /rest/mail/{id}/attachments | Returns a list of attachments for a given mail.
[**restMailIdDelete**](MailApi.md#restMailIdDelete) | **DELETE** /rest/mail/{id} | Delete an email draft
[**restMailIdGet**](MailApi.md#restMailIdGet) | **GET** /rest/mail/{id} | Get an email entry
[**restMailIdPackagesGet**](MailApi.md#restMailIdPackagesGet) | **GET** /rest/mail/{id}/packages | List email packages
[**restMailIdRecipientsGet**](MailApi.md#restMailIdRecipientsGet) | **GET** /rest/mail/{id}/recipients | List recipients
[**restMailIdScanStatusGet**](MailApi.md#restMailIdScanStatusGet) | **GET** /rest/mail/{id}/scanStatus | Get the status of a mail job based on attachment and content scan status.
[**restMailIdSettingsPut**](MailApi.md#restMailIdSettingsPut) | **PUT** /rest/mail/{id}/settings | Allow sender to update the mail setting of an email.
[**restMailIdTrackingsMeDelete**](MailApi.md#restMailIdTrackingsMeDelete) | **DELETE** /rest/mail/{id}/trackings/me | Unsubscribe user from tracking
[**restPublicMailActionsSendFilePost**](MailApi.md#restPublicMailActionsSendFilePost) | **POST** /rest/public/mail/actions/sendFile | Create a mail
[**restPublicMailIdActionsSendFilePut**](MailApi.md#restPublicMailIdActionsSendFilePut) | **PUT** /rest/public/mail/{id}/actions/sendFile | Update a mail


<a id="restFoldersIdActionsSendMessagePost"></a>
# **restFoldersIdActionsSendMessagePost**
> restFoldersIdActionsSendMessagePost(id, body, returnEntity, mode)

Create a send message email entry

Creates a send message email entry

### Example
```kotlin
// Import classes:
//import org.openapitools.client.infrastructure.*
//import org.openapitools.client.models.*

val apiInstance = MailApi()
val id : kotlin.String = id_example // kotlin.String | ID of the folder
val body : SendMessagePost =  // SendMessagePost | The email details
val returnEntity : kotlin.Boolean = true // kotlin.Boolean | Return information about newly created entity
val mode : kotlin.String = mode_example // kotlin.String | Response mode
try {
    apiInstance.restFoldersIdActionsSendMessagePost(id, body, returnEntity, mode)
} catch (e: ClientException) {
    println("4xx response calling MailApi#restFoldersIdActionsSendMessagePost")
    e.printStackTrace()
} catch (e: ServerException) {
    println("5xx response calling MailApi#restFoldersIdActionsSendMessagePost")
    e.printStackTrace()
}
```

### Parameters

Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **id** | **kotlin.String**| ID of the folder |
 **body** | [**SendMessagePost**](SendMessagePost.md)| The email details |
 **returnEntity** | **kotlin.Boolean**| Return information about newly created entity | [optional]
 **mode** | **kotlin.String**| Response mode | [optional]

### Return type

null (empty response body)

### Authorization

No authorization required

### HTTP request headers

 - **Content-Type**: Not defined
 - **Accept**: Not defined

<a id="restMailActionsCountersGet"></a>
# **restMailActionsCountersGet**
> MailCounters restMailActionsCountersGet(returnCustomWebForm)

Returns number of emails in each bucket

Returns number of emails in each bucket

### Example
```kotlin
// Import classes:
//import org.openapitools.client.infrastructure.*
//import org.openapitools.client.models.*

val apiInstance = MailApi()
val returnCustomWebForm : kotlin.Boolean = true // kotlin.Boolean | Return all emails include those with the custom web form.
try {
    val result : MailCounters = apiInstance.restMailActionsCountersGet(returnCustomWebForm)
    println(result)
} catch (e: ClientException) {
    println("4xx response calling MailApi#restMailActionsCountersGet")
    e.printStackTrace()
} catch (e: ServerException) {
    println("5xx response calling MailApi#restMailActionsCountersGet")
    e.printStackTrace()
}
```

### Parameters

Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **returnCustomWebForm** | **kotlin.Boolean**| Return all emails include those with the custom web form. | [optional]

### Return type

[**MailCounters**](MailCounters.md)

### Authorization

No authorization required

### HTTP request headers

 - **Content-Type**: Not defined
 - **Accept**: */*

<a id="restMailActionsDeletePermanentPatch"></a>
# **restMailActionsDeletePermanentPatch**
> restMailActionsDeletePermanentPatch(emailIdColonIn, partialSuccess)

Permanently deletes list of emails

Permanently deletes list of emails

### Example
```kotlin
// Import classes:
//import org.openapitools.client.infrastructure.*
//import org.openapitools.client.models.*

val apiInstance = MailApi()
val emailIdColonIn : kotlin.collections.List<kotlin.String> =  // kotlin.collections.List<kotlin.String> | A list of email ids which will be processed
val partialSuccess : kotlin.Boolean = true // kotlin.Boolean | Whether to perform action on valid items even if some ones fail
try {
    apiInstance.restMailActionsDeletePermanentPatch(emailIdColonIn, partialSuccess)
} catch (e: ClientException) {
    println("4xx response calling MailApi#restMailActionsDeletePermanentPatch")
    e.printStackTrace()
} catch (e: ServerException) {
    println("5xx response calling MailApi#restMailActionsDeletePermanentPatch")
    e.printStackTrace()
}
```

### Parameters

Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **emailIdColonIn** | [**kotlin.collections.List&lt;kotlin.String&gt;**](kotlin.String.md)| A list of email ids which will be processed |
 **partialSuccess** | **kotlin.Boolean**| Whether to perform action on valid items even if some ones fail | [optional]

### Return type

null (empty response body)

### Authorization

No authorization required

### HTTP request headers

 - **Content-Type**: Not defined
 - **Accept**: */*

<a id="restMailActionsDistributionListGet"></a>
# **restMailActionsDistributionListGet**
> DistributionList restMailActionsDistributionListGet(email, expand, emailId)

Returns list of emails inside distribution list

Returns list of emails inside distribution list

### Example
```kotlin
// Import classes:
//import org.openapitools.client.infrastructure.*
//import org.openapitools.client.models.*

val apiInstance = MailApi()
val email : kotlin.String = email_example // kotlin.String | Email address to check/expand
val expand : kotlin.Boolean = true // kotlin.Boolean | Whether to return distribution list members emails
val emailId : kotlin.String = emailId_example // kotlin.String | If specified, DL members list will contain members who actually received this email
try {
    val result : DistributionList = apiInstance.restMailActionsDistributionListGet(email, expand, emailId)
    println(result)
} catch (e: ClientException) {
    println("4xx response calling MailApi#restMailActionsDistributionListGet")
    e.printStackTrace()
} catch (e: ServerException) {
    println("5xx response calling MailApi#restMailActionsDistributionListGet")
    e.printStackTrace()
}
```

### Parameters

Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **email** | **kotlin.String**| Email address to check/expand |
 **expand** | **kotlin.Boolean**| Whether to return distribution list members emails | [optional]
 **emailId** | **kotlin.String**| If specified, DL members list will contain members who actually received this email | [optional]

### Return type

[**DistributionList**](DistributionList.md)

### Authorization

No authorization required

### HTTP request headers

 - **Content-Type**: Not defined
 - **Accept**: */*

<a id="restMailActionsReadPatch"></a>
# **restMailActionsReadPatch**
> restMailActionsReadPatch(emailIdColonIn, partialSuccess)

Mark the mail read status to true on the given email ids

Mark the mail read status to true on the given email ids

### Example
```kotlin
// Import classes:
//import org.openapitools.client.infrastructure.*
//import org.openapitools.client.models.*

val apiInstance = MailApi()
val emailIdColonIn : kotlin.collections.List<kotlin.String> =  // kotlin.collections.List<kotlin.String> | A list of email ids which will be processed
val partialSuccess : kotlin.Boolean = true // kotlin.Boolean | Whether to perform action on valid items even if some ones fail
try {
    apiInstance.restMailActionsReadPatch(emailIdColonIn, partialSuccess)
} catch (e: ClientException) {
    println("4xx response calling MailApi#restMailActionsReadPatch")
    e.printStackTrace()
} catch (e: ServerException) {
    println("5xx response calling MailApi#restMailActionsReadPatch")
    e.printStackTrace()
}
```

### Parameters

Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **emailIdColonIn** | [**kotlin.collections.List&lt;kotlin.String&gt;**](kotlin.String.md)| A list of email ids which will be processed |
 **partialSuccess** | **kotlin.Boolean**| Whether to perform action on valid items even if some ones fail | [optional]

### Return type

null (empty response body)

### Authorization

No authorization required

### HTTP request headers

 - **Content-Type**: Not defined
 - **Accept**: */*

<a id="restMailActionsRecoverPatch"></a>
# **restMailActionsRecoverPatch**
> restMailActionsRecoverPatch(emailIdColonIn, partialSuccess)

Moves the list of emails back to original bucket from trash

Moves the list of emails back to original bucket from trash

### Example
```kotlin
// Import classes:
//import org.openapitools.client.infrastructure.*
//import org.openapitools.client.models.*

val apiInstance = MailApi()
val emailIdColonIn : kotlin.collections.List<kotlin.String> =  // kotlin.collections.List<kotlin.String> | A list of email ids which will be processed
val partialSuccess : kotlin.Boolean = true // kotlin.Boolean | Whether to perform action on valid items even if some ones fail
try {
    apiInstance.restMailActionsRecoverPatch(emailIdColonIn, partialSuccess)
} catch (e: ClientException) {
    println("4xx response calling MailApi#restMailActionsRecoverPatch")
    e.printStackTrace()
} catch (e: ServerException) {
    println("5xx response calling MailApi#restMailActionsRecoverPatch")
    e.printStackTrace()
}
```

### Parameters

Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **emailIdColonIn** | [**kotlin.collections.List&lt;kotlin.String&gt;**](kotlin.String.md)| A list of email ids which will be processed |
 **partialSuccess** | **kotlin.Boolean**| Whether to perform action on valid items even if some ones fail | [optional]

### Return type

null (empty response body)

### Authorization

No authorization required

### HTTP request headers

 - **Content-Type**: Not defined
 - **Accept**: */*

<a id="restMailActionsSendFileExternalPost"></a>
# **restMailActionsSendFileExternalPost**
> Mail restMailActionsSendFileExternalPost(body, mode, with, returnEntity)

Create a mail

Create a mail

### Example
```kotlin
// Import classes:
//import org.openapitools.client.infrastructure.*
//import org.openapitools.client.models.*

val apiInstance = MailApi()
val body : BaseSendMailPostRequest =  // BaseSendMailPostRequest | 
val mode : kotlin.String = mode_example // kotlin.String | 
val with : kotlin.String = with_example // kotlin.String | 
val returnEntity : kotlin.Boolean = true // kotlin.Boolean | 
try {
    val result : Mail = apiInstance.restMailActionsSendFileExternalPost(body, mode, with, returnEntity)
    println(result)
} catch (e: ClientException) {
    println("4xx response calling MailApi#restMailActionsSendFileExternalPost")
    e.printStackTrace()
} catch (e: ServerException) {
    println("5xx response calling MailApi#restMailActionsSendFileExternalPost")
    e.printStackTrace()
}
```

### Parameters

Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **body** | [**BaseSendMailPostRequest**](BaseSendMailPostRequest.md)|  |
 **mode** | **kotlin.String**|  | [optional]
 **with** | **kotlin.String**|  | [optional]
 **returnEntity** | **kotlin.Boolean**|  | [optional]

### Return type

[**Mail**](Mail.md)

### Authorization

No authorization required

### HTTP request headers

 - **Content-Type**: Not defined
 - **Accept**: */*

<a id="restMailActionsSendFilePost"></a>
# **restMailActionsSendFilePost**
> Mail restMailActionsSendFilePost(body, mode, with, returnEntity)

Create a mail

Create a mail

### Example
```kotlin
// Import classes:
//import org.openapitools.client.infrastructure.*
//import org.openapitools.client.models.*

val apiInstance = MailApi()
val body : BaseSendMailPostRequest =  // BaseSendMailPostRequest | 
val mode : kotlin.String = mode_example // kotlin.String | 
val with : kotlin.String = with_example // kotlin.String | 
val returnEntity : kotlin.Boolean = true // kotlin.Boolean | 
try {
    val result : Mail = apiInstance.restMailActionsSendFilePost(body, mode, with, returnEntity)
    println(result)
} catch (e: ClientException) {
    println("4xx response calling MailApi#restMailActionsSendFilePost")
    e.printStackTrace()
} catch (e: ServerException) {
    println("5xx response calling MailApi#restMailActionsSendFilePost")
    e.printStackTrace()
}
```

### Parameters

Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **body** | [**BaseSendMailPostRequest**](BaseSendMailPostRequest.md)|  |
 **mode** | **kotlin.String**|  | [optional]
 **with** | **kotlin.String**|  | [optional]
 **returnEntity** | **kotlin.Boolean**|  | [optional]

### Return type

[**Mail**](Mail.md)

### Authorization

No authorization required

### HTTP request headers

 - **Content-Type**: Not defined
 - **Accept**: */*

<a id="restMailActionsTrashPatch"></a>
# **restMailActionsTrashPatch**
> restMailActionsTrashPatch(emailIdColonIn, partialSuccess)

Moves the list of emails to trash for current user

Moves the list of emails to trash for current user

### Example
```kotlin
// Import classes:
//import org.openapitools.client.infrastructure.*
//import org.openapitools.client.models.*

val apiInstance = MailApi()
val emailIdColonIn : kotlin.collections.List<kotlin.String> =  // kotlin.collections.List<kotlin.String> | A list of email ids which will be processed
val partialSuccess : kotlin.Boolean = true // kotlin.Boolean | Whether to perform action on valid items even if some ones fail
try {
    apiInstance.restMailActionsTrashPatch(emailIdColonIn, partialSuccess)
} catch (e: ClientException) {
    println("4xx response calling MailApi#restMailActionsTrashPatch")
    e.printStackTrace()
} catch (e: ServerException) {
    println("5xx response calling MailApi#restMailActionsTrashPatch")
    e.printStackTrace()
}
```

### Parameters

Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **emailIdColonIn** | [**kotlin.collections.List&lt;kotlin.String&gt;**](kotlin.String.md)| A list of email ids which will be processed |
 **partialSuccess** | **kotlin.Boolean**| Whether to perform action on valid items even if some ones fail | [optional]

### Return type

null (empty response body)

### Authorization

No authorization required

### HTTP request headers

 - **Content-Type**: Not defined
 - **Accept**: */*

<a id="restMailActionsUnreadPatch"></a>
# **restMailActionsUnreadPatch**
> restMailActionsUnreadPatch(emailIdColonIn, partialSuccess)

Mark the mail read status to false on the given email ids

Mark the mail read status to false on the given email ids

### Example
```kotlin
// Import classes:
//import org.openapitools.client.infrastructure.*
//import org.openapitools.client.models.*

val apiInstance = MailApi()
val emailIdColonIn : kotlin.collections.List<kotlin.String> =  // kotlin.collections.List<kotlin.String> | A list of email ids which will be processed
val partialSuccess : kotlin.Boolean = true // kotlin.Boolean | Whether to perform action on valid items even if some ones fail
try {
    apiInstance.restMailActionsUnreadPatch(emailIdColonIn, partialSuccess)
} catch (e: ClientException) {
    println("4xx response calling MailApi#restMailActionsUnreadPatch")
    e.printStackTrace()
} catch (e: ServerException) {
    println("5xx response calling MailApi#restMailActionsUnreadPatch")
    e.printStackTrace()
}
```

### Parameters

Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **emailIdColonIn** | [**kotlin.collections.List&lt;kotlin.String&gt;**](kotlin.String.md)| A list of email ids which will be processed |
 **partialSuccess** | **kotlin.Boolean**| Whether to perform action on valid items even if some ones fail | [optional]

### Return type

null (empty response body)

### Authorization

No authorization required

### HTTP request headers

 - **Content-Type**: Not defined
 - **Accept**: */*

<a id="restMailActionsWithdrawFilesUsersUserIdDelete"></a>
# **restMailActionsWithdrawFilesUsersUserIdDelete**
> restMailActionsWithdrawFilesUsersUserIdDelete(userId, emailIdColonIn, partialSuccess, mode)

Withdraw all files from deleted/demoted users&#39; emails

Withdraw all files from deleted/demoted users&#39; emails

### Example
```kotlin
// Import classes:
//import org.openapitools.client.infrastructure.*
//import org.openapitools.client.models.*

val apiInstance = MailApi()
val userId : kotlin.String = userId_example // kotlin.String | ID of the user to withdraw files
val emailIdColonIn : kotlin.String = emailIdColonIn_example // kotlin.String | A list of email ids which will be processed
val partialSuccess : kotlin.Boolean = true // kotlin.Boolean | Whether to perform action on valid items even if some ones fail
val mode : kotlin.String = mode_example // kotlin.String | Response mode
try {
    apiInstance.restMailActionsWithdrawFilesUsersUserIdDelete(userId, emailIdColonIn, partialSuccess, mode)
} catch (e: ClientException) {
    println("4xx response calling MailApi#restMailActionsWithdrawFilesUsersUserIdDelete")
    e.printStackTrace()
} catch (e: ServerException) {
    println("5xx response calling MailApi#restMailActionsWithdrawFilesUsersUserIdDelete")
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

<a id="restMailAttachmentsDelete"></a>
# **restMailAttachmentsDelete**
> restMailAttachmentsDelete(idColonIn)

Delete attachment(s)

Delete email attachment(s) from sent &amp; draft mail

### Example
```kotlin
// Import classes:
//import org.openapitools.client.infrastructure.*
//import org.openapitools.client.models.*

val apiInstance = MailApi()
val idColonIn : kotlin.collections.List<kotlin.String> =  // kotlin.collections.List<kotlin.String> | 
try {
    apiInstance.restMailAttachmentsDelete(idColonIn)
} catch (e: ClientException) {
    println("4xx response calling MailApi#restMailAttachmentsDelete")
    e.printStackTrace()
} catch (e: ServerException) {
    println("5xx response calling MailApi#restMailAttachmentsDelete")
    e.printStackTrace()
}
```

### Parameters

Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **idColonIn** | [**kotlin.collections.List&lt;kotlin.String&gt;**](kotlin.String.md)|  |

### Return type

null (empty response body)

### Authorization

No authorization required

### HTTP request headers

 - **Content-Type**: Not defined
 - **Accept**: Not defined

<a id="restMailAttachmentsGet"></a>
# **restMailAttachmentsGet**
> MailAttachments restMailAttachmentsGet(orderBy, limit, offset, bucket)

Get email attachments

Get email attachments from sent &amp; draft mail

### Example
```kotlin
// Import classes:
//import org.openapitools.client.infrastructure.*
//import org.openapitools.client.models.*

val apiInstance = MailApi()
val orderBy : kotlin.String = orderBy_example // kotlin.String | 
val limit : kotlin.Int = 56 // kotlin.Int | 
val offset : kotlin.Int = 56 // kotlin.Int | 
val bucket : kotlin.String = bucket_example // kotlin.String | 
try {
    val result : MailAttachments = apiInstance.restMailAttachmentsGet(orderBy, limit, offset, bucket)
    println(result)
} catch (e: ClientException) {
    println("4xx response calling MailApi#restMailAttachmentsGet")
    e.printStackTrace()
} catch (e: ServerException) {
    println("5xx response calling MailApi#restMailAttachmentsGet")
    e.printStackTrace()
}
```

### Parameters

Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **orderBy** | **kotlin.String**|  | [optional]
 **limit** | **kotlin.Int**|  | [optional]
 **offset** | **kotlin.Int**|  | [optional]
 **bucket** | **kotlin.String**|  | [optional]

### Return type

[**MailAttachments**](MailAttachments.md)

### Authorization

No authorization required

### HTTP request headers

 - **Content-Type**: Not defined
 - **Accept**: */*

<a id="restMailDelete"></a>
# **restMailDelete**
> restMailDelete(emailIdColonIn, partialSuccess)

Delete a list of email drafts

Allows a sender to delete a list of email drafts (Support up to 100 emails)

### Example
```kotlin
// Import classes:
//import org.openapitools.client.infrastructure.*
//import org.openapitools.client.models.*

val apiInstance = MailApi()
val emailIdColonIn : kotlin.collections.List<kotlin.String> =  // kotlin.collections.List<kotlin.String> | A list of email ids which will be processed
val partialSuccess : kotlin.Boolean = true // kotlin.Boolean | Whether to perform action on valid items even if some ones fail
try {
    apiInstance.restMailDelete(emailIdColonIn, partialSuccess)
} catch (e: ClientException) {
    println("4xx response calling MailApi#restMailDelete")
    e.printStackTrace()
} catch (e: ServerException) {
    println("5xx response calling MailApi#restMailDelete")
    e.printStackTrace()
}
```

### Parameters

Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **emailIdColonIn** | [**kotlin.collections.List&lt;kotlin.String&gt;**](kotlin.String.md)| A list of email ids which will be processed |
 **partialSuccess** | **kotlin.Boolean**| Whether to perform action on valid items even if some ones fail | [optional]

### Return type

null (empty response body)

### Authorization

No authorization required

### HTTP request headers

 - **Content-Type**: Not defined
 - **Accept**: Not defined

<a id="restMailEmailIdAttachmentsActionsZipGet"></a>
# **restMailEmailIdAttachmentsActionsZipGet**
> restMailEmailIdAttachmentsActionsZipGet(emailId, attachmentIdColonIn, name, ref, username, utcOffset, mode)

Download multiple attachments as zip

Download multiple attachments as zip

### Example
```kotlin
// Import classes:
//import org.openapitools.client.infrastructure.*
//import org.openapitools.client.models.*

val apiInstance = MailApi()
val emailId : kotlin.String = emailId_example // kotlin.String | Mail id to download attachments as zip
val attachmentIdColonIn : kotlin.String = attachmentIdColonIn_example // kotlin.String | Search for results that contain any of specified values of this parameter.
val name : kotlin.String = name_example // kotlin.String | The zip filename
val ref : kotlin.String = ref_example // kotlin.String | The email reference (Mandatory if the email can be accessed without authentication)
val username : kotlin.String = username_example // kotlin.String | User email of file's requestor
val utcOffset : kotlin.Int = 56 // kotlin.Int | The user timezone offset in (seconds). UTC+08:00 = 28800
val mode : kotlin.String = mode_example // kotlin.String | Response mode
try {
    apiInstance.restMailEmailIdAttachmentsActionsZipGet(emailId, attachmentIdColonIn, name, ref, username, utcOffset, mode)
} catch (e: ClientException) {
    println("4xx response calling MailApi#restMailEmailIdAttachmentsActionsZipGet")
    e.printStackTrace()
} catch (e: ServerException) {
    println("5xx response calling MailApi#restMailEmailIdAttachmentsActionsZipGet")
    e.printStackTrace()
}
```

### Parameters

Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **emailId** | **kotlin.String**| Mail id to download attachments as zip |
 **attachmentIdColonIn** | **kotlin.String**| Search for results that contain any of specified values of this parameter. |
 **name** | **kotlin.String**| The zip filename | [optional]
 **ref** | **kotlin.String**| The email reference (Mandatory if the email can be accessed without authentication) | [optional]
 **username** | **kotlin.String**| User email of file&#39;s requestor | [optional]
 **utcOffset** | **kotlin.Int**| The user timezone offset in (seconds). UTC+08:00 &#x3D; 28800 | [optional]
 **mode** | **kotlin.String**| Response mode | [optional]

### Return type

null (empty response body)

### Authorization

No authorization required

### HTTP request headers

 - **Content-Type**: Not defined
 - **Accept**: Not defined

<a id="restMailEmailIdAttachmentsActionsZipStatusGet"></a>
# **restMailEmailIdAttachmentsActionsZipStatusGet**
> restMailEmailIdAttachmentsActionsZipStatusGet(emailId, attachmentIdColonIn, ref, mode)

Get multiple attachments AV/DLP status

Get multiple attachments AV/DLP status

### Example
```kotlin
// Import classes:
//import org.openapitools.client.infrastructure.*
//import org.openapitools.client.models.*

val apiInstance = MailApi()
val emailId : kotlin.String = emailId_example // kotlin.String | The mail id
val attachmentIdColonIn : kotlin.String = attachmentIdColonIn_example // kotlin.String | Search for results that contain any of specified values of this parameter.
val ref : kotlin.String = ref_example // kotlin.String | The email reference (Mandatory if the email can be accessed without authentication)
val mode : kotlin.String = mode_example // kotlin.String | Response mode
try {
    apiInstance.restMailEmailIdAttachmentsActionsZipStatusGet(emailId, attachmentIdColonIn, ref, mode)
} catch (e: ClientException) {
    println("4xx response calling MailApi#restMailEmailIdAttachmentsActionsZipStatusGet")
    e.printStackTrace()
} catch (e: ServerException) {
    println("5xx response calling MailApi#restMailEmailIdAttachmentsActionsZipStatusGet")
    e.printStackTrace()
}
```

### Parameters

Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **emailId** | **kotlin.String**| The mail id |
 **attachmentIdColonIn** | **kotlin.String**| Search for results that contain any of specified values of this parameter. |
 **ref** | **kotlin.String**| The email reference (Mandatory if the email can be accessed without authentication) | [optional]
 **mode** | **kotlin.String**| Response mode | [optional]

### Return type

null (empty response body)

### Authorization

No authorization required

### HTTP request headers

 - **Content-Type**: Not defined
 - **Accept**: Not defined

<a id="restMailEmailIdAttachmentsIdContentGet"></a>
# **restMailEmailIdAttachmentsIdContentGet**
> restMailEmailIdAttachmentsIdContentGet(emailId, id, range, ref, mode)

Return attachment content

Returns the content of the specified attachment.                        e.g: return the file in this email attachment.

### Example
```kotlin
// Import classes:
//import org.openapitools.client.infrastructure.*
//import org.openapitools.client.models.*

val apiInstance = MailApi()
val emailId : kotlin.String = emailId_example // kotlin.String | Mail id to retrieve attachment content for
val id : kotlin.String = id_example // kotlin.String | Attachment id (frozen object id)
val range : kotlin.String = range_example // kotlin.String | Bytes range to retrieve. Example: bytes=0-1024
val ref : kotlin.String = ref_example // kotlin.String | The email reference code (Mandatory if the email can be accessed without authentication)
val mode : kotlin.String = mode_example // kotlin.String | Response mode
try {
    apiInstance.restMailEmailIdAttachmentsIdContentGet(emailId, id, range, ref, mode)
} catch (e: ClientException) {
    println("4xx response calling MailApi#restMailEmailIdAttachmentsIdContentGet")
    e.printStackTrace()
} catch (e: ServerException) {
    println("5xx response calling MailApi#restMailEmailIdAttachmentsIdContentGet")
    e.printStackTrace()
}
```

### Parameters

Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **emailId** | **kotlin.String**| Mail id to retrieve attachment content for |
 **id** | **kotlin.String**| Attachment id (frozen object id) |
 **range** | **kotlin.String**| Bytes range to retrieve. Example: bytes&#x3D;0-1024 | [optional]
 **ref** | **kotlin.String**| The email reference code (Mandatory if the email can be accessed without authentication) | [optional]
 **mode** | **kotlin.String**| Response mode | [optional]

### Return type

null (empty response body)

### Authorization

No authorization required

### HTTP request headers

 - **Content-Type**: Not defined
 - **Accept**: Not defined

<a id="restMailEmailIdAttachmentsIdPreviewGet"></a>
# **restMailEmailIdAttachmentsIdPreviewGet**
> Preview restMailEmailIdAttachmentsIdPreviewGet(emailId, id, ref, mode)

Retrieve information about the file preview of given email.

Retrieve information about the file preview of given email.

### Example
```kotlin
// Import classes:
//import org.openapitools.client.infrastructure.*
//import org.openapitools.client.models.*

val apiInstance = MailApi()
val emailId : kotlin.String = emailId_example // kotlin.String | Mail id to retrieve attachments for
val id : kotlin.String = id_example // kotlin.String | Attachment id (frozen object id)
val ref : kotlin.String = ref_example // kotlin.String | The email reference code (Mandatory if the email can be accessed without authentication)
val mode : kotlin.String = mode_example // kotlin.String | Response mode
try {
    val result : Preview = apiInstance.restMailEmailIdAttachmentsIdPreviewGet(emailId, id, ref, mode)
    println(result)
} catch (e: ClientException) {
    println("4xx response calling MailApi#restMailEmailIdAttachmentsIdPreviewGet")
    e.printStackTrace()
} catch (e: ServerException) {
    println("5xx response calling MailApi#restMailEmailIdAttachmentsIdPreviewGet")
    e.printStackTrace()
}
```

### Parameters

Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **emailId** | **kotlin.String**| Mail id to retrieve attachments for |
 **id** | **kotlin.String**| Attachment id (frozen object id) |
 **ref** | **kotlin.String**| The email reference code (Mandatory if the email can be accessed without authentication) | [optional]
 **mode** | **kotlin.String**| Response mode | [optional]

### Return type

[**Preview**](Preview.md)

### Authorization

No authorization required

### HTTP request headers

 - **Content-Type**: Not defined
 - **Accept**: */*

<a id="restMailEmailIdAttachmentsReportCsvGet"></a>
# **restMailEmailIdAttachmentsReportCsvGet**
> restMailEmailIdAttachmentsReportCsvGet(emailId)

Get a report about downloaded attachments as a CSV file

Get a report about downloaded attachments as a CSV file

### Example
```kotlin
// Import classes:
//import org.openapitools.client.infrastructure.*
//import org.openapitools.client.models.*

val apiInstance = MailApi()
val emailId : kotlin.String = emailId_example // kotlin.String | The mail id
try {
    apiInstance.restMailEmailIdAttachmentsReportCsvGet(emailId)
} catch (e: ClientException) {
    println("4xx response calling MailApi#restMailEmailIdAttachmentsReportCsvGet")
    e.printStackTrace()
} catch (e: ServerException) {
    println("5xx response calling MailApi#restMailEmailIdAttachmentsReportCsvGet")
    e.printStackTrace()
}
```

### Parameters

Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **emailId** | **kotlin.String**| The mail id |

### Return type

null (empty response body)

### Authorization

No authorization required

### HTTP request headers

 - **Content-Type**: Not defined
 - **Accept**: Not defined

<a id="restMailEmailIdAttachmentsReportGet"></a>
# **restMailEmailIdAttachmentsReportGet**
> restMailEmailIdAttachmentsReportGet(emailId)

Get a report about downloaded attachments

Get a report about downloaded attachments

### Example
```kotlin
// Import classes:
//import org.openapitools.client.infrastructure.*
//import org.openapitools.client.models.*

val apiInstance = MailApi()
val emailId : kotlin.String = emailId_example // kotlin.String | The mail id
try {
    apiInstance.restMailEmailIdAttachmentsReportGet(emailId)
} catch (e: ClientException) {
    println("4xx response calling MailApi#restMailEmailIdAttachmentsReportGet")
    e.printStackTrace()
} catch (e: ServerException) {
    println("5xx response calling MailApi#restMailEmailIdAttachmentsReportGet")
    e.printStackTrace()
}
```

### Parameters

Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **emailId** | **kotlin.String**| The mail id |

### Return type

null (empty response body)

### Authorization

No authorization required

### HTTP request headers

 - **Content-Type**: Not defined
 - **Accept**: Not defined

<a id="restMailGet"></a>
# **restMailGet**
> Mails restMailGet(isRecipient, modifiedDateColonLte, mode, sharedMailboxId, trackingOnly, senderId, read, isPreview, returnCustomWebForm, dateColonGte, isUserSent, modifiedDateColonGt, templateId, orderBy, returnEntity, modifiedDateColonLt, status, emailPackageIdColonIn, date, with, limit, emailPackageId, modifiedDate, webFormId, dateColonGt, modifiedDateColonGte, senderIdColonIn, deleted, dateColonLte, customWebFormOnly, templateIdColonIn, dateColonLt, bucket, offset)

List emails

Returns the list of all emails for this user.  This includes sent emails, received emails,draft emails, and request a file emails. 

### Example
```kotlin
// Import classes:
//import org.openapitools.client.infrastructure.*
//import org.openapitools.client.models.*

val apiInstance = MailApi()
val isRecipient : kotlin.Boolean = true // kotlin.Boolean | Unique identifier of User who receive Email
val modifiedDateColonLte : kotlin.String = modifiedDateColonLte_example // kotlin.String | Email modified date. Search for result that has this parameter value less or equal to the specified.
val mode : kotlin.String = mode_example // kotlin.String | 
val sharedMailboxId : kotlin.String = sharedMailboxId_example // kotlin.String | Shared Mailbox unique identifier. Search for result belongs to the Shared Mailbox.
val trackingOnly : kotlin.Boolean = true // kotlin.Boolean | Return only emails with tracking access
val senderId : kotlin.String = senderId_example // kotlin.String | Unique identifier of User who sent Email
val read : kotlin.Boolean = true // kotlin.Boolean | Whether the email is read or not by current user
val isPreview : kotlin.Boolean = true // kotlin.Boolean | Whether the email is a preview email
val returnCustomWebForm : kotlin.Boolean = true // kotlin.Boolean | Return all emails include those with the custom web form
val dateColonGte : kotlin.String = dateColonGte_example // kotlin.String | Email creation date. Search for result that has this parameter value greater or equal to the specified.
val isUserSent : kotlin.Boolean = true // kotlin.Boolean | Whether the email was sent by some user
val modifiedDateColonGt : kotlin.String = modifiedDateColonGt_example // kotlin.String | Email modified date. Search for result that has this parameter value greater than specified.
val templateId : kotlin.Int = 56 // kotlin.Int | Email Template unique identifier
val orderBy : kotlin.String = orderBy_example // kotlin.String | Sorting options
val returnEntity : kotlin.Boolean = true // kotlin.Boolean | 
val modifiedDateColonLt : kotlin.String = modifiedDateColonLt_example // kotlin.String | Email modified date. Search for result that has this parameter value less than specified.
val status : kotlin.String = status_example // kotlin.String | Email status
val emailPackageIdColonIn : kotlin.collections.List<kotlin.String> =  // kotlin.collections.List<kotlin.String> | Email Package unique identifier. Search for results that contain any of specified values of this parameter.
val date : kotlin.String = date_example // kotlin.String | Email creation date
val with : kotlin.String = with_example // kotlin.String | 
val limit : kotlin.Int = 56 // kotlin.Int | 
val emailPackageId : kotlin.String = emailPackageId_example // kotlin.String | Email Package unique identifier
val modifiedDate : kotlin.String = modifiedDate_example // kotlin.String | Email modified date
val webFormId : kotlin.String = webFormId_example // kotlin.String | Email web form ID
val dateColonGt : kotlin.String = dateColonGt_example // kotlin.String | Email creation date. Search for result that has this parameter value greater than specified.
val modifiedDateColonGte : kotlin.String = modifiedDateColonGte_example // kotlin.String | Email modified date. Search for result that has this parameter value greater or equal to the specified.
val senderIdColonIn : kotlin.collections.List<kotlin.String> =  // kotlin.collections.List<kotlin.String> | Unique identifier of User who sent Email Search for results that contain any of specified values of this parameter.recommended request size <= 100
val deleted : kotlin.Boolean = true // kotlin.Boolean | Indicates that Email is deleted
val dateColonLte : kotlin.String = dateColonLte_example // kotlin.String | Email creation date. Search for result that has this parameter value less or equal to the specified.
val customWebFormOnly : kotlin.Boolean = true // kotlin.Boolean | Return only emails with the custom web form
val templateIdColonIn : kotlin.collections.List<kotlin.Int> =  // kotlin.collections.List<kotlin.Int> | Email Template unique identifier. Search for results that contain any of specified values of this parameter.
val dateColonLt : kotlin.String = dateColonLt_example // kotlin.String | Email creation date. Search for result that has this parameter value less than specified.
val bucket : kotlin.String = bucket_example // kotlin.String | Email bucket
val offset : kotlin.Int = 56 // kotlin.Int | 
try {
    val result : Mails = apiInstance.restMailGet(isRecipient, modifiedDateColonLte, mode, sharedMailboxId, trackingOnly, senderId, read, isPreview, returnCustomWebForm, dateColonGte, isUserSent, modifiedDateColonGt, templateId, orderBy, returnEntity, modifiedDateColonLt, status, emailPackageIdColonIn, date, with, limit, emailPackageId, modifiedDate, webFormId, dateColonGt, modifiedDateColonGte, senderIdColonIn, deleted, dateColonLte, customWebFormOnly, templateIdColonIn, dateColonLt, bucket, offset)
    println(result)
} catch (e: ClientException) {
    println("4xx response calling MailApi#restMailGet")
    e.printStackTrace()
} catch (e: ServerException) {
    println("5xx response calling MailApi#restMailGet")
    e.printStackTrace()
}
```

### Parameters

Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **isRecipient** | **kotlin.Boolean**| Unique identifier of User who receive Email | [optional]
 **modifiedDateColonLte** | **kotlin.String**| Email modified date. Search for result that has this parameter value less or equal to the specified. | [optional]
 **mode** | **kotlin.String**|  | [optional]
 **sharedMailboxId** | **kotlin.String**| Shared Mailbox unique identifier. Search for result belongs to the Shared Mailbox. | [optional]
 **trackingOnly** | **kotlin.Boolean**| Return only emails with tracking access | [optional]
 **senderId** | **kotlin.String**| Unique identifier of User who sent Email | [optional]
 **read** | **kotlin.Boolean**| Whether the email is read or not by current user | [optional]
 **isPreview** | **kotlin.Boolean**| Whether the email is a preview email | [optional]
 **returnCustomWebForm** | **kotlin.Boolean**| Return all emails include those with the custom web form | [optional]
 **dateColonGte** | **kotlin.String**| Email creation date. Search for result that has this parameter value greater or equal to the specified. | [optional]
 **isUserSent** | **kotlin.Boolean**| Whether the email was sent by some user | [optional]
 **modifiedDateColonGt** | **kotlin.String**| Email modified date. Search for result that has this parameter value greater than specified. | [optional]
 **templateId** | **kotlin.Int**| Email Template unique identifier | [optional]
 **orderBy** | **kotlin.String**| Sorting options | [optional]
 **returnEntity** | **kotlin.Boolean**|  | [optional]
 **modifiedDateColonLt** | **kotlin.String**| Email modified date. Search for result that has this parameter value less than specified. | [optional]
 **status** | **kotlin.String**| Email status | [optional]
 **emailPackageIdColonIn** | [**kotlin.collections.List&lt;kotlin.String&gt;**](kotlin.String.md)| Email Package unique identifier. Search for results that contain any of specified values of this parameter. | [optional]
 **date** | **kotlin.String**| Email creation date | [optional]
 **with** | **kotlin.String**|  | [optional]
 **limit** | **kotlin.Int**|  | [optional]
 **emailPackageId** | **kotlin.String**| Email Package unique identifier | [optional]
 **modifiedDate** | **kotlin.String**| Email modified date | [optional]
 **webFormId** | **kotlin.String**| Email web form ID | [optional]
 **dateColonGt** | **kotlin.String**| Email creation date. Search for result that has this parameter value greater than specified. | [optional]
 **modifiedDateColonGte** | **kotlin.String**| Email modified date. Search for result that has this parameter value greater or equal to the specified. | [optional]
 **senderIdColonIn** | [**kotlin.collections.List&lt;kotlin.String&gt;**](kotlin.String.md)| Unique identifier of User who sent Email Search for results that contain any of specified values of this parameter.recommended request size &lt;&#x3D; 100 | [optional]
 **deleted** | **kotlin.Boolean**| Indicates that Email is deleted | [optional]
 **dateColonLte** | **kotlin.String**| Email creation date. Search for result that has this parameter value less or equal to the specified. | [optional]
 **customWebFormOnly** | **kotlin.Boolean**| Return only emails with the custom web form | [optional]
 **templateIdColonIn** | [**kotlin.collections.List&lt;kotlin.Int&gt;**](kotlin.Int.md)| Email Template unique identifier. Search for results that contain any of specified values of this parameter. | [optional]
 **dateColonLt** | **kotlin.String**| Email creation date. Search for result that has this parameter value less than specified. | [optional]
 **bucket** | **kotlin.String**| Email bucket | [optional]
 **offset** | **kotlin.Int**|  | [optional]

### Return type

[**Mails**](Mails.md)

### Authorization

No authorization required

### HTTP request headers

 - **Content-Type**: Not defined
 - **Accept**: */*

<a id="restMailIdActionsCopyPost"></a>
# **restMailIdActionsCopyPost**
> org.openapitools.client.infrastructure.OctetByteArray restMailIdActionsCopyPost(id, idColonIn, body, mode, with, returnEntity)

Copy attachments from mail to folder

Copy attachments from mail to folder

### Example
```kotlin
// Import classes:
//import org.openapitools.client.infrastructure.*
//import org.openapitools.client.models.*

val apiInstance = MailApi()
val id : kotlin.String = id_example // kotlin.String | The ID of the entity
val idColonIn : kotlin.collections.List<kotlin.String> =  // kotlin.collections.List<kotlin.String> | 
val body : DestinationFolderIdRequest =  // DestinationFolderIdRequest | 
val mode : kotlin.String = mode_example // kotlin.String | 
val with : kotlin.String = with_example // kotlin.String | 
val returnEntity : kotlin.Boolean = true // kotlin.Boolean | 
try {
    val result : org.openapitools.client.infrastructure.OctetByteArray = apiInstance.restMailIdActionsCopyPost(id, idColonIn, body, mode, with, returnEntity)
    println(result)
} catch (e: ClientException) {
    println("4xx response calling MailApi#restMailIdActionsCopyPost")
    e.printStackTrace()
} catch (e: ServerException) {
    println("5xx response calling MailApi#restMailIdActionsCopyPost")
    e.printStackTrace()
}
```

### Parameters

Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **id** | **kotlin.String**| The ID of the entity |
 **idColonIn** | [**kotlin.collections.List&lt;kotlin.String&gt;**](kotlin.String.md)|  |
 **body** | [**DestinationFolderIdRequest**](DestinationFolderIdRequest.md)|  |
 **mode** | **kotlin.String**|  | [optional]
 **with** | **kotlin.String**|  | [optional]
 **returnEntity** | **kotlin.Boolean**|  | [optional]

### Return type

[**org.openapitools.client.infrastructure.OctetByteArray**](org.openapitools.client.infrastructure.OctetByteArray.md)

### Authorization

No authorization required

### HTTP request headers

 - **Content-Type**: Not defined
 - **Accept**: */*

<a id="restMailIdActionsSendFileExternalPut"></a>
# **restMailIdActionsSendFileExternalPut**
> Mail restMailIdActionsSendFileExternalPut(id, body, mode, with, returnEntity)

Update a mail

Update a mail

### Example
```kotlin
// Import classes:
//import org.openapitools.client.infrastructure.*
//import org.openapitools.client.models.*

val apiInstance = MailApi()
val id : kotlin.String = id_example // kotlin.String | The ID of the entity
val body : BaseSendMailPostRequest =  // BaseSendMailPostRequest | 
val mode : kotlin.String = mode_example // kotlin.String | 
val with : kotlin.String = with_example // kotlin.String | 
val returnEntity : kotlin.Boolean = true // kotlin.Boolean | 
try {
    val result : Mail = apiInstance.restMailIdActionsSendFileExternalPut(id, body, mode, with, returnEntity)
    println(result)
} catch (e: ClientException) {
    println("4xx response calling MailApi#restMailIdActionsSendFileExternalPut")
    e.printStackTrace()
} catch (e: ServerException) {
    println("5xx response calling MailApi#restMailIdActionsSendFileExternalPut")
    e.printStackTrace()
}
```

### Parameters

Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **id** | **kotlin.String**| The ID of the entity |
 **body** | [**BaseSendMailPostRequest**](BaseSendMailPostRequest.md)|  |
 **mode** | **kotlin.String**|  | [optional]
 **with** | **kotlin.String**|  | [optional]
 **returnEntity** | **kotlin.Boolean**|  | [optional]

### Return type

[**Mail**](Mail.md)

### Authorization

No authorization required

### HTTP request headers

 - **Content-Type**: Not defined
 - **Accept**: */*

<a id="restMailIdActionsSendFilePut"></a>
# **restMailIdActionsSendFilePut**
> Mail restMailIdActionsSendFilePut(id, body, mode, with, returnEntity)

Update a mail

Update a mail

### Example
```kotlin
// Import classes:
//import org.openapitools.client.infrastructure.*
//import org.openapitools.client.models.*

val apiInstance = MailApi()
val id : kotlin.String = id_example // kotlin.String | The ID of the entity
val body : BaseSendMailPostRequest =  // BaseSendMailPostRequest | 
val mode : kotlin.String = mode_example // kotlin.String | 
val with : kotlin.String = with_example // kotlin.String | 
val returnEntity : kotlin.Boolean = true // kotlin.Boolean | 
try {
    val result : Mail = apiInstance.restMailIdActionsSendFilePut(id, body, mode, with, returnEntity)
    println(result)
} catch (e: ClientException) {
    println("4xx response calling MailApi#restMailIdActionsSendFilePut")
    e.printStackTrace()
} catch (e: ServerException) {
    println("5xx response calling MailApi#restMailIdActionsSendFilePut")
    e.printStackTrace()
}
```

### Parameters

Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **id** | **kotlin.String**| The ID of the entity |
 **body** | [**BaseSendMailPostRequest**](BaseSendMailPostRequest.md)|  |
 **mode** | **kotlin.String**|  | [optional]
 **with** | **kotlin.String**|  | [optional]
 **returnEntity** | **kotlin.Boolean**|  | [optional]

### Return type

[**Mail**](Mail.md)

### Authorization

No authorization required

### HTTP request headers

 - **Content-Type**: Not defined
 - **Accept**: */*

<a id="restMailIdActionsSendTrackingReportPost"></a>
# **restMailIdActionsSendTrackingReportPost**
> restMailIdActionsSendTrackingReportPost(id)

Send tracking report for email

Send tracking report for email

### Example
```kotlin
// Import classes:
//import org.openapitools.client.infrastructure.*
//import org.openapitools.client.models.*

val apiInstance = MailApi()
val id : kotlin.String = id_example // kotlin.String | The ID of the entity
try {
    apiInstance.restMailIdActionsSendTrackingReportPost(id)
} catch (e: ClientException) {
    println("4xx response calling MailApi#restMailIdActionsSendTrackingReportPost")
    e.printStackTrace()
} catch (e: ServerException) {
    println("5xx response calling MailApi#restMailIdActionsSendTrackingReportPost")
    e.printStackTrace()
}
```

### Parameters

Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **id** | **kotlin.String**| The ID of the entity |

### Return type

null (empty response body)

### Authorization

No authorization required

### HTTP request headers

 - **Content-Type**: Not defined
 - **Accept**: Not defined

<a id="restMailIdActionsWithdrawFilesPost"></a>
# **restMailIdActionsWithdrawFilesPost**
> restMailIdActionsWithdrawFilesPost(id, idColonIn)

Withdraw attachments from mail

Withdraw attachments from mail

### Example
```kotlin
// Import classes:
//import org.openapitools.client.infrastructure.*
//import org.openapitools.client.models.*

val apiInstance = MailApi()
val id : kotlin.String = id_example // kotlin.String | The ID of the entity
val idColonIn : kotlin.collections.List<kotlin.String> =  // kotlin.collections.List<kotlin.String> | 
try {
    apiInstance.restMailIdActionsWithdrawFilesPost(id, idColonIn)
} catch (e: ClientException) {
    println("4xx response calling MailApi#restMailIdActionsWithdrawFilesPost")
    e.printStackTrace()
} catch (e: ServerException) {
    println("5xx response calling MailApi#restMailIdActionsWithdrawFilesPost")
    e.printStackTrace()
}
```

### Parameters

Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **id** | **kotlin.String**| The ID of the entity |
 **idColonIn** | [**kotlin.collections.List&lt;kotlin.String&gt;**](kotlin.String.md)|  |

### Return type

null (empty response body)

### Authorization

No authorization required

### HTTP request headers

 - **Content-Type**: Not defined
 - **Accept**: Not defined

<a id="restMailIdAttachmentsAttachmentIdGet"></a>
# **restMailIdAttachmentsAttachmentIdGet**
> restMailIdAttachmentsAttachmentIdGet(id, attachmentId, ref)

Returns a list of attachments for a given mail.

Returns a list of attachments for a given mail.

### Example
```kotlin
// Import classes:
//import org.openapitools.client.infrastructure.*
//import org.openapitools.client.models.*

val apiInstance = MailApi()
val id : kotlin.String = id_example // kotlin.String | The ID of the entity
val attachmentId : kotlin.String = attachmentId_example // kotlin.String | The Attachment ID
val ref : kotlin.String = ref_example // kotlin.String | The email reference (Mandatory if the email can be accessed without authentication)
try {
    apiInstance.restMailIdAttachmentsAttachmentIdGet(id, attachmentId, ref)
} catch (e: ClientException) {
    println("4xx response calling MailApi#restMailIdAttachmentsAttachmentIdGet")
    e.printStackTrace()
} catch (e: ServerException) {
    println("5xx response calling MailApi#restMailIdAttachmentsAttachmentIdGet")
    e.printStackTrace()
}
```

### Parameters

Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **id** | **kotlin.String**| The ID of the entity |
 **attachmentId** | **kotlin.String**| The Attachment ID |
 **ref** | **kotlin.String**| The email reference (Mandatory if the email can be accessed without authentication) | [optional]

### Return type

null (empty response body)

### Authorization

No authorization required

### HTTP request headers

 - **Content-Type**: Not defined
 - **Accept**: Not defined

<a id="restMailIdAttachmentsGet"></a>
# **restMailIdAttachmentsGet**
> restMailIdAttachmentsGet(id, ref, limit, offset)

Returns a list of attachments for a given mail.

Returns a list of attachments for a given mail.

### Example
```kotlin
// Import classes:
//import org.openapitools.client.infrastructure.*
//import org.openapitools.client.models.*

val apiInstance = MailApi()
val id : kotlin.String = id_example // kotlin.String | The ID of the entity
val ref : kotlin.String = ref_example // kotlin.String | The email reference (Mandatory if the email can be accessed without authentication)
val limit : kotlin.Int = 56 // kotlin.Int | 
val offset : kotlin.Int = 56 // kotlin.Int | 
try {
    apiInstance.restMailIdAttachmentsGet(id, ref, limit, offset)
} catch (e: ClientException) {
    println("4xx response calling MailApi#restMailIdAttachmentsGet")
    e.printStackTrace()
} catch (e: ServerException) {
    println("5xx response calling MailApi#restMailIdAttachmentsGet")
    e.printStackTrace()
}
```

### Parameters

Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **id** | **kotlin.String**| The ID of the entity |
 **ref** | **kotlin.String**| The email reference (Mandatory if the email can be accessed without authentication) | [optional]
 **limit** | **kotlin.Int**|  | [optional]
 **offset** | **kotlin.Int**|  | [optional]

### Return type

null (empty response body)

### Authorization

No authorization required

### HTTP request headers

 - **Content-Type**: Not defined
 - **Accept**: Not defined

<a id="restMailIdDelete"></a>
# **restMailIdDelete**
> restMailIdDelete(id)

Delete an email draft

Allows a sender to delete a draft of email

### Example
```kotlin
// Import classes:
//import org.openapitools.client.infrastructure.*
//import org.openapitools.client.models.*

val apiInstance = MailApi()
val id : kotlin.String = id_example // kotlin.String | The ID of the entity
try {
    apiInstance.restMailIdDelete(id)
} catch (e: ClientException) {
    println("4xx response calling MailApi#restMailIdDelete")
    e.printStackTrace()
} catch (e: ServerException) {
    println("5xx response calling MailApi#restMailIdDelete")
    e.printStackTrace()
}
```

### Parameters

Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **id** | **kotlin.String**| The ID of the entity |

### Return type

null (empty response body)

### Authorization

No authorization required

### HTTP request headers

 - **Content-Type**: Not defined
 - **Accept**: Not defined

<a id="restMailIdGet"></a>
# **restMailIdGet**
> Mail restMailIdGet(id, mode, with, ref, returnEntity)

Get an email entry

Returns the details of a specified email which includes sender id, date, package id, etc.

### Example
```kotlin
// Import classes:
//import org.openapitools.client.infrastructure.*
//import org.openapitools.client.models.*

val apiInstance = MailApi()
val id : kotlin.String = id_example // kotlin.String | The ID of the entity
val mode : kotlin.String = mode_example // kotlin.String | 
val with : kotlin.String = with_example // kotlin.String | 
val ref : kotlin.String = ref_example // kotlin.String | The email reference (Mandatory if the email can be accessed without authentication)
val returnEntity : kotlin.Boolean = true // kotlin.Boolean | 
try {
    val result : Mail = apiInstance.restMailIdGet(id, mode, with, ref, returnEntity)
    println(result)
} catch (e: ClientException) {
    println("4xx response calling MailApi#restMailIdGet")
    e.printStackTrace()
} catch (e: ServerException) {
    println("5xx response calling MailApi#restMailIdGet")
    e.printStackTrace()
}
```

### Parameters

Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **id** | **kotlin.String**| The ID of the entity |
 **mode** | **kotlin.String**|  | [optional]
 **with** | **kotlin.String**|  | [optional]
 **ref** | **kotlin.String**| The email reference (Mandatory if the email can be accessed without authentication) | [optional]
 **returnEntity** | **kotlin.Boolean**|  | [optional]

### Return type

[**Mail**](Mail.md)

### Authorization

No authorization required

### HTTP request headers

 - **Content-Type**: Not defined
 - **Accept**: */*

<a id="restMailIdPackagesGet"></a>
# **restMailIdPackagesGet**
> Package restMailIdPackagesGet(id, ref, offset, limit, mode)

List email packages

Returns a list of packages for an email

### Example
```kotlin
// Import classes:
//import org.openapitools.client.infrastructure.*
//import org.openapitools.client.models.*

val apiInstance = MailApi()
val id : kotlin.String = id_example // kotlin.String | ID of the email
val ref : kotlin.String = ref_example // kotlin.String | The email reference code (Mandatory if the email can be accessed without authentication)
val offset : kotlin.Int = 56 // kotlin.Int | Offset
val limit : kotlin.Int = 56 // kotlin.Int | Limit
val mode : kotlin.String = mode_example // kotlin.String | Response mode
try {
    val result : Package = apiInstance.restMailIdPackagesGet(id, ref, offset, limit, mode)
    println(result)
} catch (e: ClientException) {
    println("4xx response calling MailApi#restMailIdPackagesGet")
    e.printStackTrace()
} catch (e: ServerException) {
    println("5xx response calling MailApi#restMailIdPackagesGet")
    e.printStackTrace()
}
```

### Parameters

Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **id** | **kotlin.String**| ID of the email |
 **ref** | **kotlin.String**| The email reference code (Mandatory if the email can be accessed without authentication) | [optional]
 **offset** | **kotlin.Int**| Offset | [optional]
 **limit** | **kotlin.Int**| Limit | [optional]
 **mode** | **kotlin.String**| Response mode | [optional]

### Return type

[**Package**](Package.md)

### Authorization

No authorization required

### HTTP request headers

 - **Content-Type**: Not defined
 - **Accept**: */*

<a id="restMailIdRecipientsGet"></a>
# **restMailIdRecipientsGet**
> kotlin.collections.List&lt;Recipient&gt; restMailIdRecipientsGet(id, type, ref, orderBy, offset, limit, locateId, with, mode)

List recipients

Returns a list of recipients for a given email

### Example
```kotlin
// Import classes:
//import org.openapitools.client.infrastructure.*
//import org.openapitools.client.models.*

val apiInstance = MailApi()
val id : kotlin.String = id_example // kotlin.String | email id to retrieve recipients for
val type : kotlin.collections.List<kotlin.String> =  // kotlin.collections.List<kotlin.String> | Type for Recipient. TO,CC,BCC
val ref : kotlin.String = ref_example // kotlin.String | The email reference (Mandatory if the email can be accessed without authentication)
val orderBy : kotlin.collections.List<kotlin.String> =  // kotlin.collections.List<kotlin.String> | Sorting options
val offset : kotlin.Int = 56 // kotlin.Int | Offset
val limit : kotlin.Int = 56 // kotlin.Int | Limit
val locateId : kotlin.Int = 56 // kotlin.Int | If specified, \"offset\" parameter will be ignored                                             and the page containing entity with this Id will be returned.
val with : kotlin.String = with_example // kotlin.String | With parameters
val mode : kotlin.String = mode_example // kotlin.String | Response mode
try {
    val result : kotlin.collections.List<Recipient> = apiInstance.restMailIdRecipientsGet(id, type, ref, orderBy, offset, limit, locateId, with, mode)
    println(result)
} catch (e: ClientException) {
    println("4xx response calling MailApi#restMailIdRecipientsGet")
    e.printStackTrace()
} catch (e: ServerException) {
    println("5xx response calling MailApi#restMailIdRecipientsGet")
    e.printStackTrace()
}
```

### Parameters

Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **id** | **kotlin.String**| email id to retrieve recipients for |
 **type** | [**kotlin.collections.List&lt;kotlin.String&gt;**](kotlin.String.md)| Type for Recipient. TO,CC,BCC | [optional]
 **ref** | **kotlin.String**| The email reference (Mandatory if the email can be accessed without authentication) | [optional]
 **orderBy** | [**kotlin.collections.List&lt;kotlin.String&gt;**](kotlin.String.md)| Sorting options | [optional]
 **offset** | **kotlin.Int**| Offset | [optional]
 **limit** | **kotlin.Int**| Limit | [optional]
 **locateId** | **kotlin.Int**| If specified, \&quot;offset\&quot; parameter will be ignored                                             and the page containing entity with this Id will be returned. | [optional]
 **with** | **kotlin.String**| With parameters | [optional]
 **mode** | **kotlin.String**| Response mode | [optional]

### Return type

[**kotlin.collections.List&lt;Recipient&gt;**](Recipient.md)

### Authorization

No authorization required

### HTTP request headers

 - **Content-Type**: Not defined
 - **Accept**: */*

<a id="restMailIdScanStatusGet"></a>
# **restMailIdScanStatusGet**
> restMailIdScanStatusGet(id)

Get the status of a mail job based on attachment and content scan status.

Get the status of a mail job based on attachment and content scan status.

### Example
```kotlin
// Import classes:
//import org.openapitools.client.infrastructure.*
//import org.openapitools.client.models.*

val apiInstance = MailApi()
val id : kotlin.String = id_example // kotlin.String | The ID of the entity
try {
    apiInstance.restMailIdScanStatusGet(id)
} catch (e: ClientException) {
    println("4xx response calling MailApi#restMailIdScanStatusGet")
    e.printStackTrace()
} catch (e: ServerException) {
    println("5xx response calling MailApi#restMailIdScanStatusGet")
    e.printStackTrace()
}
```

### Parameters

Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **id** | **kotlin.String**| The ID of the entity |

### Return type

null (empty response body)

### Authorization

No authorization required

### HTTP request headers

 - **Content-Type**: Not defined
 - **Accept**: Not defined

<a id="restMailIdSettingsPut"></a>
# **restMailIdSettingsPut**
> restMailIdSettingsPut(id, body)

Allow sender to update the mail setting of an email.

Allow sender to update the mail setting of an email.

### Example
```kotlin
// Import classes:
//import org.openapitools.client.infrastructure.*
//import org.openapitools.client.models.*

val apiInstance = MailApi()
val id : kotlin.String = id_example // kotlin.String | The ID of the entity
val body : SendMailSettingPutRequest =  // SendMailSettingPutRequest | 
try {
    apiInstance.restMailIdSettingsPut(id, body)
} catch (e: ClientException) {
    println("4xx response calling MailApi#restMailIdSettingsPut")
    e.printStackTrace()
} catch (e: ServerException) {
    println("5xx response calling MailApi#restMailIdSettingsPut")
    e.printStackTrace()
}
```

### Parameters

Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **id** | **kotlin.String**| The ID of the entity |
 **body** | [**SendMailSettingPutRequest**](SendMailSettingPutRequest.md)|  |

### Return type

null (empty response body)

### Authorization

No authorization required

### HTTP request headers

 - **Content-Type**: Not defined
 - **Accept**: Not defined

<a id="restMailIdTrackingsMeDelete"></a>
# **restMailIdTrackingsMeDelete**
> restMailIdTrackingsMeDelete(id)

Unsubscribe user from tracking

Unsubscribe user from tracking

### Example
```kotlin
// Import classes:
//import org.openapitools.client.infrastructure.*
//import org.openapitools.client.models.*

val apiInstance = MailApi()
val id : kotlin.String = id_example // kotlin.String | The ID of the entity
try {
    apiInstance.restMailIdTrackingsMeDelete(id)
} catch (e: ClientException) {
    println("4xx response calling MailApi#restMailIdTrackingsMeDelete")
    e.printStackTrace()
} catch (e: ServerException) {
    println("5xx response calling MailApi#restMailIdTrackingsMeDelete")
    e.printStackTrace()
}
```

### Parameters

Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **id** | **kotlin.String**| The ID of the entity |

### Return type

null (empty response body)

### Authorization

No authorization required

### HTTP request headers

 - **Content-Type**: Not defined
 - **Accept**: Not defined

<a id="restPublicMailActionsSendFilePost"></a>
# **restPublicMailActionsSendFilePost**
> Mail restPublicMailActionsSendFilePost(body, mode, with, returnEntity)

Create a mail

Create a mail

### Example
```kotlin
// Import classes:
//import org.openapitools.client.infrastructure.*
//import org.openapitools.client.models.*

val apiInstance = MailApi()
val body : BaseSendMailPostRequest =  // BaseSendMailPostRequest | 
val mode : kotlin.String = mode_example // kotlin.String | 
val with : kotlin.String = with_example // kotlin.String | 
val returnEntity : kotlin.Boolean = true // kotlin.Boolean | 
try {
    val result : Mail = apiInstance.restPublicMailActionsSendFilePost(body, mode, with, returnEntity)
    println(result)
} catch (e: ClientException) {
    println("4xx response calling MailApi#restPublicMailActionsSendFilePost")
    e.printStackTrace()
} catch (e: ServerException) {
    println("5xx response calling MailApi#restPublicMailActionsSendFilePost")
    e.printStackTrace()
}
```

### Parameters

Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **body** | [**BaseSendMailPostRequest**](BaseSendMailPostRequest.md)|  |
 **mode** | **kotlin.String**|  | [optional]
 **with** | **kotlin.String**|  | [optional]
 **returnEntity** | **kotlin.Boolean**|  | [optional]

### Return type

[**Mail**](Mail.md)

### Authorization

No authorization required

### HTTP request headers

 - **Content-Type**: Not defined
 - **Accept**: */*

<a id="restPublicMailIdActionsSendFilePut"></a>
# **restPublicMailIdActionsSendFilePut**
> Mail restPublicMailIdActionsSendFilePut(id, body, mode, with, returnEntity)

Update a mail

Update a mail

### Example
```kotlin
// Import classes:
//import org.openapitools.client.infrastructure.*
//import org.openapitools.client.models.*

val apiInstance = MailApi()
val id : kotlin.String = id_example // kotlin.String | The ID of the entity
val body : BaseSendMailPostRequest =  // BaseSendMailPostRequest | 
val mode : kotlin.String = mode_example // kotlin.String | 
val with : kotlin.String = with_example // kotlin.String | 
val returnEntity : kotlin.Boolean = true // kotlin.Boolean | 
try {
    val result : Mail = apiInstance.restPublicMailIdActionsSendFilePut(id, body, mode, with, returnEntity)
    println(result)
} catch (e: ClientException) {
    println("4xx response calling MailApi#restPublicMailIdActionsSendFilePut")
    e.printStackTrace()
} catch (e: ServerException) {
    println("5xx response calling MailApi#restPublicMailIdActionsSendFilePut")
    e.printStackTrace()
}
```

### Parameters

Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **id** | **kotlin.String**| The ID of the entity |
 **body** | [**BaseSendMailPostRequest**](BaseSendMailPostRequest.md)|  |
 **mode** | **kotlin.String**|  | [optional]
 **with** | **kotlin.String**|  | [optional]
 **returnEntity** | **kotlin.Boolean**|  | [optional]

### Return type

[**Mail**](Mail.md)

### Authorization

No authorization required

### HTTP request headers

 - **Content-Type**: Not defined
 - **Accept**: */*

