## Automating Business Owner Validation/Verification

- posted by: [LocalPCGuy](https://stackexchange.com/users/-1/17633-localpcguy) on 2012-04-22
- tagged: `business`, `business-services`, `api`, `validation`
- score: -1

We are looking for a way to validate that the person who creates an account has the ability to speak for the business in question.  (Only U.S. based businesses for now.)  And we are looking for ways to automate this validation of the business/owner, so we do not have to manually authorize every account that is created.  We are looking for something that is simple for the business owner and as real-time as possible.

(Note: This is similar to [Business Owner Validation][1], but that does not address the process being automated.)

Ideas so far have been:

 - Compare the billing address on a credit card against the business address (fails in cases where an owner uses a PO Box, personal address or corporate address as the billing address instead of the business' address.)
 - Compare business address/name against database of U.S. businesses.  (Having a hard time finding a reliable source for that database, or a service that provides a way to validate against their database using an API.)
 - Validate the email address entered, must match URL of the website for the business (businesses may not have a website, easy to provide a fake email.)
 - Use an automated phone call to the phone number placed.  (fails because a false phone number could be used, business phone number may not be where the owner is (i.e. franchise store))
 - Send a post card with pin to the billing address (probably works, but is slow.  Chance that the post card is ignored or thrown away as junk mail by someone not expecting it.)

And of course the manual fallback of requiring the business owner to scan or send in proof of the business, in the form of a license or utility bill.  Requires manual approval and is slow.

Any other ideas we have missed?  Third party services that help automate any of the above ideas are very welcome as well, particularly ones that have an API that can be integrated directly into our service.  

PS. Please do not answer with "use Google Maps API."  It is against their terms to use the Maps API without displaying a map.  If all else fails, we may look into doing just that (validate against the Maps API and display the Google Map in the verification step) but would like to avoid that option for now.

  [1]: http://answers.onstartups.com/questions/10008/business-owner-validation "Business Owner Validation"


## Answer 38443

- posted by: [Gary E](https://stackexchange.com/users/-1/2587-gary-e) on 2012-04-23
- score: 2

Your first sentance, *"We are looking for a way to validate that the person who creates an account has the ability to speak for the business in question."* doesn't match **any** of the rest of the information in your question. You list five "ideas" and not one of those addresses the question, does this person have the legal authority to represent this particular business?

I hate to break the bad news but not only is there **no automated way** to do this, there is no universal way to do this by **manually**. This problem is actually composed of **several** individual problems. 

 1. Does person A have the legal authority to speak for company B?
 2. Is the person registering actual person A?
 3. Is this registration actually for company B?




---

All content is licensed under the [CC BY-SA 3.0 license](https://creativecommons.org/licenses/by-sa/3.0/).
