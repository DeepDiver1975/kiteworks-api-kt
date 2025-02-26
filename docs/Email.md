
# Email

## Properties
Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**id** | **kotlin.String** | Email unique identifier | 
**senderId** | **kotlin.String** | Unique identifier of User who sent Email | 
**status** | **kotlin.String** | Email status | 
**type** | **kotlin.String** | Email type | 
**date** | **kotlin.String** |  | 
**emailPackageId** | **kotlin.String** | Email Package unique identifier | 
**recipients** | [**kotlin.collections.List&lt;Recipient&gt;**](Recipient.md) |  | 
**modifiedDate** | **kotlin.String** |  | 
**parentEmailId** | **kotlin.String** | Identifier of parent email | 
**subject** | **kotlin.String** |  | 
**templateId** | **kotlin.Int** | Email template unique identifier |  [optional]
**deleted** | **kotlin.Boolean** | Indicates that Email is deleted |  [optional]
**isPreview** | **kotlin.Boolean** | Indicates that email is a preview email |  [optional]
**isUserSent** | **kotlin.Boolean** | Indicates that email was sent by some user |  [optional]
**watermark** | **kotlin.String** | The watermark on the preview email |  [optional]
**&#x60;package&#x60;** | [**Package**](Package.md) |  |  [optional]
**expirationDate** | **kotlin.String** |  |  [optional]
**attachmentCount** | **kotlin.Boolean** |  |  [optional]
**sender** | [**UserBasicInfo**](UserBasicInfo.md) |  |  [optional]
**variables** | **kotlin.collections.List&lt;kotlin.String&gt;** |  |  [optional]
**secureBody** | **kotlin.Boolean** |  |  [optional]
**emailReturnReceipt** | [**kotlin.collections.List&lt;EmailReturnReceipt&gt;**](EmailReturnReceipt.md) |  |  [optional]
**error** | **kotlin.String** |  |  [optional]
**body** | **kotlin.String** | (Explicit field. May be retrieved only if mentioned in \&quot;with\&quot; parameter) |  [optional]
**rawBody** | **kotlin.String** | (Explicit field. May be retrieved only if mentioned in \&quot;with\&quot; parameter) |  [optional]
**headline** | **kotlin.String** | (Explicit field. May be retrieved only if mentioned in \&quot;with\&quot; parameter) |  [optional]
**notice** | **kotlin.String** | (Explicit field. May be retrieved only if mentioned in \&quot;with\&quot; parameter) |  [optional]
**htmlBody** | **kotlin.String** | (Explicit field. May be retrieved only if mentioned in \&quot;with\&quot; parameter) |  [optional]
**fullHtmlBody** | **kotlin.String** | (Explicit field. May be retrieved only if mentioned in \&quot;with\&quot; parameter) |  [optional]
**emailFrom** | **kotlin.String** | (Explicit field. May be retrieved only if mentioned in \&quot;with\&quot; parameter) |  [optional]
**isRead** | **kotlin.Boolean** |  |  [optional]
**bucket** | **kotlin.Boolean** |  |  [optional]
**templateBody** | **kotlin.String** | (Explicit field. May be retrieved only if mentioned in \&quot;with\&quot; parameter) |  [optional]
**webFormId** | **kotlin.String** | (Explicit field. May be retrieved only if mentioned in \&quot;with\&quot; parameter) |  [optional]
**webFormFields** | **kotlin.collections.List&lt;kotlin.String&gt;** | (Explicit field. May be retrieved only if mentioned in \&quot;with\&quot; parameter) |  [optional]
**links** | **kotlin.String** |  |  [optional]



