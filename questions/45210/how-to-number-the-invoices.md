## How to number the invoices?

- posted by: [Nimbuz](https://stackexchange.com/users/-1/19209-nimbuz) on 2012-12-22
- tagged: `invoice`
- score: 2

I've always wondered how its done, is there a standard or just everyone does it randomly?

I thought this would be good:

 1. xxxxx (5 digits for client ID)
 2. xxxxxx (6 digits for DDMMYY)
 3. xxxxx (5 digits for number of invoices generated in a single day)

eg. 00001-221212-00001

.. but it gets too long, any way to reduce the length? should I convert it to hexadecimal? So `0000122121200001` becomes `1C6EFDA181`


Thanks


## Answer 45211

- posted by: [BrianAdkins](https://stackexchange.com/users/-1/21412-brianadkins) on 2012-12-22
- score: 4

I've never been a fan of trying to build smart numbering systems for things like invoices or part numbers.   It forces you to try to anticipate all your future requirements now and hope for the best.

For related idea in the world of part numbers, read the section titled "Significant numbering schemes are quite fragile
" here:
http://www.buyplm.com/plm-good-practice/part-numbering-system-software.aspx


In your example, you are limited to 99999 clients and they will probably not have more than one  invoice in a single day. This makes your proposal very inefficient and sparsely populated. 

Also, in a few years, you may wish that you had included something like "sub-client ID" in there. 

I'm a proponent of "dumb" numbering schemes...  Just pick a sequential integer series and pull from that pool. 

You may wish to prepend a prefix such as "MCX-" for "my company x" to assist your clients in recognizing invoice numbers that belong to you. 

You could also include a check digit at the end, to decrease the probability of Mis-typing a real invoice number... Or you could simply increment your integer series by a number greater than 1 (such as 19). These methods will 'waste' numbers and be less efficient, but have other benefits. 




## Answer 45216

- posted by: [Rob](https://stackexchange.com/users/-1/22129-rob) on 2012-12-22
- score: 3

In formal invoicing system design, they generally argue for sequential invoice numbers. It facilitates an additional audit checkpoint, where you can easily identify missing invoices. Generally you need to have an integrated mechanism to ensure that someone in receivables dept isn't deleting invoices and pocketing money.

I'd suggest simple sequential number, which is the standard mechanism of most invoicing systems.

Having said that, as a small business, it's a little annoying to provide your customer a way of determining how many invoices you're cutting per month. So I've seen people employ a "customer id"-"invoice number" scheme. I really disagree with the notion of putting the date in there, though.


## Answer 45212

- posted by: [Jiří Pospíšil](https://stackexchange.com/users/-1/22213-ji-posp-il) on 2012-12-22
- score: 2

I think the most straightforward way of doing this is to just use number sequence starting at N. 

- You probably use an invoicing program anyway so you don't need to embed any information inside the invoice number - you can just look it up.
- It's much easier to type, imagine someone would enter this manually into a online banking application.


## Answer 45214

- posted by: [BMitch](https://stackexchange.com/users/-1/11142-bmitch) on 2012-12-22
- score: 0

I go with a "client id"-"sequential number" where the number of digits isn't fixed anywhere. This is as much for my internal organization (all contracts, invoices, etc have the client id and there's nothing restricting me from making the client id a project id instead, so the same client could potentially have a different number for each project).

This works for me, but I'm only sending out one invoice a month to one client at a time, and a larger scale operation would want to automate this with a single sequential number.


## Answer 45215

- posted by: [JeffO](https://stackexchange.com/users/-1/1796-jeffo) on 2012-12-22
- score: 0

I agree with the other answers. Computer applications and databases do a good job of assigning unique sequential numbers out of the box. Your system is going to require more coding, testing and user training than its worth not to mention changing the scheme in the future.

You do have to be careful with distributed systems that may have some disconnect, but that is not a reason to put any "intelligence" in the PO number. At most you would just have different starting points for each location and enough room to prevent their numbers from realistically overlapping. Office A starts with 1000000 and Office B starts with 2000000 or something like that.


## Answer 45219

- posted by: [Gary E](https://stackexchange.com/users/-1/2587-gary-e) on 2012-12-22
- score: 0

Your scheme for numbering invoices is doomed to failure, so you might want to change it now.

1) Basing the invoice number on a client ID **limits** you to that system forever. What if you start selling retail software, or services to anonymous clients in the future? Or you exceed 5 digits worth of clients??

2) Encoding the date in your invoice number makes **no sense**. Invoices are legally required to have a date on them. Why would you repeat this information in the invoice number itself?

3) Now you are aiming for 99999 invoices in a single day???

The **vast majority** of all firms pick a starting number, and increment it after each invoice. This system allows you to track any invoice, and puts no limits on how or when invoices may be generated.




---

All content is licensed under the [CC BY-SA 3.0 license](https://creativecommons.org/licenses/by-sa/3.0/).
