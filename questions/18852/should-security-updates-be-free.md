## Should security updates be free?

- posted by: [Steve Hanov](https://stackexchange.com/users/-1/1958-steve-hanov) on 2011-01-12
- tagged: `pricing`, `security`
- score: 4

A customer has found a serious security flaw in my software, over a year after their support period has ended. Should I provide a free update?

The upgrade price is substantial, so I don't want to just give them the latest version with all its new features. But that means I have to back-port the fix into the ancient version they have.


## Answer 18856

- posted by: [Jesper Mortensen](https://stackexchange.com/users/-1/1261-jesper-mortensen) on 2011-01-12
- score: 10

**I assume your software is of a type were security is an important concern.** In general, I would say:

 - **Releases which *only* address security issues should be free.** There is an old culture of free security fixes in the IT community, and if you don't adhere to this, your reputation will suffer.

 - **It's OK to limit how far back you will backport security fixes.** But you should do so pro-actively by having a clear and understandable policy statement on your web page.

 - **Don't be stingy with free upgrades to people who have helped you.** Just keep a little quiet about it, so that other customers don't necessarily hear about it, and automatically expect the same. If it would be difficult to back-port the fix to the old version this customer is using, then just offer him a one-off free upgrade with your compliments. Gain one happy customer, and move on.


## Answer 18854

- posted by: [Henry the Hengineer](https://stackexchange.com/users/-1/1692-henry-the-hengineer) on 2011-01-12
- score: 6

Benefits of Free Update:
-One happy customer
-No time spent on backporting

Costs of Free Update:
-You miss out on $X (price of upgrade)


So it comes down to whether the amount of time you spend backporting is worth $X.


## Answer 18855

- posted by: [Rowland Shaw](https://stackexchange.com/users/-1/5652-rowland-shaw) on 2011-01-12
- score: 2

If your previous version is still a supported version (for any customer), then I would expect a vendor to offer the security fixed version to customers with a current support contract, and also the customer(s) that have reported the issue, as an act of good faith. If it would be possible to invest a little effort in giving them the latest version with the new features on a time limited trial for free, then that would be ideal, as they may even choose to upgrade

If that version is no longer supported, and the issue hadn't been found and resolved in a later version, I would consider offering some form of discounted upgrade deal (maybe give them 5 user licences free for the next version, or even a straight discount)

In either situation, customer satisfaction is key -- they've already helped you, so if they don't feel they get rewarded, they may spread bad feeling about your product (maybe in conversations with other vendors whilst looking to replace your product). 

It may also be worth reviewing your internal business processes to reduce the impact on reverse integrating later security fixes into earlier versions, and other aspects of configuration management that would allow you to build historical versions as well as current and future.


## Answer 18858

- posted by: [SmartCompanySoftware](https://stackexchange.com/users/-1/1629-smartcompanysoftware) on 2011-01-12
- score: 1

Do the right thing and keep your customer happy. You could offer them a discount on the upgrade or simply fix the security flaw and move on.


## Answer 18864

- posted by: [the dictator](https://stackexchange.com/users/-1/473-the-dictator) on 2011-01-12
- score: 1

Security updates should definitely be free. First of all it's quite bad that you have a security vulnerability, it's horrible if you can sleep well by knowing that you put your client in danger and left them like that unless they pay you (*If I were a client like that, I'd quite upset and in first possible instance would replace the software with a competitor*).

The problem of fixing an old version is hard, that's one of the reasons we charge clients mandatory support fee every year and give all updates for free, which saves us this headache.

If I were you I'd go back and fix that release and then inform all clients in that release about this update, also you might even convince some of them to update the latest version.

Don't ever even think about **not** informing all of your clients in that version because it's possible to wake up a morning and learn that 75% of your clients got mass-hacked in one night. That's not a good publicity.

*P.S. Assuming your old version is not too old, for example it's normal for MS to not release an important bug fix for Windows 95. I know it's a whole different game but still..* 


## Answer 18879

- posted by: [Leonardo Herrera](https://stackexchange.com/users/-1/4283-leonardo-herrera) on 2011-01-12
- score: 1

In short: **yes**.

The actual answer is that you **must**  keep a maintenance branch in your source repository for every major release, and better make sure it can be built. This way you can provide security or bug fixes to your existing customer base without giving away new versions to non-paying customers.

Always have in mind that non-paying customers are still customers!






## Answer 18859

- posted by: [ThomPete](https://stackexchange.com/users/-1/1186-thompete) on 2011-01-12
- score: 0

Depends on what you are selling of course. If you are selling Viral Killers then charging for upgrades is how you make your money.



---

All content is licensed under the [CC BY-SA 3.0 license](https://creativecommons.org/licenses/by-sa/3.0/).
