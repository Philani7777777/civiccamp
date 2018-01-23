---
id: 515
title: 'Road Alert: Opening Up Traffic Ticket Location Data'
date: 2011-07-28T06:00:09+00:00
author: CFR Admin
layout: post
guid: http://citycampral.org/?p=515
permalink: /road-alert-opening-up-traffic-ticket-location-data/
categories:
  - Technology
  - Transit
tags:
  - Android
  - app
  - Road alert
  - sbi
  - traffic tickets
  - Wake County
  - Windows Phone 7
---
_Guest post by James Dixon_

I am sorry I missed the City Camp Meeting in early June &#8211; I didn&#8217;t know about City Camp until I demoed a Windows Phone 7 app for my neighbor who attended.  He saw the app and thought of City Camp immediately.  The phone app is called Road Alert.  What I did was to take a dump of high-frequency crash intersections data from the North Carolina Transportation Department (who were awesome in helping out btw), assign geo coordinates to the data, and serve the data up in a web service. You can read about how I applied geo coordiates to the crash data [here](http://jamessdixon.wordpress.com/2011/04/05/geocoding-apis/).  You can inspect the web service’s WSDL [here](http://www.tenfingersfree.com/roadalert/RoadAlert.svc?wsdl).  The app is in Microsoft’s certification process and should be available on App Hub within the week.  I will then port the code to iOS and Andriod.<!--more-->

I want to add additional data points to the app.  Almost everyone I demoed the app to thinks that I should add traffic ticket locations.  However, my initial attempt to secure the data in a systematic manner has failed.  So far, I have contacted:

  * [North Carolina Court System](http://www.nccourts.org/) – told me to ask individual county courts
  * [Wake County Court System](http://web.co.wake.nc.us/courts/) – told me they can’t give me the data
  * [ECitation](http://www.ecitation.nccourts.org/) – told me to contact the individual highway patrols
  * [SBI Crime Reporting](http://trafficstops.ncdoj.gov/Default.aspx) – told me to contact the court system
  * [Individual Police Departments](http://www.apexnc.org/services/police) – told me to contact the court system (I only tried Cary and Apex b/c they are closest to my house)

SBI seems like a logical place to get the data b/c they are already aggregating individual traffic records from the different cities in North Carolina.  However, they don’t require any kind of street/location data in the reports.  SBI would have to start requiring this data.

The Court System seems like the next logical place – but who wants to work with all of the different counties and their reporting systems?  I assume you can get the data because when you get a ticket, you get a bunch of letters from lawyers offering to give you a reduced sentence.  I assume they have some kind of automated system to sweep the court records.  The Wake County people I talked to wouldn’t tell me how that is done.  If worst comes to worse, you can hit the major county systems (Wake, Mecklenburg, etc..).

The individual police departments is the least desirable alternative – dealing with all of the different departments and reporting systems would be a logistical nightmare.

If anyone has any ideas, let me know.
  
<jamie@tenfingersfree.com>