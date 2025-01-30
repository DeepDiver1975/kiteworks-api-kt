
# Device

## Properties
Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**id** | **kotlin.Int** | Unique identifier of Device | 
**clientId** | **kotlin.String** | Unique identifier of client for this Device | 
**userId** | **kotlin.String** | Unique identifier of user for this Device | 
**installName** | **kotlin.String** | Install Tag name for this Device. e.g. Someone&#39;s IPhone | 
**installTagId** | **kotlin.String** | Unique identifier of install tag for this Device.Usually the serial number of Device |  [optional]
**wipeFlag** | **kotlin.String** | Flag that tells the device to remote wipe itself.      *                   0 &#x3D; not set, 1 &#x3D; set, 2 &#x3D; device has been notified, 3 &#x3D; wipe is completed |  [optional]
**mobileKeyStore** | **kotlin.String** | Key to encrypt files on this device |  [optional]
**links** | **kotlin.String** |  |  [optional]



