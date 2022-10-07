---
title: "Before You Begin"
chapter: true
weight: 10
---

![Title](/images/DevLabSetup.jpg)
## Objective

This workshop is intended as a documented and outlined guide to set up a new Genesys Cloud dev org and route both voice and digital interactions. This walkthrough will outline how to set up the basics with the goal of adding users, queues, interaction routing, etc. The end goal is to be able to send inbound intereactions through an IVR into the ACD and finally delivered to an Agent. You will learn what tools agents have at their disposal when handling the interactions and how to best leverage those tools. This document is a recommendation and may not be one-size-fits-all.


**Notes before you start**: <br>

It is recommended to use search functionality in the admin panel vs. manually trying to navigate to any of the admin sections (Please see image below)
![Search](/images/gcadmin.png)

It is highly recommended to use naming conventions when creating any items (other than location, site, and base settings) to ensure you are not developing over colleague deployments. Ex: JaneDoe_Queue or JaneDoe_Inboundflow, etc. In this workshop, we will use the convention, "YourLastName_Item", so it is quickly identifiable. It would also be in your best interest to write down each, so you may reference it without navigating the Genesys Cloud CX platform. 

## Activating Your Account
1. Click the link in your welcome email to activate the account. _It is recommended that you enter in a shared account for this initial setup, instead of a personal account, to simplify recovery for future users_

2. **Admin** > **Genesys Add Ons** > **Ensure Genesys Cloud Voice Tile is active**
![Activate ](/images/activate.jpg)

_This should be enabled by default, however non GCV org orders will require manual activation <br>
If activation is required, select the tile and activate GCV- this can take around 10 minutes to fully activate_

**Note**: You may need to skip and come back to "Ensuring Genesys Cloud Voice is Activated" as making sure the proper roles and permissions have been assigned to the user may need to be accomplished first
