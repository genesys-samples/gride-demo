---
title: "Roles & Permissions"
chapter: true
weight: 10
---
![Title](/images/UserConfig2-768x300.jpg)
## Roles and Permissions

>Each role in Genesys Cloud contains one or more permissions. The permissions allow users with that role to do >various tasks, such as create groups, set up integrations, and supervise contact center activity.

>The Employee role has the lowest level of permissions and is assigned to all users. This role cannot be removed. A user must be assigned additional roles by a Genesys Cloud Administrator to have additional permissions.
>The Admin role has permissions to make any changes to a Genesys Cloud organization. This role is automatically assigned to whoever sets up the organization. This person is responsible for inviting others to a Genesys Cloud organization and for assigning roles to invitees.





**Assiging Master Admin role to the user**

1.	Click Admin > People > **select your User Account**
2.	On the right side of the Roles screen, change “View:” from **Assigned** to **All**
3.	Assign **master admin** permissions and save the account

![Add Role](/images/RolesPic.png)

Create Role for Genesys Cloud Voice permissions

1.  Click Admin > Roles / Permissions > Click **"Add Role"**
2.	Name the role-Ex: GCV user or something you can easily find
3.	Switch to the permissions tab on the right and search for **“PureCloud Voice”** in the Permission field
4.	Check the box for all permissions and save
5.	Return to People and select your user again 
6.	Go to the right side of the Roles screen and change "View" from **Assigned** to **All**
7. Assign the GCV user you just created to yourself

![Permissions](/images/Permission.png)

**Add additional users to your organization**

**Note: Information below regarding adding additional users is for setting up actual dev environments and not in-person workshops led by Genesys**

When you create new users, all that is needed is a name and email (to send the invitation to). You may also expand to **Optional Fields** to assign fields such as Title, Department, Location, Queues, etc. should you know those details prior. There is also the option to bulk import users rather than adding users one at a time. 

If you choose to send invitations to new users later and manually set their status to inactive, when you send the invitations Genesys Cloud automatically changes their status to active <br>
1.	Click Admin <br>
2.	Under People and Permissions, click People <br>
3.	Click Add Person. The Add People to the Organization dialog box opens <br>

 

![People](/images/People.png)


4.	Click the **Person** tab.
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

#### External Contacts
Now that we have our contact center agent, let's create a customer to identify during our voice, SMS, and email interactions (During our webchat test, we'll set up a contact in the widget). 
External Contacts allows you to create a robust repository of customer data that your agents can take advantage of as they assist your customers. With External Contacts, an agent can quickly contact a customer by email, phone call, or Twitter message. During an interaction, an agent builds the interaction history for a client by verifying key contact data. The agent can quickly see who has interacted with the client and can read about your company’s relationship with them. 

As with most capabilities in Genesys Cloud, an external contact can be added from multiple locations. 

In today's workshop, 

1. Locate the **Directory** on the top-left of your UI, and click for a drop-down. 
2. Select **External Contacts**, on the far-right, choose **+Add** then **Contact**. 

![External Contact](/images/External.jpg)

Feel free to use a ficticious name here, as long as it is one that will be easily identified when the interaction comes in. After entering a name and selecting the arrow, a new screen will open with additional fields. 

3. Let's add an **Email** and **Phone Number**. 

*NOTE: These fields need to be valid, not ficticious, as this is what Genesys Cloud will reference when you call, text, and email in. Best practice would be to use your work email and any phone number you will use call/text to the org.*

4. Be sure to **Save** on the bottom-left, and we'll say goodbye to our customer for the time being. 

![External Contact](/images/Contact.jpg)