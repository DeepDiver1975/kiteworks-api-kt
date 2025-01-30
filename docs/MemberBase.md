
# MemberBase

## Properties
Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**objectId** | **kotlin.String** | Unique identifier of object | 
**roleId** | **kotlin.Int** | Unique identifier of role | 
**user** | [**User**](User.md) |  |  [optional]
**group** | [**LdapGroup**](LdapGroup.md) |  |  [optional]
**role** | [**Role**](Role.md) |  |  [optional]
**inheritRoleId** | **kotlin.Int** | Role Id inherit from parent (Explicit field. May be retrieved only if mentioned in \&quot;with\&quot; parameter) |  [optional]
**allowedFolderRoleId** | **kotlin.collections.List&lt;kotlin.String&gt;** | Allowed Folder Role Id (Explicit field. May be retrieved only if mentioned in \&quot;with\&quot; parameter) |  [optional]
**links** | **kotlin.String** |  |  [optional]



