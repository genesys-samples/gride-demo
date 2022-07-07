---
title: "Setup"
chapter: true
weight: 10
---
![Setup](/images/SMSsetup1-768x300.jpg)

## SMS Setup
Today, we'll set up the basics of SMS in Genesys Cloud CX. You'll purchase an SMS number directly from the Genesys Cloud admin portal, with Genesys being your SMS broker. You'll also import a basic Inbound Message Architect flow. Lastly, you'll connect the SMS number you purchased to the Architect flow that you imported through a messaging route. 

## Follow Along
1. Purchase a number for SMS (Note  the number you purchased, because it is difficult to find after purchase)

 ![SMS](/images/sms1.jpg) 
2. Go back into the G Ride queue and set the SMS number you just purchased as the outbound SMS number
    ![Queue Set Outbound SMS Number](/images/QueueSetSMSOutboundNumber.jpg)

3. Follow the instructions below to create an inbound message flow

![Inbound Message](/images/inboundmessage.jpg)

4. Once inside the flow, drag a "Transfer to ACD" task to the "Start menu" as seen in the image below. Click the drop-down menu and select your "G Ride" queue or the queue you created at the beginning. Hit the three dots next to the "Disconnect" Task to delete this task. Hit "Publish" once you have completed these steps.
![Inbound Message](/images/inboundmessage1.jpg)

5. Set up a messaging route to connect your inbound message architect flow and the SMS number you purchased in step two 

![Call Routing](/images/callrouting1.jpg)
![Agent Tools](/images/agenttools2.jpg)
