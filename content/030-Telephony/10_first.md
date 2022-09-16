---
title: "Location & Site"
chapter: true
weight: 10
---

![Title](/images/LocationSiteNew-768x300.jpg) 


## Telephony Options

Genesys Cloud CX is primarily available through two telephony options, Genesys Cloud Voice and BYOC (Bring Your Own Carrier). With Genesys Cloud Voice, telephony and contact center PBX is delivered by services provided by Genesys. No hardware is requireed and no alternate carrier contract. 

BYOC allows a customer to remain with their existing carrier and contract while delivering telephony through SIP trunks. Media processing is provided in the cloud. 

In today's workshop, we'll setup our environment leveraging Genesys Cloud Voice. If you're looking to use our BYOC option, you can refer to documentation here: (https://help.mypurecloud.com/articles/byoc-cloud-configuration-overview/)


## Location
1. This is the physical location your agents will reside at as their HQ. Locations are associated for emergency routing capabilities; it is not recommended using emergency services on a dev lab, but it is a required step. 


2. **Go to Admin > Locations > Click "Add Location"**

![AdminPage](/images/Locations.jpg)

3. Name your location, **"Headquarters"**, then add an address. The address must be valid, as you begin to type it out a drop-down list will begin to appear. 

4. Select one from the auto-populated options to ensure the directory has identified this as valid for 911 purposes. 

5. Add yourself as the **"Site Contact"** since the purpose is demonstration only. 

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

4. Lastly, return to the **"General"** tab and confirm the site has been selected as the default. Be sure to **Save Site**


![SiteSettings](/images/DefaultSite.jpg)
