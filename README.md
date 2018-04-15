# Getting your data on a map

This Glitch App shows you how to take any set of data points that is tagged with location information (specifically a latitude and longitude) and display it on a Mapbox map.

## Remixing ideas

### Put your own data on the map

1. Put your data in a CSV (Comma Separated Value) file, and upload it to the assets folder. 
   * *Ensure you keep the name, lat and lng fields*. The rest are optional.
   * If you need a guide of how to do this, check out [this template](https://docs.google.com/spreadsheets/d/1a4B_AkszhSRZXKkpuaZU5KTnz0RNfU_KqkwtEQPwivg/edit#gid=0) (which you can make your own copy of, and then Export as CSV).
   * You can get lat/lng information from Google Maps:
     * Desktop: right click on the map and select "What's here?". The lat/lng is displayed at the bottom of the page. 
     * Mobile: long press on the point on the map that you care about. You'll see a pair of numbers pop up in the search bar - latitude is first, and longitude is second.
2. Click on the file in the folder to get the URL, and replace the value of "url" in the ajax call to the spreadsheet in index.html with your new URL.

## Notes
At some point, you should get your own (free!) API key from Mapbox - otherwise you will risk that your site stops working after a while. The key used in this project will be frequently refreshed, and should only be used when you're starting out with this Glitch app. 

Details on how to do this:

1. Create an account here: [https://www.mapbox.com/signup/](https://www.mapbox.com/signup/)
   * Feel free to ignore the setup wizard that follows, and go straight to [https://www.mapbox.com/account/](https://www.mapbox.com/account/) to find your access token (which looks something like the screenshot below.
   ![screenshot of location of access token on mapbox's site](https://cdn.glitch.com/9cf2405b-5bb9-4e97-86b3-19f1788db8b8%2Fmapbox-access-token.png?1516717036892)
2. Copy the token, and replace the value of mapboxgl.accessToken in index.html with your token.

## More remix ideas coming soon!

### Change the style of the pop-ups

### Change the map theme

### Change the icon

### Set different icons for each category of place

### Zoom in when you click on a group of overlapping icons
