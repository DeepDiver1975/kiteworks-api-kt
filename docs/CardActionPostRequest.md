
# CardActionPostRequest

## Properties
Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**action** | [**inline**](#Action) | Action to take (e.g. dismiss, retry, delete) | 
**type** | [**inline**](#Type) | Type of card to retrieve. Available card type(s): content_encryption,email_json_migration,event_log_partitioning_migration,system_security_scanning,events_table_monitor,appadmin_db,sysadmin_db,sysadmin_hosts | 
**fileId** | **kotlin.collections.List&lt;kotlin.Int&gt;** | List of File IDs to retry encryption |  [optional]
**storageType** | **kotlin.String** | Storage type for files (either &#39;user_files&#39; or &#39;replication_files&#39;) |  [optional]
**emailId** | **kotlin.collections.List&lt;kotlin.Int&gt;** | List of Email IDs to retry migrating to JSON format |  [optional]
**volume** | **kotlin.String** | Volume for files |  [optional]
**hostId** | **kotlin.String** | Host ID |  [optional]


<a id="Action"></a>
## Enum: action
Name | Value
---- | -----
action | retry, delete


<a id="Type"></a>
## Enum: type
Name | Value
---- | -----
type | content_encryption, email_json_migration, event_log_partitioning_migration, system_security_scanning, events_table_monitor, appadmin_db, sysadmin_db, sysadmin_hosts



