## What to consider when licensing source code

- posted by: [Paul Stovell](https://stackexchange.com/users/-1/13821-paul-stovell) on 2011-10-12
- tagged: `legal`, `pricing`, `license`
- score: 10

Component vendors like [Syncfusion][1] and [Infragistics][2] often make source code available to their customers (at an additional fee). Some benefits of this would appear to be:

 1. Enable customers to make changes they need
 2. Empower customers to find and fix issues, and even contribute the changes back
 3. Protect the customer in the case of the component vendor collapsing

Assuming there are benefits to a startup in licensing their source code, what needs to be considered? What general terms would you expect to see (a lawyer can help write it, but I'm looking for general points)?

For example, I would expect the customer has the right to:

 - Download, read, and modify the source code
 - Compile and make use of their own modifications
 - Distribute their changes in a compiled form
 - Take backups of the source code for their own use

The customer would probably *not* have the right to:

 - Distribute the source code to third parties
 - Use the source code to create a competing product
 - Receive any kind of support for their modifications (though questions are welcome)

What other rights/responsibilities should I consider when drafting a source code license?

Lastly, what information will I need from the customer? Should I insist on getting a full legal name and address, or is "bob@hotmail.com" still fine?

(This is related to [this question][3]. However, that question focuses on whether licensing source is a good idea. My question is: assuming it is a good idea, what are some of the details to consider?)


  [1]: http://www.syncfusion.com/sales/faq
  [2]: http://www.infragistics.com/products/license.aspx
  [3]: http://answers.onstartups.com/questions/17657/should-we-license-our-source-code


## Answer 31414

- posted by: [Robin Vessey](https://stackexchange.com/users/-1/984-robin-vessey) on 2011-10-13
- score: 5

**Key thing you missed for the agreement**.

They shouldn't be allowed to sell their new version of your code as an independant component, only within a larger project as a "building block". Otherwise, if I'm a component vendor, I can resell your stuff by changing a few property names and fixing a bug ... personally I don't think thats shouldn't be part of the rules. 

They can submit the change back to you and if you don't take it on you get the right to say "Yes they can or no they can redistribute" ... possibly you open a market place to allow them to resell their "flavour" of yours or something as a seperate business model. BUT get first right of refusal.

**The good and bad to consider**.

Bad points:

 - **Everyone can see how you did it**. If its tricky or unique then you have given stuff away.
 - **You will be asked a million questions** about some decision you made that the average developer doesn't understand ... either setup a stackoverflow tag to answer them under like Xamerin (MonoTouch) do OR understand your potentially going to be stuck providing lots of support to the newbies.

Good points:

 - **Customers feel safer "taking the risk"** because its not a closed entity. Nothing worse than investing in a component that looks fantastic from a new vendor and 6 months later you discover that they got bored and no longer sell and support the component. This is one of the major barriers to entry for new players, selling the source is the key way of mitigating this problem.
 - **You get feedback and improvements from your customers**. If you in it for the long haul this is a key way to gain acceptance and win over people to talk about you "they included MY patch in their main product!!!", with a thankyou in the About page on the website this goes a long way both with product improvement and with marketing ground swell.
 - **You have an additional revenue stream** from selling the source code. 
 - **You could have an additional revenue stream** providing "support tickets" for newbies wanting to hassle you personally. Individuals aren't likely to pay but larger companies will pay to get the answer sorted and let them get on with the $2M project that is now running behind.

The component vendors generally aren't doing anything super special or tricky with their development, people pay because its hours they haven't had to spend themselves developing and debugging. If your stuff fits into this "save me time" catagory then your pretty safe that your not giving away anything. 

**Lastly the legal agreement**.

You want more detail because I can type in me@me.com and you have no idea who it was that just got the source code so you have no way of enforcing the agreement (thus may as well not have it). 

More importantly you want to ask for all their other details like country, name, company, EMAIL, etc for marketing and demographic understanding so that you know exactly who to target with advertising and who to contact again when you have "Awesome component #2" to sell. 



## Answer 50789

- posted by: [tyoc213](https://stackexchange.com/users/-1/14572-tyoc213) on 2013-09-04
- score: 0

Some links

http://choosealicense.com/ from https://help.github.com/articles/open-source-licensing

Another Good one http://www.codinghorror.com/blog/2007/04/pick-a-license-any-license.html a little less https://github.com/blog/1530-choosing-an-open-source-license and more linked to the github usage.

http://creativecommons.org/choose from creative commons 

http://www.oss-watch.ac.uk/resources/licdiff


Finally you need to learn about `copyright` and `intellectual property`... I think intellectual property gives you right to choose a license.

Also, see that you can dual license something if you are the "owner" or the original.


I HOPE someone clarify more on the last points about IP, copyright and dual, extra licensing and change from one type to another type of license when for example you have closed source and want to change to public, or that you have one license in your files and later you want to change it and so on.




---

All content is licensed under the [CC BY-SA 3.0 license](https://creativecommons.org/licenses/by-sa/3.0/).
