## What are the details of a magStripe (on credit cards) read by ATMs to verify the card?

- posted by: [Hasitha](https://stackexchange.com/users/-1/27741-hasitha) on 2013-09-05
- tagged: `credit-cards`, `bank`, `validation`
- score: 0

I'm a developer, interested in developing a mobile app related to ATMs which would have virtual credit cards. I've been trying to find a way how card details are validated by ATMs, hence needed to know what are the details of a magnetic stripe that the ATM reads to validate the card. 
In the below link, I found that the POS terminal checks the record of the magnetic stripe for Merchant ID, Valid card number, Expiration date, Credit card limit and Card usage to vaidate the card >>  http://money.howstuffworks.com/personal-finance/debt-management/magnetic-stripe-credit-card1.htm

Could anyone please confirm if the ATM too checks only for the above details i found in the link? Else, what are the actual details of a magnetic-stripe of the credit-card that the ATM reads for validation?


## Answer 50799

- posted by: [Gary E](https://stackexchange.com/users/-1/2587-gary-e) on 2013-09-05
- score: 1

Either you did not read the details of your link thouroughly, or you don't understand what they mean. The magnetic stripe on a credit card or ATM card contains a **limited** amount of data. You can buy credit card readers for less than $50 and run your cards through to see what comes out. It is basically what is printed on the card, minus the security code.

The ATM **does not validate** anything. The ATM simply takes this information, along with a manually entered PIN number, and sends that information on to a merchant gateway. The merchant gateway routes the information to bank computers for that particular card. Algorithms at that computer determine whether or not the transaction should be accepted or denied, depending on the credit card holder's credit status, the location of the transaction, and special circumstances. So, for example, my ATM card will not normally work in China, but by calling my bank I can activate the ATM card in China for a specific period of time, and for specific maximum amounts.

The algorithms for validating a purchase vary by bank.




---

All content is licensed under the [CC BY-SA 3.0 license](https://creativecommons.org/licenses/by-sa/3.0/).
