## Protecting works for being able to prove later "I've done this on this date"

- posted by: [Grzegorz Wierzowiecki](https://stackexchange.com/users/-1/19173-grzegorz-wierzowiecki) on 2012-08-27
- tagged: `intellectual-property`, `copyright`
- score: 1

How to protect digitalized works for later prove we've had this and that on that date ?

Example: John Doe wants to protect his works on 2011 to be able to prove in future (let's say 2022) that he has done it in past (2011).

I've read somewhere here (I can't find post) an idea about putting things into external well dated repo, like [GitHub](http://github.com) (they offer paid private repos).

Do you think is it a good idea ?
(My feeling is about using at least two of such)

Maybe just checksums of works ?
(Using a few different checksum functions as checksum/hash function might be compromised in future, as it happened to md5)

Any other suggestions about respected services with dated logs, that might be used to prove your authorship for given date ?
Or maybe other ways of protection?


## Answer 41653

- posted by: [Faster Solutions](https://stackexchange.com/users/-1/19103-faster-solutions) on 2012-08-28
- score: 1

<p>If you want proof that you had item "A" at time "B" then your best bet is simply to hire a local lawyer.  You send them your copyrighted material and they take receipt of it and keep it in a safe location.  This covers off a number of points:</p>

<ul>
<li>Whomever you are using to prove your copyright needs to be impartial.  Family and friends don't count.</li>
<li>You'll want whomever keeps your copyrighted material to ensure that it doesn't get lost, burnt, etc.  Good lawyers who deal with this kind of thing will have this in place.</li>
</ul>

<p>There are also online providers for this kind of thing.  <a href="https://secure.copyrightservice.co.uk/" rel="nofollow">UKCS</a> provides this kind of service and I am sure there are other national providers.</p>

<p>If you want it done properly you'll need to pay out cash for this.</p>

<p>On the flip side, if you do find that someone is using your copyrighted material then, before you engage with them, get their documents/web-site/whatever notorised by a solicitor/lawyer.  This will provide independent evidence that you were having your copyright infringed in the event that they then change their documents/web-site/whatever in order to avoid further action.</p>

<p>Finally:  mailing stuff to yourself is basically worthless.  If you want it done properly involve a lawyer.</p>

<p>Edit:</p>

<p>You don't need to do this in every country for which you want to enforce copyright.  The reason you use a lawyer is to have someone impartial who will verify your copyright claim and provide evidence to substantiate it.  Obviously, you want to choose a lawyer from countries with strong legal systems (US, UK, Canada, etc) as these will hold more weight than countries where corruption is more of an issue (Nigeria, etc).</p>



## Answer 41673

- posted by: [Sachin Shekhar](https://stackexchange.com/users/-1/17838-sachin-shekhar) on 2012-08-29
- score: 1

Almost all major countries have `Copyright Act`. Contact local consultancies, lawyers etc. to know how to use it. Googling can also help.

There's no other more reliable way than legally copyright your work.

When it comes to GitHub type services, there's no guarantee that it'll survive by 2022 or not. Plus, an attack on their servers can screw things up silently.


## Answer 41679

- posted by: [kizzx2](https://stackexchange.com/users/-1/4628-kizzx2) on 2012-08-29
- score: 1

IANAL but IMO the technically robust way to do it would be to do [cryptographic timestamping](https://en.wikipedia.org/wiki/Trusted_timestamping).

As a first step you would create your own private key to sign the PDF file. You can prove originality of the file by proving that you possess the private key. To make it look more legitimate buy a key from "Root CAs" like Thawte, Comodo, VeriSign and friends.

So you would [pick a timestamping authority/service provider](http://google.com/search?q=timestamping+authority), send them the file (perhaps in PDF because many providers make timestamping PDFs really easy). You'll get back a file with the timestamped "certificate" in it. The cryptography will prove that you have created the contents in the PDF file at the stamped time (exact working mechanism in the Wikipedia link above).

Caveat: This cryto thing is as secure as the private key. So if your timestamping authority's private key or your own private key get stolen, one can question the validity of your claim.


## Answer 41918

- posted by: [Logan Besecker](https://stackexchange.com/users/-1/17539-logan-besecker) on 2012-09-11
- score: 0

If you live in the USA then this solution is cheap and pretty solid.  

You can print out your work / copy it and send it to yourself in the mail.  Once you receive the letter, don't open it until you need it!  Ideally you should print out another copy to keep with the letter (ie: paper clip the two together or keep them together in a file.)  Please note: the copy that is not mailed is just for self reference incase you forget what is inside it.

All letters/packages sent via the US postal service* are stamped with a date as well as which post office the letter was processed at.  Since the US postal service  is a federal organization, it carries a lot of weight in court.  Just make sure to seal the letter up nicely and keep it in a safe place until you need it.

*all letters and packages that I've seen from the US postal service anyway





---

All content is licensed under the [CC BY-SA 3.0 license](https://creativecommons.org/licenses/by-sa/3.0/).
