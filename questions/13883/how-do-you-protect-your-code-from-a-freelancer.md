## How do you protect your code from a freelancer?

- posted by: [Community](https://stackexchange.com/users/-1/-1-community) on 2010-09-04
- tagged: `intellectual-property`, `software`
- score: 7

I want to hire a freelancer to fix some bugs on my startup code. How can I protect the code from being stolen?




## Answer 13885

- posted by: [Ross](https://stackexchange.com/users/-1/1390-ross) on 2010-09-04
- score: 8

You can't. But if you product is modularized you can expose some modules to the freelancer not the whole product.


## Answer 13902

- posted by: [JeffO](https://stackexchange.com/users/-1/1796-jeffo) on 2010-09-05
- score: 4

Only hire people with strong reference and want to maintain their reputation. Otherwise, you'll spend too much time trying to police them. 


## Answer 13964

- posted by: [Ricardo](https://stackexchange.com/users/-1/42-ricardo) on 2010-09-09
- score: 2

Hire someone you know. If you don't know anyone, then just check for references, and also try to create a good work relationship with that person once you start working with him/her. Nowadays is easier to find a lot of information about a person's reputation just by looking online... 

In the end, there is really nothing that will prevent someone from stealing code if that is what they really want to do, that is why is a good thing in my own opinion to find people trustworthy and maintain a good relationship with them so you don't have to worry about these things every time you need to hire someone to do a small change to your code. 


## Answer 25497

- posted by: [A-b](https://stackexchange.com/users/-1/10721-a-b) on 2011-05-26
- score: 2

There is a difference.<br><br>
You can protect your idea from developers, but cannot protect your code, some parts will always be reused but you should not care about code, its the idea that matters.

You need to be a developer yourself (or have at least one trusted developer at hand) to be able to protect your idea from freelancers.<br><br>
Do the design yourself and target a modular structure. Be clear and precise with requirements as this will help when integrating.<br><br>
Distribute module development among freelancers and keep the integration part for yourself (or your trusted developer) so only one person will have access to all the code and will know what is being actually done.<br><br>
 The good thing about modular structures is that most of your freelancers will not even have the idea what they are actually building. <br><br>
This approach is very good and helps in scaling your application too. Only drawback is slightly larger initial costs.


## Answer 50990

- posted by: [Adam C](https://stackexchange.com/users/-1/27921-adam-c) on 2013-09-17
- score: 0

I worked with a team developing software based around various parts of the globe. The setup, although did not reduce the risk to zero, has so far protected the assets.

We have some servers at a location where all development work is done. These are windows servers. The developers login to the server where they do not have administration rights, copy/paste and RDP file transfer are disabled. 

This means they cannot copy things to/from that server. 

The server has no outbound internet access other than to a list of pre allowed IP addresses which the developers request via senior staff. There is a CISCO router for this. 

File transfers where done with a Senior staff who would copy files to/from the server manually after inspecting what the files actually where. It's now automated via an email approval system. 

Might sound overkill but keeping the code is important and keeping the development in this kind of infrastructure prevents any other back doors/viruses from getting into the systems. 


## Answer 51010

- posted by: [Mr Jack](https://stackexchange.com/users/-1/27312-mr-jack) on 2013-09-18
- score: 0

<p>You cannot. If you want someone to work on your code, he can always steal it, unless you allow untested code. If you want cheap labor, that is the risk. Otherwise, have it in-house and hire local programmers who if you find steal your code, you can have some form of recourse against them. </p>



## Answer 51011

- posted by: [EfficientLeader](https://stackexchange.com/users/-1/27825-efficientleader) on 2013-09-18
- score: 0

<p>I couldn't add a edit/add comment to above module Answer.</p>

<p>If necessary, they may need to build a special test application so that they only improve the components they need to.  This is safer than an open contract, especially if dealing with code.    Another issue is that version control often exposes all code, so you'll want to modularize ACCESS to the code repository.</p>



## Answer 13887

- posted by: [NetTecture](https://stackexchange.com/users/-1/3350-nettecture) on 2010-09-04
- score: -3

This is called "contract". Ever heard of it? You make a contract specifying damages if the freelancer does that. Then you enforce it using something called a "court".

That said, that is it. Freelancers can still steal your code. There is no protection, except not giving them access to the code, which is kind of hard if... they shall debug it.



---

All content is licensed under the [CC BY-SA 3.0 license](https://creativecommons.org/licenses/by-sa/3.0/).
