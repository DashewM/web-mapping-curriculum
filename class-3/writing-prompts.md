### Intro to interactivity

**What are some strategies interactive map developers can use to ensure maps with a lot of interactions are not overwhelming?
Why do we use the term “map user” instead of “map reader?”**
With lots of interactions, it becomes easy for a map to be cluttered and a webpage to become bloated. TO prevent this, we can branch interctions so they are not all surface level. For example, if we are looking at state populations, we can first click on a state, then look at that state's particular populations. We may then have options to compare states, etc. Basically, we do not want to overload a user wth interactions, but give them a few options and let them explore and dig deeper into the data. We use the term "map user" insted of "map reader" because our audience is not simply reading the map, they are interacting with it on a deeper level.

### Common types of interaction

**What is geocoding and how might you add it to an interactive map?**
Geocoding is the process of turning search queries (addresses, place names, etc) into real world locations with coordinates. By using existing APIs, like Mapbox GL JS, we can add a search bar into our webpages which already has geocoding properties built in. Most map users are accustomed to having conveniences like a search bar, so it is useful in almost every map application.
### Intro to events

**What is an event?**
Events let you know when a user has done a thing on your page. Events help drive user interactions with a wepage instead of just running a code or funtion as soon as the webpage is opened. Events are created, listened for, and then executed.

**Describe an example of how you could use an event listener with an interactive map.**
One example of an event listener being used with an interactive map is a button that takes the user to x location. The button needs to have an event listener to wait for a click event to happen, and when it hears that click event, it causes the function of flying to x location to run. Listeners are useful when we want things to occur at a certain time after a user has done a certain thing.
