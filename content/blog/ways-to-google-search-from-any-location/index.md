---
title: Ways to search on Google from any location
date: "2022-11-05T22:12:03.284Z"
description: "VPNs are the usual and well-known option for this. VPN providers have servers in different locations and let you use them as a proxy in exchange for money."
---

VPNs are the usual and well-known option for this. VPN providers have servers in different locations and let you use them as a proxy in exchange for money.

In the case of Google Search, there are a couple of [ways it uses to determine location](https://valentin.app/gs-location-changer.html)) like IP address(provided by your ISP) and the Geolocation API(Browser).

Below are some ways to bypass these logics and visit Google Search Results for your desired location:

## UULE Parameter
UULE is a handy search parameter made by Google Ads to help themselves easily see how their search results vary from location to location. It's pretty useful to us.
It looks like this: &uule=w+CAIQICIdTG9uZG9uLEVuZ2xhbmQsVW5pdGVkIEtpbmdkb

When you append this to a search URL like this https://www.google.com/search?q=[search-term]&oq=[search-term], you'll get search results for London, UK.
Try this: https://www.google.com/search?q=kittens&oq=kittens&uule=w+CAIQICIdTG9uZG9uLEVuZ2xhbmQsVW5pdGVkIEtpbmdkb20&hl=en&gl=uk

The UULE parameter consists of w+CAIQICI + [string length] + [base-64 encoded location]

### Tool for checking SERP by location
Here's a [tool to check unlimited number of search results by location](https://obscurious.xyz/geolocation-serp/)

## Location Override in Dev tools
Open Dev tools in your Browser. Click in this order -> three dots -> sensors. You'll see something like this screenshot from Chrome:

![[image.png]](./image.png)

Select any pre-set location or enter the coordinates of any corner in the world. To find the coordinates of any corner in the world, head to Google Maps. Copy the latitude and longitude from the URL(selected in screenshot below for reference)

![[screenshot1.png]](./screenshot1.png)
Paste these two in the dev tools. It works. You might need to click on "use precise location" or "update location" and reload your results. You might want to perform the search in Incognito too.

I performed a search in Boring, Oregon, USA. I'm getting the results for Damascus, Oregon, USA, while I sit here here in India.

![[screenshot2.png]](./screenshot2.png)

**Advantage of this over the UULE:** You can use this to make any website feel you are where you specify you are. UULE is only for Google search.

So you can prevent a website from redirecting you to a page meant for your location.

## One thing that beats them all
Get this extension: [https://chrome.google.com/webstore/detail/gs-location-changer/blpgcfdpnimjdojecbpagkllfnkajglp](https://chrome.google.com/webstore/detail/gs-location-changer/blpgcfdpnimjdojecbpagkllfnkajglp)
