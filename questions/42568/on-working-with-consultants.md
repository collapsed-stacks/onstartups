## On working with consultants

- posted by: [Charles Martin](https://stackexchange.com/users/-1/20101-charles-martin) on 2012-10-11
- tagged: `intellectual-property`, `contract`, `consulting`, `legal-documents`
- score: 2

I have been asked by many startups to help them with their core machine learning IP

Unlike outsourced software development, machine learning is difficult to outsource or even to specify because it requires working deeply with the company data and product to invent trade secrets and even patents for the firm

There are very few machine learning professionals in the industry and the work does require experience and usually a PhD.  

This raises the price and makes the contracts more complicated 

What kind of contractual relationship would be ideal for both the startup to retain their IP and for the consultant to work with 2 or more clients at the same time, and over a period of time

That is, what is the best way for the firm to be sure their trade secrets wont be revealed, but also allows the consultant to work with his/her own developer stock of code and algorithms in order to solve related mathematical problems




## Answer 42583

- posted by: [Andrew Smith](https://stackexchange.com/users/-1/18504-andrew-smith) on 2012-10-12
- score: 1

Of course you can supply test data. It's also not a rocket science.

For example, consider simple learning machine, which is categorizing email as spam or ham.

Normally developer has to make classifying engine, and for this, he can use a set of any generic email messages, and use them to train the engine.

This way, he splits his own email into two parts - ham and spam, and trains the engine, hence he can fully make it.

Then, he can install it on the mail server, and it will just work, so he doesnt need to actually look into emails, because his engine is learned, and it will self-learn over time from just this base data.

You can also obfuscate the data, and make the engine to be user-friendly with user based training.



---

All content is licensed under the [CC BY-SA 3.0 license](https://creativecommons.org/licenses/by-sa/3.0/).
