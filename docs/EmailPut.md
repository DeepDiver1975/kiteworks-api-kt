
# EmailPut

## Properties
Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**status** | [**inline**](#Status) | Email status | 
**emailPackageId** | **kotlin.Int** | Email Package unique identifier |  [optional]
**secureBody** | **kotlin.Boolean** |  |  [optional]
**modifiedDate** | [**java.time.LocalDate**](java.time.LocalDate.md) |  |  [optional]
**parentEmailId** | **kotlin.Int** | The identifier of forwarded email |  [optional]


<a id="Status"></a>
## Enum: status
Name | Value
---- | -----
status | queued, draft, sent, error



