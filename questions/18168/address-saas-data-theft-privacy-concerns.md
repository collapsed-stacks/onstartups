## Address SAAS Data Theft/ Privacy concerns

- posted by: [Community](https://stackexchange.com/users/-1/-1-community) on 2010-12-23
- tagged: `legal`, `saas`, `privacy`, `data-protection`
- score: 3

We have a SAAS product for a specific industry where we host this application for multiple companies. Since they belong to the same industry one of the key concerns of my potential customers is the data theft or privacy. How can I alleviate these concerns? Any thoughts?

Additional information: 
We are using Amazon web-services as one of our first step to increase the confidence of our to-be customers. It is NOT technical issue but the potential damage I can do to them by selling their valuable client's data to their competitors. 

Again many thanks for your inputs so far.



## Answer 18174

- posted by: [Jetti](https://stackexchange.com/users/-1/5405-jetti) on 2010-12-23
- score: 3

Just go through how you have made your service secure and that it has been created in a way that only allows people to access their own accounts. If they have any individual questions beyond that, talk with them and let them know that their data is in safe hands.


## Answer 18183

- posted by: [Jesper Mortensen](https://stackexchange.com/users/-1/1261-jesper-mortensen) on 2010-12-23
- score: 1

<blockquote>
  <p>one of the key concerns of my potential customers is the data theft or privacy. How can I alleviate these concerns?</p>
</blockquote>

<p>Are you <em>certain</em> that it's a key concern? I ask because enterprise'y people often ask for all kinds of paperwork without really understanding it/needing it. If it's really a <em>key</em> concern, then IMHO you need to consider many things...</p>

<p><strong>On the IT / software side:</strong></p>

<ul>
<li><p>Consider perhaps not using common application development platforms, but using "accepted enterprise standards" like <a href="http://www.salesforce.com/platform/" rel="nofollow">Salesforce's Force platform</a>.</p></li>
<li><p><strong>Or</strong>, using common tools like SQL databases, but developing a true <a href="http://en.wikipedia.org/wiki/Multitenancy" rel="nofollow">multi-tenant data architecture</a>, and write a fancy whitepaper about the approach you're using. (Hard to do.)</p></li>
<li><p><strong>And/or</strong> offering a dedicated virtualized environment (one set of EC2 instances exclusively for use by one customer) (sell this as a very expensive add-on if at all possible).</p></li>
<li><p><strong>Additionally</strong>, write some nice whitepapers about your security audit methodology, certifications, etc. Maybe contract a small security audit company somewhere write an objective report on their findings on your architecture. In general, produce paper that shows compliance to industry standards.</p></li>
</ul>

<p><strong>On the people &amp; process side:</strong></p>

<ul>
<li><p>Clear confidentiality agreements with all employees and external temporary contractors. Make them really solid, and use a good lawyer.</p></li>
<li><p>A clear Privacy Policy and Terms of Service on your site. See the past answers here, fx <a href="http://answers.onstartups.com/users/1841/dana-shultz">Dana Shultz's answers</a>. These documents are important in a B2B setting, and getting them right is not trivial -- use a good lawyer.</p></li>
<li><p>Really design with security and data confidentiality in mind -- have a good process around security audits and architecture reviews.</p></li>
</ul>

<blockquote>
  <p>We are using Amazon web-services as one of our first step to increase the confidence of our to-be customers.</p>
</blockquote>

<p>Actually, I don't think that is a positive thing. There is lots and lots of confusion about what "the Cloud" is among my large-company friends. I would not disclose <em>how</em> my service is hosted, but instead focus on <em>methodologies</em> and <em>certifications</em> -- my own methodologies for security audits fx, and the hosting centers certifications (fx SAS 70). But don't take my word for this -- ask some potential customers of yours.</p>



## Answer 18176

- posted by: [Ricardo](https://stackexchange.com/users/-1/42-ricardo) on 2010-12-23
- score: 0

I agree with Jetti. It would also help if you are using a reliable hosting/cloud provider company such as Rackspace, Amazon or Microsoft (Azure) to host this SaaS application and all of the data. These companies have gone through a lot of time (and money) to make sure the data and servers are not compromised. 

So, even if yours is a startup, you can explain how all of the servers and data are very well protected (physically and electronically) by very high standards by the companies hosting the application and data. 

There is also the application security which Jetti already mentioned where you can describe how the data for each customer is kept private, etc...




## Answer 18182

- posted by: [jorgem](https://stackexchange.com/users/-1/180-jorgem) on 2010-12-23
- score: 0

<p>The solution you describe is also known as a multi-tenant, where multiple customers data is stored in one DB. There are a lot of benefits of this approach (one backup, less DB management, etc)</p>

<p>The big problem I have seen with this in the field is that if you have bugs in your SQL, it is quite easy for a SQL SELECT statement to pull multiple companies' data if you forget (or make a mistake) with the WHERE COMPANYID='xxx'. If you botch this, suddenly your customer may see ANOTHER customer's data on their screens. When this happens, customers freak out!</p>

<p>Similarly, if a hacker manages to perform a SQL injection attack, they may be able to see data for all customers, just by getting into your one database.</p>

<p>So, the alternative is to give each customer their own database. And connect to a different database depending on the company/customer that logs in. Then it is not possible to get data from ANOTHER company by accident. But it can be harder to manage. For example, there are often limits on the number of databases a single database server can handle.</p>

<p>So what to do? Most customers are not going to care that much, and if you do a great job, you'll never see a problem. If you are careful, a multi-tenant solution is easier to maintain and may be easier to develop.</p>

<p>I have also worked at companies where ONE customer was so picky that they required their own database -- even though the solution was multi-tenanted. And we did it for them to get the deal.</p>

<p>There are a lot of resources on this issue on the internet:</p>

<ul>
<li>Stack Overflow <a href="http://stackoverflow.com/questions/4115233/multiple-databases-vs-one-database-with-ids-used-to-separate-organizations">discussion</a></li>
<li>Joel Spolsky talked about it on his podcast <a href="https://stackoverflow.fogbugz.com/default.asp?W24218" rel="nofollow">here</a></li>
</ul>




---

All content is licensed under the [CC BY-SA 3.0 license](https://creativecommons.org/licenses/by-sa/3.0/).
