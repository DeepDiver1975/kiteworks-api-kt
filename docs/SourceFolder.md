
# SourceFolder

## Properties
Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**id** | **kotlin.String** | Unique SourceContent identifier | 
**name** | **kotlin.String** | Name of source content | 
**parentId** | **kotlin.String** | Parent ID of Source | 
**type** | **kotlin.String** | Type of Object | 
**wopiapp** | **kotlin.Boolean** | WOPI info for iOS app | 
**created** | **kotlin.String** | Time of Source created in UTC timestamp |  [optional]
**modified** | **kotlin.String** | Time of Source modified in UTC timestamp |  [optional]
**status** | **kotlin.String** | Status of the source |  [optional]
**deleted** | **kotlin.Boolean** | Whether the file is deleted |  [optional]
**path** | **kotlin.String** | Shows object full path |  [optional]
**userRoleId** | **kotlin.Int** | Current user role id (Explicit field. May be retrieved only if mentioned in \&quot;with\&quot; parameter) |  [optional]
**creator** | [**UserBasicInfo**](UserBasicInfo.md) |  |  [optional]
**permissions** | [**kotlin.collections.List&lt;Permission&gt;**](Permission.md) | Current user&#39;s permissions (Explicit field. May be retrieved only if mentioned in \&quot;with\&quot; parameter) |  [optional]
**rootId** | **kotlin.String** | Root Id (Explicit field. May be retrieved only if mentioned in \&quot;with\&quot; parameter) |  [optional]
**pathIds** | **kotlin.String** | Path Ids (Explicit field. May be retrieved only if mentioned in \&quot;with\&quot; parameter) |  [optional]
**sourceTypeId** | **kotlin.String** | Source Type (Explicit field. May be retrieved only if mentioned in \&quot;with\&quot; parameter) |  [optional]
**totalFilesCount** | **kotlin.String** | Total Files Count (Explicit field. May be retrieved only if mentioned in \&quot;with\&quot; parameter) |  [optional]
**totalFoldersCount** | **kotlin.String** | Total Folders Count (Explicit field. May be retrieved only if mentioned in \&quot;with\&quot; parameter) |  [optional]
**links** | **kotlin.String** |  |  [optional]
**isFavorite** | **kotlin.Boolean** | Indicates that Folder is marked as favorite for current user |  [optional]



