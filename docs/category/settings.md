# settings.md

# Syslog - Settings

## Public Fields

| Field | Value | **Explanation** |
| --- | --- | --- |
| timestamp | ISO 8601 timestamp format | The date and time the event has been triggered. |
| team_id | Integer | Splashtop Team ID. |
| category | String | Splashtop events category. |
| kind | String | Splashtop events kind under specific category. |
| action | **add** or **update** or **delete** | The event operating action type in the event. |
| account | String | The user account that initiated the specific event. |
| source_agent | **browser** or **client** or **streamer** or **openapi** or **scim** or **system** | The origin client of the specific event. |
| source_address | String | IPv4 format. The origin IP address in the specific event. |
| source_version | String | The origin client version in the specific event. |
| source_os | String | The origin operating system in the the event. |
| source_name | String | The origin client name in the specific event. |
| target_agent | **browser** or **client** or **streamer** | The target device type in the event. |
| target_address | String | IPv4 format. The target IP address in the event. |
| target_version | String | The target agent version in the event. |
| target_os | String | The target agent platform in the event |
| target_name | String | The target device name in the event. |
| target_account | String | The target user account in the event. |
| result | String | Success or failure of the event. |

## AD Server

### **Events and triggers**

| **Event** | **Trigger** |
| --- | --- |
| adserver_added | A new AD server has been added and saved. |
| adserver_ldap_updated | The LDAP address of an AD server has been updated. |
| adserver_name_updated | The name of an AD server has been updated. |
| adserver_removed | An existing AD server has been deleted. |

### **Fields**

| **Field** | **Value** | **Explanation** |
| --- | --- | --- |
| target | String | The name of the target AD server. |
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

## Unattended Access

### **Events and triggers**

| **Event** | **Trigger** |
| --- | --- |
| team_grant_granular_file_transfer_download_updated | The admin-configurable value of the file transfer (download) has been updated for the team. |
| team_grant_granular_file_transfer_upload_updated | The admin-configurable value of the file transfer (upload) has been updated for the team. |
| team_grant_granular_remote_command_updated | The admin-configurable value of the remote command has been updated for the team. |
| team_grant_granular_remote_print_updated | The admin-configurable value of the remote print has been updated for the team. |
| team_grant_granular_request_permission_updated | The admin-configurable value of the request permission to connect has been updated for the team. |
| team_grant_granular_text_copy_paste_local_remote_updated | The admin-configurable value of the copy and paste (from local to remote) has been updated for the team. |
| team_grant_granular_text_copy_paste_remote_local_updated | The admin-configurable value of the copy and paste (from remote to local) has been updated for the team. |
| team_grant_granular_watermark_protection_updated | The admin-configurable value of the watermark protection has been updated for the team. |
| team_granular_file_transfer_download_admin_updated | The team’s granular control of the file transfer (download) for admins has been updated. |
| team_granular_file_transfer_download_member_updated | The team’s granular control of the file transfer (download) for members has been updated. |
| team_granular_file_transfer_upload_admin_updated | The team’s granular control of the file transfer (upload) for admins has been updated. |
| team_granular_file_transfer_upload_member_updated | The team’s granular control of the file transfer (upload) for members has been updated. |
| team_granular_remote_command_admin_updated | The team’s granular control of the remote command for admins has been updated. |
| team_granular_remote_command_member_updated | The team’s granular control of the remote command for members has been updated. |
| team_granular_remote_print_admin_updated | The team’s granular control of the remote print for admins has been updated. |
| team_granular_remote_print_member_updated | The team’s granular control of the remote print for members has been updated. |
| team_granular_request_permission_admin_updated | The team’s granular control of the request permission to connect for admins has been updated. |
| team_granular_request_permission_member_updated | The team’s granular control of the request permission to connect for members has been updated. |
| team_granular_text_copy_paste_local_remote_admin_updated | The team’s granular control of the copy and paste (from local to remote) for admins has been updated. |
| team_granular_text_copy_paste_local_remote_member_updated | The team’s granular control of the copy and paste (from local to remote) for members has been updated. |
| team_granular_text_copy_paste_remote_local_admin_updated | The team’s granular control of the copy and paste (from remote to local) for admins has been updated. |
| team_granular_text_copy_paste_remote_local_member_updated | The team’s granular control of the copy and paste (from remote to local) for members has been updated. |
| team_granular_watermark_protection_admin_updated | The team’s granular control of the watermark protection for admins has been updated. |
| team_granular_watermark_protection_member_updated | The team’s granular control of the watermark protection for members has been updated. |
| team_granular_request_permission_admin_updated | The team’s granular control of the request permission to connect for admins has been updated. |
| team_granular_request_permission_member_updated | The team’s granular control of the request permission to connect for members has been updated. |
| team_granular_centralized_session_recording_unattended_admin_updated | The team’s granular control of the centralized session recording (unattended) for admins has been updated. |
| team_granular_centralized_session_recording_unattended_member_updated | The team’s granular control of the centralized session recording (unattended) for members has been updated. |
| team_grant_granular_rcentralized_session_recording_unattended_updated | The admin-configurable value of the centralized session recording (unattended) has been updated for the team. |
| team_granular_system_tools_admin_updated | The team’s granular control of the system tools (unattended) for admins has been updated. |
| team_granular_system_tools_member_updated | The team’s granular control of the system tools (unattended) for members has been updated. |
| team_grant_granular_system_tools_updated | The admin-configurable value of the system tools (unattended) has been updated for the team. |
| team_granular_request_permission_rdp_admin_updated | The team’s granular control of the request permission to connect (RDP session) for admins has been updated. |
| team_granular_request_permission_rdp_member_updated | The team’s granular control of the request permission to connect (RDP session) for members has been updated. |
| team_grant_granular_request_permission_rdp_updated | The admin-configurable value of the  request permission to connect (RDP session) has been updated for the team. |
| team_remove_offline_computers_days_updated | The offline computer policy settings have been updated. |
| team_session_indicator_remote_session_type_updated | The display type of the remote session indicator has been updated. |
| team_session_indicator_background_action_type_updated | The display type of the background action session indicator has been updated. |
| team_centralized_session_recording_disabled | The centralized session recording function has been disabled for unattended access at the team level. |
| team_centralized_session_recording_enabled | The centralized session recording function has been enabled for unattended access at the team level. |
| team_concurrent_session_disabled | The concurrent session has been disabled for unattended access. |
| team_concurrent_session_enabled | The concurrent session has been enabled for unattended access. |
| team_device_redirect_disabled | The device redirection function has been disabled for unattended access at the team level. |
| team_device_redirect_enabled | The device redirection function has been enabled for unattended access at the team level. |
| team_file_transfer_disabled | The file transfer function has been disabled for unattended access. |
| team_file_transfer_enabled | The file transfer function has been enabled for unattended access. |
| team_keystroke_paste_disabled | The paste clipboard as keystrokes function has been disabled for unattended access. |
| team_keystroke_paste_enabled | The paste clipboard as keystrokes function has been enabled for unattended access. |
| team_mac_address_restriction_disabled | The MAC address restriction has been disabled at the team level. |
| team_mac_address_restriction_enabled | The MAC address restriction has been enabled at the team level. |
| team_mac_address_restriction_updated | The settings of the MAC address restriction have been updated. |
| team_rdp_computer_disabled | The RDP computer has been disabled at the team level. |
| team_rdp_computer_enabled | The RDP computer has been enabled at the team level. |
| team_remote_command_disabled | The remote command function has been disabled at the team level. |
| team_remote_command_enabled | The remote command function has been enabled at the team level. |
| team_remote_mic_disabled | The remote microphone function has been disabled at the team level. |
| team_remote_mic_enabled | The remote microphone function has been enabled at the team level. |
| team_remote_print_disabled | The remote print function has been disabled at the team level. |
| team_remote_print_enabled | The remote print function has been enabled at the team level. |
| team_remote_reboot_disabled | The remote reboot computer function has been disabled at the team level. |
| team_remote_reboot_enabled | The remote reboot computer function has been enabled at the team level. |
| team_remote_voice_call_disabled | Remote session voice call has been disabled. |
| team_remote_voice_call_enabled | Remote session voice call has been enabled. |
| team_remote_wakeup_disabled | The remote wakeup function for computers has been disabled at the team level. |
| team_remote_wakeup_enabled | The remote wakeup function for computers has been enabled at the team level. |
| team_remote_web_app_disabled | The Web app for unattended access has been disabled. |
| team_remote_web_app_enabled | The Web app for unattended access has been enabled. |
| team_remove_offline_computers_disabled | The offline computer policy has been disabled at the team level. |
| team_remove_offline_computers_enabled | The offline computer policy has been enabled at the team level. |
| team_session_chat_disabled | The pre-session chat function has been disabled at the team level. |
| team_session_chat_enabled | The pre-session chat function has been enabled at the team level. |
| team_session_recording_disabled | The local session recording has been disabled at the team level. |
| team_session_recording_enabled | The local session recording has been enabled at the team level. |
| team_ssh_session_disabled | The SSH computer has been disabled at the team level. |
| team_ssh_session_enabled | The SSH computer has been enabled at the team level. |
| team_text_copypaste_disabled | The copy and paste function has been disabled at the team level. |
| team_text_copypaste_enabled | The copy and paste function has been enabled at the team level. |
| team_vnc_session_disabled | The VNC computer has been disabled at the team level. |
| team_vnc_session_enabled | The VNC computer has been enabled at the team level. |
| team_wacom_bridge_disabled | The Wacom Bridge function has been disabled at the team level. |
| team_wacom_bridge_enabled | The Wacom Bridge function has been enabled at the team level. |
| team_watermark_disabled | The watermark function has been disabled for unattended access. |
| team_watermark_enabled | The watermark function has been enabled for unattended access. |
| team_system_tool_enabled | The system tools has been enabled for unattended access. |
| team_system_tool_disabled | The system tools has been disabled for unattended access. |
| team_close_banner_remote_session_enabled | The function of allowing users to close the indicator banner has been enabled for remote sessions. |
| team_close_banner_remote_session_disabled | The function of allowing users to close the indicator banner has been disabled for remote sessions. |
| team_close_banner_background_action_enabled | The function of allowing users to close the indicator banner has been enabled for background action sessions. |
| team_close_banner_background_action_disabled | The function of allowing users to close the indicator banner has been disabled for background action sessions. |
| team_save_off_session_chat_transcript_enabled | The save off-session chat transcript has been enabled at team level. |
| team_save_in_session_chat_transcript_enabled | The save in-session chat transcript has been enabled for unattended access. |
| team_save_off_session_chat_transcript_disabled | The save off-session chat transcript has been disabled at team level. |
| team_save_in_session_chat_transcript_disabled | The save in-session chat transcript has been disabled for unattended access. |

### **Fields**

| **Field** | **Value** | **Explanation** |
| --- | --- | --- |
| grant_granular_file_transfer_download | **on** or **off** | The admin has been granted or not granted the permission to configure file transfer (download). |
| grant_granular_file_transfer_upload | **on** or **off** | The admin has been granted or not granted the permission to configure file transfer (upload). |
| grant_granular_remote_command | **on** or **off** | The admin has been granted or not granted the permission to configure remote command. |
| grant_granular_remote_print | **on** or **off** | The admin has been granted or not granted the permission to configure remote print. |
| grant_granular_request_permission | **on** or **off** | The admin has been granted or not granted the permission to configure request-to-connect permission . |
| grant_granular_text_copy_paste_local_remote | **on** or **off** | The admin has been granted or not granted the permission to configure copy and paste (from local to remote). |
| grant_granular_text_copy_paste_remote_local | **on** or **off** | The admin has been granted or not granted the permission to configure copy and paste (from remote to local). |
| grant_granular_watermark_protection | **on** or **off** | The admin has been granted or not granted the permission to configure watermark protection. |
| granular_file_transfer_download_admin | **on** or **off** | The team’s granular control of the file transfer (download) for admins has been turned on or off. |
| granular_file_transfer_download_member | **on** or **off** | The team’s granular control of the file transfer (download) for members has been turned on or off. |
| granular_file_transfer_upload_admin | **on** or **off** | The team’s granular control of the file transfer (upload) for admins has been turned on or off. |
| granular_file_transfer_upload_member | **on** or **off** | The team’s granular control of the file transfer (upload) for members has been turned on or off. |
| granular_remote_command_admin | **on** or **off** | The team’s granular control of the remote command for admins has been turned on or off. |
| granular_remote_command_member | **on** or **off** | The team’s granular control of the remote command for members has been turned on or off. |
| granular_remote_print_admin | **on** or **off** | The team’s granular control of the remote print for admins has been turned on or off. |
| granular_remote_print_member | **on** or **off** | The team’s granular control of the remote print for members has been turned on or off. |
| granular_request_permission_admin | **on** or **off** | The team’s granular control of the request permission to connect for admins has been turned on or off. |
| granular_request_permission_member | **on** or **off** | The team’s granular control of the request permission to connect for members has been turned on or off. |
| granular_text_copy_paste_local_remote_admin | **on** or **off** | The team’s granular control of the copy and paste (from local to remote) for admins has been turned on or off. |
| granular_text_copy_paste_local_remote_member | **on** or **off** | The team’s granular control of the copy and paste (from local to remote) for members has been turned on or off. |
| granular_text_copy_paste_remote_local_admin | **on** or **off** | The team’s granular control of the copy and paste (from remote to local) for admins has been turned on or off. |
| granular_text_copy_paste_remote_local_member | **on** or **off** | The team’s granular control of the copy and paste (from remote to local) for members has been turned on or off. |
| granular_watermark_protection_admin | **on** or **off** | The team’s granular control of the watermark protection for admins has been turned on or off. |
| granular_watermark_protection_member | **on** or **off** | The team’s granular control of the watermark protection for members has been turned on or off. |
| granular_request_permission_admin | String | The team’s granular control of the request permission to connect for admins has been turned on or off. |
| granular_request_permission_member | String | The team’s granular control of the request permission to connect for members has been turned on or off. |
| granular_centralized_session_recording_unattended_admin | **on** or **off** | The team’s granular control of the centralized session recording (unattended) for admins has been turned on or off. |
| granular_centralized_session_recording_unattended_member | **on** or **off** | The team’s granular control of the centralized session recording (unattended) for members has been turned on or off. |
| grant_granular_rcentralized_session_recording_unattended | **on** or **off** | The admin has been granted or not granted the permission to configure centralized session recording (unattended). |
| granular_system_tools_admin | **on** or **off** | The team’s granular control of the system tools (unattended) for admins has been turned on or off. |
| granular_system_tools_member | **on** or **off** | The team’s granular control of the system tools (unattended) for members has been turned on or off. |
| grant_granular_system_tools | **on** or **off** | The admin has been granted or not granted the permission to configure system tools (unattended). |
| granular_request_permission_rdp_admin | String | The team’s granular control of the request permission to connect (RDP session) for admins has been turned on or off. |
| granular_request_permission_rdp_member | String | The team’s granular control of the request permission to connect (RDP session) for members has been turned on or off. |
| grant_granular_request_permission_rdp | **on** or **off** | The admin has been granted or not granted the permission to configure request permission to connect (RDP session). |
| remove_offline_computers_days | String | The computer offline day threshold for offline computer policy. |
| exec_at | String | The daily time of running the offline computer policy. |
| session_indicator_type | **Both** or **Pop-up** or **Banner** or **None** | The indicator type for remote session or background actions. |

## User Settings

### **Events and triggers**

| **Event** | **Trigger** |
| --- | --- |
| team_group_manager_disabled | Group manager role has been disabled at the team level. |
| team_group_manager_enabled | Group manager role has been enabled at the team level. |
| team_member_connect_active_session_disabled | The function of allowing member roles to connect to the active session has been disabled. |
| team_member_connect_active_session_enabled | The function of allowing member roles to connect to the active session has been enabled. |
| team_member_create_multi_session_disabled | The function of allowing member roles to establish multiple sessions concurrently has been disabled. |
| team_member_create_multi_session_enabled | The function of allowing member roles to establish multiple sessions concurrently has been enabled. |
| team_member_disconnect_session_disabled | The function of allowing member roles to disconnect the active session has been disabled. |
| team_member_disconnect_session_enabled | The function of allowing member roles to disconnect the active session has been enabled. |
| team_member_reboot_disabled | The function of allowing member roles to reboot computers and Streamers has been disabled. |
| team_member_reboot_enabled | The function of allowing member roles to reboot computers and Streamers has been enabled. |
| team_member_see_group_disabled | The function of allowing member roles to see all groups has been disabled. |
| team_member_see_group_enabled | The function of allowing member roles to see all groups has been enabled. |
| team_remote_reboot_action_updated | The settings of allowing member roles to reboot computers and Streamers have been updated. |
| team_member_permission_for_computer_notes_updated | The settings of member’s permission for computer notes have been updated. |

### **Fields**

| **Field** | **Value** | **Explanation** |
| --- | --- | --- |
| remote_reboot_member | **Restart streamer
Normal reboot
Safe-mode reboot** | Actions that member role is allowed to perform on the computers. |
| permission_for_computer_notes | **cannot view and edit** or **view only** or **view and edit** | Whether member role cannot view and edit the computer notes, can only view the computer notes, or can view and edit the computer notes. |