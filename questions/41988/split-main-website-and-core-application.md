## Split main website and core application

- posted by: [Grzegorz](https://stackexchange.com/users/-1/19509-grzegorz) on 2012-09-13
- tagged: `website`, `domain`, `webapp`, `organization`
- score: 2

I have question about some organizational issue. Is a good idea to split my main information website (home, about, contact, ...) and my core application service to domain and subdomain? 

For example:

 - main site *product.com*
 - core service *dashboard.product.com*

All links from my main website like login/register will be point direct to subdomain. In this approach it could be possible to implement two parts of the system in different technologies.

What do you think about this idea? Do you have any suggestions?




## Answer 41989

- posted by: [ToddBFisher](https://stackexchange.com/users/-1/15045-toddbfisher) on 2012-09-14
- score: 2

In general I have seen this type of thing work out well. For example in my current company we have a marketing/informative site built in basic HTML/JavaScript. We also have our main web application build with C# ASP.NET that does a lot of the heavier stuff. 

Dividing the sites into two works out well; our designers are in charge of promoting the marketing site and our developers are in charge of ensuring the web app site is up and functional, which empowers then to focus on their respective strengths. Of course they do go back and forth as needed but for the most part any updates or feature requests are handled efficiently this way.

Our web app does require tighter security, and having the sites split allows us to better control that as well. Any features that our designers want to implement on the marketing site doesn't need to go through as much scrutiny as what we put on our secure web app site. Our web app site requires a user log in, the marketing site does not.

Another benefit in our specific case, we only wanted our marketing site to be picked up by the search engines. Keeping them separate allowed us to effectively hide, for the most part, our user authenticated web app to the general public.

In the rare and hopefully unlikely event that one site may be down, you can also use the other site to post up a status to your users as well.

With using different web technologies, for smaller businesses it's generally a good idea to use the same across the board, that way you only have to look for one kind of developer instead of two when you hire in the future. But if in your specific case you find it makes more sense to keep the technologies different, for example one site is using a pre-built CMS and the other is not, then splitting the site will more efficiently allow you that freedom as well.


## Answer 41990

- posted by: [Joel Friedlaender](https://stackexchange.com/users/-1/5543-joel-friedlaender) on 2012-09-14
- score: 1

Yes you should definitely do this.

Advantages:

 - If your software goes down (more likely than website), your website will still be up (and people will come looking there if software is down).

 - You can make changes and deploy to the website without affecting your app and vice versa.

 - You can give access to your website to a design/web company to make changes without jeopardising security of your app.

 - It gives you flexibility to use the apps domain/subdomain for application specific email functionality.

 - As you mentioned, it's much easier to use separate technology for the application this way

 - If you get a ton of traffic to your website, it won't affect the applications performance

I could go on, but I just see way too many advantages and no real disadvantages.



---

All content is licensed under the [CC BY-SA 3.0 license](https://creativecommons.org/licenses/by-sa/3.0/).
