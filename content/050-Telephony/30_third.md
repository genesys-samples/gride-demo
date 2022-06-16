---
title: "WebRTC Phone Setup"
chapter: false
weight: 30
---
![Test](/images/testing2.jpg)
## Create a WebRTC Base Setting
1. Before you can create a phone, create a base settings configuration for that phone model. The base settings configuration contains a group of settings found on the Base Phone and Base Line Appearance tabs that define how a particular phone model is to operate in Genesys Cloud. Once you create a base settings configuration, you can save it with the default settings or you can customize the settings. These settings can be quickly referenced to streamline new phone provisioning. 
Phone Management is under the Telephony category where your site was just setup. Select "Base Settings" then "Add Base Settings". Enter a name such as "General WebRTC" then search in the "Phone Make and Model" field for Genesys Cloud WebRTC Phone". Save your base setting.

![BaseSettingsConfig](/images/BaseSettings.jpg)

## Create a WebRTC Phone for Your User
1. Genesys Cloud supports the WebRTC technology with the Genesys Cloud WebRTC phone. Provisioning a Genesys Cloud WebRTC phone for a user creates a specific phone line for that user. The Genesys Cloud WebRTC phone does not require the installation of a software client on the PC. You use the Genesys Cloud call controls for the WebRTC phone calls.
Return to the Phone Management menu and select "Add Phone". Best practice is to name your phone after the user who will be associated with it. Select the WebRTC Base Setting you created in the previous step. Select the site you created in the previous chapter. Finally, select the agent who will be using it. 

![WebRTCPhoneSettings](/images/PhoneSetup.jpg)

## Activating Your Phone
1. From the Genesys Cloud CX UI, locate the red phone icon on the left toolbar. Select the "Phone Details" icon on the slide out menu. Click the "Select Phone" for search for the name if your phone. Your WebRTC setup is now complete, assigned to the appropriate agent, and ready to handle voice interactions. 

![PhoneAssignment](/images/PhoneSelect.jpg)