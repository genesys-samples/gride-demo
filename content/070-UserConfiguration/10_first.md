---
title: "User Configuration"
chapter: true
weight: 10
---
# Roles and Permissions

Each role in Genesys Cloud contains one or more permissions. The permissions allow users with that role to do various tasks, such as create groups, set up integrations, and supervise contact center activity.

The Employee role has the lowest level of permissions and is assigned to all users. This role cannot be removed. A user must be assigned additional roles by a Genesys Cloud Administrator to have additional permissions.
The Admin role has permissions to make any changes to a Genesys Cloud organization. This role is automatically assigned to whoever sets up the organization. This person is responsible for inviting others to a Genesys Cloud organization and for assigning roles to invitees.




Follow along 
Associate Master Admin role to the user
1.	Admin > People > select your user account
2.	On the right side of the Roles screen, change “View:” from Assigned to All
3.	Assign master admin permissions and save the account

![Add Role](/images/RolesPic.png)

Create Role for Genesys Cloud Voice permissions
Admin > Roles / Permissions > Add Role
1.	Name the role
2.	Switch the permissions tab and search “PureCloud voice” in the Permission   field
3.	Check the box for all permissions and save
4.	Return to People and select your user again. 
5.	Go to the Roles screen and make sure to assign this GCV role to your user.

![Permissions](/images/Permission.png)