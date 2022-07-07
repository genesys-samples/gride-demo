---
title: "Location & Site"
chapter: false
weight: 20
---
![Test](/images/testing2.jpg)
## Location
>This is the physical location your agents will reside at as their HQ. Locations are associated for emergency >routing capabilities; it is not recommended to use emergency services on a dev lab, but it is a required step. 

2. Go to Admin> Locations> **Click "Add Location"** 

![AdminPage](/images/Locations.jpg)

3. Name your location "Headquarters", then add an address. Please input a valid address from the drop down that appears as you begin typing. Select one from the auto-populated options to ensure the directory has identified this as valid for 911 purposes

4. Add yourself as the "Site Contact" since this is for demonstration purposes only
5. Check the box for "Make this location available for use on sites" 
6. Add an emergency number

![LocationDetails](/images/LocationsPopup.jpg)

## Site

>A site is the home of a set of phones. The site defines the call classification rules, outbound routing rules, and >the telephony properties for dialing. This is also where Outbound Routing will reference a Number Plan. Sites must >be tied to physical Locations defined.

![AdminDirectory](/images/Site.jpg)

1. Create a new site and name it "My Site". Associate your Location, select a time zone, and leave Media Model as "Cloud"

![SiteDetails](/images/SiteSetup.jpg)

2. Navigate to Outbound routes within the newly created site and under "Select External Trunks" ensure the “PureCloud Voice – AWS” Trunk is associated. Make sure to "Enable" the State as well. 

![OutboundRoutingDetails](/images/OutboundRoute.jpg)

3. Lastly, return to the "General" tab and confirm the site has been selected as the default.

![SiteSettings](/images/DefaultSite.jpg)
