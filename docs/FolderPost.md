
# FolderPost

## Properties
Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**name** | **kotlin.String** | Folder name | 
**description** | **kotlin.String** | Folder description |  [optional]
**syncable** | **kotlin.Boolean** | Indicates that folder is syncable. Can only be set at a top level folder. |  [optional]
**expire** | [**java.time.LocalDate**](java.time.LocalDate.md) | The folder expiration date. Applicable to top level folders |  [optional]
**fileLifetime** | **kotlin.Int** | The file&#39;s lifetime in the folder |  [optional]
**secure** | **kotlin.Boolean** | Indicates whether folder is secure. Only top level folders under user&#39;s root folder can be set to secure |  [optional]



