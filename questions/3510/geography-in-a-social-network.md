## Geography in a social network

- posted by: [Joseph Turian](https://stackexchange.com/users/-1/423-joseph-turian) on 2009-11-12
- tagged: `profile`, `geography`, `social-network`
- score: 3

I want to make a global social network, in which users can search for nearby users.

What is the preferred way to allow users to easily specify where they are located?

Zip code would be accurate, but is US-only.

Lat/long would be accurate, but it is too difficult for mom and dad types.

Drop-down menu of continent, country, province, major city is simple, but perhaps not that accurate if someone lives somewhere remote or in between two major cities.

My question isn't how to convert an address to a lat/long.
My question is what is the most idiot-proof user interface to get a user's address within a few miles.

Your thoughts?


## Answer 3522

- posted by: [Arpit Tambi](https://stackexchange.com/users/-1/309-arpit-tambi) on 2009-11-12
- score: 4

<p>See this - <a href="http://developer.mapquest.com/" rel="nofollow">http://developer.mapquest.com/</a></p>

<p>Since you are starting up I guess it would be best that you don't develop such a thing in house and use 3rd party solutions. I think mapquest lets you do what you are trying to achieve. Also see the Google API - <a href="http://code.google.com/apis/maps/" rel="nofollow">http://code.google.com/apis/maps/</a></p>

<p>If you want to develop your own solution (which is good for a scalable platform), there is something called - <a href="http://en.wikipedia.org/wiki/Great-circle%5Fdistance" rel="nofollow">Great circle distance</a></p>

<p>See for more details - <a href="http://stackoverflow.com/questions/1631710/strategies-for-large-volume-of-location-geocoding" rel="nofollow">http://stackoverflow.com/questions/1631710/strategies-for-large-volume-of-location-geocoding</a></p>



## Answer 3511

- posted by: [Oleg Barshay](https://stackexchange.com/users/-1/1098-oleg-barshay) on 2009-11-12
- score: 2

Unless you are trying to connect next door neighbors, I would imagine City + Country should be sufficient...  Make them select a country from a drop down and type the city or better yet, a single free-form auto-completing text field.  

If the city is ambiguous/misspelled or you don't have it in your database, ask the user for clarification (e.g. which state, zip code or near which major city).  You would need a decently large database of cities and their GPS coordinates but you can purchase this type of information (quick Google search: http://www.geodatasource.com/).




## Answer 3516

- posted by: [Gabriel Magana](https://stackexchange.com/users/-1/1158-gabriel-magana) on 2009-11-12
- score: 1

Some good comments on this already.  I'll add one more thing:  I have worked on global financial systems before and I can tell you that the databases you can purchase (for example, the ISO location database, which lists country-territory/state-city-global_coordinates and at first seems ideal for your needs) are woefully incomplete.

Don't get me wrong, they are a great starting point, it's much better than having nothing.  You'll just need to build expandability from the very beginning.  Allow your users to build upon it, add a city that is not there, or add a neighborhood to a city (for example, NYC in the USA is the only place where people routinely specify where they are from within a city (the borough, such as Queens, Manhattan, etc...).  You would do well to accommodate that, specially given that people from other places in the work do this more routinely (and each city subdivision or neighborhood is markedly different from the next, so people in, say, Mexico city really do care what part of Mexico city other people are from).

If your project is all about location and finding people based on it, it would pay off if you make your mechanism a accommodating as possible, so spend some really good time on this.  Allow people to tell you as easily as possible where they are at, and allow people to add their location to your database as easily as possible.


## Answer 3514

- posted by: [Clint](https://stackexchange.com/users/-1/1100-clint) on 2009-11-12
- score: 0

Implement a global map mashup that allows users to navigate to their part of the globe and mark their exact location. Your application would then obtain the lat/long and store that in the backend, keeping all location data uniform.

It may also be beneficial to provide an alternative locating system, such as choosing a major city and country. It gives the user the option to choose the most familiar interface. Although, providing many ways to do the same task can be a bad design.

It is best to test all viable options and let your users tell you what they prefer.


## Answer 3536

- posted by: [Jason](https://stackexchange.com/users/-1/2-jason) on 2009-11-12
- score: 0

Check out http://weather.com.

You enter a free-form location and if it's ambiguous they present you with a short list of options.

You can also use the person's IP address to get an approximation.  That would be bad if it were ALL you used, but for example you can use that to pin down the country so the rest of your city/region/zip search isn't presenting options from across the globe.

For a decent, free IP address -> location database, see http://maxmind.com.  Don't use the Google IP stuff -- it barely works.


## Answer 3548

- posted by: [scunliffe](https://stackexchange.com/users/-1/1103-scunliffe) on 2009-11-13
- score: 0

I quite like a simple autocomplete textbox.

After 2 characters, run a search and return the top 10-20 results... re-filtering on each additional character as typed.

Thus if I type "**tor**" I typically see "**Toronto, Canada**" in the results almost immediately.

And for cases where there are lots of dupes... just list them e.g.:

    Springfield, Sangamon, IL, USA
    Springfield, Hampden, MA, USA
    Springfield, Lane, OR, USA
    Springfield, Clark, OH, USA
    Springfield, Fairfax, VA, USA

However if you need geo-location that is more pin-point than a city this might not be as robust as you want.



---

All content is licensed under the [CC BY-SA 3.0 license](https://creativecommons.org/licenses/by-sa/3.0/).
