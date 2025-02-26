
# EmailPost

## Properties
Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**templateId** | **kotlin.Int** | Email template unique identifier | 
**status** | [**inline**](#Status) | Email status | 
**senderId** | **kotlin.Int** | Unique identifier of User who sent Email |  [optional]
**emailPackageId** | **kotlin.Int** | Email Package unique identifier |  [optional]
**secureBody** | **kotlin.Boolean** |  |  [optional]
**modifiedDate** | **kotlin.String** |  |  [optional]
**parentEmailId** | **kotlin.Int** | The identifier of forwarded email |  [optional]


<a id="Status"></a>
## Enum: status
Name | Value
---- | -----
status | queued, draft, sent, error



