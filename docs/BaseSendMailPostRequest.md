
# BaseSendMailPostRequest

## Properties
Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**returnReceipts** | **kotlin.collections.List&lt;kotlin.String&gt;** | List of to download notification&#39;s recipients&#39; email |  [optional]
**sharedMailboxId** | **kotlin.String** | The shared mailbox ID |  [optional]
**uploading** | **kotlin.Boolean** | Indicate whether upload is still in progress. Prevents sending if is set to true. |  [optional]
**preview** | **kotlin.Boolean** | Indicate that sending/saving mail as preview mail. |  [optional]
**to** | **kotlin.collections.List&lt;kotlin.String&gt;** | List of to recipients&#39; email |  [optional]
**acl** | [**inline**](#Acl) | The access control. |  [optional]
**webFormFields** | **kotlin.String** | The mail&#39;s web form fields. |  [optional]
**parentEmailId** | **kotlin.String** | The parent mail id used for mail threading. Applicalble only when type is &#39;forward&#39; or &#39;reply&#39; |  [optional]
**includeFingerprint** | **kotlin.Boolean** | Indicate that including fingerprint inside the mail. |  [optional]
**expire** | **kotlin.String** | The mail&#39;s expiry. |  [optional]
**watermark** | **kotlin.String** | The watermark on the preview mail. Applicable only when the preview is set. |  [optional]
**bcc** | **kotlin.collections.List&lt;kotlin.String&gt;** | List of bcc recipients&#39; email |  [optional]
**body** | **kotlin.String** | The mail&#39;s body. |  [optional]
**trackingAccess** | **kotlin.collections.List&lt;kotlin.String&gt;** | List of tracking access&#39; email |  [optional]
**isSelfReturnReceipt** | **kotlin.Boolean** | Send download notification to sender. (deprecated should use returnReceipts instead) |  [optional]
**subject** | **kotlin.String** | The mail&#39;s subject. |  [optional]
**webFormId** | **kotlin.String** | The mail&#39;s web form Id. |  [optional]
**notifyExpired** | **kotlin.Boolean** | Indicate whether to send notification email to sender when email expired |  [optional]
**selfCopy** | **kotlin.Boolean** | Indicate that sending a copy to sender. |  [optional]
**files** | **kotlin.collections.List&lt;kotlin.String&gt;** | List of file&#39;s ID |  [optional]
**cc** | **kotlin.collections.List&lt;kotlin.String&gt;** | List of cc recipients&#39; email |  [optional]
**secureBody** | **kotlin.Boolean** | Indicate that the mail is secure message. |  [optional]
**type** | [**inline**](#Type) | The mail type. Default value is original |  [optional]
**draft** | **kotlin.Boolean** | Indicate saving mail as draft. |  [optional]


<a id="Acl"></a>
## Enum: acl
Name | Value
---- | -----
acl | verify_recipient, no_auth, otp, internal, anyone_auth


<a id="Type"></a>
## Enum: type
Name | Value
---- | -----
type | original, forward, reply, resend



