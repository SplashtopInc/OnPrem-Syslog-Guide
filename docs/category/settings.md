# Syslog - Settings

<!-- 
# 这是注释
## Public Fields

| Field | Value | **Explanation** |
| --- | --- | --- |
| timestamp | ISO 8601 timestamp format | The date and time the event has been triggered. |
| team_id | Integer | Splashtop Team ID. |
| category | String | Splashtop events category. |
| kind | String | Splashtop events kind under specific category. |
| action | **add** or **update** or **delete** | The event operating action type in the event. |
| source_agent | **browser** or **client** or **streamer** or **openapi** or **scim** or **system** | The origin client of the specific event. |
| source_address | IPv4 format | The origin IP address in the specific event. |
| source_version | String | The origin client version in the specific event. |
| source_os | String | The origin operating system in the the event. |
| source_name | String | The origin client name in the specific event. |
| target_agent | **browser** or **client** or **streamer** | The target device type in the event. |
| target_address | IPv4 format | The target IP address in the event. |
| target_version | String | The target agent version in the event. |
| target_os | String | The target agent platform in the event |
| target_name | String | The target device name in the event. |
| target_account | String | The target user account in the event. |
-->

## AD Server

### **Events and triggers**

| **Event** | **Trigger** |
| --- | --- |
| adserver_added | A new AD server has been added and saved. |
| adserver_ldap_updated | The LDAP address of an AD server has been updated. |
| adserver_name_updated | The name of an AD server has been updated. |
| adserver_removed | An existing AD server has been removed. |

### **Fields**
| **Field** | **Value** | **Explanation** |
| --- | --- | --- |
| account | String | The user account that initiated the specific event. |
| target | String | The name of the target AD server. |
| result | String | Success or failure of the event. |
| ldap_addr | String | The added/updated LDAP address of the AD server. |
| name | String | The updated name of the AD server. |


## SMTP Server

### **Events and triggers**

| **Event** | **Trigger** |
| --- | --- |
| smtp_server_added | A new SMTP server has been added and saved. |
| smtp_server_disabled | An SMTP server has been disabled. |
| smtp_server_enabled | An SMTP server has been enabled. |
| smtp_server_removed | An existing SMTP server has been deleted. |
| smtp_server_updated | An existing SMTP server has been modified and saved. |
| gateway_url_updated | The Splashtop Gateway URL has been modified and saved. |

### **Fields**

| **Field** | **Value** | **Explanation** |
| --- | --- | --- |
| target | String | The target SMTP server address or specific configuration items such as gateway_url, address, email. |
| old_url | String | The previous Gateway URL. |
| old_addr | String | The previous SMTP server address. |
| old_mail | String | The previous sender Email address. |
| new_url | String | The updated Gateway URL. |
| new_addr | String | The updated SMTP server address. |
| new_email | String | The updated sender Email address. |
