## Invoicing customers that pay with Paypal or Google Wallet

- posted by: [dev.e.loper](https://stackexchange.com/users/-1/14028-dev-e-loper) on 2012-11-25
- tagged: `payments`, `billing`, `paypal`, `invoice`
- score: 0

I have an online service for which customer subscribes and pays a monthly fee. They use Paypal or Google Wallet to make these payments. Customers are starting to ask for invoices. Is there a way for Paypal or Google Wallet to generate these invoices? Do I have to manually generate these invoices for customer (and if so, what is the standard template for invoices)?


## Answer 44610

- posted by: [Duncan Fairley](https://stackexchange.com/users/-1/21183-duncan-fairley) on 2012-11-30
- score: 2

<p>I don't have any experience with Google Wallet, but Paypal has invoices, yes. You can invoice customers manually, but that probably wouldn't work too well with your by-the-month billing. One option is to use their <a href="https://cms.paypal.com/cms_content/US/en_US/files/developer/PP_InvoicingAPIGuide.pdf" rel="nofollow">invoicing API</a>, which will generate the invoices programmatically. </p>




---

All content is licensed under the [CC BY-SA 3.0 license](https://creativecommons.org/licenses/by-sa/3.0/).
