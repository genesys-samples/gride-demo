---
title: "Setup"
chapter: true
weight: 10
---
![Title](/images/WebMessage1-768x300.jpg)
## Web Message Setup

Genesys Cloud CX is a true omnichannel platform, allowing for digital channels in addition to voice. One of those channels, web messaging, allows for an asynchronous experience where customers can return and resume where they left off. Web Messaging can also be enhanced with native Genesys digital bot flows. These A.I. driven bots allow for customers to accomplish their goals without the need of connecting with an agent. Of course, the ability to escalate to a live agent is always an option too. With attachments, co-browse, knowledgebase articles, and Predictive Engagement, Web Messaging is a versatile Genesys Cloud CX tool. 

![Web Message](/images/Messenger.jpg)

## Web Message Flow

Before we begin setting up our Web Message tool, we'll first need a message flow to route our interactions through. 

Follow the instructions below to create an inbound message flow:

* From the **Admin** page, locate and click **Architect**
* From the Architect home page, click or hover over the **Flows** menu and select **Inbound Message**
* Click **+ Add** The Create Flow dialog box opens
* In the Name field, type a unique name for the inbound message flow
* Click **Create Flow**

![Architect](/images/MessageFlow.jpg)

Once inside the flow, drag a **Transfer to ACD** task into the Initial State box and between **Start** and **Disconnect** as seen in the image below.

 Click the drop-down menu and select the queue you created at the beginning. Click the three dots next to the **Disconnect** Task to delete this task. Click **Save** & **Publish** once you have completed these steps
![Inbound Message](/images/inboundmessage1.jpg)

## Web Message Configuration

Now that we have our flow created, let's configure our messenger. Navigate back to the **Admin** page and find **Messenger Configurations** under the **Message** category.

Start by selecting **New Configuration** and give it a name based on the naming convention you had previously decided on. You can see there are some appearance options for the widget including color, position, and how to initiate the widget. We'll move past these for now and select our languages. 

The **Supported Languages** is a drop-down with all current supported languages within Genesys Cloud CX. After checking those needed, you'll then select the **Default Language**. When completed click **Save New Version**. 

![WebMessage Config](/images/Configuration.jpg)

In this workshop we did not touch on the additional tabs "Apps" and "Support Center" but feel free to learn more about web messaging options through our Resource Center and how you can further customize the Web Messenger tool.

On the left toolbar we can now select **Messenger Deployments** followed by **New Deployment**

As with each piece of our setup, we'll name it based on our naming convention. Then, scroll down and find **Select Configuration**. Once selected, you'll locate the configuration you built in the previous step. As you build more configurations or alter your current one, you'll have the option to select which version you wish to use for the current deployment. Click **Save**

You then have the option to decide whether you'd like to run this deployment on a specific site or set of sites, or to allow it to run on all domains. For demo purposes, it is best practice to select **Allow all domains**. 

Finally, we'll select the flow we had created earlier in Architect. Don't forget to **Save**

![WebMessage Config](/images/Deployment.jpg)

## Demo Extension Tool

The Demo Extension is ideal to quickly show your customer what it would be like to have their corporate website powered by Genesys Cloud CX. The Demo Extension tool showcases Genesys CX Widgets and Predictive Engagement, whether it be direct routing or leveraging Genesys Dialog Engine Bot Flows for self-service. 

The extension can be in three working states. The state applies per tab. These states are:

“OFF”: both Inspection and Injection are red. The extension has no impact on the browsed site.

“Demo Edit” mode: both Inspection and Injection are green. In this mode, you can add HotSpots (actions attached to selected elements) by using your mouse right-click and chosing the action to execute. Any {element, action} pair is highlighted with a green border line for you to identify what has been built.

“Demo Execution” mode: Injection is green and Inspection is red. This mode does not have the highlighted elements that do trigger the click actions. The site looks completely normal, but the actions associated to the elements will trigger when you click on them. To help you remember where to click and in what order, the extension icon will show the action name when hovering on active elements. Also, a counter will increment on the extension icon to indicate that the action triggered when the element has been clicked.

#### Tool Installation

Click https://chrome.google.com/webstore/detail/genesys-gdemo-extension/jiilhcbdojcdonkigflgmdnljialgmfh to add the Genesys Cloud Demo Extension tool to your Chrome browser.

![Demo Extension Tool](/images/DemoExtension.jpg)

* Open the Genesys Extension Tool and select Options
* Click on ‘Add Org’
* Select your Org region (Environment dropdown)
* Click on ‘Login to Org’ - a new tab will open to your Org’s login page
*In the new tab, login to your Org - the extension will pull the required configuration data from your Org and the tab will automatically close after few seconds
* Select the appropriate queue
* Check the box to enable Web Messaging and add your Web Deployment you had previously created
* Hit ‘Save’

![Demo Extension Tool](/images/ExtensionTool.jpg)