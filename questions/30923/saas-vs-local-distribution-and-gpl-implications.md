## SaaS vs local distribution and GPL implications

- posted by: [Mr. Schwabe](https://stackexchange.com/users/-1/5593-mr-schwabe) on 2011-10-02
- tagged: `saas`, `licensing`, `gpl`
- score: 0

Let's say our theoretical company has a SaaS product for which we charge $xx per month.   The product is entirely web based and the backend includes GPL code.

As I understand it, since our product is not actually "distributed" it is not bound by the GPL license.  

However, let's say some of our big clients are willing to pay top dollar for a local deployment that they can run within their own intranet.   We are in a position to do that for them.  Perhaps by preloading our product on a server workstation and physically shipping it to the client. 

Would GPL apply to this latter arrangement? Ie- would we have to provide the entire source code for our product? 


## Answer 30928

- posted by: [JohnGB](https://stackexchange.com/users/-1/9668-johngb) on 2011-10-02
- score: 2

GPL would still apply in your first case, it is just that the terms of it don't affect you very much.

The terms of GPL are that if you distribute the code, you have to make it freely available for others to build on - just as you have.  In the second case, you will legally have to release your source code and make it freely available.

It's the price you pay for free access to some awesome software.

Companies are (slowly) starting to accept the model of SaaS, and in some cases actually prefer it.  It is very likely that issues you face now with companies wanting a local deployment will not be there in a few years time.





## Answer 30992

- posted by: [romaninsh](https://stackexchange.com/users/-1/13659-romaninsh) on 2011-10-03
- score: 1

Unfortunately GPL means that you must pass the code along with your software. The company who received it can then distribute it further. You might try to sign an agreement to prevent this, but it would be the breach of GPL:

http://www.gnu.org/licenses/gpl-faq.html#DoesTheGPLAllowNDA

The best thing I can think of would be:

 - Extract GPL code from your code base
 - Write instructions for your client on how to install GPL product then integrate it with your commercial code.
 - Software running on Linux does not need to be GPL. Plugin running on wordpress does not need to be GPL. Interpretations here may vary.
 - You can build the solution on your client's behalf by combining components.

Depending on the type of your software this might or might not work.



---

All content is licensed under the [CC BY-SA 3.0 license](https://creativecommons.org/licenses/by-sa/3.0/).
