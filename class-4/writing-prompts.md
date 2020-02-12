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

**What does the getDistrictNumber() function do?**

**Looking at the callback to map.on('click',...), what is e and why do we need it?**
