---
title: "WebRTC Phone Setup"
chapter: true
weight: 30
---
![Title](/images/WebRTC-768x300.jpg)
## Create a WebRTC Base Setting

 Before you can create a phone, create a base settings configuration for that phone model. The base settings configuration contains a group of settings found on the Base Phone and Base Line Appearance tabs that define how a particular phone model is to operate in Genesys Cloud. Once you create a base settings configuration, you can save it with the default settings or you can customize the settings. These settings can be quickly referenced to streamline new phone provisioning. 


1. Click Admin> Phone Management> Click "Base Settings"

2.  Select **"Add Base Settings"**. Enter a name such as **"General WebRTC"** then search in the "Phone Make and Model" field for **Genesys Cloud WebRTC Phone"**. 

3. Click **"Save base setting"**


![BaseSettingsConfig](/images/BaseSettings.jpg)

## Create a WebRTC Phone for Your User

 Genesys Cloud supports the WebRTC technology with the Genesys Cloud WebRTC phone. Provisioning a Genesys Cloud WebRTC phone for a user creates a specific phone line for that user. The Genesys Cloud WebRTC phone does not require the installation of a software client on the PC. You use the Genesys Cloud call controls for the WebRTC phone calls.

1.  Click  Admin> Phone Management> Click "Add Phone"** *Best practice is to name your phone after the user who will be associated with it.* 
 
 2. Select the **WebRTC Base Setting** you created in the previous step. 
 
 3. Select the **site** you created in the previous chapter. 
 
 4.  Select the **agent** who will be utilizing the WebRTC phone.  


![WebRTCPhoneSettings](/images/PhoneSetup.jpg)

## Activating Your Phone

1. Locate the phone icon on the left toolbar. Note: The phone maybe red with a line through it because you don't have a phone assigned.  

2. Select the **"Phone Details"** icon on the slide out menu. 

3. Click the **"Select Phone"** for search for the name if your phone. Your WebRTC setup is now complete, assigned to the appropriate agent, and ready to handle voice interactions. 


![PhoneAssignment](/images/PhoneSelect.jpg)