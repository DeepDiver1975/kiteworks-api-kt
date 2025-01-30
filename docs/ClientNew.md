
# ClientNew

## Properties
Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**id** | **kotlin.String** | Unique Client identifier | 
**name** | **kotlin.String** | Client name | 
**description** | **kotlin.String** | Client description |  [optional]
**redirectUri** | **kotlin.String** | Redirect URL of this client |  [optional]
**scope** | **kotlin.String** | API entities which this client can access |  [optional]
**flag** | **kotlin.Int** | Flags for Client. e.g. NO_CONSENT:1, DISABLED:2, HIDDEN:4, NO_EXPIRY_TOKEN :8 |  [optional]
**flow** | **kotlin.Int** | Oauth flow for this client.                         e.g. AUTH_CODE:1, CLIENT_CREDENTIAL:2, SIGNATURE:4, REFRESH_TOKEN:8 |  [optional]
**signatureKey** | **kotlin.String** | Signature Key for client |  [optional]
**accessTokenLifetime** | **kotlin.Int** | Life time for access token of client in hours. e.g. 5&#x3D;5 hours |  [optional]
**refreshTokenLifetime** | **kotlin.Int** | Life time for refresh token of client in hours |  [optional]
**whiteList** | **kotlin.String** | List of applications on the device that the client can call out to |  [optional]
**askPin** | **kotlin.Int** | Whether PIN should be requested of user using this client |  [optional]
**pinTimeout** | **kotlin.Int** | Time out for pin of client in minutes |  [optional]
**maxPinAttempts** | **kotlin.Int** | Max attempts that user can try to enter PIN before wipe occurs |  [optional]
**type** | **kotlin.Int** | Client Type. e.g. ACCELLION:1, MOBILE:2, OUTLOOK:4, SYNC:8, SHAREPOINT:16, IMPORTED:32 |  [optional]
**touchId** | **kotlin.Boolean** | Indicates whether touch Id is enabled |  [optional]
**clipboardEnabled** | **kotlin.Boolean** | Indicates whether clipboard is enabled |  [optional]
**autoUpdate** | **kotlin.Boolean** | Indicates whether auto update is enabled |  [optional]
**installer** | **kotlin.String** | Get the installer information |  [optional]
**emailMatch** | **kotlin.Boolean** | Indicates whether external email match with kw email |  [optional]
**minVersion** | **kotlin.Int** | Minimum API version of client |  [optional]
**links** | **kotlin.String** |  |  [optional]
**clientSecret** | **kotlin.String** | Client Secret |  [optional]



