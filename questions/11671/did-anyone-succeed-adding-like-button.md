## Did anyone succeed adding "Like" button?

- posted by: [usabilitest](https://stackexchange.com/users/-1/3024-usabilitest) on 2010-06-01
- tagged: `facebook`
- score: 1

I saw the new Facebook "Like" button on many site and noticed that some of them did not work properly. Today I decided to give it a whirl and alas, can't seem to get it to work on my site. Continue to get the following error:

***You must specify an URL as part of this widget or API.***

I searched the web and it appears that I'm not a lone in getting this marvel of technology to perform. 

Anyone had luck with getting it to work?


## Answer 11673

- posted by: [Michael](https://stackexchange.com/users/-1/2774-michael) on 2010-06-01
- score: 3

You'll want to integrate your Like button something like this...

Note the src attribute of the iframe tag below.  You'll set the href query parameter to the encoded URL of the page you want to register as "liked" when the user clicks the Like button.  In this example, the URL is http://www.mysite.com/page, so the encoded URL is http%3A%2F%2Fwww.mysite.com%2Fpage


    <iframe src="http://www.facebook.com/plugins/like.php?href=http%3A%2F%2Fwww.mysite.com%2Fpage&amp;layout=standard&amp;show_faces=true&amp;width=360&amp;action=like&amp;font=lucida+grande&amp;colorscheme=light" scrolling="no" frameborder="0" allowTransparency="true"></iframe> 


In addition, if you want to customize how the item shows up in the user's Facebook feed, you'll want to add two meta tags to the head tag of your page.

    <meta property="og:title" name="og:title" content="Name of the page" /> 
    <meta property="og:site_name" name="og:site_name" content="Name of the site" /> 



---

All content is licensed under the [CC BY-SA 3.0 license](https://creativecommons.org/licenses/by-sa/3.0/).
