---
title: "Setup"
chapter: true
weight: 10
---
![Setup](/images/SMSsetup1-768x300.jpg)

## SMS Setup
Today, we'll set up the basics of SMS in Genesys Cloud CX. You'll purchase an SMS number directly from the Genesys Cloud admin portal, with Genesys being your SMS broker. You'll also import a basic Inbound Message Architect flow. Lastly, you'll connect the SMS number you purchased to the Architect flow that you imported through a messaging route. 

## Follow Along
1. Navigate to **Admin** screen > Search for **SMS Number Inventory** 
2.  When the SMS Number Inventory page appears, press **Purchase** in top right corner 
3. Fill in appropriate fields to search for number to purchase 
4. To view available numbers to purchase click **Search** 
5.  Click **Buy Now** > When the Confirm Number Purchase dialog appears 
6. click **Buy**  _(Note the number you purchased, because it is difficult to find after purchase)_

  
7. Go back into the queue you created earlier > Set the SMS number you just purchased as the outbound SMS number
    ![Queue Set Outbound SMS Number](/images/QueueSetSMSOutboundNumber.jpg)

8. Follow the instructions below to create an inbound message flow:

9. From the Architect home page, click or hover over the **Flows** menu and select **Inbound Message**
10. Click **+ Add** The Create Flow dialog box opens
11. In the Name field, type a unique name for the inbound message flow
12. Click **Create Flow**

13. Once inside the flow, drag a **Transfer to ACD** task to the **Start menu** as seen in the image below 
14. Click the drop-down menu and select the queue you created at the beginning 
15. Click the three dots next to the **Disconnect** Task to delete this task 
16.  Click **Publish** once you have completed these steps
![Inbound Message](/images/inboundmessage1.jpg)

17. Navigate to **Admin** screen > Search for **Message Routing** 
18.  Click **+** > Click **Select Flow** > Begin typing the first few letters of the inbound message flow you want to use and select from the list 
19. Under **Addresses** click **+** > Click **Select Address** > Click number you want to add 
20. Click **Add** > Click **Save**
Set up a messaging route to connect your inbound message architect flow and the SMS number you purchased in step two 

![Call Routing](/images/callrouting1.jpg)