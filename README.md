# Nadav's Data Essay

For my project, I chose to create visualizations of the most common butterfly species in Delaware County using data from the citizen science platform iNaturalist. To obtain the dataset, I created a query with the following filters: Taxon: Butterflies, Quality Grade: Research, Place: Delaware County, US, PA, Date Range: 2020-03-01 to 2025-03-26. After submitting the request, I received a notification the next day that my data was available for download. I then downloaded the dataset, extracted the CSV file from the ZIP folder, and uploaded it into Excel for cleaning.

The original dataset contained 14 columns, many of which included unnecessary information such as usernames and links to observations. I deleted the columns I didn’t need, ultimately keeping only four: common name, latitude, longitude, and date observed. Then I filtered the common name data alphabetically to have all the species listed together and used Excel functions to count the number of observations per species. From this I identified the ten most frequently observed species. I recorded these species and their observation counts in a separate sheet, and then removed the data for species that did not appear in the top ten. Additionally, I used an Excel function to convert the date observed column from number format to text format.

After cleaning the data, I was ready to import it to the web-based platform Flourish to create my visualizations. I chose Flourish because of its clean aesthetic and its compatibility to generate both a chart and a map visualization. Creating the chart visualization was pretty intuitive, but the map visualization required more messing around with to achieve my desired results. One of the biggest challenges was finding a pre-existing geometry shapefile for the Delaware County layer, which I was ultimately able to source from a Flourish template for US counties.

In the end, I successfully created both a chart and an interactive map visualization, which can be viewed below alongside an explanation of the data and its potential limitations.

## Top Butterfly Species in Delaware County 
The chart below displays the top ten most frequently observed butterfly species in Delaware County from March 2020 to March 2025. The data is sourced from the citizen science platform iNaturalist.

<iframe title="Top 10 Butterfly Species in Delaware County 2020-2025" aria-label="Chart Visualization" id="flourish-chart-22354618" src="https://public.flourish.studio/visualisation/22354618/embed" scrolling="no" frameborder="0" style="width: 0; min-width: 100% !important; border: none;" height="463" data-external="1"></iframe><script type="text/javascript">!function(){"use strict";window.addEventListener("message",(function(a){if(void 0!==a.data["datawrapper-height"]){var e=document.querySelectorAll("iframe");for(var t in a.data["datawrapper-height"])for(var r,i=0;r=e[i];i++)if(r.contentWindow===a.source){var d=a.data["datawrapper-height"][t]+"px";r.style.height=d}}}))}(); </script>

According to the chart, the most common butterfly species in Delaware County over the past five years has been the Huron Sachem (Atalopedes huron). Although not apparent from its name, the Huron Sachem is a species of Skipper butterfly, a group that has made numerous appearances in the top ten list. The Huron Sachem is joined by the Zabulon Skipper, Peck's Skipper, and Silver-spotted Skipper as the most common Skipper species in Delaware County. From this data, we can infer that Delaware County provides suitable habitat for Skipper species, which typically reside in grass prairies or along coastal marshes.

Another takeaway comes from the high number of Monarch butterflies observed over the past five years. Monarch butterflies only lay their eggs on Milkweed plants, meaning that a high count of Monarchs in Delaware County also suggests that the county provides suitable conditions for Milkweed to thrive.


## Top Species Distribution Map
This map displays the geographic distribution of the top ten species of butterfly observations across Delaware County. Each point represents a recorded sighting (color-coded based off species) and includes the date that observation was made. This map is interactive and you can click on the species in the legend to turn them on or off!
<iframe title="Flourish Map" aria-label="Map Visualization" id="flourish-map-22404731" src="https://public.flourish.studio/visualisation/22404731/embed" scrolling="no" frameborder="0" style="width: 0; min-width: 100% !important; border: none;" height="463" data-external="1"></iframe><script type="text/javascript">!function(){"use strict";window.addEventListener("message",(function(a){if(void 0!==a.data["datawrapper-height"]){var e=document.querySelectorAll("iframe");for(var t in a.data["datawrapper-height"])for(var r,i=0;r=e[i];i++)if(r.contentWindow===a.source){var d=a.data["datawrapper-height"][t]+"px";r.style.height=d}}}))}(); </script>

Unfortunately, there aren't too many concrete takeaways we can observe from this map. For starters, the Delaware County shapefile is a solid color and doesn't show geographic or ecological features. Additionally, since these observations are uploaded by citizens, it doesn't provide a comprehensive view of all the species present in Delaware County; rather, it displays the most common species uploaded by iNaturalist users.

That said, we can see that the data is pretty dispersed, meaning that most areas in Delaware County provide suitable habitats for these species. Another thing to note is that some points are georeferenced outside the boundaries of Delaware County. This is most likely due to one of two reasons: either the observation’s conservation status is classified as vulnerable or endangered, meaning the exact coordinates are masked and the point is placed within a radius of the initial location, or the Delaware County shapefile is using a different projection system than iNaturalist, causing the points to be slightly shifted due to this georeferencing difference.

Nevertheless, the visualization is interesting and can be used to compare species against each other, depending on which species the user wants to show on the map.

## Bibliography
