## I want to make my new website open to public access, but

- posted by: [Community](https://stackexchange.com/users/-1/-1-community) on 2010-01-10
- tagged: `website`, `marketing`, `beta`
- score: 6

I have developed a website. On the one hand, I want people to know my website so I want to make the website open to public access, and on the other hand,I fear that my website is not secure enough, some hackers may crack my website, besides I have not created a formal "Terms of service". How can I deal with this issue?


## Answer 6267

- posted by: [Elie](https://stackexchange.com/users/-1/1752-elie) on 2010-01-10
- score: 4

<p>Considering there's no information about your website, you've made this particularly hard to answer.</p>

<p>First, you can create a rough draft of your Terms of Service by copying and modifying from some other site similar to your own that has a public TOS. </p>

<p>Second, before your site can get hacked, a hacker has to:</p>

<ol>
<li>Find your site</li>
<li>Decide it's worth hacking</li>
</ol>

<p>Now, without knowing what your site is, it makes it difficult to determine whether your site is worth hacking. Some things you should make sure you're doing are encrypting all sensitive data (if you're using PHP, salt and hash the data using the built-in MD5 function).</p>

<p>For more things to consider, look at <a href="http://stackoverflow.com/questions/72394/what-should-a-developer-know-before-building-a-public-web-site" rel="nofollow">this question on Stack Overflow</a> and the first answer.</p>



## Answer 6286

- posted by: [ConsultUtah](https://stackexchange.com/users/-1/567-consultutah) on 2010-01-11
- score: 2

<p>Here is a great start for your terms of service, [Automattic, the team behind wordpress, has placed][1] theirs under an acceptable license.</p>

<p>As for security, let's go over a few basics:</p>

<p> 1. Do you store credit card info?  If you do, do not pass go and do not collect $200, find a different way.  Very few companies are capable of properly storing credit card info.  
 2. Do you have users passwords in plaintext in your db. If you do, MD5 or better is your friend use it. 
 3. Does the site run on a server that has a firewall installed?
 4. If it is a vps, physical server etc, are all ports except 80 and possibly 443 blocked?
 5. In your coding, did you use parameterized queries?  If not, fix that code. 
 6. In your coding, do you sanitize everything passed to you from the web and HTML encode anything that the user might have entered that gets displayed in the HTML?  If not, fix it. 
 7. Are the passwords for admin logins relatively secure?  If not, fix it. </p>

<p>If you've got the bases above covered, you are better than a good portion of the web.  </p>

<p>Those are the most basic steps for determining if your site is ready to go up security wise.  </p>

<p> 
  [1]: <a href="http://en.wordpress.com/tos/" rel="nofollow">http://en.wordpress.com/tos/</a></p>




---

All content is licensed under the [CC BY-SA 3.0 license](https://creativecommons.org/licenses/by-sa/3.0/).
