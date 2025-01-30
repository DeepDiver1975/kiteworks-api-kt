
# ClientNewPut

## Properties
Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**name** | **kotlin.String** | Client name | 
**description** | **kotlin.String** | Client description | 
**redirectUri** | **kotlin.String** | Where the server send the code that client can redeem access token.                         e.g. https://HOST/rest/callback.html | 
**scope** | **kotlin.String** | API entities which this client can access | 
**signatureKey** | **kotlin.String** | Signature Key for client |  [optional]
**accessTokenLifetime** | **kotlin.Int** | Life time for access token of client in hours. e.g. 5&#x3D;5 hours |  [optional]
**refreshTokenLifetime** | **kotlin.Int** | Life time for refresh token of client in hours |  [optional]



