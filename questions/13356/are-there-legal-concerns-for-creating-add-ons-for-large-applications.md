## Are there legal concerns for creating add ons for large applications?

- posted by: [Joe Doyle](https://stackexchange.com/users/-1/1601-joe-doyle) on 2010-08-10
- tagged: `legal`, `tools`
- score: 0

I know this is more of a legal/lawyer question, but I'm sure others have run across this at some point so any insight is helpful.

I'm looking to create a mISV which builds and sells add on tools for large enterprise applications. The products I want to work with don't have APIs for directly accessing information, but store the majority of their data in a SQL database, so it is visible without reverse-engineering formats. The companies that create these applications have partner programs, but they are only for sales channel relationships, not technical ones.

Are there issues with creating products that work with the large applications without establishing a relationship/partnership with the company first?

Microsoft doesn't seem to require any sort of partnership to create 3rd party tools for their products. Do other large companies allow the same thing (Oracle, EMC, Autonomy) or does it vary?



## Answer 13358

- posted by: [John Bogrand](https://stackexchange.com/users/-1/3577-john-bogrand) on 2010-08-10
- score: 2

So yes I’m not a lawyer, so prior to making a decision suggest getting appropriate legal counsel.
So based on the legal decision on jail breaking of the iphone (http://arstechnica.com/tech-policy/news/2010/07/apple-loses-big-in-drm-ruling-jailbreaks-are-fair-use.ars )as long as the code is owned and operated by the person you should be able to provide a way to modify what it does legally.  

Things to consider:
<li>Does the customer have a warranty with the underlying platform that the add-on change affect?  If it invalidates the warranty and something happens it may cost you customers and/or cause legal liability.  

<li>I’d also suggest consider the possible liability for breaking a standard functionality in the platform that your code is changing.

But I’d suggest that liability and legal issues you would have are very similar to creating any software product and are from the customer point of view.  You don’t have a legal issue with the platform company you’re using as a base as long as the customer is already paying license fees and such for it and you’re not imbedding code from it without permission and without the license being paid.



## Answer 13359

- posted by: [Dana Shultz](https://stackexchange.com/users/-1/1841-dana-shultz) on 2010-08-10
- score: 1

If I understand correctly, you want to write applications that access customers' SQL data.

The providers of the software that created the customer data have no rights to that data and, thus, cannot legally interfere with your using it.

Hope this answers your Q.

Disclaimer: This post does not constitute legal advice and does not establish an attorney-client relationship.



---

All content is licensed under the [CC BY-SA 3.0 license](https://creativecommons.org/licenses/by-sa/3.0/).
