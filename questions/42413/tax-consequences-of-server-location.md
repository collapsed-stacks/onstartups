## Tax consequences of server location

- posted by: [Yrlec](https://stackexchange.com/users/-1/8548-yrlec) on 2012-10-04
- tagged: `tax`, `usa`, `server`
- score: 1

We are about to set up our production environment in AWS and are wondering about the tax consequences of where the servers are located. We are a Swedish start-up and since AWS is cheapest in the US we'd love to place the servers there but we've heard that we might risk double taxation if we do that (i.e. both Sweden and the US will tax us).

Do you guys have any experience having the servers in the US for non-US start-ups?


## Answer 42414

- posted by: [littleadv](https://stackexchange.com/users/-1/13808-littleadv) on 2012-10-04
- score: 4

<p>Several links for you:</p>

<ol>
<li><a href="http://www.kpmginstitutes.com/taxwatch/insights/2012/pdf/state-taxation-cloud.pdf" rel="nofollow">KPMG Paper on (US) State taxation of cloud services</a>.</li>
<li><a href="http://www.cbiz.com/page.asp?pid=9313" rel="nofollow">CBIZ article on the same (which is shorter, but essentially repeats
the same as KPMG)</a>.</li>
<li><a href="http://www.portal.state.pa.us/portal/server.pt/document/1259986/sut-12-001_pdf" rel="nofollow">Pennsylvania State tax authority ruling on this issue re the
servers in PA</a>.</li>
</ol>

<p>Bottom line is that your concern is valid, and there are definitely potential tax pitfalls in this model. You should find a tax accountant who's specializing on this, and also look into the US-Sweden tax treaty to see if there's a clause that protects you in any way (there should definitely be a clause to avoid double taxation).</p>

<p>As you can see from the example  of the PA ruling, if your servers are in PA, you'll be required to collect sales taxes from users that reside in PA. That includes you (moot, since you're in Sweden), and your users (which you don't know where they are).</p>

<p>I would assume that the server providers (Amazon?) can help you with finding the information relevant to the State in which the servers would be located (maybe that particular state doesn't charge any taxes?). Re the US Federal taxes - as I said: tax accountant and the treaty.</p>




---

All content is licensed under the [CC BY-SA 3.0 license](https://creativecommons.org/licenses/by-sa/3.0/).
