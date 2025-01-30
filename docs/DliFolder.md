
# DliFolder

## Properties
Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**id** | **kotlin.String** | Unique identifier of object | 
**name** | **kotlin.String** | Object name | 
**parentId** | **kotlin.String** | Parent Folder identifier | 
**userId** | **kotlin.String** | Unique identifier of Object creator | 
**type** | **kotlin.String** |  | 
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
**description** | **kotlin.String** | Folder description |  [optional]
**syncable** | **kotlin.Boolean** | Indicates that folder is syncable. Can only be set at a top level folder. |  [optional]
**fileLifetime** | **kotlin.String** | The file&#39;s lifetime in the folder |  [optional]
**members** | [**kotlin.collections.List&lt;MemberBase&gt;**](MemberBase.md) | Folder members list (Explicit field. May be retrieved only if mentioned in \&quot;with\&quot; parameter) |  [optional]
**secure** | **kotlin.Boolean** | Indicates that Folder is secure. Only top level folders under user&#39;s root folder can be set to secure |  [optional]
**isFavorite** | **kotlin.Boolean** | Indicates that Folder is marked as favorite for current user (Explicit field. May be retrieved only if mentioned in \&quot;with\&quot; parameter) |  [optional]
**pushedFilesCount** | **kotlin.Int** | Count of pushed files inside folder (Explicit field. May be retrieved only if mentioned in \&quot;with\&quot; parameter) |  [optional]
**path** | **kotlin.String** | Shows folder full path up to folder on which current folder has permissions |  [optional]
**currentUserRole** | [**Role**](Role.md) |  |  [optional]
**totalFilesCount** | **kotlin.Int** | Count of files inside folder (Explicit field. May be retrieved only if mentioned in \&quot;with\&quot; parameter) |  [optional]
**totalFoldersCount** | **kotlin.Int** | Count of child folders (Explicit field. May be retrieved only if mentioned in \&quot;with\&quot; parameter) |  [optional]
**totalMembersCount** | **kotlin.Int** | Count of folder&#39;s members (Explicit field. May be retrieved only if mentioned in \&quot;with\&quot; parameter) |  [optional]
**isShared** | **kotlin.Boolean** | Indicates that Folder is shared to users/groups (Explicit field. May be retrieved only if mentioned in \&quot;with\&quot; parameter) |  [optional]
**avStatus** | **kotlin.String** | Check folder availability status according to AV settings and folder files scanned/infected status (Explicit field. May be retrieved only if mentioned in \&quot;with\&quot; parameter) |  [optional]
**dlpStatus** | **kotlin.String** | Check folder availability status according to DLP settings and folder files scanned/infected status (Explicit field. May be retrieved only if mentioned in \&quot;with\&quot; parameter) |  [optional]
**maxFolderExpiration** | **kotlin.String** | Get profile max folder expiration as a date |  [optional]
**maxFileLifetime** | **kotlin.String** | Get profile max file lifetime |  [optional]



