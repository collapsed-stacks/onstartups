## Business Owner Validation

- posted by: [Brian Wigginton](https://stackexchange.com/users/-1/845-brian-wigginton) on 2010-04-09
- tagged: `business`
- score: 5

If I were to start a business listing, and I want business owners to be able to signup for the service and edit/update their listing, what's the best way to validate that a person that calls is indeed the owner of the business?


## Answer 10011

- posted by: [Keith DeLong](https://stackexchange.com/users/-1/888-keith-delong) on 2010-04-09
- score: 2

1. For Sole Proprietors, the common practice is to have them send a copy of their local business license. It confirms them as a legitimate, active business owner.

2. For Corporations, who is the 'owner' you are looking for? CEO, President, a majority share holder? Whatever position you are looking to validate, it won't be difficult for them to send you satisfactory evidence of their position.


## Answer 10012

- posted by: [Gary E](https://stackexchange.com/users/-1/2587-gary-e) on 2010-04-09
- score: 2

There is no easy way to do this. 

You could ask for their company web site address and their email address. If the email address domain does not match the web site, you might have a problem.




## Answer 10015

- posted by: [Jesper Mortensen](https://stackexchange.com/users/-1/1261-jesper-mortensen) on 2010-04-09
- score: 1

<p>US or global? Do you need the actual owner (with the understanding that there may not be a clear majority owner), or just someone who works in the company and has some authority?</p>

<p>I think the method used by Google Apps is the one simplest to automate and scale globally -- require them to make a unique change to their domain's DNS, or upload a file to their website.</p>

<p>Depending on your state, there might be a electronic registry you can purchase a subscription for. I don't know about Texas, but in Denmark the governments "Commerce and Companies Agency" maintains an electronic database of all company registrations which you can subscribe to. Additionally, some providers of yellow pages have enriched versions of the same data available for subscription.</p>

<p>Side note 1: If I was contacted out of the blue, and asked to fax a number of papers to verify ownership, in order to gain access to a webpage... I would almost certainly not agree to that.</p>

<p>Side note 2: Be careful about publicizing information about companies without their consent. See the <a href="http://37signals.com/svn/posts/1650-get-satisfaction-or-else" rel="nofollow">Get Satisfaction debacle</a>...</p>



## Answer 10016

- posted by: [Jay Neely](https://stackexchange.com/users/-1/1801-jay-neely) on 2010-04-09
- score: 1

<p>Google Maps and other local maps services with business listings just call the phone number provided in the business listing: <a href="http://maps.google.com/support/bin/static.py?page=guide.cs&amp;guide=21029&amp;topic=21034" rel="nofollow">http://maps.google.com/support/bin/static.py?page=guide.cs&amp;guide=21029&amp;topic=21034</a></p>



## Answer 10036

- posted by: [vnchopra](https://stackexchange.com/users/-1/2821-vnchopra) on 2010-04-10
- score: 0

I think Brian is on to a pretty cool idea. If you want to have business owners list their businesses on a website(after you have attracted them to your website), I think using both Keith DeLong's idea and Gary E's idea and combining these two would be great.

And if there were a problem with the email address matching, what you could do is send a confirmation email to that email, and if it's accepted then you can have that email address and the business listed. 

You could probably implement Keith's first point after they have signed up and listed themselves that way.



---

All content is licensed under the [CC BY-SA 3.0 license](https://creativecommons.org/licenses/by-sa/3.0/).
