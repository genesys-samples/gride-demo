---
title: "SMS"
chapter: false
weight: 30
---
![Setup](/images/setup2.jpg)
## Genesys Cloud SMS
Customers often want to contact businesses in the same way they would contact friends and family. SMS allows for a more convienent, asynchronous mode of communication. Using SMS, customers can avoid calling and waiting on hold for an available agent. SMS also allows customers to engage "on the go" without a dedicated mobile app. Also, because customers engage by SMS at faster rates than any other messaging channel, the organization can resolve issues more quickly.

SMS interactions are routed by the same orchestration engine as other media types in Genesys Cloud CX, and that is through Architect. Architect allows you to perform data dips, engage with Bots, attach routing logic and much more. 

With agents communicating via SMS, the agent can keep the message open and use SMS like a chat channel, or close the SMS message after replying. If the agent keeps the conversation open, the system immediately displays each customer response to the agent, using SMS messages as a chat channel. If the agent closes the conversation but the customer replies within 72 hours, the conversation reopens (after 72 hours, the system creates a new conversation) and routes to the last agent that handled the SMS. If that agent is unavailable, the system routes the message by ACD to the next available agent.

 ![SMS](/images/SMSicon.png)

## What We Will Build Today
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





