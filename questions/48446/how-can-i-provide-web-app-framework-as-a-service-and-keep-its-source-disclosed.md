## How can I provide web app framework as a service and keep its source disclosed?

- posted by: [sawa](https://stackexchange.com/users/-1/25283-sawa) on 2013-04-08
- tagged: `webapp`, `platforms`
- score: 0

I am developing something like a web application framework in Ruby, and I want to turn that into a business. The application is provided as a single library, and can be used by simply `require`-ing it into the main file of the application. It does not require the application to be given in a fixed directory structure as in Ruby on Rails.

In what ways can I serve the framework to customers while keeping the source code disclosed? I think that obfuscation of Ruby code may be broken in a matter of time, so I do not want to distribute the source code directly to the customer. Rather, I am thinking of a PaaS business, where the customers can work on their application that uses the framework.

Which technical business models would work in this case?


## Answer 48455

- posted by: [Jesper Mortensen](https://stackexchange.com/users/-1/1261-jesper-mortensen) on 2013-04-08
- score: 5

<blockquote>
  <p>I am thinking of a PaaS business, where the customers can work on their application that uses the framework</p>
</blockquote>

<p>The problem with that is your customers would evaluate you on uptime track record, scalability, and vendor lock in risks. You'd need to handle all the concerns of a true PaaS platform like Amazon EC2 or Google App Engine. You could outsource some of that by running on top of EC2 like Heroku does -- but your customers would want to see a technical track record and depth of know-how similar to what Heroku has.</p>

<hr>

<p><a href="http://en.wikipedia.org/wiki/Interpreted_language">Ruby is an interpreted language</a>. Therefore it is not practically possible to prevent users of the library to access the source code.</p>

<p>Your two options are:</p>

<ul>
<li><p><strong>Handle it legally.</strong> Have a sufficiently clear, legally valid, and enforceable <a href="http://answers.onstartups.com/questions/tagged/terms-and-conditions">End User License Agreement or license contract</a> made by a good lawyer. And then rely on just the protection available to you by intellectual property laws.</p></li>
<li><p><strong>Turn it into a web service,</strong> i.e. JSON over HTTPS, as @SamerBechara already suggested. This way you'd have both intellectual property protection, and the very strong practical protection of the code running on your own servers, behind an API you can access control &amp; rate limit.</p></li>
</ul>

<p>My experience shows that plenty of software developers pirate their own software. It's more common the less wealthy a region is. Unless your software does something very unusual, or you know your customers very well. it's probably very unwise to just rely on copyright law.</p>



## Answer 48454

- posted by: [Samer Bechara](https://stackexchange.com/users/-1/25769-samer-bechara) on 2013-04-08
- score: 2

The only reliable way to not share your source code would be to create a client-server based API system, where you provide them with a file which just calls the methods on your own server. They will have access to the file's source code, but it will not matter, because it cannot work on its own. 



---

All content is licensed under the [CC BY-SA 3.0 license](https://creativecommons.org/licenses/by-sa/3.0/).
