## Java and .net software market, what are the differences?

- posted by: [UnStartup](https://stackexchange.com/users/-1/2189-unstartup) on 2010-01-07
- tagged: `software`
- score: 2

If one was to write a web application (commercial), what differences market wise is there between the java world and .net?

Say I build an ecommerce application, would I be locking myself into a specific target market if I wrote it in java as compared to .net?

Do people looking for java solutions tend to always look for an open source alternative whereas .net is comfortable with paying?

One point took make note of I know, is that not everyone makes a purchase decision based on the target platform, it really depends if its an end user type product or one more geared towards the technically inclined.  But let's put that point aside and just focus on the differences when it comes down to what platform you develop the software on (java versus .net).


## Answer 6147

- posted by: [skillguru](https://stackexchange.com/users/-1/742-skillguru) on 2010-01-07
- score: 2

It has been discussed here in detail
http://answers.onstartups.com/questions/5179/net-vs-j2ee-java-vs-php/5220#5220


## Answer 6148

- posted by: [Michael Trafton](https://stackexchange.com/users/-1/19-michael-trafton) on 2010-01-07
- score: 2

This answer applies to software that you will be installing in a customer's environment (not hosted SaaS).

We are a Java shop that sells to large corporate clients (Fortune 500s). Most of those companies can support both Java and Microsoft, although most prefer Microsoft. In the past few years, I've seen more and more of my clients de-commissioning Java applications and replacing them with .Net applications. The reason is that they believe Microsoft applications are easier to support (not always true, but that's their perception), and also because it's much easier for them to find developers that know Microsoft than it is to find Java developers. So when they need to customize the software, they want to be able to use Microsoft technologies.

I also sell to mid-market companies (those between $50 MM and $1 Billion in revenue), and most of them are Microsoft shops with much less sophisticated IT departments than the Fortune 500 companies. So while the largest companies can support pretty much any technology, the smaller ones wouldn't know how to support Java if their lives depended on it.

My experience is that companies who favor Java DO NOT assume all Java applications are open source. In fact, most enterprise software written in Java is NOT open source at all. A lot of Java development tools (Eclipse, Tomcat, JBoss, Spring, Hibernate, etc.) are open source, but the Java-based software that companies install is typically commercial software.

eCommerce applications are one place where Java may beat out Microsoft, since many of the best eCommerce tools are Java based (ATG, Endeca, etc.).


## Answer 6146

- posted by: [Brian Deterling](https://stackexchange.com/users/-1/496-brian-deterling) on 2010-01-07
- score: 1

If it's a hosted app, i.e. your company is running it, I'd say, not much difference. Users won't even be able to tell so go with what you know or can find good developers to create.  Although keep in mind that you can typically run a Java stack for cheaper than Windows.  

If your customers are going to have to install it, you have to be more careful.  I've seen Microsoft shops accept a J2EE app before (grudgingly on the part of IT), but I haven't seen many J2EE shops accept a .net app. Part of the reason is that I can install Tomcat on any existing Windows box and have a J2EE app up and running for no additional cost, but I can't install IIS on a Linux/UX box so the customer may have to buy new hardware.  I'd give Java a slight edge (unless you know your target market prefers .net), but probably not enough to switch if I were already doing .net development.



---

All content is licensed under the [CC BY-SA 3.0 license](https://creativecommons.org/licenses/by-sa/3.0/).
