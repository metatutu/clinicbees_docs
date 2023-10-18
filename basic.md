## User Roles

After your _**Clinic Bees**_ is setup, all users on the Slack workspace of the clinic is able to access the service.
There are 3 different roles, and one user is with one specific role at a time based on the configuration by owner:

* **Owner role**

This is basically the owner of the Slack workspace and the Clinic Bees system.
It will automatically detect the owner from Slack workspace settings.
The Primary Workspace Owner will be assumed the Owner of the _**Clinic Bees**_ system for this workspace as well.

>[!TIP]
>Check Slack workspace members via Administration/Manage members to see full user list of the Slack workspace.
![Manage members](images/slack-admin-members.png)


* **Admin role**

This is a role with permissions to access everyone's data and access to performance settings such as focus.
Owner could delegate some users with Admin role, so that Admin users could be shared some duties with Owner
and help Owner to manage the whole system in clinic.

Owner could [assign](reference/commands_sys.md#assign-admin) or 
[revoke](reference/commands_sys.md#revoke-admin) the Admin users.

* **User role**

If a user is neither a Owner nor a Admin, then it's a general user in the system.