---
title: "Agent Tools"
chapter: true
weight: 40
---
![Agent Tools](/images/Webchat4-768x300.jpg)
## Digital Interaction Tools

When handling digital interactions in Genesys Cloud CX, a series of tools are available out-of-the-box. Some may depend on your licensing tier, or permissions based on your user role. 

![Digital Interactions](/images/digitalinteraction.jpg)

***Blind Transfer*** - A blind transfer allows you to transfer an interaction immediately to a person or queue. If you perform a blind transfer to a queue, Genesys Cloud remembers the skills-based information applied to the original call by default. 

***Hang-up*** - Ends the interactions and sends the agent to their After Call Work(ACW).

***Script*** - The written words and logic an agent follows while processing a call. A script can contain multiple pages of narrative mixed with fields for updating data collected or updated by the agent. Scripts can be created for inbound or outbound interactions.

***Canned Responses*** - Canned responses are pre-written answers to commonly asked questions that you can use during an interaction, by either reading the response to a customer, or by inserting the response into a chat, email, or tweet.

***Notes*** - You can make notes about an interaction during the interaction or while in after call work (ACW). If you enter notes for an interaction and then transfer that interaction to another agent, the notes remain with the interaction. Because notes are part of the interaction, the receiving agent can also see them.

***Wrap-up Code*** - Wrap-up codes indicate the nature of an interaction. Agents specify wrap-up codes after completing an interaction; for example, a completed sale, a customer dissatisfied with service, or a billing problem.

***Screen Share*** - Screen share uses WebRTC to send and receive the screen share. Sharers only require a WebRTC compatible application to share their screens. You can either include the WebRTC capable Chromium Embedded Framework in your desktop application, or direct customers to use a WebRTC compatible web browser, such as Firefox or Google Chrome. For web chat, Genesys Cloud shares the security key behind the scenes, with no action needed from the agent. After Genesys Cloud connects the screen share session, the agent can see the sharer’s screen, and either the agent or the sharer can end the screen share.

***Customer Journey*** - You can view the following information, depending on how Predictive Engagement is configured:
* Visitor details, such as the visitor’s name, status, and number of visits.
* Visit dates and duration. If the visitor has multiple dates, select the date you want to see more information about.
* Visit Journey information, including pages visited and actions on those pages during the selected visit. To see more information about the actions performed, click the action’s icon.
* Segments assigned to the interaction for the selected visit.
* Outcome scores for the selected visit.
* Other visitor information, such as location, device type, operating system, and browser type. 


![Blind Transfer](/images/blindtransferandhangup.jpg)


**Genesys Cloud maintains a consistent user experience across the platform. For this reason, it is easy for agents to master the art of taking interactions. Scripts, customer profile, canned responses, notes, and adding wrap-up codes are exactly the same for digital and voice interactions.**