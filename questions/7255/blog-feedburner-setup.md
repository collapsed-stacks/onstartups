## Blog feedburner setup

- posted by: [Eric Amzalag](https://stackexchange.com/users/-1/2302-eric-amzalag) on 2010-01-28
- tagged: `blog`
- score: 0

Im having some trouble setting up the feedburner link for my blog. I want to get my blog up and running but am hesitant to do so until things are working properly.

Right now when someone clicks the "Heads or a Tale" link next to the customary RSS icon, it simply sends them back to the blog page rather then the feed link.

Heres a link to it so you can see what i mean: [Heads or a Tale][1]


However, when you click on the RSS icon it brings up the feed page. Does anyone know how I can make it so that clicking on the "Heads or a Tale" link will also send the user to the feed subscription page? I'd very much appreciate the advice.


  [1]: http://www.headsoratale.com


## Answer 7256

- posted by: [ThomPete](https://stackexchange.com/users/-1/1186-thompete) on 2010-01-28
- score: 1

<p>go to <a href="http://www.superuser.com" rel="nofollow">superuser.com</a></p>



## Answer 7321

- posted by: [Steve Wilkinson](https://stackexchange.com/users/-1/2177-steve-wilkinson) on 2010-01-29
- score: 1

<p>You could use the Wordpress <strong><a href="http://blog.slaven.net.au/wordpress-plugins/wordpress-feed-locations-plugin/" rel="nofollow">Feed Locations</a> plug-in</strong> - my understanding is that it does the substitution for you without you having to edit any pages.  I started with this but I am now using the rather good <strong><a href="http://diythemes.com/thesis/" rel="nofollow">Thesis theme</a></strong> which has this feature built in.</p>

<p>It may be obvious, but once you have got everything up and running, subscribe to your blog by both email and through your blog reader so you can see what everyone sees - sometimes you need to tweak something like fonts for readibility, for example.</p>



## Answer 7266

- posted by: [JeffO](https://stackexchange.com/users/-1/1796-jeffo) on 2010-01-28
- score: 0

Do a text search on your code. Your link that isn't going where you want:

        <a class='rsswidget' href='http://www.headsoratale.com' 
    title='all things Business, Politics, Philosophy, + More'
    >Heads or a Tale</a>

The href should be:  

    'http://feeds.feedburner.com/HeadsoraTale' 




## Answer 7331

- posted by: [Eric Amzalag](https://stackexchange.com/users/-1/2302-eric-amzalag) on 2010-01-29
- score: 0

<p>The solution was actually pretty simple. I just needed to go to feedburner, get the HTML code for the feed button, and then create a text widget in my side bar to place the HTML in. Now the button works properly, and <a href="http://www.headsoratale.com" rel="nofollow">Heads or a Tale</a> is ready to run.</p>




---

All content is licensed under the [CC BY-SA 3.0 license](https://creativecommons.org/licenses/by-sa/3.0/).
