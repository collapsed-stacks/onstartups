## User account management

- posted by: [Alex](https://stackexchange.com/users/-1/2543-alex) on 2010-05-26
- tagged: `tools`
- score: 1

Is there a simple user account management tool?  
An table: username, encrypted password, name. And an embeddable form to fill and update the password. 

Our potential users aren't tech savvy enough to use OpenId.  
There is no database so far and it's much easier for us to keep it this way. 

If this is a bad idea, please tell me why.

Thanks!  
Alex


## Answer 11530

- posted by: [Jesper Mortensen](https://stackexchange.com/users/-1/1261-jesper-mortensen) on 2010-05-26
- score: 1

<p>You could try to ask this question on Stackoverflow.com (with more information); maybe they can think of something better.</p>

<p>Assuming we're talking about a web application, you could use something like <a href="https://rpxnow.com/" rel="nofollow">RPX</a> (a hosted user authentication service), <a href="http://www.facebook.com/advertising/?connect" rel="nofollow">Facebook Connect</a>, or Microsoft's Live ID.</p>

<p>On .NET something like <a href="http://www.dotnetinvoice.com" rel="nofollow">Dot Net Invoice</a> could be helpful -- but it's way overkill for simple user authentication, and it probably requires a database.</p>

<p>Just about every modern web application framework should make user accounts <a href="http://docs.djangoproject.com/en/dev/topics/auth/" rel="nofollow">simple to implement</a>. And for most web frameworks you can find <a href="http://github.com/jongeorge1/Who-Can-Help-Me" rel="nofollow">sample applications</a>, from which you can more or less copy'n'paste a working accounts and permissions system. People generally use SQL databases for this kind of stuff, because they are a good solution to this problem.</p>

<p>Personally, I would never outsource user accounts to something like RPX. Users are your company's life and blood, and creating your own user account system is simple. Risking that some users don't understand the login process and abandon the site simply isn't worth it.</p>

<p>If my app was deeply integrated with Facebook, Microsoft Live, or some other large online world, then I would utilize the platforms user authentication <em>to make things easier for the end users</em>. If my app was strongly oriented towards geeks and Internet-sawwy people, then I might use a combination of self-hosted authentication and OpenID, because <a href="http://serverfault.com/questions/23429/is-open-id-better-than-the-usual-login-system">some of those users prefer OpenID</a>. In all other situations I would use a self-hosted, inhouse developed user management &amp; permissions system, based on email address &amp; password, because that's what most non-technical users know and expect.</p>




---

All content is licensed under the [CC BY-SA 3.0 license](https://creativecommons.org/licenses/by-sa/3.0/).
