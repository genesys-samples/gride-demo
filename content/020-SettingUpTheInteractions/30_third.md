---
title: "SMS"
chapter: false
weight: 30
---

## Genesys Cloud SMS
Customers often want to contact businesses in the same way they would contact friends and family. SMS allows for a more convienent, asynchronous mode of communication. Using SMS, customers can avoid calling and waiting on hold for an available agent. SMS also allows customers to engage "on the go" without a dedicated mobile app. Also, because customers engage by SMS at faster rates than any other messaging channel, the organization can resolve issues more quickly.

SMS interactions are routed by the same orchestration engine as other media types in Genesys Cloud CX, and that is through Architect. Architect allows you to perform data dips, engage with Bots, attach routing logic and much more. 

With agents communicating via SMS, the agent can keep the message open and use SMS like a chat channel, or close the SMS message after replying. If the agent keeps the conversation open, the system immediately displays each customer response to the agent, using SMS messages as a chat channel. If the agent closes the conversation but the customer replies within 72 hours, the conversation reopens (after 72 hours, the system creates a new conversation) and routes to the last agent that handled the SMS. If that agent is unavailable, the system routes the message by ACD to the next available agent.

## What We Will Build Today
Today, we'll set up the basics of SMS in Genesys Cloud CX. You'll purchase an SMS number directly from the Genesys Cloud admin portal, with Genesys being your SMS broker. You'll also import a basic Inbound Message Architect flow. Lastly, you'll connect the SMS number you purchased to the Architect flow that you imported through a messaging route. 

## Follow Along
 1. Purchase a number for SMS - https://help.mypurecloud.com/articles/purchase-sms-long-code-numbers/ 
 2. Go back into the G Ride queue and set the SMS number you just purchased as the outbound SMS number
    ![Queue Set Outbound SMS Number](/images/QueueSetSMSOutboundNumber.jpg)
 3. Import the following architect Message flow below following these steps - https://help.mypurecloud.com/articles/import-export-call-flow/
    - [Inbound Message Flow](../../imports/GRide100MessageFlow_v1-0.i3InboundMessage)
        - right click the link and save as
 4. Set up a messaging route to connect your inbound message architect flow and the SMS number you purchased in step 4 - https://help.mypurecloud.com/articles/add-inbound-message-route/
