---
title: "Roles & Permissions"
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
Admin > Roles / Permissions > Click "Add Role"
1.	Name the role-Ex: GCV user or something you can easily find
2.	Switch to the permissions tab on the right and search for “PureCloud voice” in the Permission field
3.	Check the box for all permissions and save
4.	Return to People and select your user again 
5.	Go to the right side of the Roles screen and change "View" from Assigned to All
6. Assign the GCV user you just created to yourself

![Permissions](/images/Permission.png)

Add people to your organization
When you create new users, Genesys Cloud automatically sets their status as active whether you send the invitation now or later.
If you choose to send invitations to new users later and manually set their status to inactive, when you send the invitations Genesys Cloud automatically changes their status to active <br>
1.	Click Admin <br>
2.	Under People and Permissions, click People <br>
3.	Click Add Person. The Add People to the Organization dialog box opens <br>
 

![People](/images/People.png)

4.	Click the Person tab.
5.	Complete the mandatory Name and Email fields. 
6.	(Optional) Enter additional information by clicking Optional Fields. 
7.	Note: The Manager field is optional but recommended. Genesys Cloud uses manager assignments to create hierarchy views
8.	(Optional) To add the person to a queue, do the following:
9.	Under Assign Queues, begin typing the first few letters of the desired queue
10.	Select it from the list
11.	Note: Make sure you assign the Employee role, along with any other role. Typically, the employee role is assigned by default. However, manually adding roles during user creation overrides the employee’s assigned default.
12.	(Optional) To add roles for the person, do the following:
13.	Under Assign Roles, begin typing the first few letters of the desired role
14.	Select it from the list
15.	Assign additional roles as necessary 
16.	Send the invite automatically by selecting Send invite now 
17.	Note:  The people you add cannot join Genesys Cloud until they receive an invite. If you don’t do this now, remember to do it later
18.	Click Create
