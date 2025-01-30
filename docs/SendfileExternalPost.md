
# SendfileExternalPost

## Properties
Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**to** | **kotlin.collections.List&lt;kotlin.String&gt;** |  |  [optional]
**cc** | **kotlin.collections.List&lt;kotlin.String&gt;** |  |  [optional]
**bcc** | **kotlin.collections.List&lt;kotlin.String&gt;** |  |  [optional]
**files** | **kotlin.collections.List&lt;kotlin.String&gt;** |  |  [optional]
**acl** | [**inline**](#Acl) |  |  [optional]
**expire** | [**kotlinx.datetime.Instant**](kotlinx.datetime.Instant.md) |  |  [optional]
**draft** | **kotlin.Boolean** |  |  [optional]
**preview** | **kotlin.Boolean** | Indicates that email is a preview email |  [optional]
**watermark** | **kotlin.String** | The watermark on the preview email |  [optional]
**secureBody** | **kotlin.Boolean** |  |  [optional]
**selfCopy** | **kotlin.Boolean** |  |  [optional]
**includeFingerprint** | **kotlin.Boolean** |  |  [optional]
**parentEmailId** | **kotlin.Int** |  |  [optional]
**isSelfReturnReceipt** | **kotlin.Boolean** |  |  [optional]
**returnReceipts** | **kotlin.collections.List&lt;kotlin.String&gt;** |  |  [optional]
**type** | [**inline**](#Type) | Email type |  [optional]
**uploading** | **kotlin.Boolean** | Indicates whether upload is still in progress. Prevents sending if is set to true. |  [optional]
**body** | **kotlin.String** |  |  [optional]
**subject** | **kotlin.String** |  |  [optional]


<a id="Acl"></a>
## Enum: acl
Name | Value
---- | -----
acl | verify_recipient, no_auth, otp, internal, anyone_auth


<a id="Type"></a>
## Enum: type
Name | Value
---- | -----
type | original, resend, forward, reply



