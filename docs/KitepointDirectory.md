
# KitepointDirectory

## Properties
Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**id** | **kotlin.String** | Unique identifier of object | 
**name** | **kotlin.String** | Object name | 
**userId** | **kotlin.String** | Unique identifier of Object creator | 
**parentId** | **kotlin.String** | Parent Folder identifier | 
**created** | [**kotlinx.datetime.Instant**](kotlinx.datetime.Instant.md) | Object creation date |  [optional]
**deleted** | **kotlin.Boolean** | Indicates that object is deleted |  [optional]
**permDeleted** | **kotlin.Boolean** | Indicates that object is permanently deleted |  [optional]
**expire** | [**kotlinx.datetime.Instant**](kotlinx.datetime.Instant.md) | Object expiry date |  [optional]
**modified** | [**kotlinx.datetime.Instant**](kotlinx.datetime.Instant.md) | Object modification date |  [optional]
**parent** | [**Folder**](Folder.md) |  |  [optional]
**permalink** | **kotlin.String** | Object permalink |  [optional]
**creator** | [**UserBasicInfo**](UserBasicInfo.md) |  |  [optional]
**permissions** | [**kotlin.collections.List&lt;Permission&gt;**](Permission.md) | Current user&#39;s permissions (Explicit field. May be retrieved only if mentioned in \&quot;with\&quot; parameter) |  [optional]
**vendorDocId** | **kotlin.String** | Vendor document id (Explicit field. May be retrieved only if mentioned in \&quot;with\&quot; parameter) |  [optional]
**vendorDocName** | **kotlin.String** | Vendor document name (Explicit field. May be retrieved only if mentioned in \&quot;with\&quot; parameter) |  [optional]
**source** | **kotlin.Int** |  |  [optional]
**links** | **kotlin.String** |  |  [optional]
**type** | **kotlin.String** | Object type. Type kd is kitepoint folder |  [optional]
**path** | **kotlin.String** | Parent folders path |  [optional]
**isFavorite** | **kotlin.Boolean** | Indicates that Folder is marked as favorite for current user (Explicit field. May be retrieved only if mentioned in \&quot;with\&quot; parameter) |  [optional]
**eCObject** | **kotlin.String** | Unique identifier of kitepoint directory |  [optional]
**eCUUID** | **kotlin.String** | ECUuId |  [optional]



