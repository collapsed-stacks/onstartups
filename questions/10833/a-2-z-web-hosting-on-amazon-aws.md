## A-2-Z web hosting on Amazon AWS

- posted by: [JDelage](https://stackexchange.com/users/-1/2505-jdelage) on 2010-05-03
- tagged: `website`, `hosting`, `beginning`
- score: 1

All,

I am studying web dvp, and one of my classes is project-based.  We have to build a functional site that demonstrate our understanding of:

- HTML,  
- CSS,  
- Javascript,  
- php,  
- MySQL,  
- And potentially Ajax or some other web component.
    
For the project, we can use a local server using WampServer and basically build the site entirely on our laptop.  However I would like to create a real site, and I thought it would be a good way to familiarize myself with Amazon's AWS services.  So if I purchase a domain name, can I rely on AWS to host the site from A-t-Z?  I understand I can use AWS to host content, the database, and do the background computations, if needed.  What are the parts that AWS cannot help me with?

Second, is there good documentation for a beginner to navigate AWS and learn how to use it (either on Amazon, or some 3rd party sites, or even a good book, as long as is up to date).  The ideal documentation would be a tutorial on creating a web site from a-to-z on AWS, as detailed as possible.

As you can guess, I have limited understanding of the IT issues.  I hope you can help me.

Thank you,

JDelage

PS:  Please keep the answers AWS-specific.  At this point, I am only interested in alternative services to the extent that they plug a hole in Amazon's offering.




## Answer 10840

- posted by: [Jesper Mortensen](https://stackexchange.com/users/-1/1261-jesper-mortensen) on 2010-05-03
- score: 3

<blockquote>
  <p>can I rely on AWS to host the site from A-t-Z? [...] What are the parts that AWS cannot help me with?</p>
</blockquote>

<p>As you present your case, AWS can host all that you need. There are no parts pertaining to <em>running</em> your site that AWS can't help you with. However, you need to <strong>install</strong> operating systems, install web servers, SQL database servers et cetera; and you need to <strong>develop</strong> your site, i.e. create the HTML / CSS / PHP etc.</p>

<blockquote>
  <p>good documentation for a beginner to navigate AWS and learn how to use it</p>
</blockquote>

<p>Sure, the <a href="http://aws.amazon.com/" rel="nofollow">AWS site</a>, their developer center, and their public forums come to mind. There are books providing a more comprehensive coverage of AWS by now, but I don't have any recommendations. Try the AWS forums for book recommendations and tips about good starting points.</p>

<p>A side note: My experience at the university was that teachers wanted to see the <em>assignment</em> answered well, and did not care too much for non-curriculum extras. You might get a better grade if you stick to the assigned task, and do it very well.</p>



## Answer 10847

- posted by: [Andrew Watson](https://stackexchange.com/users/-1/1739-andrew-watson) on 2010-05-04
- score: 2

There are pre-built AWS EC2 "AMI" or machine images that already have all the software you need setup and configured.  You should use one of them (Fedora most likely) to minimize the amount of tweaking required to get up and running.



---

All content is licensed under the [CC BY-SA 3.0 license](https://creativecommons.org/licenses/by-sa/3.0/).
