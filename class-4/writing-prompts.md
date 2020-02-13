### Objects recap

**An object is a series of ____’s : ____’s**
An object is a series of keys : values, or key value pairs.

**What kinds of things can be included in an object?**
Many things can be included inside an object. Numbers, text, strings, variables, and fucntions can all be included in an object.
### Intro to “client-side”

**What does client-side rendering mean in the context of web maps?***
Client-side means that the map and its components are rendered (or drawn) on the user's computer instead of sent over to the user's computer by the server. This allows for dynamic interaction with the map.

**Why is it possible for Mapbox GL JS to place labels dynamically as you interact with the map?***
THis is possible due to the fact that Mapbox GL JS renders maps client-side, as well as the fact that Mapbox Studio uses vector data tiles. Because of this, any interactions between the user and the map can be rendered in real-time on the user's computer, rather than being prerendered and sent over by an outside server.

**Jurisdiction finder recap** For the following 3 prompts, reference the working file and README.md in the jurisdiction finder explanation folder in the main class repo.

**Describe how feature gets to the makeFeatureLabel() function.**
First, `map.queryRenderedFeatures` is used to return the list of features when the user clicks on the map. A further argument of layers is added so that only features in the layer class are retrieved. The features are then looped through, and HTML values describing each one are stored. `featureToHtml` makes this data human readable, and finally, `makeFeatureLabel` translates this human readable data from each layer into a nice, neat format that we want in our table.

**What does the getDistrictNumber() function do?**
`getDistrictNumber()` takes the feature that is clicked, and retrieves both the corresponding layer of that data as well as the ID number for the district. Since each data source has a specfic attribute name, we need this function to distinguish between the layers and fetch the correct ID number for the clicked district.

**Looking at the callback to map.on('click',...), what is e and why do we need it?**
The "e" stands for event, and it is a placeholder in the `map.on('click',...)` for the function of the event which is defined below within the {} brackets. Once the map is clicked, the function of e is executed. However, I believe that this e function would have to be defined differently every time, as it isn't assinged as a variable to house that function, so can be used multiple times, but this might be wrong.
