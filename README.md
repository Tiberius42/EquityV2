# LAHacks: P!ng

By Shwe++
(Leo Zhuang, Liam Karl, Louise Schul, Samuel Sommerer)

## P!ng: What's happening?!

Whether you’re in Santa Monica pier or Downtown LA, there is always something happening around the corner. With P!ng, you can see what other people are experiencing all around you! P!ng is an Android app that utilizes Google Maps and Firebase to share what people are reacting to. 

### Trending Now

Living in a city like Los Angeles, you're a busy person. You work hard, and you value your time off. But as anyone who's been to Santa Monica can tell you, even the beach is busy! There’re just too many magicians, dancers, singers, shops, and waves to keep track of all at once. It’s not just Santa Monica either. No matter where you go, there’s always something interesting happening just around the corner that you might be missing out on and too many options to choose from.

That’s where P!ng comes in. A social media app that focuses on connecting users to localized events and activities, P!ng allows normal people like you to let each other know what’s going on!! Users can tag local happenings by creating “pings” at their locations. Each ping includes a caption and a reaction, and, when posted, shows up on a map that everybody can see and view. Pings start out small and translucent on the map, but as other users see and like them, they grow more opaque and visible. This way, the most interesting events stand out above the others, and you’ll have a much easier time finding fun things to do around you! Say you just finished lunch in Downtown LA and don’t know what to do next. All you need to do is take a look at P!ng to how where people are reacting to street performers, art, or other crazy things that are happening near you!

### Under Construction (Like Always)

When we think of cities, we normally think of permanent structures – buildings, roads, and other infrastructure. But often what defines a city and its culture are temporary and informal – it wouldn’t be the same without the artists and musical performers, festivals and celebrations, or even food trucks! We’ve developed P!ng to be a platform for city residents to quickly express their feelings and connect with others over the vibrant culture of their city.

Unlike services like Google Maps, TripAdvisor, and Yelp, P!ng capitalizes on the spontaneous nature of city life. To make this easier, P!ng focuses on emotions – users select an emotion to sum up every message they ping. Additionally, when users browse the map of nearby posts, they’ll see a collection of emotions, where frequently liked messages stand out from the crowd. 

P!ng encourages users to appreciate the temporary and informal nature of cities by allowing them to make and browse spontaneous and subjective posts in their area.

### Quaranteam

In the current, international period of intense social distancing, it can be difficult to connect with others in so many meaningful ways that once felt normal. The precious little moments that make up face-to-face interaction in our community can be lost on us when social encounters are so rare. Despite these challenges, our app allows those small, yet treasured moments to be cherished even when isolation predominates our lives. 

It might feel lonesome being home yet another day due to the threat of COVID-19. However, seeing our neighbors and friends just a walk away pinging all about the intrigue in their area connects us in a uniquely spatio-social way rivalled by few social media applications. On Twitter or Instagram, you can see what people are doing and thinking, but it’s all too easy to forget how close we really are to each other when all you see is a block of text or a selfie. P!ng offers what others cannot in these trying, solitary times: a sense of closeness.

## Technical Details

### Overview

P!ng is an Android app written in Java with Android Studio. It makes use of Google Maps API and Firebase.

### Google Maps

As a location-oriented social media app, Google Maps provides the foundation of Ping’s functionality. We are able to access the geographic coordinates of users with Google’s location services, from which the users can then ping specific positions on a global map based on their current location. Our pings update on the map immediately as you send them, so users can traverse an entire feed of others’ pings just by viewing different areas on the map. The functionality offered by Google Maps ensures that our users can both post pings, as well as view pings by others with particular locations in mind. The content of our platform is thus well-suited to supporting a variety of location-based services.

### Firebase

For this application, we needed some way to store all the pings that users will make. We used firebase to store all our data. The two areas where we used it primarily was fetching all our markers to place them into the map

### Map Markers

In order to distinguish between pings with different emotions, we wanted to have custom map markers. Each map marker design is stored as SVG paths in an XML file and then converted to a bitmap image when the app loads. Everytime a ping is logged, it stores the location, along with the emotion that was tagged with it. This allows us to place the appropriate marker at the correct location. Additionally, new markers start at a lower opacity and become more opaque as they receive more likes. This means that frequently liked messages stand out.

## Future Ideas

We got a lot done in 36 hours, but we know our app can grow so much more! Going forward, we want to add additional functionality for pings. In particular, pings could include pictures or short videos.

Additionally, we could potentially incorporate other social media platforms. Since many Twitter and Snapchat posts are tagged with location, these posts could be included as pings on our map, allowing users to interact with a wider range of sources.

An option to ping specific points of interest and businesses, as opposed to pings solely being used to direct to particular coordinates, may be an interesting way to expand the possibilities of how users interact with pings. Looking for what restaurants are trendy or what scenic nature trails are most popular would be very easily and naturally achieved by seeing the popularity and content of pings at those particular points of interest, for example. 

P!ng could also be used to send brief updates about an ongoing situation. Since it caters to people in nearby areas, local leaders could use the app to update individuals about public events, school closings, weather, and unusual situations.

<br/>
Made with Firebase and Google Maps.
