---
title: "Inbound Voice"
chapter: false
weight: 10
---

## Genesys Cloud Inbound Voice
While new communication channels continue to crop up, the importance of voice remains. The speed and agility of the Genesys™ Genesys Cloud CX™ contact center platform connects your customer engagement with the telephony option that best fits your business needs. The widest variety of voice services connectivity options in the industry gives customers unparalleled flexibility and choice. Customers can choose Genesys Cloud CX Voice (Genesys telecom) for VoIP, use the cloud-based Bring Your Own Carrier (BYOC) option. Customers can keep a carrier contract or existing PBX infrastructure, or consolidate using Genesys as a single vendor for all needs. Customers who choose Genesys Cloud CX are often attracted to the cloud technologies and microservices architecture that provide speed, stability, and agility for their business. Adopting a cloud solution for voice services is a future-proof approach—extending these same cloud benefits across a customer’s entire communications system.

#### Genesys Cloud CX Voice
Genesys Cloud CX Voice is an internet-based telephony service provided by Genesys that, when activated, provides public telephony access to Genesys Cloud CX services.

#### Bring Your Own Carrier (BYOC)
Genesys Cloud CX BYOC refers to the ability for customers to define SIP trunks between Genesys Cloud CX and third-party devices or services.

## What We Will Build Today
#### Queues

Today for inbound voice we will walk you through creating the backbone of your contact center. Genesys Cloud CX's ACD engine uses a Queue based routing system with the ability to attach skills, languages and priority to the routing logic. We will keep it simple today and simply start with a basic queue. 

Genesys Cloud CX queues are by default equipped for omnichannel communications. Throughout this workshop, we will be routing all media types to the same queue. 

#### Telephony

We will also be using Genesys Cloud CX Voice services today. As mentioned above, we give you the flexbility to either bring your own carrier or to use Genesys as the carrier. Either option within Genesys Cloud CX is easily managed and allows you to take advantage of cloud voice services that can be deployed in days with no hardware required. The only steps that you'll need to take today to set up Genesys Cloud CX Voice is to purchase a phone number and assign that number to a call route. Pretty simple, right?

#### Architect

Setting up inbound voice capabilities also requires an Architect flow. As a matter of fact, we will be importing architect flows for every media type that we will set up today. Architect is a powerful tool that comes with Genesys Cloud CX. 

Architect is an easy-to-learn drag and drop web-based design tool that creates flows for media types. Architect uses menus and straight-to-queue logic most often associated with traditional auto-attendants. However, it also incorporates advanced, feature-rich logical operations such as non-menu digit collection, External Data Access (data dips), conditional logic, and expression editing to help develop the IVR functionality. Architect also provides centralized prompt management with multi-language support.

Important for todays workshop, Architect also has an export and import option. What this will allow us to do is to simply give you a downloadable file for an architect flow and then you can simply import that file into your architect flow in your instance of Genesys Cloud CX. Architect is a powerful tool and it's very fun to learn how to build Architect flows from scratch, but it is not the objective in today's workshop. We will save that for another day!

## Follow along

 1. Create a new queue and name it "G Ride" - https://help.mypurecloud.com/articles/create-queues/
    - It is important to follow the naming convention because it will affect later steps.
    - Add yourself as a member of the queue
2. Purchase a phone number for voice - https://help.mypurecloud.com/articles/purchase-did-numbers/
3. Go back into the G Ride queue and add an outbound calling number with the number you purchased for voice
![Queue Set Calling Party Number](/images/QueueSetCallingParty.jpg)
4. Import the following Inbound Voice architect flow following these instructions - https://help.mypurecloud.com/articles/import-export-call-flow/
    -  [Inbound Voice Flow](../../imports/GRide100InboundVoice_v1-0.i3InboundFlow)
        - Right click the link and save as