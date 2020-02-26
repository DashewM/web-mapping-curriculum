### Data prep and analysis

**Find at least two web mapping examples that allow for user analysis. For each example provide: 1) a link to the web map and 2) a description of the user analysis**
1.http://www.therefugeeproject.org/#/2018
This map, of refugee origins and destinations allows users multiple tools to visualize the data in different ways, such as migration destination, country of origin, and giving access to data in graph formats. The user can look at data as far back as 1980 for every country, and see major news from that country in that year which may have drawn migration or emigration. The user can thus draw their own conclusions about the phenomenon of migration and why it has happened in this way for the last 40 years.

2.https://evictionlab.org/map/#/2016?geography=states&type=er
A map we have examined previously, the Eviction Lab map allows for a ton of user interaction with the data. It allows the user to go back to 2000 in order to compare current data, and even lets the user compare the data between multiple states. It is a great map that presents the data in a way that allows for much user analysis depending on what is needed.

**Give an example of static data you might include on a web map. How is your example different from dynamic data?**
An example of static data that might be inlcuded on a map would be, in terms of our project, the points regarding homeless services. These points are fixed and do not change with user interaction, and simply exist to illustrate or show the user something. Dynamic data is anaylzed as or right before it is being displayed, and may update depending on the user's interactions with the map.

**Under what circumstances might you want to do some data prep in desktop GIS before incorporating data into your web map? Give an example of the type of data that might apply here.**
Desktop GIS would be useful for manipulating data that needs to be joined to another dataset or a dataset that needs to be slimmed down before being rendered on the webmap. If, for example, we were combining a dataset for the location of homeless encampments with a dataset of the time of the calls, we would first do this in desktop GIS before using this data on the webmap.

**What are some data characteristics that can impact rendering speed? How might you address these issues?**
Characteristics that can impact rendering speed include the size of the dataset, the number of layers being displayed, and the number of elements present on the page. The easiest way to address this is to clean and trim the dataset, deleting all unnecesary rows and columns.

**What is turf.js? Give an example of how you could apply a turf operation to a web map.**
turf.js is an open source geospatial analysis tool which can be used in Javascript and has similar functionality to some of the operations in ArcMap. An example of a turf operation being applied to a webmap can be found in our homework. Turf allows us to perform operations like identifying points within a polygon. If, for example, we wanted to make a map that told us what species live in a given area that the user clicks on, we could use the point in polygon feature of turf.js to return a list of points in the polygon where the user clicks.

### Inline writing prompts

**Describe where the centroids variable comes from. How is it possible for you to reference this variable when you didn't declare it?**
The centroids variable comes from the linked file suppied for homework. By linking this file with a script tag, the program knows it exists. Since within this file var `var centriods` is defined, we can reference it now that it is linked.

**Why might you want to create the 'centroids-selected' layer after you've created the 'centroids' layer?**
We create two layers so that we are able to style the selected centroids differently than the unselected ones.

**Should you set the marker's lngLat and add it to the map? Why or why not?**
You should not. The marker needs to appear whereever the user clicks, so setting its location to a specified longitude and latitude will not allow the user to interact with the map.

**How did you know which arguments to pass to the pip() function?**
In the code, it specifies that the `pip()` function accepts `pointsFeatureCollection`, which I assume is the `centroids` variable, and `polygon`, which I would assume is the created search radius. However, I ran into errors with this set of arguments and could not get the function to operate correctly.
