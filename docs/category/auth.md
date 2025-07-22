# Syslog - Auth

## **Account**

### **Events and triggers**

| **Event** | **Trigger** |
| --- | --- |
| account_added | A new account has been added and saved. |
| account_changed | An existing account has been modified and saved. |
| account_removed | An existing account has been deleted. |

### **Fields**

| **Field** | **Value** | **Explanation** |
| --- | --- | --- |
| name | string | The name of the account. |
| username | string | The username of the account |
| password | *** | Indicates if the password has changed. The actual string is never supplied. |
| auto_rotate_credentials | **1** or **0** | **1:** Enables the automatic rotation for this account.**0:** Disables the automatic rotation for this account. |
| allow_simultaneous_checkout | **1** or **0** | **1:** Account can be checked out and used by multiple users or sessions at the same time.**0:** Account can be checked out and used by single user at the same time. |
| personal | **1** or **0** | **1:** Is a personal account.**0:** Is a shared account. |
| group | string | The unique identifier of the account group. |

## **Account group**

### **Events and triggers**

| **Event** | **Trigger** |
| --- | --- |
| account_group_added | A new account group has been added and saved. |
| account_group_changed | An existing account group has been modified and saved. |
| account_group_removed | An existing account group has been deleted. |

### **Fields**

| **Field** | **Value** | **Explanation** |
| --- | --- | --- |
| id | string | The unique identifier of the account group. |
| name | string | The name of the account group. |
| description | string | The description of the account group. |

## **Account Jump Item association**

### **Events and triggers**

| **Event** | **Trigger** |
| --- | --- |
| account_jump_item_association_added | An association with a Jump Item was added for the account. |
| account_jump_item_association_changed | An association with a Jump Item was changed for the account. |
| account_jump_item_direct_association_added | The account is allowed to be injected for the specific Jump Items. |
| account_jump_item_direct_association_removed | The account is removed from the allowed list to be injected for the specific Jump Items. |

### **Fields**

| **Field** | **Value** | **Explanation** |
| --- | --- | --- |
| id | number | The unique identifier of the association. |
| account_group_id | number | The unique identifier of the account group. |
| account_id | number | The unique identifier of the account. |
| criteria | string | A JSON representation of the filters, e.g., **{"name":["name"],"host":["hostname"],"tag":["tag"],"comment":["comments"],"shared_jump_groups":[3]}** Valid only when the filter type is **criteria**. |
| filter_type | **applicablenot_injectablecriteria** | The filter type of the association. |

## **Accounts changed**

### **Events and triggers**

| **Event** | **Trigger** |
| --- | --- |
| accounts_changed | A group of one or more accounts was modified. |

### **Fields**

| **Field** | **Value** | **Explanation** |
| --- | --- | --- |
| accounts_id | comma-delimited list | The unique identifier of the vault accounts. |
| new_group | string | The unique identifier of the target account group. |

## **Admin password reset to factory default**

### **Events and triggers**

| **Event** | **Trigger** |
| --- | --- |
| admin_password_reset_to_factory_default | The **Reset Admin Account** button has been clicked, reverting a site’s administrative account to its default credentials. |

## **API account**

### **Events and triggers**

| **Event** | **Trigger** |
| --- | --- |
| api_account_added | A new API account has been added and saved. |
| api_account_changed | An existing API account has been modified and saved. |
| api_account_removed | An existing API account has been deleted. |

### **Fields**

| **Field** | **Value** | **Explanation** |
| --- | --- | --- |
| client_id | string | The OAuth client ID. |
| client_secret | *** | Indicates the OAuth client secret. The actual string is never supplied. |
| comments | string | Any comments associated with this API account. |
| enabled | **1** or **0** | **1:** This API account is enabled.**0:** This API account is disabled. |
| id | string | The unique identifier of the API account. |
| ip_addresses | comma-delimited list | The list of network address prefixes from which this account can authenticate. |
| name | string | The name of the API account. |
| permissions:backup | **1** or **0** | **1:** This API account may use the backup API.**0:** This API account may not use the backup API. |
| permissions:command | **denyread_onlyfull_access** | Whether this API account is disallowed to use the command API, has read-only access to the command API, or has full access to the command API. |
| permissions:reporting:archive | **1** or **0** | **1:** This API account may use the archive API.**0:** This API account may not use the archive API. |
| permissions:reporting:license | **1** or **0** | **1:** This API account may use the license reporting API.**0:** This API account may not use the license reporting API. |
| permissions:reporting:presentation | **1** or **0** | **1:** This API account may use the presentation reporting API.**0:** This API account may not use the presentation reporting API. |
| permissions:reporting:support | **1** or **0** | **1:** This API account may use the support reporting API.**0:** This API account may not use the support reporting API. |
| permissions:reporting:syslog | **denyread_onlyfull_access** | Whether this API account is disallowed access syslog reports, has read-only access to syslog reports, or has full access to syslog reports. |
