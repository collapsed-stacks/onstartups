## Would users want name.mydomain.com/ or mydomain.com/name for their profile?

- posted by: [Community](https://stackexchange.com/users/-1/-1-community) on 2010-01-12
- tagged: `technical`
- score: 0

I'm building a myspace-like site for users and was wondering which method I should go with. I'm familiar with the SEO and technical aspects of a subdomain as opposed to a subdirectory setup. I'm basically wondering if users find username.mydomain.com/ for their profile page more attractive than mydomain.com/username. This would be a paysite, so I am trying to think of what's most attractive for users.

Any thoughts on this? If you want to remind me of the SEO/technical differences too, I'm all ears. :)

Thank YOU! 


## Answer 6376

- posted by: [Arkaaito](https://stackexchange.com/users/-1/2221-arkaaito) on 2010-01-12
- score: 2

For me, personally, it depends on whether there's one page or multiple pages.  If it's just a single profile page, mydomain.com/username.  If there are multiple pages, though, such as a blog and bio or bio and contribution statistics, I decidedly prefer username.mydomain.com unless there are non-user subdomains (e.g. meta.mydomain.com, guest.mydomain.com).

[Note: I'm giving you my take because I think I'm fairly representative, but I haven't performed market research to back up that conviction.]


## Answer 6379

- posted by: [apsurd](https://stackexchange.com/users/-1/2186-apsurd) on 2010-01-12
- score: 2

I can tell you from a performance standpoint, using subdomains is *slower* just because the dns lookup takes longer, since myname.yousite.com is not the same dns lookup as secondname.yoursite.com 
This is as opposed to if you only had yoursite.com, that lookup can be cached and would be faster. However I am no expert in dns so someone please correct me if I'm wrong.

One great reason to use subdomains is if you ever want to use domain mapping. That is if you ever want to allow your users to map domain names to their profiles. So rather than go to user.yoursite.com/coolpage, a user can map his domain to work like so : customdomain.com/coolpage which would work seamlessly on both ends. (which is very cool)

If you have no intention to offer custom domains, my advice would be to use yoursite.com/user because its easier to implement and because depending on your user demographic, not all people are accustomed to omitting "www" and entering a subdomain to access websites - it's just unatural.


## Answer 6382

- posted by: [ilker Aksu](https://stackexchange.com/users/-1/942-ilker-aksu) on 2010-01-12
- score: 2

Technically, If you allow user content on their pages  
subdomain.yoursite.com  is easier to isolate for security purposes.  
Cookies do not (so security token) span other users sites.





---

All content is licensed under the [CC BY-SA 3.0 license](https://creativecommons.org/licenses/by-sa/3.0/).
