---
title: "Location & Site"
chapter: false
weight: 20
---
![Title](/images/Telephony3.jpg)
## Location
1. This is the physical location your agents will reside at as their HQ. Locations are associated for emergency routing capabilities; it is not recommended using emergency services on a dev lab, but it is a required step. 

2. Go to Admin> Locations> Click "Add Location" 

![AdminPage](/images/Locations.jpg)

3. Name your location, "Headquarters", then add an address. The address must be valid, as you begin to type it out a drop-down list will begin to appear. Select one from the auto-populated options to ensure the directory has identified this as valid for 911 purposes. Add yourself as the "Site Contact" since the purpose is demonstration only. Check the box for "Make this location available for use on sites". Add an emergency number

![LocationDetails](/images/LocationsPopup.jpg)

## Site

1. A site is the home of a set of phones. The site defines the call classification rules and outbound routing rules as well as the telephony properties for dialing. This is also where Outbound Routing will reference a Number Plan. Sites must be tied to physical Locations defined.

![AdminDirectory](/images/Site.jpg)

2. Create a new site and name it "My Site". Associate your Location, select a time zone, leave Media Model as "Cloud"

![SiteDetails](/images/SiteSetup.jpg)

3. Navigate to Outbound routes within the newly created site and under "Select External Trunks" ensure the “PureCloud Voice – AWS” Trunk is associated. Make sure to "Enable" the State as well. 

![OutboundRoutingDetails](/images/OutboundRoute.jpg)

4. Lastly, return to the "General" tab and confirm the site site has been selected as the default.

![SiteSettings](/images/DefaultSite.jpg)


THIS IS A TEST