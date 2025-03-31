# Nadav DataEssay

A template for publishing Nadav's data essay in GitHub pages 

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
