
# BaseChunkUploadRequest

## Properties
Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**compressionSize** | **kotlin.Int** | The upload content size after compression | 
**originalSize** | **kotlin.Int** | The original upload content size before compression | 
**compressionMode** | [**inline**](#CompressionMode) | The compression mode. Available option \&quot;NORMAL\&quot;, \&quot;GZIP\&quot; and \&quot;ZLIB\&quot; | 
**content** | **kotlin.String** | The upload content. Base64 encoded if upload in json format | 
**overwrite** | **kotlin.Boolean** | Indicate that the file will be overwritten without versioning if file with same name exists |  [optional]
**lastChunk** | **kotlin.Int** | Indicate if this upload is the last chunk of the file. 1 |  [optional]
**index** | **kotlin.Int** | The chunk index. Starts from 1 |  [optional]


<a id="CompressionMode"></a>
## Enum: compressionMode
Name | Value
---- | -----
compressionMode | NORMAL, GZIP, ZLIB



