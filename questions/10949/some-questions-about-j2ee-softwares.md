## some questions about J2EE softwares

- posted by: [Community](https://stackexchange.com/users/-1/-1-community) on 2010-05-08
- tagged: `enterprise`
- score: 0

how common is it for J2EE applications to use open source libraries or packages ?
is this common ? say a company takes a GPL library and incorporates into their enterprise software....or would you have to write EVERYTHING from scratch :(

how are java enterprise applications requiring server side logic, delivered by the vendor to the client ? do they deliver the actual hardware server with everything installed ? or is it commonly expected for you to provide the hosting. what if the client wants the server on their company premise....JSP codes are exposed when an IT guy pokes around at the source...

java apps can be decompiled and source code exposed, what type of legal paper would you need to draft to protect your asset and Intellectual property to the company you are selling to ?





## Answer 10954

- posted by: [Benjamin Wootton](https://stackexchange.com/users/-1/2094-benjamin-wootton) on 2010-05-08
- score: 1

<p>The question might be better for <a href="http://www.stackoverflow.com" rel="nofollow">Stack Overflow</a>.  I'll have a stab though in case it's interesting to anyone. </p>

<p>The answer to each of your questions are 'it depends':</p>

<p>Open source libraries - I've never seen a JEE project yet that didn't at least have some dependency on some open source library.  The specific restrictions will depend on the actual open source license that applies to your library.  GPL doesn't necessarily pollute your code base in the way you describe if you are just linking to the library.  </p>

<p>Packaging - JEE apps can in theory be packaged as an application server agnostic EAR or WAR file.  Others might include some embedded application server to make it simpler for the end user.  Some might use an installer and some might just provide everything pre-configured on hardware or 'appliance'.  It all depends on cost, sophistication of end user, market breadth etc.</p>

<p>Decompilation - there is a technical solutions which will get you 90% of the way if you are concerned about this.  Google for obfuscation tools which will hide the symbols and logic in your code from prying eyes.  </p>

<p>I'm a JEE developer in the day job and think it's an excellent platform for enterprise development.  It probably wouldn't be my first choice for a product that was going to be widely distributed to customers though.  </p>



## Answer 10955

- posted by: [James Black](https://stackexchange.com/users/-1/1074-james-black) on 2010-05-08
- score: 1

In Java programming, probably moreso than .NET programming, open-source software is used a great deal in project, if nothing else then by including some of the common-* libraries from the Apache project.  You will also find Spring being used a great deal, and various projects from Google code may be found.  You will find some many open-source .NET programs that are just ports of Java open-source projects.

As Benjamin mentioned, for packaging, EAR and WAR files are very common, but for a complicated application you may have several EAR files that need to be installed, but you may find other programs are also needed to help facilitate integrating with other enterprise applications.

For example, you may want to include JAX-WS 2.2 if you need some features there for webs ervices, that aren't included in java distributions.  If you are using Grails to do your front-end then that will be in a common library directory so your various ear files can use it.  So, an installer would be useful.

You may need to support multiple application servers, so different configuration files may be needed to get everything working better.

Then you have database support, as you will want to support multiple databases, otherwise you are limiting your market to just those that have the software you choose to support.

Anything can be decompiled, even if it is just looking at the assembly code of a C program, to see how it works.  This is just a fact in the computer world.

But, you can make it hard enough to look at that it may not be worth the effort to go through these steps.

You can get fairly standard legal contracts that state it is a violation of the agreement to decompile or modify the code, but that is best handled between you and a lawyer.

If you are really concerned about people getting any access to your code, then have your J2EE app go to your company site for the processing, but, then you have limited your market again, because some companies have policies that forbid such software, as everything needs to be hosted on-site.

So, decide what market you are interested in, then start to look at what you can do to not limit who can use your application within your target market, by looking at commonly used databases, application servers, what languages are used on the servers, what policies may constraint your design.



---

All content is licensed under the [CC BY-SA 3.0 license](https://creativecommons.org/licenses/by-sa/3.0/).
