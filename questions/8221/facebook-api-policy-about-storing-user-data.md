## Facebook API policy about storing user data

- posted by: [Michal Slocinski](https://stackexchange.com/users/-1/1732-michal-slocinski) on 2010-02-19
- tagged: `facebook`, `api`, `terms-and-conditions`
- score: 3

recently more and more apps appear that retrieve data from Facebook and store it in some form for further processing purposes.

Examples:

 - www.joelonsoftware.com/items/2010/02/18.html
 - www.flowtown.com
   
I have also idea for an application / service that would use Facebook API in similar way but during analysis phase I came across Facebook platform API policy page (http://developers.facebook.com/policy/) which says:

> You must not store or cache any data
> you receive from us for more than 24
> hours unless doing so is permitted by
> the offline exception, or that data is
> explicitly designated as Storable
> Data.

Of course - I've no idea how in reality 2 products above work internally, perhaps they refresh data they receive from Facebook every 24 hours but I do have some doubts about it. I expect that from purely engineering point of view, refreshing data for potentially hundreds of thousands or even millions of accounts is too complex process that would require significant amount of processing power.

I'm stuck at the moment because I've an idea which I believe is good one, but I don't want to invest my time in something that is not 100% crystal clear and legal. 

Another thing is that relying on any such free API is in general very risky since terms and conditions may change over night. 

Do you have any thoughts on this? Is there any legal way around this policy?


## Answer 8227

- posted by: [Jacob](https://stackexchange.com/users/-1/2355-jacob) on 2010-02-19
- score: 2

<p>The "Stored Data" page from the Facebook developers wiki has some more information on what data can be stored indefinitely. You'll have to Google that since I'm a new user and can only post one link... I am not a lawyer, but it seems that anything other than this data must be purged after 24 hours. </p>

<p>According to the "Stored Data" section on <a href="http://wiki.developers.facebook.com/index.php/Random%5Fquestions" rel="nofollow">this page</a> the best way around this is to use infinite sessions and refresh the data every &lt; 24 hours. It does seem like this would be a performance issue if you have a lot of data stored, but to stay legal it sounds like this is the route you must take.</p>



## Answer 20242

- posted by: [Community](https://stackexchange.com/users/-1/-1-community) on 2011-02-14
- score: 0

I've read all the forums, and the facebook developer policy and did not succeed in finding the answer to this simple questions:

1.    "How long can we persist user information such as name, surname and picture in our database?"

2.    "Provided that our application currently requests offline_access permission, how long can we persist user information such as name, surname and picture in our database?"

Thank you in advance, all your help will be highly appreciated.

Regards,
Marian



---

All content is licensed under the [CC BY-SA 3.0 license](https://creativecommons.org/licenses/by-sa/3.0/).
