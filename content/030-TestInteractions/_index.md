---
title: "Test the Interactions"
chapter: true
weight: 30
---

# Genesys Workshop Series

# Test Interactions

### Welcome

By the end of this section you should have a fully operational omnichannel contact center. Inbound voice, SMS, chat and email will be routed to your user and you will be able to accept and answer interactions. 

> This workshop is focused on teaching the team how to test the following interaction channels: voice, chat, email and SMS to ensure they are being routed correctly. User should already have completed previous module.

## Test an Incoming Voice Interaction
1. The first step in testing a voice interaction is ensuring you have the correct inbound voice number to dial. Navigate to the admin page and search for "DID" and click "DID Numbers"

![DID](images/DID.jpg)

2. Navigate to the DID number that is assigned to your inbound flow and save that number to your personal device

![inboundflow](images/inboundflow.jpg)



3. Navigate to the Interactions pane on the left side of the screen and ensure you are set to "On-Queue" (found at top right of screen)

![interactionpane](images/interactionpane.jpg)

4. Dial the DID number from a personal phone and select "answer" when the interaction comes through

![incomingcall](images/incomingcall.jpg)



## Test an SMS Interaction

  1. The first step in testing an SMS interaction is ensuring you have the correct number. Navigate to the admin page and search for "SMS" and click "Number Inventory"

  ![sms](images/sms.jpg)

  2. Navigate to the SMS Number that is assigned to your inbound SMS flow and save that to your personal device

  ![smsnumber](images/smsnumber.jpg)

3. Navigate to the Interactions pane on the left side of the screen and ensure you are set to "On-Queue" (found at top right of screen)

![interactionpane](images/interactionpane.jpg)

4. Text the SMS number from a personal phone and select "answer" when the interaction comes through

![incomingsms](images/incomingsms.jpg)

## Test a Chat Interaction

1. The first step in testing a chat interaction visiting the Genesys Cloud CX Developer center 
https://developer.genesys.cloud/developer-tools/#/webchat

2. Navigate to the Deployment dropdown and ensure you have selected the "G-Ride" Deployment and ensure the ""Queue" field is set to "G-Ride"

![devcenter](images/chatdev.jpg)

3. Navigate back to the Genesys environment and to the Interactions pane on the left side of the screen and ensure you are set to "On-Queue" (found at top right of screen)

![interactionspane](images/interactionpane.jpg)

4. Navigate back to the Developer Center and select "Start Chat" to begin the chat interaction

![startchat](images/startchat.jpg)

5. Navigate back to the Genesys Environment and select "answer" when chat interaction comes through

![incomingchat](images/incomingchat.jpg)

## Test an Email Interaction

1. The first step in testing an email interaction is ensuring you have the correct email address. Navigate to the admin page and search for "SMS" and click "Number Inventory"

![adminemail](images/adminemail.jpg)

2. Navigate to the email address that is assigned to your queue and save that to the email you will use to trigger an interaction

![emailaddress](images/emailaddress.jpg)

3. Navigate to the Interactions pane on the left side of the screen and ensure you are set to "On-Queue" (found at top right of screen)

![interactionpane](images/interactionpane.jpg)

4. Send an email to your queue from a personal email address and select "answer" when the interaction comes through

![incomingemail](images/incomingemail.jpg)