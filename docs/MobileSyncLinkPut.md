
# MobileSyncLinkPut

## Properties
Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**ref** | **kotlin.String** | Shortlink handle. Example:abcdefg12 |  [optional]
**expire** | [**java.time.LocalDate**](java.time.LocalDate.md) | Expiration date |  [optional]
**entityTypeId** | **kotlin.String** | Unique identifier of entity type.      *     1 &#x3D; object,      *     2 &#x3D; email_package,      *     3 &#x3D; verification_code,      *     4 &#x3D; email_preview_package,      *     5 &#x3D; file_request,      *     6 &#x3D; add_file      *     7 &#x3D; password_reset,      *     8 &#x3D; gdrive_oauth,      *     9 &#x3D; connector_oauth,      *     10 &#x3D; comment,      *     11 &#x3D; task,      *     12 &#x3D; mobile_sync,      *     13 &#x3D; password_set,      *     14 &#x3D; event,      *     15 &#x3D; mail |  [optional]
**entityId** | **kotlin.String** | Unique identifier of entity |  [optional]
**length** | **kotlin.String** | Length of shortlink |  [optional]



