## Feedback on Build-Operate-Transfer Outsourcing Model

- posted by: [PhilR](https://stackexchange.com/users/-1/1612-philr) on 2009-12-11
- tagged: `outsourcing`
- score: 5

Our company is investigating a couple of outsourcing companies and operating models and one that we're starting to lean towards is the Build-Operate-Transfer (BOT) model with a firm that has some specific domain expertise we're looking for.

The model is that:

 - the outsourcing firm will establish a separate subsidiary for us focused on developing an aspect of our product
 - they will seed this company with engineers with domain expertise from their existing company
 - they will grow the company by recruiting new engineers and we will be involved in that recruiting process
 - they will operate the company for 12-24 months and bill at a fixed rate per engineer
 - we will then buy out the company from them at the end of the period at some predetermined fixed rate and take over operation of the company

The advantages for us are lower upfront costs as we build up our operations.

So I'm looking for general feedback from others on their experiences with this sort of model, what to look out for and what are some best practices.

Also I'm interested in any feedback on the financial aspects.

 - Should we expect (or push for) a reduced operating rate in the initial period since the expectation is that will be recouped when the operation is transfered?
 - What are typical models for the transfer price at the end of the operate period? Is it a simple multiple of engineering salaries?

Thanks

Phil


----------
*Jason and Shree, thank you for your answers. I'm replying to them here due to the comment length limitation*

Ultimately our goal is to have an offshore subsidiary as part of the global development team.  However in the early stages of the company we don't want the expense and hassle of establishing that subsidiary.  We do however want to leverage the cost advantages of an offshore team for a portion of our product.  We do only have one product but it's fairly large and we'll keep some of the key development in house but want to outsource other elements.

The concern I have had with traditional outsourcing relationships is that the team members may move around in the company or leave the company, one of the advantages of the BOT model is that we're building a team that will be become employees.  So we invest in building a team and eventually take over the operation of that team with this BOT model.

We are also looking at other options including a straight outsourcing model, starting the offshore company now (and looking at headhunting fees) etc but when this BOT model came up I saw that it had some attractive attributes but I didn't have any direct experience with it, hence the question to this community.

I have found that there are multiple firms that offer this model, so it doesn't appear to be that rare.  Here's a reference: [Build Operate Transfer: Tensilica’s Experience in Offshoring Engineering to India][1] and an [update][2] (pdf). 


  [1]: http://www.sourcingmag.com/content/c060320a.asp
  [2]: http://iis-db.stanford.edu/evnts/4587/Tensilica.pdf


## Answer 4932

- posted by: [Jason](https://stackexchange.com/users/-1/2-jason) on 2009-12-11
- score: 3

Although I tend to agree with Tim -- that this doesn't sound like a good model in the first place -- I'll try to answer your question.

I don't like the idea of you buying it back from them.  I don't see the point in this extra transaction -- they are consultants so why not just pay them as consultants where part of the contract is a "bonus" or something in lieu of purchase?  Stock purchases are complex, especially if this is international, so why bother?

I think you need to decide whether these guys are consultants or employees.  If they're consultants, they should be paid appropriately and there's no sense in more money later on.  If they're employees, why not just use a head-hunter willing to take a *delayed* fee?

One advantage is "seeding with developers with domain expertise," but this sounds fishy to me.  If by "domain" you just mean "familiar with the general technology," this isn't different from any other kind of hiring.  If you mean "familiar with our target market," I'm doubtful there's much truth to that.

To answer you last questions about typical models for initial rates and transfers, *this isn't typical* so I don't think there are normal best practices.  Surely there's another, simpler way to manage this.

Finally, to briefly argue my original point, what would prevent another consulting shop -- or them for that matter -- from knocking this off with their own "domain experts?"  I can see where this would work -- if the company's success is not dependent on the technology.  For example, anyone can knock off a basic Twitter, but it doesn't matter because Twitter has the eyeballs and everyone else has a chicken/egg problem.  If you're "in the drivers seat" in that sense, then I think this *does* make sense, except for the complex transfer stuff.


## Answer 5371

- posted by: [Ivan Paramonau](https://stackexchange.com/users/-1/2005-ivan-paramonau) on 2009-12-22
- score: 2

<p>The conclusion to which I arrived after my 10 yrs in (offshore) outsourcing business is this: outsourcing is like eating <a href="http://en.wikipedia.org/wiki/Fugu" rel="nofollow">fugu</a> - it may be delicious, but you better trust the chef. </p>

<p>So, here are my concerns about BOT model:</p>

<ul>
<li><p>what would make service provider be motivated to get the best talent for your project? If you are paying flat rate, with no incentives, it means you would perhaps be getting mediocre resources. </p></li>
<li><p>there is no labor market on Earth where you would be able to force employees not to leave. People need to be motivated not to. What would force service provider to represent your best interest with this regard? Stock options after 1-2 years isn't such a great incentive as it would mean service provider would also need to be passionate about project. Passion is found where providers are doing product development, not where they do the resource management.</p></li>
<li><p>After 12-24 hrs you will be on your own to get people attracted to you as employer. It takes deep market/culture understanding to cope with this challenge. </p></li>
<li><p>Offering the service provider stock options as the incentive for representing your best interest is double-edged sword. Imagine that other (or all) clients are doing the same. In this case, you are relying onto provider's judgment about potential of their clients when they prioritize who gets what resources... !!</p></li>
</ul>

<p>This said, about 'delicious' side of outsourcing:</p>

<ul>
<li><p>I would rather invest time &amp; money into building/setting up the development process, when you are not dependent on service provider. It means - you can pull your project out and switch horses any time.</p></li>
<li><p>Make sure not to step into service provider specific tools that you use. All repositories &amp; data ideally are easy to migrate</p></li>
<li><p>Don't create single points of failures. Means that no critical knowledge should reside in the hands of single person (what if he quits tomorrow?). </p></li>
<li><p>Make sure the code is properly documented so that knowledge transfer to new project members is piece of cake.</p></li>
<li><p>Test automation is key not to get dependent on QA. Even if some of the testers drops out, you would still have basic coverage.</p></li>
<li><p>Make sure that project management process is in pattern with industry standards. I would suggest Scrum as it seems to work best among agile approaches for outsourcing. </p></li>
<li><p>Team motivation does require your time. Weekly team demoes and discussions so everyone involved understands the business behind the project would help. But more important - engineers need the success stories and recognition. If you work on the project for 2 years in stealth mode, it kills people's inspiration. Engineers need shorter lead times. </p></li>
</ul>

<p>This way you would still be good on cost, would likely get much higher results, and also - not locked down to single service provider. </p>



## Answer 4933

- posted by: [Community](https://stackexchange.com/users/-1/-1-community) on 2009-12-11
- score: 1

I have seen similar models in other Domains, (Not in the product development though).

There are similarities to this model, with what most major companies do with their strategic investment groups, Where instead of diluting the brand name for failed products, they fund small firms to develop products and or markets for them, and support the operations as an external consulting company until the product is successful, and then Buy it out. In case the product fails to fill in the gap, they close down the operation. 


## Answer 6978

- posted by: [Community](https://stackexchange.com/users/-1/-1-community) on 2010-01-22
- score: 0

I just read about your concern on going forward with the BOT model. Per my understanding this is the best model when we talk about Outsourcing. To my knowledge the most important concern is the right Outsourcing partner. If you have the partner who takes up its job seriously and not just another contract then you would most likely have a successful subsidiary running in a years time in an offshore location.

Talking about BOT Model, I think it offers you the privilege of setting up a captive unit, with the added advantage of conserving initial investment and management effort and legal issues + protection of your Intellectual Property. All in all a very smart deal. Just be careful when choosing your partner in the Offshore location as that partner would be your representative in the Offshore location, so the right talent and right management would be in its hands.

Frankly am in favour of this model coz my company offers the same and I have made some good research on it and have not found flaws in the model as such apart from a couple of things mentioned above. 

All the best.

Regards,
Ridhima


## Answer 18612

- posted by: [Jeremy Parsons](https://stackexchange.com/users/-1/4291-jeremy-parsons) on 2011-01-06
- score: 0

Outsourcing boils down to a trade of risks and resources, and in the optimum case, all parties win, because

 - The risks are managed by the party that knows them better

 - Resources (time, money, people, expertise) are obtained and transferred efficiently

BOT outsourcing is a 'third way' to the classic build-or-buy choice for new operations, and works to the same endpoint - at completion, the operation is yours.

Your question is essentially about how relatively to weight the month-by-month payment for the build-operate phase and the completion payment for the transfer.

The way you've described things, the outsourcing company is going to seed the team. That suggests you will expect a relatively short time before you start to see the results you want. Let's say your endpoint is to get to 100 units of work per quarter by month 24, the profile might be something like this:

Q1=0 Q2=5 Q3=15 Q4=30 Q5=50 Q6=70 Q7=85 Q8=100 Q9=100 Q10=100

If you were doing the build yourself, you would either expect a long run-in - because you'd be feeling your way cautiously - or front-loaded costs - because you'd be investing in premium hires and top-end consultancy support in order to get started well. You have the domain expertise to know what you want by way of outputs and maybe 80% of your existing processes will be transferred. So the final transfer is going to be low risk for you - you will not be dependent on the outsourcer's expertise.

On that basis, I'd be going for the opposite answer than you've suggested - being prepared to pay more in that first year for the heavy lifting, and minimising the transfer price. That still gives you a far better cash flow, and it positions the provider premium against the risk you don't want to manage. 

Your way round - concentrating the premium at the end - would better-suited either to a situation where the value doesn't start to flow until towards the end of the project (which is common for a venture involving the first use of new technology), or in the case that the transfer itself is high risk (for instance, when expertise is concentrated in a few individuals). 


## Answer 18613

- posted by: [alphadogg](https://stackexchange.com/users/-1/3197-alphadogg) on 2011-01-06
- score: 0

<p>The two main problems with <strong>any</strong> offshoring model for startups:</p>

<ul>
<li>Any technology development is not just raw R&amp;D, but has to be closely integrated with the business. There are real-time, heavy pressures on agility and turn-arounds that make having your talent in-house and plugged into the "devil-in-details" of the business indispensable. Models change daily, markets shift, etc. Outsourcing places extra layers of roadblocks to making this a less painful thing. In large businesses where there are multiple layers of bureaucracy and things change more slowly, the overhead of outsourcing is lost in the miasma.</li>
<li>Offshoring rates are nowhere near as good as they used to be. To get quality offshore talent starts at least at $40/hr blended. Anything below has always been a crappy experience. Hiring a decent, in-house dev anywhere short of overblown places like Silicon Valley, should cost about as much. I discuss this and other ideas at length <a href="http://paultiseo.wordpress.com/2009/02/10/outsourced-or-in-house-developers/#comment-69" rel="nofollow">here</a>.</li>
</ul>

<p><em>"Should we expect (or push for) a reduced operating rate in the initial period since the expectation is that will be recouped when the operation is transfered?"</em></p>

<p>Well, if they are smart and if they give up something upfront, it has to have some extra payout on the end. That reduced operating rate is, in fact, an investment on their part.</p>

<p><em>"What are typical models for the transfer price at the end of the operate period? Is it a simple multiple of engineering salaries?"</em></p>

<p>I would ask a valuation expert familiar with this type of scenario.</p>



## Answer 18626

- posted by: [Jesper Mortensen](https://stackexchange.com/users/-1/1261-jesper-mortensen) on 2011-01-06
- score: 0

**The "Build-Operate-Transfer" model is valid enough.** Several of the outsourcing providers I've worked with in Ukraine state that they're open for this kind of arrangement.

That said, I have never been personally involved in any deals like this. My feeling is that companies who buy outsourced teams want reassurance that they can leave the outsourcing provider, if needed. Thus the providers say "Yeah, we can do that", but they don't really push forward on it -- if possible, they prefer to keep the regular outsourcing agreement going.

IMHO, if you're ready to consider outsourcing (and in general, I think outsourcing is often a bad fit for startups), then **it makes sense to pursue this**. If nothing else, it could be a way to get better deal terms on team transfer upon cancellation of the agreement. Try *very hard* to get deal terms which enable you to move your team away.

The default deal terms with most providers are that the team stays with the provider, and you're forbidden to hire any of them for 2 years after ending the outsourcing agreement. This effectively means that if you do great work on building and motivating a great team, then the provider 'controls' the deal, because you can't leave the provider without also losing your people.

Then, about actually *operating* a subsidiary in an overseas location yourself -- **I'm not too sure about that one**. I know what it takes to run a company in Ukraine, and the culture and procedures are massively different from my home country -- it's a lot of work to run a company there. Effectively, you will have to hire local management, and you'll be completely dependent on them -- if the overseas management wants to deceive you then they can. Don't underestimate what it requires to run a company in Ukraine, India, or wherever you're looking.





---

All content is licensed under the [CC BY-SA 3.0 license](https://creativecommons.org/licenses/by-sa/3.0/).
