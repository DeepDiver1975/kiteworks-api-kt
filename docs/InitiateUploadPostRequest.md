
# InitiateUploadPostRequest

## Properties
Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**filename** | **kotlin.String** | File name | 
**totalChunks** | **kotlin.Int** | Total chunks amount |  [optional]
**clientModified** | **kotlin.String** | File modified date set from client |  [optional]
**totalSize** | **kotlin.Int** | Total file size |  [optional]
**clientCreated** | **kotlin.String** | File created date set from client |  [optional]
**resume** | **kotlin.Boolean** | Indicate if this is resume upload and only applicable when same file name already exists. Currently only used internally in SFTP |  [optional]



