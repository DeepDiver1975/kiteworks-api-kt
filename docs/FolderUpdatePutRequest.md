
# FolderUpdatePutRequest

## Properties
Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**clientId** | **kotlin.String** |  |  [optional]
**secure** | **kotlin.Boolean** | Indicates whether folder is secure. Only top level folders under user&#39;s root folder can be set to secure |  [optional]
**vendorDocName** | **kotlin.String** |  |  [optional]
**description** | **kotlin.String** | Folder description |  [optional]
**fileLifetime** | **kotlin.Int** | The file&#39;s lifetime in the folder |  [optional]
**name** | **kotlin.String** | Folder name |  [optional]
**applyFileLifetimeToFiles** | **kotlin.Boolean** | (optional) Apply file lifetime setting to existing files. Applicable when fileLifetime is set |  [optional]
**applyFileLifetimeToNested** | **kotlin.Boolean** | (optional) Apply file lifetime setting to nested folders. Applicable when fileLifetime is set |  [optional]
**expire** | **kotlin.String** | The folder expiration date. Applicable to top level folders |  [optional]
**vendorDocId** | **kotlin.String** |  |  [optional]
**syncable** | **kotlin.Boolean** | Indicates that folder is syncable. Can only be set at a top level folder |  [optional]



