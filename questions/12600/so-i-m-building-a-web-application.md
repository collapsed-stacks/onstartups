## So I'm building a web application

- posted by: [Ev Conrad](https://stackexchange.com/users/-1/2862-ev-conrad) on 2010-07-08
- tagged: `web`, `apps`, `application`, `content`, `management`
- score: 1

I'm building a pretty standard web application - login, do some searches via some well defined paramaters, get a list of results, drill down on a result to see details about the results.  While I've done this a lot before, I've always built them from scratch.  Should I be looking at a content management platform?  I'm interested in hearing what others have done, as well as if there are some prefab tools that will help me do this without having to build it from scratch.  For example, if it were 'brochureware' about my company and/or products, I would use WordPress, or simply an web site template.  For an application (again, primarily search using a set of predefined parameters (textboxes, radio buttons, checkboxes, etc), getting a set of results, then being able to click on a result to drill down into its details - is there an easier way of building this than from scratch?  Thanks in advance!

-e-


## Answer 12623

- posted by: [Wil](https://stackexchange.com/users/-1/3747-wil) on 2010-07-09
- score: 1

I can't comment yet since I don't have enough rep, but how deeply technical are you?  Which languages are you comfortable working in?  The different languages all have tools to help with some of this stuff.  Are you looking for free or are willing to pay?

Basically, I think you are looking for grid based controls/plugins that can take your data, allow you to easily sort/page/display/drilldown/etc am I correct?  

The thing you are talking about is technically called "master-detail".  There are alot of example of this in PHP, but I am not sure of any script you can just use.

If you are using ASP.NET, the master-detail views are what you are looking for.  A tutorial exists here http://msdn.microsoft.com/en-us/library/aa581796.aspx


## Answer 13879

- posted by: [Ricardo](https://stackexchange.com/users/-1/42-ricardo) on 2010-09-04
- score: 1

For something as simple as to what you are describing, I will build it from scratch and save it as a template for others to use or even sell to whom might be interested... You are a software developer, coding and building something from scratch is what we (developers) enjoy the most, heck I do it just for the fun of it! Just open your code editor and start coding away, you know what you want and what it should look like, correct?

If you are just not in the mood for coding, then consider one of the many .NET toolkits and open source projects on asp.net, there are a lot of projects in there that will help you get you started:

http://www.asp.net/community/projects

Here's another resource:

http://www.codeplex.com/

Note: I am giving you the links for .NET resources since you mentioned you are a .NET developer.



## Answer 12625

- posted by: [JeffO](https://stackexchange.com/users/-1/1796-jeffo) on 2010-07-09
- score: 0

SharePoint does this 'out of the box' and offers nearly unlimited customization, but this is a Microsoft platform which probably needs .NET development tools unless you like doing things the hard way.

There are several open source document management systems out there which would cater to LAMP, Python, Ruby, etc.

Since you do this a lot, you have a market for these types of sites and I can't see why you couldn't create some scripts & templates of your own to speed up development.





## Answer 15233

- posted by: [Anatoly G](https://stackexchange.com/users/-1/4495-anatoly-g) on 2010-10-18
- score: 0

.NET maybe an expensive way to get your startup off the ground. Unless you do the Bizspark program, even VMs with Windows are more expensive than their linux counterparts. But that's an aside.

It's always nice to start w/ some framework that allows you to build things quickly and easily without writing too much of the same boilerplate. If you're OK with going outside of .NET, there are a lot of open-source frameworks that give you the ability to easily add any component your site needs.

Ones you may want to look into: Grails, Django, Ruby on Rails

When evaluating each, make sure to look at the plugins and the user communities around these projects. You'll find that's the best indicator how easily it will be to grow with that product.



## Answer 17945

- posted by: [Jason Swett](https://stackexchange.com/users/-1/5327-jason-swett) on 2010-12-17
- score: 0

In my opinion, you get the most bang for your buck if you learn a framework. You get a lot more leverage that way than if you start from scratch, but you're not limited the way you would be working with WordPress, Drupal or other CMSs. The big frameworks are symfony for PHP, Django for Python, and Rails for Ruby. It can be a steep learning curve but, in my opinion, well worth the trouble.



---

All content is licensed under the [CC BY-SA 3.0 license](https://creativecommons.org/licenses/by-sa/3.0/).
