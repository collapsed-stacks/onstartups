## Why some websites give access to their data through REST APIs?

- posted by: [Victor](https://stackexchange.com/users/-1/28042-victor) on 2013-10-13
- tagged: `webservices`, `api`, `data-request`
- score: 3

<p>Quite a lot of websites (glassdoor for example) give access to data about jobs, salaries, etc. through a REST API. So basically I can make an API call, get results and show the data on my website. But isn't this stealing traffic from glassdoor?</p>

<p>If people can get the data on my site why would they visit glassdoor? Why does glassdoor bother giving away data for free?</p>



## Answer 51366

- posted by: [Robin Vessey](https://stackexchange.com/users/-1/984-robin-vessey) on 2013-10-13
- score: 6

<p>You are not stealing traffic from them, you are accessing data they have collected from their traffic. </p>

<p>Reason they do it is it creates an ecosystem around their core platform. </p>

<p>The benefit to them is they become a central point of reference for other systems, like login and like with Facebook. </p>

<p>The chance of you wasting your time to build the same site and having your site be something that competes with them for their actual target market is very low. Remember the technical solution is only 20%-30% of the battle, there is marketing, relationships and for that site a strong network effect that you don't have.</p>

<p>Their intent is to provide you with the data you need to build something cool on top, which in turn helps them be a relevant big player in the eco-system. </p>

<ul>
<li>If developers use their service, there are other services they can also benefit from</li>
<li>If big players use their service then they can charge for it at scale. </li>
<li>IF they are showing you some info, there is probably a lot more under the hood that you can't get to without paying for it.</li>
<li>Every request for data you make gives them a wealth of info about what people are interested in, where they are coming from and gives them insight into what to focus their efforts on.</li>
</ul>

<p><strong>As for what you should do with the API</strong>: </p>

<p>Build something on top, which uses their data, is very cool, gets people using it, extends where they are going (say an iPhone or Android interface) and then present yourself as a buy out target for them. </p>

<p>This is a far more effective strategy for you than trying to do a copy cat site.</p>




---

All content is licensed under the [CC BY-SA 3.0 license](https://creativecommons.org/licenses/by-sa/3.0/).
