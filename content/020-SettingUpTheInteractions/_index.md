---
title: "Setting Up the Interactions"
chapter: true
weight: 20
---

## Objective

By the end of this section, you should have an omnichannel contact center in the works. You’ll learn the steps to set up inbound voice, SMS, chat and email. So let’s get into the details, please follow along.

## Follow Along

 1. Create a new queue and name it "G Ride" - https://help.mypurecloud.com/articles/create-queues/
    - It is important to follow the naming convention because it will affect later steps.
    - Add yourself as a member of the queue

 2. Purchase a phone number for voice - https://help.mypurecloud.com/articles/purchase-did-numbers/
 2. Create a v1 chat widget - https://help.mypurecloud.com/articles/create-a-widget-for-web-chat/ 
 3. Follow the steps at this link to set up inbound email - https://help.mypurecloud.com/articles/register-domain-redirect-inbound-messages/  
    - Under "Add the inbound email address to the domain", you will do number 3 for routing to a queue instead of number 4 for routing to a flow. You will have this email domain route straight to the G Ride queue that you created earlier.
    
    ![Email Domain Set Up](/images/EmailSetUp.jpg)

 4. Purchase a number for SMS - https://help.mypurecloud.com/articles/purchase-sms-long-code-numbers/ 
 5. Go back into the G Ride queue and add an outbound calling number with the number you purchased for voice, an outbound SMS number with the SMS number your purchased, and an outbound email domain with the email you purchased. The screenshots below should help.

 ![Queue Set Calling Party Number](/images/QueueSetCallingParty.jpg)

![Queue Set Outbound SMS Number](/images/QueueSetSMSOutboundNumber.jpg)

![Queue Set Outbound Email Domain](/images/SetOutboundEmail.jpg)

6. Import the following architect flows below following these steps - https://help.mypurecloud.com/articles/import-export-call-flow/
    - In architect, you are able to import flows for every media type. We are giving you two flows for import; an inbound voice flow and a message flow. Be sure to navigate to the correct flow type in architect before following the import steps.

   ![Import both inbound call and inbound message](/images/Architect_Screen_shot.jpg)

   -  [Inbound Voice Flow](../../imports/GRide100InboundVoice_v1-0.i3InboundFlow)
        - Right click the link and save as
    - [Inbound Message Flow](../../imports/GRide100MessageFlow_v1-0.i3InboundMessage)
        - right click the link and save as
 7. Set up a call route to connect your inbound call architect flow to the DID that you purchased in step 1 - https://help.mypurecloud.com/articles/add-a-call-route/
    - You only need to do the step for "Create a call route entry and associate telephone numbers"
8. Set up a messaging route to connect your inbound message architect flow and the SMS number you purchased in step 4 - https://help.mypurecloud.com/articles/add-inbound-message-route/
9. Update your utilization settings to match this screenshot - https://help.mypurecloud.com/articles/configure-utilization-at-the-org-level/ 

    ![Utilization Settings](/images/Utilization.jpg)
    