
# PackagePut

## Properties
Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**selfCopy** | **kotlin.Boolean** | Send a copy of the Email to yourself. True or False |  [optional]
**includeFingerprint** | **kotlin.Boolean** | Include file fingerprint in email |  [optional]
**expire** | **kotlin.String** | Expiration date of package in hours |  [optional]
**fileCount** | **kotlin.Int** | Set number of files included in the Email package |  [optional]
**deleted** | **kotlin.Boolean** | Whether this Email package was deleted or not |  [optional]
**acl** | [**inline**](#Acl) | Indicates whether the recipient is required to sign in (verify_recipient)      *                  or if they can download without signing in (no_auth) |  [optional]


<a id="Acl"></a>
## Enum: acl
Name | Value
---- | -----
acl | verify_recipient, no_auth, otp, internal, anyone_auth



