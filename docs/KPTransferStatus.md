
# KPTransferStatus

## Properties
Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**id** | **kotlin.String** | Unique identifier | 
**transactionId** | **kotlin.String** | Transaction Id | 
**kPObjectId** | **kotlin.String** | KP Object Id | 
**fileHandle** | **kotlin.String** | File name | 
**userId** | **kotlin.String** | User Id | 
**errCode** | **kotlin.String** | Error Code | 
**status** | **kotlin.String** | Status of ec file transaction:                                             0 - received request,                                             1 - in progress,                                             2 - completed successfully,                                             99 - transfer failed |  [optional]
**avStatus** | **kotlin.String** | AV Status (allowed|disallowed|scanning) |  [optional]
**dlpStatus** | **kotlin.String** | DLP Status (allowed|disallowed|scanning) |  [optional]



