## How to trust my developers?

- posted by: [kavoir.com](https://stackexchange.com/users/-1/18378-kavoir-com) on 2012-06-13
- tagged: `trust`
- score: 3

Is there any usable mechanism to ensure I can trust my developers so that they can't do anything stealthily harmful to my product / business in the code? Such as changing my PayPal email to his or redirecting my customers to his website?

They work full-time for me.

Does PayPal has any such features or do I have to come up with something on my own to make sure of this?

Any ideas or insights would be very much appreciated.


## Answer 39898

- posted by: [NetTecture](https://stackexchange.com/users/-1/3350-nettecture) on 2012-06-13
- score: 5

> Is there any usable mechanism to ensure I can trust my developers so that they can't do anything 
> stealthily harmful to my product / business in the code?

No. There are hundreds of things that all help a little, but they will cost you.

> such as changing my PayPal email to his or redirecting my customers to his website?

Developers shouldn't have access to the website in production. They develop and test, then hand that over to the administrative team. You do have an administrative team with full security clearance and background check in place? However, that is where the "cost" factor comes in.

Developers need a copy of the database? Well, cleanse it from all information insecure - can happen automatic once there is a program for that written (costs). Stuff like randomizing names and credit card numbers, etc. Or have the developers well under contract -legally, NDA, background check. That happened in my last consulting job, we got fully checked to see the real time operations database. Randomizing and cleaning will greatly cost you, though. 

Paylap - sure. Why should they not work against a second paypal account with corporate credit cards to test? 

At the end it is a cost issue. Suing people and checking their background are the best options, plus, as I said, separating development from operations. However, this costs quite a lot. Every code should be reviewed by 2 independant - possibly external - parties. I was in one project where this happened - full code review on every release by an external auditor. 



## Answer 39900

- posted by: [Christian](https://stackexchange.com/users/-1/9952-christian) on 2012-06-13
- score: 4

In case you do not have the money for two separate teams like "Operations" and "Devs" or in case you are looking into the "DevOps" thing:

- if you have more than one developer, give root access to the production machine to the ones your trust much. The root machine were your app resides is the most problematic place in your setup, because a developer could replace your code with his

- make up an intrusion detection system. This is not only good for nasty devs, it is also good for external hackers. IDS can detect if somebody breaks into your system  and changes things. Give this access to another developer who has NO access to the website on the same machine. If you don't want the complexity, you could try to make up an cronjob which checks your delivery packages with an MD5 string or something like that on a regular basis (minutes or so).

- make deployments in pear review only. Two devs deploy to production: one does the website stuff, the other one reconfigures the intrusion detection system (with a new MD5). this way the two devs will control themselves. Chances are very low that both are corrupt. 

With this easy steps you could make your deployment more safe. If the MD5 is wrong, your IDs should send an email that your jar is corrupt. Probably the IDS should make a copy of the deliverables to another folder which is not accessible for the website for a root cause analysis.

In addition:

- every committer with access to the machine has his own login (not shared login credentials)

- send yourself a logfile with the last logins each day (there are tools for it)

- ask the developers for an automated report of sales from your system and compare it with your paypal account

More tips for developing:

People could code corrupt code and just commit it to the source base as it would be regular.

- Make regular peer reviews on a regular basis. This also helps to keep your code clean.

- Make up commit notifications (somebody does commit code - an email with the changes to every dev goes out).

Well, that all should help you until you have a huge team :-) In any case, whatever you do, keep in mind **everything** can be hacked. The best is, you just employ people you really trust.



## Answer 39906

- posted by: [jsz](https://stackexchange.com/users/-1/13035-jsz) on 2012-06-13
- score: 2

Yes there is. And it's pretty straight forward: Pay them enough.


## Answer 39920

- posted by: [kalingga](https://stackexchange.com/users/-1/10666-kalingga) on 2012-06-14
- score: 1

Technical way would be a good idea. But basically to trust your developers, I would suggest you to have better relationship with your developers. Trust which is built on day by day activity is more solid. Having more interactions with your developers would make you better in knowing them, their characters, their ability, their visions, and etc. And they will know you better. If they know you better, and feel aligned by your visions or having same passion with you, it will give you positive impact to your business.


## Answer 39922

- posted by: [Global nomad](https://stackexchange.com/users/-1/8622-global-nomad) on 2012-06-14
- score: 0

(Since this hasn't been mentioned in answers so far)

 - You can learn to program yourself. Then you can verify what the   
   "maybe untrustworthy" developers are doing.
 - You can persuade a technical co-founder (who then is able to verify
   the developers' work). But then how do you trust your technical
   co-founder?



## Answer 39981

- posted by: [Wolf5370](https://stackexchange.com/users/-1/18438-wolf5370) on 2012-06-17
- score: 0

The developers should not be directly touching production until delivery time. Delivery packages can be protected and checks (such as hashes) can ensure the code does not change between development and delivery. Checks can be made on the delivery packages (code to be delivered). The cost of a security team to check can be factored in if you can afford it - it can be worthwhile.
Certainly have all code QA's before delivery. Do not give the paypal details out, make that change yourself on the delivery day - don't hard code such things, put them where they are secure and can be set by you easily. 
Be careful who you allow access to production - allow temporary access during delivery and remove it afterwards.
Finally (or should be initially) hire people that have a good rep and work history (check refs). Most developers are not thieves, they earn too much to rick losing the rep that will carry them from job to job to bother with changing PayPal accounts (which will be found out and traced very quickly - which they know) - if its an audit trail for a major investment bank then worry, otherwise, be wise in hiring and diligent during delivery.



---

All content is licensed under the [CC BY-SA 3.0 license](https://creativecommons.org/licenses/by-sa/3.0/).
