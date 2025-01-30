
# ContactBase

## Properties
Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**id** | **kotlin.Int** | Contact unique identifier | 
**userId** | **kotlin.String** | Contact owner unique identifier | 
**name** | **kotlin.String** | Contact name | 
**modified** | [**java.time.LocalDate**](java.time.LocalDate.md) | Contact modification date |  [optional]
**created** | [**java.time.LocalDate**](java.time.LocalDate.md) | Contact creation date |  [optional]
**items** | [**kotlin.collections.List&lt;ContactItem&gt;**](ContactItem.md) | List of emails contained by Contact |  [optional]
**links** | **kotlin.String** |  |  [optional]



