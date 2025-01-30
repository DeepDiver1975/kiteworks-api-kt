
# VersionPut

## Properties
Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**name** | **kotlin.String** | File name | 
**versionNumber** | **kotlin.Int** | File version number |  [optional]
**deleted** | **kotlin.Boolean** | Indicates whether the version has been deleted |  [optional]
**fingerprint** | **kotlin.Int** | The fingerprint that uniquely identifies the original file |  [optional]
**clientCreated** | **kotlin.Int** |  |  [optional]
**clientModified** | **kotlin.Int** |  |  [optional]
**status** | **kotlin.String** |  |  [optional]
**propertySize** | **kotlin.Int** | The file size |  [optional]
**user** | [**User**](User.md) |  |  [optional]
**id** | **kotlin.Int** | The file unique identifier |  [optional]
**flag** | **kotlin.Int** | Bitwise flag to indicate whether the version has been quarantined. Possible numeric values are: 2: quarantined, 0: not quarantined  |  [optional]
**archived** | **kotlin.Int** | Idicates whether this version has been archived |  [optional]
**objectId** | **kotlin.Int** | The object ID |  [optional]
**location** | **kotlin.Int** | The file location of this version |  [optional]
**created** | [**java.time.LocalDate**](java.time.LocalDate.md) | The date this version is created |  [optional]
**mime** | **kotlin.String** | The file mime type |  [optional]
**backend** | **kotlin.String** | Storage backend type s3, atmos, or acfs used to store the file |  [optional]
**file** | [**org.openapitools.client.infrastructure.OctetByteArray**](org.openapitools.client.infrastructure.OctetByteArray.md) |  |  [optional]



