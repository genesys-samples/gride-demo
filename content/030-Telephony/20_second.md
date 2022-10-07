---
title: "Telephony"
chapter: true
weight: 20
---
![Title](/images/Telephony2New-768x300.jpg)

## Purchase a Phone Number

>Purchase phone numbers directly from within Genesys Cloud Voice using the Number Purchase portal. **NOTE: We will be purchasing a phone number in this module. It is important that you write down the number prior to clicking "Complete Purchase."**

## Follow along

**Note**: It is required to order a minimum of one number, but it is recommended to order 1 number for each user that will be using Dev Lab. Telephony charges are billed to you so purchase these at your org - https://help.mypurecloud.com/articles/genesys-cloud-voice-pricing/ 

1.	Click Admin > Number Management > **Click "Purchase Number"** <br>

	(_If you do not see Number Management in the Admin panel, you made need to log out and back in to refresh your newly added permissions_)
	
2.	Search for a DID number by area code or city/state _(Please write this phone number down as you will not be able to find this later)_

3.	Check the boxes next to each number you are going to purchase (with at least one being emergency capable) and complete purchase

6. Check the box for **"Make this location available for use on sites"**. 

7. Add an emergency number.


![LocationDetails](/images/LocationsPopup.jpg)

## Site


 A site is the home of a set of phones. The site defines the call classification rules and outbound routing rules as well as the telephony properties for dialing. This is also where Outbound Routing will reference a Number Plan. Sites must be tied to physical Locations defined.

![AdminDirectory](/images/Site.jpg)

1. **Go to Admin> Site> Click "Create Site"**

2.  Create a new site and name it **"My Site"**. 

3. Associate your Location, select a time zone, leave Media Model as "Cloud"

![SiteDetails](/images/SiteSetup.jpg)

3. Navigate to Outbound routes within the newly created site and under **"Select External Trunks"** ensure the “PureCloud Voice – AWS” Trunk is associated. Make sure to **"Enable"** the State as well. 

![OutboundRoutingDetails](/images/OutboundRoute.jpg)

4. Lastly, return to the **"General"** tab and confirm the site site has been selected as the default.


![SiteSettings](/images/DefaultSite.jpg)
