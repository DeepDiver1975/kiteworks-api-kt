
# Version

## Properties
Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**id** | **kotlin.String** | Unique identifier of the file version | 
**versionNumber** | **kotlin.Int** | File version number | 
**userId** | **kotlin.String** | Unique identifier of User who created File Version | 
**name** | **kotlin.String** | File name | 
**objectId** | **kotlin.String** | Unique identifier of the file | 
**deleted** | **kotlin.Boolean** | Indicates whether the version has been deleted |  [optional]
**created** | [**java.time.LocalDate**](java.time.LocalDate.md) | File Version creation date |  [optional]
**propertySize** | **kotlin.Int** | File content size |  [optional]
**fingerprint** | **kotlin.String** | File content fingerprint |  [optional]
**fingerprintAlgo** | **kotlin.String** | File content fingerprint algo |  [optional]
**backend** | **kotlin.String** | Storage backend used by File |  [optional]
**mime** | **kotlin.String** | File mime type |  [optional]
**creator** | [**UserBasicInfo**](UserBasicInfo.md) |  |  [optional]
**clientCreated** | [**java.time.LocalDate**](java.time.LocalDate.md) | Original created time of the file |  [optional]
**clientModified** | [**java.time.LocalDate**](java.time.LocalDate.md) | Original modified time of the file |  [optional]
**avStatus** | **kotlin.String** | Check file availability status according to AV settings and file scanned/infected status |  [optional]
**dlpStatus** | **kotlin.String** | Check file availability status according to DLP settings and file scanned/infected status |  [optional]
**adminQuarantineStatus** | **kotlin.String** | Check file availability status according admin quarantined status.  |  [optional]
**storageAvailable** | **kotlin.Boolean** | Boolean value that shows if this file is available on any volume |  [optional]
**fingerprints** | **kotlin.collections.List&lt;kotlin.String&gt;** | Array of all file fingerprint objects |  [optional]
**tags** | [**kotlin.collections.List&lt;Tag&gt;**](Tag.md) | Array of tag objects |  [optional]
**links** | **kotlin.String** |  |  [optional]



