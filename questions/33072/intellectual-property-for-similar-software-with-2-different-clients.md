## Intellectual Property for similar software with 2 different clients

- posted by: [Roger](https://stackexchange.com/users/-1/14705-roger) on 2011-11-28
- tagged: `legal`, `intellectual-property`
- score: 2

I run a business developing my own software that I license out, but also coding projects for businesses at hourly rate.  So clients employ me as a contractor to do this.

Many of these projects are web applications and have similar consistent features, such as a user login, input validation, server side request handling and so on.

Most businesses actually don't do any sort of contract, and to my understanding this means I hold the copyright.

So if one company that I code a web application for wants me to sign a contract stating that they own the copyright, how does that effect things in this situation?  I'm a big fan of re-usable code for generic things, and even if I didn't re-use it, the code would end up looking the same.  This is the part that becomes confusing.

If I have code that is common and not top secret application logic, how can I deal with this situation with multiple projects for different clients?

Thanks!


-----

p.s. I know the end result is to seek legal advice, I just want to try and be informed first.


## Answer 33073

- posted by: [Misha](https://stackexchange.com/users/-1/14706-misha) on 2011-11-28
- score: 1

Quite apart from seeking IP-related legal advice I would make the following observations (this is what I do):

 - If you bring to the project code that will reduce the time for development, state this up front
 - Keep the generic and the project-specific code separate
 - State that the generic code is your IP but grant the client a non-exclusive license to do whatever they want with it
 - Let them know that the project-specific code is theirs and you won't use it in any other project

There are standard licenses and contracts that you can obtain and sign, but these are the basics. I find that smaller companies are fine with this as long as everything works and that they can do what they like with the code. Big companies can often have unwieldy procedures so they can be harder to deal with, but in the end you should be able to get there.




## Answer 33102

- posted by: [Ralph Miller](https://stackexchange.com/users/-1/14720-ralph-miller) on 2011-11-28
- score: 0

<p>First, I am not a lawyer, so yes, do consult a lawyer for legal advice.</p>

<p>Things like authentication are pretty standard these days. Much of that type of code is probably already found in a repository. If you utilize this, since you are not the owner of the code, the company you develop for technically cannot own it. All they own is the custom development, which may include the implementation of business logic or the way in which you tie pieces of code together. </p>

<p>In fact, if you're not using GitHub, check out their <a href="http://Github.com/explore" rel="nofollow">repositories</a>. </p>

<p>Along those lines, you might consider creating your own code repository for all those consistent features using GitHub, and release it using  MIT or creative commons license. </p>

<p>Otherwise, make sure you don't sign any contracts that give up your rights to code you've developed but may wish to reuse for future projects. </p>



## Answer 33129

- posted by: [Snoopy](https://stackexchange.com/users/-1/8919-snoopy) on 2011-11-29
- score: 0

I do the same and i added a few notes to my contracts, but this is for sure specific for each country.

"cost-sharing" is something every customer understands and agrees to. Another alternative is that you sell Modules for a fixed price like a Login Module, CMS Module etc., and just bill the domain specifc stuff based on an hourly rate. The domain specific part can be exclusive, but here it depends where the main knowledge comes from. If its not customer internal knowledge i would limit exlusivity to maximum of a year.



---

All content is licensed under the [CC BY-SA 3.0 license](https://creativecommons.org/licenses/by-sa/3.0/).
