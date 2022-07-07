---
title: "SMS"
chapter: true
weight: 60
---

![Setup](/images/SMSsetup-768x300.jpg)

## Objective

Customers often want to contact businesses in the same way they would contact friends and family. SMS allows for a more convienent, asynchronous mode of communication. Using SMS, customers can avoid calling and waiting on hold for an available agent. SMS also allows customers to engage "on the go" without a dedicated mobile app. Also, because customers engage by SMS at faster rates than any other messaging channel, the organization can resolve issues more quickly.

SMS interactions are routed by the same orchestration engine as other media types in Genesys Cloud CX, and that is through Architect. Architect allows you to perform data dips, engage with Bots, attach routing logic and much more. 

With agents communicating via SMS, the agent can keep the message open and use SMS like a chat channel, or close the SMS message after replying. If the agent keeps the conversation open, the system immediately displays each customer response to the agent, using SMS messages as a chat channel. If the agent closes the conversation but the customer replies within 72 hours, the conversation reopens (after 72 hours, the system creates a new conversation) and routes to the last agent that handled the SMS. If that agent is unavailable, the system routes the message by ACD to the next available agent.



