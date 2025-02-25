
# NoteFile

## Properties
Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**id** | **kotlin.String** | Unique identifier of object | 
**name** | **kotlin.String** | Object name | 
**parentId** | **kotlin.String** | Parent Folder identifier | 
**userId** | **kotlin.String** | Unique identifier of Object creator | 
**propertySize** | **kotlin.String** | File content size | 
**type** | **kotlin.String** |  | 
**locked** | **kotlin.Int** | Unique identifier of User who locked a File | 
**wopiapp** | **kotlin.Boolean** | WOPI info for iOS app | 
**created** | **kotlin.String** | Object creation date |  [optional]
**deleted** | **kotlin.Boolean** | Indicates that object is deleted |  [optional]
**permDeleted** | **kotlin.Boolean** | Indicates that object is permanently deleted |  [optional]
**expire** | **kotlin.String** | Object expiry date |  [optional]
**modified** | **kotlin.String** | Object modification date |  [optional]
**parent** | [**Folder**](Folder.md) |  |  [optional]
**permalink** | **kotlin.String** | Object permalink |  [optional]
**creator** | [**UserBasicInfo**](UserBasicInfo.md) |  |  [optional]
**permissions** | [**kotlin.collections.List&lt;Permission&gt;**](Permission.md) | Current user&#39;s permissions (Explicit field. May be retrieved only if mentioned in \&quot;with\&quot; parameter) |  [optional]
**vendorDocId** | **kotlin.String** | Vendor document id (Explicit field. May be retrieved only if mentioned in \&quot;with\&quot; parameter) |  [optional]
**vendorDocName** | **kotlin.String** | Vendor document name (Explicit field. May be retrieved only if mentioned in \&quot;with\&quot; parameter) |  [optional]
**source** | **kotlin.Int** |  |  [optional]
**links** | **kotlin.String** |  |  [optional]
**mime** | **kotlin.String** | File MIME type |  [optional]
**fingerprint** | **kotlin.String** | File content fingerprint |  [optional]
**lockUser** | [**User**](User.md) |  |  [optional]
**clientCreated** | **kotlin.String** | Original created time of the file |  [optional]
**clientModified** | **kotlin.String** | Original Modified time of the file |  [optional]
**members** | [**kotlin.collections.List&lt;Member&gt;**](Member.md) | File members list (Explicit field. May be retrieved only if mentioned in \&quot;with\&quot; parameter) |  [optional]
**overriddenExpire** | **kotlin.Boolean** | Indicates that file expire is overridden |  [optional]
**originalFileId** | **kotlin.String** | File identifier from which this file was copied from |  [optional]
**pushedObject** | [**PushedObject**](PushedObject.md) |  |  [optional]
**avStatus** | **kotlin.String** | Check file availability status according to AV settings and file scanned/infected status |  [optional]
**dlpStatus** | **kotlin.String** | Check file availability status according to DLP settings and file scanned/infected status |  [optional]
**adminQuarantineStatus** | **kotlin.String** | Check file availability status according to admin quarantined status |  [optional]
**storageAvailable** | **kotlin.Boolean** | Boolean value that shows if this file is available on any volume |  [optional]
**lastModifiedBy** | [**User**](User.md) |  |  [optional]
**roleId** | **kotlin.String** | Highest role |  [optional]
**isShared** | **kotlin.String** | File shared |  [optional]
**fingerprints** | **kotlin.collections.List&lt;kotlin.String&gt;** | Array of file fingerprint objects |  [optional]
**tags** | [**kotlin.collections.List&lt;Tag&gt;**](Tag.md) | Array of tag objects |  [optional]



