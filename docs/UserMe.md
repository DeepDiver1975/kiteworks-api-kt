
# UserMe

## Properties
Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**id** | **kotlin.String** | The unique identifier of the user | 
**basedirId** | **kotlin.String** | The unique identifier of the user&#39;s root kiteworks directory.      *                  Only folder creation is allowed on user&#39;s base directory. | 
**email** | **kotlin.String** | The user&#39;s email | 
**mydirId** | **kotlin.String** | The unique identifier of the user&#39;s mydir directory.      *                  mydir directory stores copies of files from email attachments and user&#39;s profile image.      *                  mydir is not visible to end users | 
**name** | **kotlin.String** | The name of the user | 
**syncdirId** | **kotlin.String** | Id of sync dir | 
**created** | **kotlin.String** | User creation date |  [optional]
**userTypeId** | **kotlin.Int** | The unique identifier of the user type |  [optional]
**&#x60;internal&#x60;** | **kotlin.Boolean** | Indicates that the user is an internal user |  [optional]
**profileIcon** | **kotlin.String** | User profile icon link |  [optional]
**extDL** | **kotlin.Boolean** | Indicates that the user is External Distribution List |  [optional]
**metadata** | [**kotlin.collections.List&lt;UserMetadata&gt;**](UserMetadata.md) | List of user&#39;s metadata |  [optional]
**adminRoleId** | **kotlin.Int** |  |  [optional]
**links** | **kotlin.String** |  |  [optional]
**serviceName** | **kotlin.String** | Service name |  [optional]



