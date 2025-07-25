# Syslog - Settings

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
