---
title: "Inbound Voice"
chapter: true
weight: 40
---

![Setup](/images/Inbound-768x300.jpg)
## Objective

By the end of this section, you will have a functional inbound voice channel. You’ll learn the steps to set up inbound voice, how to test to ensure inbound voice interactions are being routed correctly, how to troubleshoot, and any tools available to agents during voice interactions.

Voice interactions are calls that appear in the Interactions panel and are related to queues. Unlike other calls made from Genesys Cloud, the agent receives credit for these calls because the call statistics are associated with a queue.  

Voice interactions could be:

part of an outbound campaign, such as a fundraiser or sale.
outbound calls placed by the agent on behalf of a queue to contact a specific person and still receive metrics.
inbound calls placed by customers, such as a help hotline. 
Genesys Cloud uses automatic call distribution (ACD) to route inbound voice interactions and outbound campaign voice interactions to agents in queues. Genesys Cloud routes calls to agents based on a queue’s evaluation and routing methods. For example, Genesys Cloud could route a call to an agent because that agent speaks the same language as the customer, has a particular skill, or is the next available agent. 

![Inbound](/images/norwood.jpg)