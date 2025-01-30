
# AdminFolderPutRequest

## Properties
Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**ids** | **kotlin.collections.List&lt;kotlin.String&gt;** | List of folder object ID to be updated | 
**applyToNestedFiles** | **kotlin.Boolean** | Apply expire to files under child folders |  [optional]
**applyTo** | [**inline**](#ApplyTo) | Apply expire to folder only / files only / folder and files |  [optional]
**expire** | **kotlin.String** | Expire date |  [optional]


<a id="ApplyTo"></a>
## Enum: applyTo
Name | Value
---- | -----
applyTo | folders_only, files_only, folders_and_files



