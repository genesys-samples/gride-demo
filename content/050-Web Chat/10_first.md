---
title: "Setup"
chapter: true
weight: 10
---
![Setup](/images/Webchat1-768x300.jpg)
## Web Chat Setup

The web chat channel is an invaluable tool for communicating and engaging with customers to provide better service for answering questions, completing orders, general guidance on company’s product and features, and personalized customer support. With this solution, Genesys improves handle time, first contact resolution, agent utilization, and customer satisfaction.

![Web Chat](/images/webchat.png)

## Webchat Flow

Similar to our inbound voice module, we'll need an inbound flow to leverage routing capabilties and deliver webchats to the appropriate queue based on the intent of the customer. 

1. Click **Admin Page**. 
2. Click **Architect** tool and choose **Inbound Chat** from the drop-down menu. 
3. Click **+ Add**. We'll continue to use the same naming convention we have previously in this workshop, then **Create Flow**. 

We'll dive further into routing capabilties in our Archiect Workshop, but the chat toolbar is similar to what you'll find in other media type flows as well. When implementing self-service, Genesys Cloud easily integrates with Google DialogFlow and Amazon Lex along with our own native Bot Flows for both chat and voice. 

For now, we'll showcase how simplistic a flow can be, and simply.

1. Choose **Transfer to ACD** by dragging and dropping it onto the flow. 
2. All that's left is to decide which **Queue** we'll be routing to. Now **Save** and **Publish**

![Web Chat](/images/ChatFlow1.jpg)

## Genesys Widgets

Genesys offers three native versions of widgets as well as the option to integrate to a third party. Different versions of the widgets come with different benefits and features that you can enable. We recommend that you check out our comparison doc for our chat widgets. https://help.mypurecloud.com/articles/widget-feature-comparison/

Widgets allow you to add web chat to your website so customers can chat with agents directly from their browsers. When you create a widget in the Genesys Cloud CX Admin console, a deployment key will be created. The deployment key will help identify the configuration settings for the widget when you put the widget onto your website.

Having a website is not a prerequisite for this workshop. Instead, we will be routing chat interactions through our Genesys Cloud Demo Extension tool. Before we install the extension tool, let's first set up our widget within the Genesys Cloud CX org. **Note:** The maximum number of widget deployments in one org is 25. 

1. Click Admin, search for **Widgets**. 
2. Click **Create Widget** and give it a name using our standard naming convention. No description is neccesary in this workshop. 
3.  Assign **Version 2** under **Widget Type**. 
4. Choose the flow to route to, created above and finally be sure to **Save**

>## Demo Extension Tool
>
>The Demo Extension is ideal to quickly show your customer what it would be like to have their corporate website powered by Genesys Cloud. The Demo Extension showcases Genesys GX Widgets, Predictive Engagement and lets you engage with PureCloudNow or your own Genesys Cloud organization.
>
>The extension offers 2 main features categories:
    Widgets v1 based channels: chat v1, cobrowse/screenshare, email, callback
    Widgets v2 chat with Predictive Engagement (Predictive Engagement)
>
>The extension can be in three working states. The state applies per tab. These states are:

* "OFF": both Inspection and Injection are red. The extension has no impact on the browsed site.

* "Demo Edit" mode: both Inspection and Injection are green. In this mode, you can add HotSpots (actions attached to selected elements) by using your mouse right-click and chosing the action to execute. Any {element, action} pair is highlighted with a green border line for you to identify what has been built.

* "Demo Execution" mode: Injection is green and Inspection is red. This mode does not have the highlighted elements that do trigger the click actions. The site looks completely normal, but the actions associated to the elements will trigger when you click on them. To help you remember where to click and in what order, the extension icon will show the action name when hovering on active elements. Also, a counter will increment on the extension icon to indicate that the action triggered when the element has been clicked.

#### Installation

Click https://chrome.google.com/webstore/detail/genesys-gdemo-extension/jiilhcbdojcdonkigflgmdnljialgmfh to add the Genesys Cloud Demo Extension tool to your Chrome browser. 

![DemoExtension Installer](/images/DemoExtension.jpg)

1. Open the Genesys Extension Tool and select **Options**
2. Click on 'Add Org'
3. Select your Org region (Environment dropdown)
4. Click on 'Login to Org' - a new tab will open to your Org's login page
5. In the new tab, login to your Org - the extension will pull the required configuration data from your Org and the tab will automatically close after few seconds
6. Select the appropriate queue
7. Check the box to enable **Web Chat V2** and select the widget in **Deployment Key (V2)**
8. Hit 'Save'

![DemoExtension Installer](/images/ExtensionOptions.jpg)