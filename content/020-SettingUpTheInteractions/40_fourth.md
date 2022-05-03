---
title: "Email"
chapter: false
weight: 40
---

## Genesys Cloud Email
Email is still one of the most reliable and desired ways for customers to interact with companies for support. Genesys Cloud CX automatically distributes emails to the best-fit agent based on content analysis and keywords. Genesys Email Routing streamlines your response process using email automation functionality that enables you to monitor, measure, and optimize your email flow to create a better customer experience.

Genesys Cloud routes incoming email messages through ACD just like it routes calls and chats, using the same routing and evaluation methods. When routing email messages, Genesys Cloud considers skills, language, priority, and agent utilization. 

Your Genesys Cloud account can have a maximum of two email domains with up to 500 associated email addresses per domain. You assign each email address to a queue, and can configure it to have an associated language, skill, and priority. Genesys Cloud ACD routes each incoming message to a member of the queue. Configured routing and evaluation methods help to determine the best available agent to handle the interaction.

When an agent handles an email interaction, it'll route to them like any other digital channel. Once they reply, the interaction will be cleared from their interaction panel. However, it is common that email communication may have multiple replies needing to go to the customer. Because of this, when a customer replies back to the email, Genesys Cloud CX will route to the agent who was the responder for seamless communication as long as that agent is available.

## What We Will Build Today
Today, we'll set up a email domain within Genesys Cloud CX that routes automatically to a queue. Email domains have the option to either route straight to a queue or to an architect flow for additional processing. You might want your email domain to route to an architect flow if you wanted to do automatic responses, data dips or attach skills to the email. For our scenario, we'll just have the email go straight into the G Ride queue that we configured earlier. 

## Follow Along
 1. Follow the steps at this link to set up aninbound email domain - https://help.mypurecloud.com/articles/register-domain-redirect-inbound-messages/  
    - Under "Add the inbound email address to the domain", you will do number 3 for routing to a queue instead of number 4 for routing to a flow. You will have this email domain route straight to the G Ride queue that you created earlier.
    
    ![Email Domain Set Up](/images/EmailSetUp.jpg)

 2. Go back into the G Ride queue and update the outbound email address to the email domain you just set up.

    ![Queue Set Outbound Email Domain](/images/SetOutboundEmail.jpg)
 
 3. Update your utilization settings to match this screenshot. This will allow us to handle all the media types we just set up simultaneously as an agent.  - https://help.mypurecloud.com/articles/configure-utilization-at-the-org-level/ 

    ![Utilization Settings](/images/Utilization.jpg)
