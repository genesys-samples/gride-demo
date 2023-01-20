---
title: "Setup"
chapter: true
weight: 10
---

---
![Setup](/images/Email1-768x300.jpg)

## Email Setup
Email is still one of the most reliable and desired ways for customers to interact with companies for support. Genesys Cloud CX automatically distributes emails to the best-fit agent based on content analysis and keywords. Genesys Email Routing streamlines your response process using email automation functionality that enables you to monitor, measure, and optimize your email flow to create a better customer experience.

Genesys Cloud routes incoming email messages through ACD just like it routes calls and chats, using the same routing and evaluation methods. When routing email messages, Genesys Cloud considers skills, language, priority, and agent utilization. 

Your Genesys Cloud account can have a maximum of two email domains with up to 500 associated email addresses per domain. You assign each email address to a queue, and can configure it to have an associated language, skill, and priority. Genesys Cloud ACD routes each incoming message to a member of the queue. Configured routing and evaluation methods help to determine the best available agent to handle the interaction.

When an agent handles an email interaction, it'll route to them like any other digital channel. Once they reply, the interaction will be cleared from their interaction panel. However, it is common that email communication may have multiple replies needing to go to the customer. Because of this, when a customer replies back to the email, Genesys Cloud CX will route to the agent who was the responder for seamless communication as long as that agent is available.

![Email](/images/email.png)

## What We Will Build Today
Today, we'll set up a email domain within Genesys Cloud CX that routes automatically to a queue. Email domains have the option to either route straight to a queue or to an architect flow for additional processing. You might want your email domain to route to an architect flow if you wanted to do automatic responses, data dips or attach skills to the email. For our scenario, we'll just have the email go straight into the G Ride queue that we configured earlier. 

## Follow Along
 1. Navigate to **Admin** screen > Search for **Email** under **Contact Center** 

 2. Click **Add Domain** > From **Domain Type** list, select **Genesys Cloud** > In the **Domain name** box, type the email subdomain (for example, yourAccountname), which appends with **.myPureCloud.com** 

 3. Click **Save**. The email address page opens for the new domain

 2. Next, add the inbound email address to the domain. 
 3. Click **Add email address** > In the **Email Address** box, type the email address the customer uses to send an email  
 4. Under **Email Routing**, select **Always route to this queue** 
 5. Click the **Queue** list and choose the desired queue > In the **Skills** box, optionally add any ACD skills to ensure that associated emails route to an agent with matching skills 
 
 6. Click the **Language** list and optionally choose a language > Under **Spam Routing** choose "Disconnect all email that is detected as spam" > Click **Save**

 
**_For today's workshop, be sure to route to a queue instead of a flow as outlined in this screenshot_** 
    
 ![Email Domain Set Up](/images/EmailSetUp.jpg)

 3. Go back into the queue >  update the **Outbound Email Address** to the email domain you just set up

    ![Queue Set Outbound Email Domain](/images/SetOutboundEmail.jpg)
 
 4. Navigate to **Admin** > Search for **Utilization** 
 5. Under **Maximum Capacity**, specify the number of interactions to allow for each interaction type. For example, if you want an agent to work on up to four emails at one time, then set the Email maximum capacity to 4 > To ensure that non-ACD interactions are not interrupted by ACD interactions, select the **Block calls when on a non-ACD call (excludes transfers) check box** > 
 **Ensure utilization matches the screenshot below**
 6. Click **Save**
  
 
    ![Utilization Settings](/images/Utilization.jpg)