# 💃 NightCrawler 🕺

We created a night-out planner which allows you to search for a inputed location, or use your current location, and find nearby events. You can then add an event to your 'Night-Out'. From here, you are given the option to find nearby restaurants and bars, and add them to your night aswell. We created a database for our users to save their nights and allow different users to log in and out. We called on 3 API's; Google Maps, MapBox and Predict HQ, which we will go into more detail below.

## 🧞 About Us 🧜‍♀️

Night-Out Planner was created by Harry ([harrygturner](https://github.com/harrygturner)) and Claudia ([claudifox](https://github.com/claudifox)).

## MVP 🎭

We wanted our app to fulfill the following:
1. User should be able to search for a location ✅ 
2. User should be able to find events in a nearby radius ✅
3. User should be able to find the top 20 events as rated by Predict HQ ✅
4. User should be able to log in ✅
5. User should be able to save events, and have them persist on the database ✅

## Stretch Goals 🍔🍔

In order to further our app, we wanted to:
1. Allow a user to search for restaurants in the nearby vicinity to the event ✅
2. Allow a user to save their restaurant choice to their night, and have them persist as a whole 'night-out' on the database ✅
3. Implement CSS which is aesthetically pleasing to work with MapBox's styling ✅

## Super Stretch Goals 🍸🍸🍸

We wanted to also achieve these goals if we got the time towards the end of the week:
1. Allow a user to search for both restaurants and bars, and add a mixture of both to their 'night-out' ✅
2. When a user selects an events and adds it to their night, the other events are removed from the map ✅

## APIs

([MapBox API](https://docs.mapbox.com/mapbox-gl-js/overview)) --
We used MapBox to render the map on the page, and built layers to create the different markers for events. 

([Google Places API](https://developers.google.com/places/web-service/intro)) --
We used Google Places to find nearby restaurants and bars to events, we used the coordinates of our chosen event to find the 20 nearest restaurants/bars.  

([Predict HQ API](https://developer.predicthq.com/)) --
We used Predict HQ to find the top 20 rated events near to your chosen/current location. This can vary from DJ residencies, to plays, to lectures.

Our biggest issue with the APIs was that Google and MapBox take coordinates in the opposite order. Make sure you have you longitude and latitude the right way round!

## Demo





## The Project Requirements

Must be a HTML/CSS/JS frontend with a Rails API backend. These should live in two separate repositories. All interactions between the client and the server should be handled asynchronously (AJAX).

Must render out a resource with at least one has-many relationship (that's two resources total) in the JSON.For example, if we were building Instagram, we might display a list of photos with associated comments. Both resources should be editable.

Must use your Rails API and a form generated by the client to create a resource and render the response without a page refresh. For example, if you create a new Photo post, and form data would be serialized, and submitted via an AJAX POST request, with the response being the new object in JSON and then appending that new photo to the DOM using JavaScript (ES6 Template Literals, can help out a lot with this).

No user authentication with passwords. When the page refreshes the current user will effectively be signed out. The way you learned this in the previous module relied on the fact that Rails was sending small pieces of data (cookies/sessions) back and forth along with every request and response. Now, we have two separate applications and need to use a slightly different pattern. We'll look at patterns for dealing with client-side auth later in the semester, so you'll have plenty of time to deal with this case.
