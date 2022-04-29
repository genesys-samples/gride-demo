---
title: "Voice Interaction"
chapter: false
weight: 30
---

## Scenario

1. Call the phone number purchased earlier that's tied to the call flow  uploaded. In the IVR, you will hear the prompt and then be routed to queue. If your user is on-queue, the interaction will be routed to you and interrupt the digital interactions.

    NOTE: If you're calling from the phone number listed on your user profile, the interaction will not route to you. Please ensure that the ANI you're calling from is separate than the primary voice number listed in GCCX.

2. Accept the voice interaction as outlined in the example below. If you don't accept before being timed-out and moved to not-responding status, change your status back to on-queue and the interaction will be routed back to you. Once you have accepted the interaction, you should have three interactions, with voice being the top option due to priority.

    ![Picture](/images/Accept_Voice.png)

3. Walk through the call controls showcased at the top of the screen. Then, move to the agent tools on the right side, specifically, the [Notes](https://help.mypurecloud.com/articles/enter-notes-for-an-interaction/) section. Add a note to the interaction that says, "Requested transfer to another agent. Have already authenticated, you're speaking with Veronica." 
    
    Once the note has been completed, move back to the call controls and access the [Consult Transfer](https://help.mypurecloud.com/articles/consult-transfer-a-call/) option. Search for a specific user within your organization, but do not transfer. Then, search for the "G Ride" queue that was created for this workshop. Transfer the interaction to that queue. 

    ![Picture](/images/CallControls_Consult.png)

    If you are the only agent available in this queue, the interaction will route back to you. Accept the interaction and located the notes. There should be an orange dot highlighting that a note has been passed with this interaction. Verify and read the notes. 

    ![Picture](/images/Notes.png)

    Keep  You have now completed the scenario.
