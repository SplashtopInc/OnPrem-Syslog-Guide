# Syslog - Log

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
