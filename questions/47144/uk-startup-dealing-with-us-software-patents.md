## UK Startup dealing with US Software Patents

- posted by: [MikeH](https://stackexchange.com/users/-1/23871-mikeh) on 2013-02-04
- tagged: `saas`, `patent`
- score: 9

As the owner of a UK software company, I'd like to finish a SaaS application I've had in development for a while and sell it as a monthly subscription service. The software could be sold worldwide.

I don't believe that the software infringes any patents, but there are definitely some ridiculous 'obvious' US patents in this product's niche.

What I'm trying to establish is an absolute worst case should a US company take any legal action against us given that:

- The service would be hosted on servers in the UK or Ireland
- My company is UK based and I have no assets or interests in the US
- We would likely have US customers
- I would probably price in US dollars, but payment would be into UK bank accounts.

My research seems to suggest that the worst case would be a US company seeking some sort of restriction on us selling to the US. I'm not sure how that works given that the software would be hosted in the UK.

I realise that the folks on here aren't lawyers and that I should get one to be certain of any advice. However, any information or would be helpful at this point.

Edit: To clarify, these are US patents. I know of no global, EU or UK patents that are relevant to me. Furthermore, my understanding is that software cannot be patented in the UK and EU


## Answer 48953

- posted by: [drllau](https://stackexchange.com/users/-1/26055-drllau) on 2013-05-04
- score: 2

<p>Patents grant the inventor exclusive rights to manufacture, offer to sell, sell or use the invention in the jurisdiction of question. I refer you to the recent caselaw of <a href="http://law.justia.com/cases/federal/appellate-courts/cafc/09-1372/09-1372-2012-08-31.html" rel="nofollow">Akamai v Limelight</a> where a content distribution network (hearsay a variant of Squid proxy) was alleged infringed by a competiting offer which asked the users to perform a crucial subset. The judges rules that yes, there was infringement (that was split amongst the defendant and users) but left the open question whether LIABILTY was split. The Federal Circuit said that infringement may be induced (imagine being egged on by crack seller to buy across the street).</p>

<p>So this opens up a can of worms international jurisdiction-wise as some countries are liberal in software patents whereas others is not allowable patent subject matter (eg China). At worst, your patent heavy might sue your US customers. Now it may be a situation of FUD but as Kim DotCom shows, killing one monkey (whether legally or not) to scare a hundred works. </p>

<blockquote>
  <p>Furthermore, my understanding is that software cannot be patented in the UK and EU</p>
</blockquote>

<p>Unfortunately here I can tell you unambiguously that your understanding is misplaced. The EU patent law does not technically allow for software but the courts have allowed improvements of technical effect to be patentable. So a clever patent attorney can twist an instance into a class in such an obfuscated manner to pass muster in the european jurisdiction. So sorry, nobody is safe from patent trolls.</p>

<p>I'm sorry to say that the whole mess looks like unlike to come to any resolution in the near future (at least on international level). Even NZ which was supposed to be the first country to explicitly disallow software patents has had its <a href="http://nzoss.org.nz/content/no-software-patents-petition%E2%80%8E" rel="nofollow">wording weakened</a>. As Bismark noted, <strong>laws are like sausages, tis better not to see them being made</strong>. The good news is that the latest reading of the <a href="http://www.iitp.org.nz/newsletter/article/430" rel="nofollow">Patent Bill</a> clarified the issue. So depending on the architecture, a tactical location of some backend services may give you the <a href="http://www.wipo.int/sme/en/documents/freedom_to_operate.html" rel="nofollow">freedom to operate</a> as most patent trolls should find it rather difficult to finangle <a href="http://clendons.co.nz/protecting-ip-in-a-post-software-patent-environment.html" rel="nofollow">dubious</a> software patents.</p>

<p>The techno-legal problem is that you want the patent-infringement claim to fall on the NZ entity, and not the US/European/etc customer and to avoid the situation of induced infringement which potentially could still be liable. There are principles which can apply from (economic) tort in proximal causal event. The PaaS needs to be designed to issue letters of immunity so that the any potential claims fall within the NZ data jurisdiction (software patent equivalent of The LotR <a href="http://lotr.wikia.com/wiki/Battle_of_the_Black_Gate" rel="nofollow">Battle of Black Gate</a>).</p>



## Answer 47145

- posted by: [Yorick](https://stackexchange.com/users/-1/22512-yorick) on 2013-02-04
- score: -1

You are absolutely correct that you should consult an attorney for this question.

As you sense, the worst case scenario is costly and drawn-out litigation.  In assessing the risk of this, you might look at the following:

 - Is the patent holder a large multinational like Microsoft, Apple, or Google with a track record of aggressively enforcing patents?
 - Does the patent holder have corresponding patents in the UK & EU, or are their holdings limited to the US?
 - Because this is software, and you are familiar with the difference in UK/US patentability, is your product free-standing? how is it sold, and is it re-sold in the US? is it specific to certain hardware that may find itself in the US?
 - Have you analyzed the patents for validity, enforceability, and claim scope?
 - Do you have patents to offer a cross-license? (Maybe it does make sense to seek US patents on your software?)

As a start-up you have to pick what is important to you.  If your venture is small, maybe you can defer some patent-legal services.  The well-funded entities realise that the opposition is often greater than the execution in patent skirmishes.  When you do consult an attorney, try to find someone with US ITC experience if there is any concern about hardware with infringing software entering the US.  You can be in the clear, but customers being accused of infringement or having hardware seized at the border with your software will be bad for business.  Good luck.




## Answer 47146

- posted by: [royal1122](https://stackexchange.com/users/-1/17308-royal1122) on 2013-02-04
- score: -2

First of all, it depends whether the said patent is a US patent or a "Global" patent (there is not such thing as a global patent, you have to apply in each country that has a patent system). So if the said patent has been granted in UK as well, they can come after you easily.

However, if the patent is in US alone, they can sue you in a US court. You dont have to reply, and the court will most likely give them a judgement by default. Then comes the most difficult part (for them). They will have to get your domain-name banned in the USA, that is stop it from being accessed in the US. Its really difficult (maybe impossible) to get done, especially with the SOPA/PIPA stalled last year. There really is no other way for them to make you stop doing business in the US.




---

All content is licensed under the [CC BY-SA 3.0 license](https://creativecommons.org/licenses/by-sa/3.0/).
