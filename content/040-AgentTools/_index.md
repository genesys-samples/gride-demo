---
title: "Agent Tools"
chapter: false
weight: 40

---
# Genesys Workshop Series

# Agent Tools

## Welcome


The purpose of this scenario is to showcase the tools that agents utilize during interactions. Multiple, disparate systems for voice, mobile, web chat, self-service, social media, CRM, etc., each with their own user interface, makes it difficult for contact centre agents to deliver effortless customer service. Genesys delivers an integrated, omnichannel experience to ensure agents have full insight into customer information and can deliver a personalized customer experience.
> This workshop is focused on teaching the team how to utlize agent tools during the following interaction channels: voice, chat, email and SMS. User should already have completed previous modules and should have a voice, chat, email and SMS interactions answered and sitting on the interaction panel screen.


## Voice Interaction Tools

As noted above, please ensure you have answered a voice interaction and it is sitting on your interaction panel as seen in the picture below

![VoiceInteraction](images/voiceinteractionpanel.jpg)

*Dialpad*- Agent is able to enter numbers that automated call systems recognize, such as an account number or a menu selection, during a voice interaction or active business user call. 

*Mute/Unmute*- Agent can mute themselves if necessary

*Pause*- Agent can place a customer on hold

![Dialpad](images/dialpad.jpg)

*Blind Transfer*- Agent can transfer an interaction immediately to a person or queue

*Consult Transfer*-Agent can connect with another agent before transferring the call 

![Consult](images/Consulttransfer.jpg)

*Start/End Secure Pause*- Agent is able pause a recording during an interaction in order to protect sensitive, private, or secure information, such as a credit card number. The agent can still hear the customer, but Genesys Cloud does not record the interaction during the secure pause. This secure pause can also be embedded in the script.

*Hang-up*- Agent can hang up at the conclusion of the call. 

![SecurePause](images/securepause.jpg)


*Script*- Agents are given written words and logic to follow while processing a call. A script can contain multiple pages of narrative mixed with fields for updating data collected or updated by the agent. Scripts can be created for inbound or outbound interactions.

![Script](images/script.jpg)

> #### Scripts display editable records and directions to each agent that handles a particular type of interaction. Scripts present agents with details about the callers or contact, often with fields for collecting or updating information. The script seen in these images is an example and can be completely customized and configured by queue or type of interaction.
 &nbsp;

*Google Search*- Agent is able to search on Google and find public information about this customer such as social media

![Google](images/google.jpg)


*Legal Disclaimer*-In the event that an agent must say statements verbatim to stay in compliance, the legal disclaimer button allows them to pop over to their statement, read it verbatim, and return to the script.

![Legal Disclaimer](images/legaldisclaimer.jpg)

*Screen Pop*- Agents can navigate to the frequently used external websites. For example, if an agent has to check UPS or Fedex tracking, administrators can configure the "Screen Pop" button to directly open those websites so agents can save time and help the customer faster.

![Screen Pop](images/screenpop.jpg)

*Update Info*-Agents can update the customer record. In this example, the system is doing a data dip and presenting the CRM customer record. For example, Betty Suarez calls in and tells the agent she moved to Dallas and doesn't live in Austin anymore. An agent can easily update this information and it will update the CRM customer record.

![Update Info](images/updateinfo.jpg)

*Secure Flow*- Agents are able to process confidential personal information such as social security numbers, credit card numbers, etc. The "secure flow" button differs from a secure pause in that the "secure flow" button is setup so that an agent is not able to take any confidential information unless this button has been selected. This button automatically stops/resumes the recording accordingly.

![Secure Flow](images/secureflow.jpg)

*CRM Data*- Scripts allow administrators to present data from external systems such as CRMS. In this case, the system is doing a data dip into the 3rd party CRM to present relevant information to the agent. As noted above, it is a bi-directional integration so an agent can update information and send it back to the CRM.

![CRM](images/crmdata.jpg)

*Account*-Agents are given more insight into a customer's account and service information. In this case, the agent can see account information and additional details.

![Account](images/account.jpg)


![Account Info](images/accountinfo.jpg)

*Screen Share*- A screen share allows an agent to see the customer's screen with their permission. Agents can see what customers do in real time. Agents have to request and receive permimssion from a customer to initiate a screen chat. For voice, the agent verbally communicates the security key to the sharer, who then types in a form. For web chat, Genesys Cloud shares the security key behind the scenes, with no action needed from the agent. 

![Screen Share](images/screenshare.jpg)

*Agent Assist*-Agent Assist provides real-time transcription of a customer call and knowledge suggestions that update automatically based on the context of the conversation. Knowledge suggestions include FAQ or knowledge article recommendations that make agents more efficient and knowledgable. Agents no longer search for information by themselves and can focus on their discussons with customers. In this example, the customer stated they wanted to change their address. Agent assist suggested a relevant article with a 97% confident rating. The agent can then give feedback on whether this article was helpful or not.

![Agent Assist](images/agentassist.jpg)








