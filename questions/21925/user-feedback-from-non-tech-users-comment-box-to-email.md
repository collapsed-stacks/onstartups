## User feedback from non-tech users - comment box to email

- posted by: [tucson](https://stackexchange.com/users/-1/2407-tucson) on 2011-03-20
- tagged: `website`, `customer-feedback`
- score: 0

I would like to give my users a way to give me feedback on my website.
Users are non-technical.

I saw a simple comment box on this page at Olark:
[http://www.olark.com/developer][2]

![enter image description here][1]

It seems to be a DISQUS service, but I cannot figure out what service this is...

Would you have any recommendation for a comment box/form, with message going to an email address?


  [1]: http://i.stack.imgur.com/VmtAs.png
  [2]: http://www.olark.com/developer


## Answer 21938

- posted by: [Platinum Azure](https://stackexchange.com/users/-1/8767-platinum-azure) on 2011-03-21
- score: 1

You can have a form that posts an HTTP request to a server-side script (e.g., PHP, Rails controller action, Django request, etc.), which then sends an e-mail with the comment to a specific address that you put in the code or configuration.

You don't need to use DISQUS-- it's not that hard to roll your own if you're a programmer. (Of course, if you're not, you might want to learn that first or find someone who knows it!)



---

All content is licensed under the [CC BY-SA 3.0 license](https://creativecommons.org/licenses/by-sa/3.0/).
