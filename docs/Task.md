
# Task

## Properties
Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**id** | **kotlin.Int** | Task unique identifier | 
**assigneeId** | **kotlin.String** | Assigned User unique identifier | 
**due** | [**java.time.LocalDate**](java.time.LocalDate.md) | Task due date | 
**userId** | **kotlin.String** | Identifier of User who created a Task | 
**created** | [**java.time.LocalDate**](java.time.LocalDate.md) | Task creation date | 
**status** | **kotlin.String** | Task status | 
**assignee** | [**User**](User.md) |  |  [optional]
**parentId** | **kotlin.Int** | Parent Comment identifier |  [optional]
**objectId** | **kotlin.String** | Object identifier Task belongs to |  [optional]
**user** | [**User**](User.md) |  |  [optional]
**modified** | [**java.time.LocalDate**](java.time.LocalDate.md) | Task modification date |  [optional]
**contents** | **kotlin.String** | Task content |  [optional]
**deleted** | **kotlin.Boolean** | Indicates that Task is deleted |  [optional]
**folderId** | **kotlin.String** | Identifier of Object&#39;s parent Folder |  [optional]
**file** | [**org.openapitools.client.infrastructure.OctetByteArray**](org.openapitools.client.infrastructure.OctetByteArray.md) |  |  [optional]
**permissions** | [**kotlin.collections.List&lt;Permission&gt;**](Permission.md) | Current user&#39;s permissions (Explicit field. May be retrieved only if mentioned in \&quot;with\&quot; parameter) |  [optional]
**links** | **kotlin.String** |  |  [optional]



