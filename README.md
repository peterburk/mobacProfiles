mobacProfiles
=============

MOBAC profiles for every country

0. TL;DR
- Get your country profile
- Add it to your MOBAC folder
- Set your export format
- Delete excess zoom levels
- Click "Create Atlas"

1. What is MOBAC?
http://mobac.sourceforge.net

Mobile Atlas Creator is an amazing app that allows you to download map tiles in lots of standard formats. 
I use it to get Google Maps offline on my iPhone using Galileo, and Mac using Leaflet. It also works with RMaps on Android.

To download the map tiles, you usually select a rectangle using MOBAC, and a maximum zoom level. 
When I travel, I like to download the entire country's map at a low zoom level (14).
I then select the areas where I plan to go at a higher zoom level (18). That way, I'm unlikely to be lost. 

2. What are MOBAC profiles?
The problem is, most countries are not rectangular. 
Since MOBAC 1.9.15, it has been possible to import GPX tracks into MOBAC to select non-rectangular regions. 
I found GPX maps of many countries around the world, and converted them to MOBAC profiles. 
For the remaining countries, I found GeoJSON borders, converted those to GPX, and converted those to MOBAC profiles. 

The result is an XML file for each country, at the maximum zoom level of 18. 

3. How do I use these files with MOBAC?
- Download the MOBAC profile for the country of your choice.
- Copy it into the MOBAC1.9.15 folder. 
- Launch MOBAC, and choose an atlas export format. 
- Open the drop-down menu inside "Saved profiles" on the bottom left of the screen. 
- Choose the country profile. 
- Click "Load"
- Click "Create Atlas"

4. What if I want another atlas format?
The profiles were created using the AFTrack format. 
There is no good reason for that, except that it was the first in the list alphabetically. 
To convert the format:
- Click the "Atlas" menu at the top of the screen
- Click "Convert Atlas Format"
- Choose your preferred atlas format (Galileo for Galileo on the iPhone, MBTiles for Leaflet on the Mac). 

5. What if I want another zoom level?
The zoom level for these profiles is 18. That is the maximum for most map sources, and shows a lot of detail. 
Actually downloading a large country at zoom level 18 will take up a HUGE amount of disk space. 
If you bandwidth is capped by your internet service provider, you should think twice about using MOBAC at all. 
For reference, Japan at zoom level 16 is about 2 GB. Zoom level 18 would be much more. 
To reduce the zoom level:
- Go to Atlas Content on the left.
- Open the drop-down for the polygon [country name] 18 (usually there's only one per country, unless there are many islands).
- Right click on [country name] 18 18. 
- Click "Delete".
- Repeat for all unwanted zoom levels. 

6. How do I add Google Maps?
Short answer: it's copyright infringement. Don't do it. 
Long answer: Study how to set up custom mapsources using XML. There are some clues on the MOBAC forum. Good luck :). 