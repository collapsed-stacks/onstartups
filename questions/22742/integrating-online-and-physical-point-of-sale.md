## Integrating Online and Physical Point of Sale

- posted by: [michaelmichael](https://stackexchange.com/users/-1/9115-michaelmichael) on 2011-04-01
- tagged: `software`, `ecommerce`
- score: 0

Is there any robust software solution that could integrate an ecommerce site and a physical point of sale?

My father has an established small business in a specialized industry. He's asked me to help him design a website that would take his catalog online and allow orders through the website. I think this has great potential, as none of his competitors have anything similar.

My first hurdle is integrating a new online ordering/inventory management system with the existing one. He's using Sage Businessworks for inventory management, customer information, and point of sale. Businessworks has no API, and no way to write to the database except by using the application itself.

Is it preferable (or even tenable) to make the website order-taking process "manual", that is, the order is received, an employee confirms that stock is on-hand, and inputs the transaction through the existing point of sale and sends a confirmation email to the customer?


## Answer 27550

- posted by: [edralph](https://stackexchange.com/users/-1/9362-edralph) on 2011-07-15
- score: 1

<p><strong>Your first instinct to integrate with the existing order management system is spot on</strong>.  For truly joined up online/offline sales pipeline you do need your online orders coming into the same system that handles everything else.</p>

<p>You mention that SB doesn't have an API, but I think you can import orders into the system <a href="http://www.sagebusinessworks.com/Customer-Resources/Product-Information/~/media/Category/SageSolutions/BusinessWorks/Assets/Documents/Import_OEquote_so_V2011.pdf" rel="nofollow">via CSV files</a>.  If you can demonstrate that you can get an order into the system via a CSV file, you can then develop your online order system towards producing CSV files that get imported on a schedule into Sage.</p>

<p>When they get imported into Sage, make sure you flag them as online orders so you can do order reporting segmented by channel.</p>



## Answer 27548

- posted by: [ekalaivan](https://stackexchange.com/users/-1/11991-ekalaivan) on 2011-07-15
- score: 0

Have you researched Enstore and Checkout?  They are Mac-based retail store software and online store solution. 


## Answer 27554

- posted by: [rtacconi](https://stackexchange.com/users/-1/11992-rtacconi) on 2011-07-15
- score: -1

Ideally you should have the ecommerce managing everything and use the ecommerce's catalog even locally. This opens you to be dependent to the Internet connection you have: it must be reliable and have a backup link. I would not use a CSV file, it is primitive, old fashioned and unpractical. You should move Sage to another software of interact with its DB, with is not a good thing (and database should be access from only its own applicaiton). There are softwares managing POS, catalogs and ecommerce, have a look on Google.



---

All content is licensed under the [CC BY-SA 3.0 license](https://creativecommons.org/licenses/by-sa/3.0/).
