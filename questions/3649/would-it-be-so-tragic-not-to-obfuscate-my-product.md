## Would it be so tragic not to obfuscate my product?

- posted by: [Nestor Sanchez A](https://stackexchange.com/users/-1/1476-nestor-sanchez-a) on 2009-11-15
- tagged: `software`
- score: 3

Disclaimer: I'm not sure if this is for a programming or startup forum, anyway...

Hello,
I'm building a software (a concept-mind-mapping/diagramming product in .NET) and seeing trouble with obfuscation (alteration of deliverable code to difficult decompilation):
It cost money and time to make it work ok, and I think hackers will break it anyway, so...

It would be so damaging not to obfuscate it?
Maybe somebody here had the bad experience of being hacked and found a clone of his product?


## Answer 3651

- posted by: [James Black](https://stackexchange.com/users/-1/1074-james-black) on 2009-11-15
- score: 4

Obfuscation doesn't take any time, but Proguard costs a small bit of money.

Hackers will break it, but do you want to leave your car door open, or lock it, knowing that it can still be stolen?

Obfuscation will also help to make the final code smaller, as it gets rid of unneeded code, at times, so that is also helpful.

If you don't mind that people can easily decompile it to see how your program works, then just distribute it as it is, and since you are so helpful, just compile it in debug mode. :)

Obfuscation just makes it more difficult, and if it isn't trivial then it may require someone that has much more experience, and then it is a matter of whether that person will want to be bothered to hack your application.

I can clone your application by using it though, so looking at the code isn't necessarily needed, but I think the other benefits of obfuscation, and the fact that you just pay a price while compiling, makes it worth it.


## Answer 3681

- posted by: [Mike](https://stackexchange.com/users/-1/1230-mike) on 2009-11-16
- score: 2

<p>You said you are building it in .NET, in which case you are in luck. <a href="http://code.google.com/p/babelobfuscator/" rel="nofollow">Babble Obfuscator</a> is free and easy to setup in .NET. I've used it to obfuscate an ASP.NET website and SharePoint solution dlls (both coded in C# with ASP.NET ascx/aspx code-behinds) and it works great. Like all obfuscators, if someone really wants your code and is prepared to spend money and/or time they will get it. But why make it easy for all the wanna-be hackers out there? .NET code is so easy to disassemble with Reflector or ildasm, and Babel Obfuscator prevents both from working.</p>

<p>After some tweaking I found I got the best results from Babel after making as many classes as possible have a private or non-public scope. Keep in mind you cannot use the new Visual Studio 2008 code-signing and instead have to use snk keys.</p>



## Answer 3652

- posted by: [Jesper Mortensen](https://stackexchange.com/users/-1/1261-jesper-mortensen) on 2009-11-15
- score: 1

<p>Well, it depends.</p>

<p>One thing you can do is simply outrun the bad guys, i.e. add lots of compelling features in the later versions, so that everyone would want to use the later versions. If you do this, then maybe you don't need to add obfuscation and license management to the first version(s).</p>

<p>On the other hand, obfuscation should be completely safe, and more or less free of charge on most platforms today. I don't know about .NET obfuscation, but try Googling it and try asking over at <a href="http://stackoverflow.com/" rel="nofollow">stackoverflow.com</a> ; I would guess there are OK open-source or inexpensive .NET obfuscators available.</p>

<p>Another thing is some sort of license management system. Again, I don't know what the top contenders on .NET are; I would propose to ask over at <a href="http://www.oisv.com/" rel="nofollow">OISV</a> , <a href="http://www.asp-shareware.org/" rel="nofollow">Shareware Professionals</a> or <a href="http://discuss.joelonsoftware.com/" rel="nofollow">Joel's forum</a>.</p>



## Answer 3677

- posted by: [Jeff](https://stackexchange.com/users/-1/876-jeff) on 2009-11-16
- score: 0

Aren't you jumping the gun a bit? First, you have to make your software successful before anyone is going to try to steal it. While IP protection is be important at any stage of development, don't spend too many of your resources on it.--Focus on getting your code to market and selling it. If you focus on the customer you will by default 'outrun the bad guys' as Jesper Mortensen suggests. 


## Answer 3709

- posted by: [Winfield](https://stackexchange.com/users/-1/1020-winfield) on 2009-11-16
- score: 0

If you're building a web application in .NET, why are you even concerned about obfuscation?!  Your application lives on your servers, obfuscation adds very little protection for the hassle.

If I'm mistaken and this is not a web application, why would you choose desktop software in this day and age?


## Answer 3889

- posted by: [Scott](https://stackexchange.com/users/-1/1133-scott) on 2009-11-20
- score: 0

I found this article really insightful when thinking about this topic http://www.kalzumeus.com/2006/09/05/everything-you-need-to-know-about-registration-systems/

I think you have to learn to live with the fact that pirates will hack you. They have a lot of time, and tools, and incentive to do it. The harder you make it to steal your product, the bigger the risk you take that you'll also make your paying users unhappy. 

(So make it just hard enough that the mostly-honest people won't steal it.)


Someone else (Joel? asmartbear?) once made an observation that he didn't care about competitors reverse engineering his app because that means those guys are busy playing catch up... leaving him free to make his app easier to use, more beautiful, and feature rich. So the takehome lesson there is to use a code obfuscation tool if it's convenient, but not to spend a lot of time or effort on it.





## Answer 3937

- posted by: [Brandon](https://stackexchange.com/users/-1/18-brandon) on 2009-11-21
- score: 0

It depends on your market. If you are planning to sell this to businesses, then it almost certainly does not matter. Businesses pay for software that provides more value than it costs. Furthermore, in general, they will not get your software from warez/crack sites. There's too much downside for them especially if your software is not providing enough value to justify buying it.

If you're selling to individuals, it *might* be important to obfuscate, depending on who the individuals are. Are you selling to a demographic that will steal software? If so, then by all means. If not, then it probably does not matter. Just make sure you make it easy for users to buy it and obvious to them that the software is not freeware.





---

All content is licensed under the [CC BY-SA 3.0 license](https://creativecommons.org/licenses/by-sa/3.0/).
