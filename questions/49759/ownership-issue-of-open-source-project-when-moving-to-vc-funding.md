## Ownership Issue of Open Source project when moving to VC funding

- posted by: [Kim Prisin](https://stackexchange.com/users/-1/26877-kim-prisin) on 2013-07-03
- tagged: `legal`, `getting-started`, `open-source`
- score: 3

An open source project I designed & developed as my thesis in grad school has been continuing development through a non profit organization that hired me full time. Throughout my work there, I've continued to be the only designer and developer on the project.

I never signed a contract specifying the work I was doing is property of the non profit, but they have been paying for me to continue work on it. 

Now, there are potential VC investors that want to support the project, and I'm not sure if I want the non profit to be attached to the project, as their infrastructure has hindered the development so far (being extremely unorganized and slow moving).

Can I gracefully remove myself from the organization and move into a VC stage, even though they've funded my development for the past year? 


## Answer 49762

- posted by: [cdkMoose](https://stackexchange.com/users/-1/12756-cdkmoose) on 2013-07-03
- score: 3

IANAL, but absent details in a contract, this could get messy.  If you work for them, they pay you, and this is what you work on when you are at work, it seems they could make a strong case for at least partial ownership.  It would certainly be hard for you to say it's all yours when they have been the ones putting up the money.

I think you should contact a lawyer before you have any discussions with VCs.



## Answer 49765

- posted by: [CaseySoftware](https://stackexchange.com/users/-1/11314-caseysoftware) on 2013-07-04
- score: 1

Completely agreed with cdkMoose on this one, but to add to it..

If the code is GPL so you could take the code and fork it under a different name.. 
but you'll never be able to change to another license without getting sign off from all the copyright holders. Which leads back to the question of who owns the code you're writing.

If your contract/job description doesn't specify, it will probably fall back to the rules in your jurisdiction and whether you are an employee or a contractor. Anything "work for Hire" is the employer's by default.

Of course, if this is GPL 3 instead of GPL 2, it can get even more problematic.

I recently managed to relicense software from GPL 2 back to the BSD which it started under. It was *NOT FUN* and took multiple years. If you go that direction, my posts might help you:

The how: http://web2project.net/2011/01/web2project-license-change/

The why: http://web2project.net/2013/06/why-would-we-re-license-web2project/


## Answer 49768

- posted by: [Christian](https://stackexchange.com/users/-1/9952-christian) on 2013-07-04
- score: 1

<p>If you have signed something which gives the non-profit distribution rights to your code, they can distribute it as they wish. I believe a working contract has the same function. You cannot easily change the license from GPL to another, as they have a word to say here. This is my understanding, but you should definitely contact a lawyer and ask if you, has the guy with the intellectuel property, can take the code and relicense it.</p>

<p>In theory, if you have the IP, <a href="http://www.gnu.org/licenses/gpl-faq.html#ReleaseUnderGPLAndNF" rel="nofollow">you can use the code in non free programms</a>. But your lawyer must tell you if you still have the IP.</p>

<p>If you can't relicense it, you are bound to the same terms as everybody else. Speak, GPL. You are able to fork the code to f. e. GitHub and work further, But you need to make the source code available for free. Please note, this does not necessary mean "downloadable for everyone". But it does mean, if your customer/user asks for the code, he needs to be able to get it.</p>

<p>Please see: <a href="http://www.gnu.org/licenses/gpl-faq.html#GPLRequireSourcePostedPublic" rel="nofollow">does the GPL required that sc ... be posted to the public</a></p>

<p>There are certain "options" in the GPL, which make it almost impossible to get the code. For example, you had once to pay for xt:commerce download. Please note, not for the software, just for the download (bandwith) etc. Also please be aware, when I faced this before ages, I was really upset. And the GPL allowed to redistribute the code. Plenty other people uploaded the package to various webspaces.</p>

<p>Please see: <a href="http://www.gnu.org/licenses/gpl-faq.html#DoesTheGPLAllowMoney" rel="nofollow">does the GPL allow me to sell copies of the program</a></p>

<p>The GPL is not permissive when you extend the software. But you might find an option to "not link" to the GPLed code. I mean, your business could develop a GPLed software. In addition it could develop some other software which uses, but doesn't link to the GPLed software. There are some cirstumances when it is allowed to build non-gpled sowftware along with GPLed. This is a bit cumbersome, but possible. <a href="http://www.gnu.org/licenses/gpl-faq.html#GPLInProprietarySystem" rel="nofollow">Please read details in the FAQ</a>.</p>

<p>Finally I would like to say that "Open Source Software" can be a business model. Look at Red Hat. They distribute GPL'ed software, but their main income is the service around it. </p>

<p>Look at <a href="http://zurmo.org" rel="nofollow">Zurmo</a> a smaller company. Their software is free, but they provide a SaaS and of course services.</p>

<p>I find the "using the GPL" option much better than to mess with IP and lawyers. If you have the option to work along with what you have now, I would do that.</p>

<p>I believe if you have an clue about the GPL things and can explain the pros and the cons properly to your investor, you might come up with an interesting business model which is attracting to him. I don't consider "open source" a blocker. I write a lot of Open Source myself, because i see business chance in here. The only difference is, I use the Apache License which is ways more permissive (please note, there is a can of worms if you open the discussion which license is better - leave it close, for the sake of a healthy mind).</p>




---

All content is licensed under the [CC BY-SA 3.0 license](https://creativecommons.org/licenses/by-sa/3.0/).
