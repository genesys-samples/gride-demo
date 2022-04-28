---
title: "Digital Interactions"
chapter: false
weight: 20
---

## Digital Interactions

The purpose of this scenario is to showcase utilization and how we can manage an omnichannel approach.

1. If not already on-queue, toggle the on-queue switch so that your status is "on-queue." From here, we're going to trigger two interaction types - email, and chat.

2. Send an email to the email address domain you created within the Genesys Cloud CX admin panel. If set up appropriately, it will route directly to the "G Ride" Queue and to your user in the [Agent Interface](https://help.mypurecloud.com/articles/about-agent-interactions/). Once routed, accept.

3. It's time to route a chat. This will eventually be replaced with a web messaging option in this workshop. You must login in using your GC CX credentials or be. Go to the [Developer Tools Website](https://developer.genesys.cloud/) and reference the [Chat Tool](https://developer.genesys.cloud/developer-tools/#/webchat) linked here. It should look like the example below:

    ![Picture](images/DevTools_Chat.png)

    Choose the "G Ride" chat deployment and queue that you created earlier. Fill out the chat data (which is optional). When ready, hit the start chat icon at the bottom of the page. It should create a chat interaction that routes into queue if configured correctly. If on-queue and utilization is configured appropriately, it will be routed to you as an agent. Hit accept.

4. Start walking through the interface as an agent, toggling through the interaction tools listed at the top:

    ![Picture](images/Chat_Email.png)

    You will see similarities in the interaction tools throughout all interaction types, with voice being the only channel with different options. Once comfortable, move to the agent tools on the right side of the screen.

    ![Picture](images/AgentTools_Canned.png)

    Ensure you're in the chat interaction, but canned responses work in all digital channels. Click specifically on the canned response section. Find the folder that you created, search for the response and click the button to add it as a response. Once you have proofread, hit send. For further information on canned responses and managing libraries, [reference this link](https://help.mypurecloud.com/articles/about-canned-responses/).

5. Once you have successfully moved through the digital interactions and the tools associated, it's time to move into the next scenario. Please stay connected to the email and chat interactions. You have now completed the scenario.