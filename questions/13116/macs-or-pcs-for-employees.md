## Macs or PCs for employees?

- posted by: [Jason Cianchette](https://stackexchange.com/users/-1/277-jason-cianchette) on 2010-07-28
- tagged: `computers`, `office`
- score: 3

When I started my company I bought myself a Mac because that is what I wanted.  I have since purchased Macs for each new employee.  I like having a standard platform and I thought that working with a Mac was a small perk.  

I was shocked to learn today that one of my employees really hates Macs and would have much preferred a Windows PC.

Should I buy him a Windows PC?  I want him to be happy and productive, but what is best for the company?

So, should I stick with just Macs or have both Macs and PCs depending on the preference of each employee?


## Answer 13118

- posted by: [Jesper Mortensen](https://stackexchange.com/users/-1/1261-jesper-mortensen) on 2010-07-28
- score: 7

<p>Do you have, or do you plan within near future to get a structured internal IT setup? I mean shared account management (Active Directory alike), centralized security updating of clients, file and print servers, software installation push, and perhaps central backup of client PCs.</p>

<p><strong>If so,</strong> then having multiple operating systems is a horrible pain in the ... neck. And this is true for any combination of Windows, Linux and OS X. In short, as a small shop, don't try to do this. There are ways of handling this, f.x. Active Directory Group Policies on the Windows PCs and <a href="http://www.puppetlabs.com/" rel="nofollow">Puppet</a> for the Mac &amp; Linux boxes, but it is very time consuming.</p>

<p><strong>If all your computers are self-managed islands unto themselves,</strong> i.e. each employee keeps his own PC in order and shares data with the others over platform-independent webapps, then it doesn't make any difference IMHO. In that case, I'd say give the Windows guy the PC that makes him happy and productive.</p>

<p>Of course, you may have nothing centralized yet, but hoping to get there in the future. If so, then I'd say take a hard look at <em>when</em> you'll realistically be ready to do this.</p>



## Answer 13126

- posted by: [jimg](https://stackexchange.com/users/-1/2380-jimg) on 2010-07-28
- score: 4

Religious battles aside, choice of platform should be driven purely on what makes them more productive. Standardization is for large companies - if your high producers desire a specific setup, are technical enough to handle it, then I would lean towards making them productive. I would hate to force a development crew to standardize on windows if some are linux command line gurus, others like fast windows boxes, and ui / ux types like macs.   

Yes, one platform is easier to support, but if simplifying support is the core rationale to making it the same, then I'd suggest you get a better support person. 




## Answer 13117

- posted by: [NetTecture](https://stackexchange.com/users/-1/3350-nettecture) on 2010-07-28
- score: 3

Mac. I do not like them, too - and once you get bigger they are clumsy to manage, bad in hardware for servers and just EXPENSIVE (what is the new ATI 4850 update? 315 EUR - instead of 80 EUR for a graphics card on PC's).

But given your exisitng infrastructure - stick to what you have. There are a LOT of costs added to having ONE guy with another OS to support.


## Answer 13131

- posted by: [Apollo Sinkevicius](https://stackexchange.com/users/-1/2119-apollo-sinkevicius) on 2010-07-29
- score: 3

For scalability, yes, standardization is important. But I can tell you from my own experience of helping build companies past the 50+ employee mark, even at about a hudred, you can still have a mixed Win/OSX/Linux environment. Give people what they need to get the work done and keep your personal preferences to yourself.

P.S. I am surprised when Macheads are surprised someone does not like Macs. I bought one... and that is the last Apple product I am buying.


## Answer 13119

- posted by: [mark stephens](https://stackexchange.com/users/-1/212-mark-stephens) on 2010-07-28
- score: 1

You can use VMware or Parallels to run Windows software on a Mac. If you are spending lots of applications on the Internet it does not really matter what they use.


## Answer 13122

- posted by: [John Bogrand](https://stackexchange.com/users/-1/3577-john-bogrand) on 2010-07-28
- score: 1

In general I would go with the tools that the employee needs and works best with.  

But the issues relating to this are implementation which are technical and what type of environment you have in the work place.  Are there a bunch of security concerns, remote access, network file drives with some type of server secuirty and such?  If you have the know how in the work place then it may make sense to identify what the project would take and make the environment available for both Windows and Macs.  If the implementation is easy and low cost I think its a no brainer and please the employee and if it is difficult or expensive then depending on what that employee does and the real bennefit to the Windows system vs mac it comes down to a cost ben analysis.



---

All content is licensed under the [CC BY-SA 3.0 license](https://creativecommons.org/licenses/by-sa/3.0/).
