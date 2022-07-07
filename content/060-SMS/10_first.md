---
title: "Setup"
chapter: true
weight: 10
---
![Setup](/images/SMSsetup1-768x300.jpg)

## SMS Setup
Today, we'll set up the basics of SMS in Genesys Cloud CX. You'll purchase an SMS number directly from the Genesys Cloud admin portal, with Genesys being your SMS broker. You'll also import a basic Inbound Message Architect flow. Lastly, you'll connect the SMS number you purchased to the Architect flow that you imported through a messaging route. 

## Follow Along
1. Navigate to **Admin** screen > Search for **SMS Number Inventory** > When the SMS Number Inventory page appears, press **Purchase** in top right corner > Fill in appropriate fields to search for number to purchase > To view available numbers to purchase click **Search** > Click **Buy Now** > When the Confirm Number Purchase dialog appears, click **Buy**  _(Note the number you purchased, because it is difficult to find after purchase)_

  
2. Go back into the queue you created earlier > Set the SMS number you just purchased as the outbound SMS number
    ![Queue Set Outbound SMS Number](/images/QueueSetSMSOutboundNumber.jpg)

3. Follow the instructions below to create an inbound message flow

![Inbound Message](/images/inboundmessage.jpg)

4. Once inside the flow, drag a **Transfer to ACD** task to the **Start menu** as seen in the image below > Click the drop-down menu and select the queue you created at the beginning > Click the three dots next to the **Disconnect** Task to delete this task > Click **Publish** once you have completed these steps
![Inbound Message](/images/inboundmessage1.jpg)

5. Navigate to **Admin** screen > Search for **Message Routing** > Click **+** > Click **Select Flow** > Begin typing the first few letters of the inbound message flow you want to use and select from the list > Under **Addresses** click **+** > Click **Select Address** > Click number you want to add > Click **Add** > Click **Save**
Set up a messaging route to connect your inbound message architect flow and the SMS number you purchased in step two 

![Call Routing](/images/callrouting1.jpg)