**What is the difference between raster and vector data?

Raster data is stata from satellites and other forms of remote sensing which is displayed in grids and cells. In terms of webmapping, raster tiles are simply images. A map is made up of many of these images. Vector data consists of points, lines and polygons. They also store data seperate from where the rendering takes place. These can be manipulated much more easily than having to render thousands of images for new raster tiles, and this is what Mapbox Studio takes advantage of to be able to create highly customizable map styles.

**Why do "slippy maps" exist?

Slippy makps exist because in the early days of web mapping, maps had to be reloaded every time the extent of the map was changed. This created a need for maps to load faster, and this was done by rendering all the tiles around the cursor so that one could maneuver around the map with minimal loading. By moving the cursor, which causes the tiles to load, you are "slipping" through the map.

**Why would you want to install a dedicated text editor?

Installing a dedicated text editor helps us to keep our code clean and clear. Writing code in Word or Notepad is almost impossible, as you cannot see what level certain things are on, where the opening and closing brackets are, and what parts belong under what tags. Text editors also have some level of automation to make the process of writing code more streamlined.

**What is Leaflet?

Leaflet is an open-source library for webmaps. It uses JavaScript and is free to use to anyone who wants to create maps. We can use the work done on Leaflet to streamline the process of creating a map.

**How has web map rendering changed over the years?

In the beginning, web maps were rendered one tile at a time on the webpage. Then, once the tile standardization was created, web maps were rendered as x amount of tiles on screen depending on the zoom extent. Tiles adjacent were even prerendered for seamless panning. Now, MapBox has created a system of vector tiles which can be easily edited on the fly. This allows for changes to be made to maps without having to completely re-render millions of map tiles.

**What is the basemap-overlay paradigm and how are GL maps different?

The basemap-overlay paradigm is the dominant way webmaps are rendered. It takes data, styles it to a specfic scale and extent, and exports it as an image. These images become map tiles. Data was thus overlayed on a basemap, but every time you want to change something about this data or the styling, you needed to re-render all of the tiles. GL maps are different because they use vector data. Thus, the data is seperate from the tiles. It renders maps with vector tiles in the browser rather than retrieving images from a server, and makes on the fly edits and lots of other cool things possible.

**Head to the Mapbox GL JS examples page (https://www.mapbox.com/mapbox-gl-js/example/simple-map/) and pick two examples under the user interactions section. What kind of interactions do you see? Why might you use each of those interactions?

One interaction here is to adjust a layer's opacity. This can be very useful if there are multiple layers, and we want to see how they compare or interact. Another is to filter symbols by toggling a list. This is useful for someone who is looking for a particular icon or place on a map. If there are too many icons. the user interface is cluttered and it is hard for this person to find what they are looking for, so being able to disable icons is very user-friendly.
