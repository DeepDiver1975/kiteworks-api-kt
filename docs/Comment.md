
# Comment

## Properties
Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**id** | **kotlin.Int** | Comment unique identifier | 
**parentId** | **kotlin.Int** | Parent Comment unique identifier. Exists if comment is a reply. | 
**objectId** | **kotlin.String** | Unique identifier of commented Object. | 
**userId** | **kotlin.String** | Unique identifier of comment author. | 
**contents** | **kotlin.String** | Comment content. | 
**folderId** | **kotlin.String** | Unique identifier of commented Object parent Folder. |  [optional]
**created** | [**java.time.LocalDate**](java.time.LocalDate.md) | Comment creation date. |  [optional]
**modified** | [**java.time.LocalDate**](java.time.LocalDate.md) | Comment modification date |  [optional]
**deleted** | **kotlin.Boolean** | Indicates that comment is deleted. |  [optional]
**isComment** | **kotlin.Boolean** |  |  [optional]
**&#x60;object&#x60;** | [**BaseObject**](BaseObject.md) |  |  [optional]
**author** | [**UserBasicInfo**](UserBasicInfo.md) |  |  [optional]
**parent** | [**Comment**](Comment.md) |  |  [optional]
**permissions** | [**kotlin.collections.List&lt;Permission&gt;**](Permission.md) | Current user&#39;s permissions (Explicit field. May be retrieved only if mentioned in \&quot;with\&quot; parameter) |  [optional]
**links** | **kotlin.String** |  |  [optional]



