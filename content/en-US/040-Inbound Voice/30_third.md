---
title: "Troubleshooting"
chapter: true
weight: 30
---


![Test](/images/Inbound3-768x300.jpg)

## Voice Troubleshooting
If voice interactions are not being routed to the correct agent/queue or are not appearing in the interaction pane, please walk through the following troubleshooting tips:

* [Confirm agent is a member of the queue that was created at the beginning of the workshop](https://workshop.genesys.com/workshops/gride-demo/040-inbound-voice/10_first.html#Followalong)

* [Confirm calling number is tied to flow](https://workshop.genesys.com/workshops/gride-demo/040-inbound-voice/10_first.html)

* [Confirm agent status is set to "On-Queue"](https://workshop.genesys.com/workshops/gride-demo/040-inbound-voice/20_second.html)

* New hybrid sites do not have a phone trunk defined by default. You will need to manually define one in Edge Groups. If you receive this error message below when attempting to route a voice interaction, confirm an Edge Group has been defined. You can find those instructions [Here](https://workshop.genesys.com/workshops/gride-demo/030-telephony/10_first.html)

![Address of Reference](/images/AoR.jpg)

 If interactions are still not being routed correctly, please contact us at Workshops@genesys.com.

