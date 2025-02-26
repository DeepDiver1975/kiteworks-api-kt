
# RequestFilePut

## Properties
Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**to** | **kotlin.collections.List&lt;kotlin.String&gt;** | Email recipients | 
**subject** | **kotlin.String** | Email subject |  [optional]
**body** | **kotlin.String** | Email body |  [optional]
**expire** | **kotlin.String** | Expiration date for the requestFile link. The link becomes unusable after this date,                         but the files uploaded using this link will follow the expiry setting of the folder. |  [optional]
**count** | **kotlin.Int** | The remaining uploads allowed |  [optional]
**requireAuth** | **kotlin.Boolean** | Whether uploader needs to sign in to upload files |  [optional]
**actionId** | **kotlin.Int** | Whether uploader can view &#x3D; 1 or download &#x3D; 2 |  [optional]
**files** | **kotlin.collections.List&lt;kotlin.String&gt;** | File IDs that requester may want to include and available for uploaders to see/download |  [optional]
**secureBody** | **kotlin.Boolean** |  |  [optional]



