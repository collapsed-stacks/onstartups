## Legal or Ethical Responsibility to Safely Store Passwords

- posted by: [Yuck](https://stackexchange.com/users/-1/11398-yuck) on 2011-11-23
- tagged: `legal`, `security`, `privacy`
- score: 9

I'm working as a technical advisor to a start-up company. The company licenses its product (a web and mobile application) to large groups of people who then use it for a relatively short period of time.

As part of my technical review I noticed that the development team is storing user credentials in **clear text**. I immediately advised my client of this and recommended that passwords be encrypted securely using any of a number of well-documented best practices.

It turns out that the software has a few features that would be considerably difficult - although not impossible - to implement without having access to the raw password. One example is printing "user passes" that have a user name and password on them for easy access to the system. I've also advised against this practice, but let's for the moment assume I'm going to lose that battle.

My concern for my client is that a number of things could happen with this information that may result in litigation troubles.

* A disgruntled employee may leave the company and easily export this information before doing so. It doesn't help that the development works remotely in another country and can be difficult to supervise.
* Since user account names are email addresses, it's possible for some users of the system to utilize a common password across all their accounts. This would be an easy attack vector to script and try to gain access to email accounts, and in turn much more sensitive information.
* I believe that by now most users of web applications have some implicit trust in administrators to keep their private information securely stored.

Ethical issues are, sadly, less of a concern here at the moment. What immediate **legal responsibility** does my client have when it comes to this?


## Answer 32920

- posted by: [Keith DeLong](https://stackexchange.com/users/-1/888-keith-delong) on 2011-11-23
- score: 6

It's an ethical, legal and liability issue. 

Since a password is by nature a security precaution, it's perfectly proper for users to assume the developer/distributor used reasonable techniques to ensure customer security. Knowledge of the dangers (and poor practice) of storing clear text passwords -- and a failure to act on this knowledge -- is unethical. 

It opens the door to accusations of negligence and financial liability if users suffer loss (or are even exposed to the risk of loss) by this negligence. 

IANAL. I'd get a legal opinion on your responsibilities. 



## Answer 32924

- posted by: [Jesper Mortensen](https://stackexchange.com/users/-1/1261-jesper-mortensen) on 2011-11-23
- score: 5

<p>To answer definitively is hard, because laws are different from country to country, and with global Internet services it's often unclear which country is the governing one.</p>

<p>It can be a contractual issue, for example with the credit card / payments providers. The  <a href="http://selfservice.kb.net/display/2n/_index1.aspx?tab=faq&amp;r=0.3188623" rel="nofollow">PCI Data Security Standard</a> can be kind of vague and hard to follow, but <a href="https://www.pcisecuritystandards.org/pdfs/navigating_pci_dss_v1-1.pdf" rel="nofollow">section 8.4 is generally taken to mandate encrypted storage of all passwords</a> including end-user passwords.</p>

<p>It's absolutely a <strong>potential customer trust / basic competency issue.</strong> We know humans re-use passwords, so the potential negative consequences for your users if you're breached are severe. Password hashing has been debated over and over, and competent developers know that hashing passwords is common best practice. (By the way, the commonly recommended password hash algorithms are <a href="http://security.stackexchange.com/questions/211/how-to-securely-hash-passwords">bcrypt or PBKDF2-SHA256, or possibly scrypt</a>)</p>

<p>It's absolutely a <strong>potential major publicity / marketing issue.</strong> If your database is hacked and plain-text passwords are stolen, then you're pretty much <strong>guaranteed</strong> to get very very bad publicity. There have been <a href="https://encrypted.google.com/search?sourceid=chrome&amp;ie=UTF-8&amp;q=passwords%20stolen" rel="nofollow">many cases over the years</a>, and in most cases mass media picks up on the story and end users are enraged.</p>

<blockquote>
  <p>What immediate legal responsibility does my client have</p>
</blockquote>

<p>For that kind of assessment you'd need to see a qualified lawyer, and to be clear about where you're incorporated, where your servers are located, and where your users are located. But if your customers are spread out over the world, then <em>it's probably cheaper to just follow accepted best practice and hash passwords with bcrypt/PBKDF2, than to obtain a full legal analysis</em>.</p>



## Answer 32943

- posted by: [Gary E](https://stackexchange.com/users/-1/2587-gary-e) on 2011-11-23
- score: 2

<p>You need to point your client to the Sony security breach and the thousands of lawsuits that followed (and are still on going). Here's just one example of a class action lawsuit:</p>

<p><a href="http://www.gamerslawsuit.com/?gclid=CJm--5fozawCFQrHKgodIn3hpg" rel="nofollow">Motley Rice LLC</a></p>

<p>Can your client afford to defend against something like this? If not, they need to follow <strong>current</strong> standard security practices. That means they <strong>NEVER</strong> store a password, either in the clear or encrytped. You store only a salted hash of the password. If that makes your companies software work incorreclty, your company needs to change its software, or the way it operates.</p>



## Answer 32946

- posted by: [maple_shaft](https://stackexchange.com/users/-1/14070-maple-shaft) on 2011-11-24
- score: 2

**There is no justifiable business reason** for anybody to know the password to a user account except for the user himself.  That is the point of a password, it is his/her little secret.

If the user forgets their password then have them reset it.  If the administrators need to know the password to obtain software access to the account, then that is a **serious and gross negligence** of the software design.

And it goes beyond being ethically and morally repugnant and grossly negligent, it is also a major legal liability.  While it may not be a criminal offense in all regions, it certainly is justifiable grounds for civil suits as the damage this can do to a user is potentially catastrophic.


## Answer 32919

- posted by: [fobo](https://stackexchange.com/users/-1/14484-fobo) on 2011-11-23
- score: 1

<p>I heard in some jurisdictions (France?) companies have a legal responsibility to store unobfuscated personal details of their users to be used by state institutions (like law enforcement) when necessary.</p>

<p>YMMV</p>

<p>Yea, here you go:</p>

<p><a href="http://www.techdirt.com/articles/20110303/03520213350/france-goes-overboard-data-retention-wants-user-passwords-retained.shtml#comments" rel="nofollow">France Goes Overboard In Data Retention: Wants User Passwords Retained</a></p>



## Answer 32926

- posted by: [maciej](https://stackexchange.com/users/-1/14311-maciej) on 2011-11-23
- score: 1

Legal issues usually deal with personally identifiable information. Can you identify a person by looking at their password? No. So it is more of a ethical problem. However, does having someone's password lead to personal information? then it is a legal problem as well. 
But like Jesper said, why not cover all ends: 1) encrypt all you user data, personally identifiable or not, 2) keep personal and non-personal data on separate db servers (so hacking one does not automatically gives them everything), etc. etc



---

All content is licensed under the [CC BY-SA 3.0 license](https://creativecommons.org/licenses/by-sa/3.0/).
