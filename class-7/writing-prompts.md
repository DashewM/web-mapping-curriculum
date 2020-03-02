### Web app cartography

**Color plays a significant role in the visualization of map data. What are some important considerations to keep in mind when choosing the appropriate color scheme for your map?**
It is always important to keep in mind that color has meaning. IF we are making a map about politics for example, it makes sense to assign Democrat to blue and Republican to red, but be careful about how these colors are used in other contexts. Some people associate red with bad, for example. These meanings change culturally and from person to person, so it is always a good idea to consider your audience when deciding on your map colors. It is also important to keep in mind how people with colorblindness will view your map. Will the values still make sense, or will they be confusing? Maps should be accessible, so this is important to keep in mind.

**Why might you want to avoid using a rainbow color scheme?**
Rainbow color schemes have no logical color ramp or purpose behind the colors applied to the values. It is difficult to see any relationship between the colors and the data presented, and thus is difficult to even read the map. Maps are supposed to be effective tools for visualizing data, so it is very important that the the map is legible in the first place and the colors have a reason for being what they are.

**List and describe 2-3 different thematic map types**

Choropleth maps are maps that show values geographically in a color gradiant, with the lighter colors representing lower valuers and darker colors representing higher values. The colors are assigned to geographic polygons at the corresponding level. For example, we would use a choropleth map to show percentage of college educated adults in the United States.

A dot density map presents data more based around freauency. The more an event happens or the higher the concentration, the more dots are in any given area. A dot density map could be used to show bike accidents in San Francisco. Each dot could correspond to a single event, or to any assigned value if working with a large dataset.

**What type of data is appropriately respresented by a sequential color scheme? What about a diverging color scheme?**

Sequential maps are just as they sound: they show a range of a value from small to large. If we are only showing one value, the color should remain constant but go from a gradiant of light to dark as the value increases.

Diverging color scheme maps are useful for showing data that is particularly divergent in one or both directions from the mean. Two colors are assigned to the low and high points of the dataset, and slowly become more towards a middle color (usually white or yellow) as the values approach the mean. This type of data is great at highlighting a mean, or highlighting variation among the dataset if there are many values above and many values below the mean. The colors here are usually opposites on the color wheel, but this does not necessarily have to be true.

**Can you name any tools (either from the presentation or your web travels) that would be helpful for choosing colors?**

The website ColorBrewer, linked in the presentation, seems very useful for picking map colors. https://carto.com/carto-colors/ is another useful tool. Finally, I often use color from images I find on the web, and use an html color from image website to get the proper color codes.

### CORS and working with external data

**In your own words, describe why web map developers have to think about CORS.**

Most of the time, a web map developer will not have all of the resources they are using to build their map downloaded or hosted on their own machine. This is especially true for large or inaccessible datasets. In this case, one needs to link to an outside source. THis is when CORS comes into play. Because your map will not be hosted on the same URL as much of the resources you are accessing (photos, data, etc), you will run into CORS errors. Luckily, there are ways to get around this, but is a persistant problem that always must be considered.

**What is the concept of "separation of concerns?"**

Basically, this means we should keep different types of code in different places. HTML should be in one documentm JavaScript in another, and CSS in a third. All these documents acan be linked so that the webpage still operates, but it makes each document more readable and easier to work with. It also may decrease load times.
