---
title: Agent Tools
chapter: true
weight: 40
---
![Test](/images/Inbound4-768x300.jpg)

## Voice Interaction Tools

When handling voice interactions in Genesys Cloud CX, a series of tools are available out-of-the-box. Some may depend on your licensing tier, or permissions based on your user role. Each plays its part in providing the agent with relevant data to successfully handle the interaction, and create a personalized, smooth experience for the customer. 

![Voice Interaction](/images/Voiceinteractiontools.jpg)

***Dialpad***- The dialpad allows you to enter numbers that automated call systems recognize, such as an account number or a menu selection. Genesys Cloud plays a DTMF sound for each number you select.

***Mute/Unmute***- Mute disables the agent’s microphone. The customer cannot hear what the agent is saying, but the agent can hear the customer.

***Hold***- Hold places the customer on hold. The agent cannot hear the customer, and the customer cannot hear the agent. 

![Dialpad](/images/Dialpad.jpg)

Genesys Cloud CX supports two types of transfers: a blind transfer (all interaction types) and a consult transfer (call interactions). Both transfer types allow you to see an agent's status before transferring to ensure someone will be there on the other end to assist the customer. When transferring to a queue, you'll have line of sight into the queue's estimated wait time, how many agents are tied to the queue, and how many interactions are currently being handled by media type. 

***Blind Transfer***- A blind transfer allows you to transfer an interaction immediately to a person or queue.

***Consult Transfer***-A consult transfer allows you to connect with a person or queue before transferring a call.

![Consult](/images/Consulttransfer.jpg)

***Start/End Secure Pause***- You're able to hit the "secure pause" in order to stop the recording of the call (both audio and screen recordings), input the credit card number, and end the "secure pause" to resume the recording. This ensures no confidential information is recorded. You can still hear the customer and speak to them during this secure pause, but the system does not record the interaction at this time. This secure pause can also be embedded in the script, which we will discuss later. Secure pauses can also be triggered through APIs and 3rd parties.
https://appfoundry.genesys.com/filter/genesyscloud


***Hang-up***- When you're finished with the interaction, you can hit this button to end the call and begin your after-call work.

![SecurePause](/images/securepause.jpg)


***Script***- Scripts are a way for  supervisors to give you words and logic to follow when taking interactions. Scripts can contain the exact words you are supposed to say when speaking to a customer, 3rd party websites you frequently have to visit, customer data from a 3rd party system, and more! This is useful for newer agents who may not know what to say when taking a call or even for experienced agents to reference, and it saves time by having the most important tools on the same page. Scripts are completely customizable and configurable by queue and interaction type. Below is an example of what a script can look like! 

![Script](/images/script.jpg)

***Screen Pop***- A screen pop application delivers an incoming call to an agent, along with data pertaining to the call or caller. For example, a customer with Salesforce.com or another CRM application may use caller id information to lookup the customer’s record in the CRM. The agent is delivered a ‘screen pop’ of the caller’s account via their Salesforce.com web browser. Or, the script for an outbound dialing campaign can populate the agent’s display with information pertaining to the call, the customer, and the campaign.

![Screen Pop](/images/screenpop.jpg)

***Screen Share***- A screen share allows you to see the customer's screen in real-time,  with their permission of course. Agents have to request and receive permimssion from a customer to initiate a screen chat. For voice, you can verbally communicate the security key to the customer, who will then type that number into a form on your website. For web chat, Genesys Cloud shares the security key behind the scenes, with no action needed you. A screen share is always linked to the original interaction, in this case a voice interaction. For quality management purposes, this interaction will show as one singular interaction.

![Screen Share](/images/screenshare.jpg)

***Agent Assist***-Agent Assist provides real-time transcription of a customer call and knowledge suggestions that update automatically based on the context of the conversation. Knowledge suggestions include FAQ or knowledge article recommendations that make agents more efficient and knowledgable. You don't have to waste time searching for information and can focus on your discussons with customers. 

![Agent Assist](/images/agentassist.jpg)

***Profile***- The customer profiles gives more information about the customer. You can see more customer details and notes that other agents have made about this customer. Its always best to have as much information as possible about the customer to ensure you're delivering a *personalized* experience. 

***Notes***- You can make notes about an interaction during the interaction or while in after call work (ACW). If you enter notes for an interaction and then transfer that interaction to another agent, the notes remain with the interaction. Because notes are part of the interaction, the receiving agent can also see them.

![Profile](/images/profile.jpg)

***Schedule a Callback***- A callback is an outbound call requested by a contact. Agents can schedule a callback during a voice interaction. At the scheduled date and time, Genesys Cloud routes the interaction to an agent. To route the callback to you, select Route callback to me if possible. By default, scheduled callbacks route to the queue that received the original interaction. If your admin has enabled owned callbacks, to take ownership of a callback, select Take Ownership. The callback waits for you to become available for the time configured by your admin.

![Callback](/images/callback.jpg)

***Wrap-up Codes***- Wrap-up codes indicate the nature of an interaction. Agents specify wrap-up codes after completing an interaction; for example, a completed sale, a customer dissatisfied with service, or a billing problem.

![Wrapup](/images/wrapup.jpg)
&nbsp;

#### You have finished routing your first inbound interaction into Genesys Cloud CX. Now that we have completed voice, let's move on to digital interactions. Remember, Genesys Cloud CX has the ability to route voice, webchat, web messaging, email, SMS, and Social all natively. 

