## Windows VPS on Amazon EC2

- posted by: [Puneet Gangal](https://stackexchange.com/users/-1/439-puneet-gangal) on 2010-04-18
- tagged: `hosting`
- score: 0

For you all Amazon EC2 experts out there, I have a question. In looking through Amazon EC2 documentation, I see that you can have a Windows Server machine with 1.7GB RAM, 1 EC2 core CPU, 160 GB disk space (aka Small Instance), and if you choose a Reserved Instance, you pay $227 plus 0.05 per hour, which is about $36 a month if it runs 24/7. Am I missing something, or signing up like that will give me a fully functional Windows Server VM (a VPS) on Amazon EC2. It does say, they will allow you to install SQL Express. I am evaluating this for a client, and I am thinking this may actually work (at $55/month factoring in the one-time fee), this may be a good solution to have a Windows Server VM to host a web app. or Am I missing something? 


## Answer 10357

- posted by: [Community](https://stackexchange.com/users/-1/-1-community) on 2010-04-18
- score: 1

We have exactly that instance running SQL server. Yep, sounds exactly right. You'll just have a typical dedicated server on EC2. watch out for SMTP issues and SSL issues if you need either. Both down to 'elastic' IP address that some mail servers confuse for dynamic IP.  


## Answer 10529

- posted by: [Community](https://stackexchange.com/users/-1/-1-community) on 2010-04-23
- score: 0

<p>You can have usual instance where data will be lost at instance termination. But you can attach EBS volume to it, so data that are stored at EBS volume will not be lost and you can reattach it to another instance.</p>

<p>Or you can boot instance from EBS. So in addition to terminate you will have ability to stop it (without any data lost) and start again from this point. But you will have to pay for stopped instance as for EBS volume in any case.</p>

<p>So I think first option is cheaper and can save you from data lost.</p>

<p>By the way, if you are developing in Visual Studio you can find this addin useful <a href="http://www.ec2studio.com" rel="nofollow">www.ec2studio.com</a>. It allows to manage EC2 directly from Visual Studio.</p>



## Answer 10530

- posted by: [Jesper Mortensen](https://stackexchange.com/users/-1/1261-jesper-mortensen) on 2010-04-23
- score: 0

<p>Good answers already. But while there are quite many webapp entrepreneurs here, you might get better answers at the Amazon AWS forums.</p>

<blockquote>
  <p>good solution to have a Windows Server VM to host a web app</p>
</blockquote>

<p>Yes, that's what it is intended for. And while Windows on EC2 is not the most common combination (Linux is far more prevalent), I still guess enough people use this for it to be well debugged and stable.</p>

<p>You should also check out <a href="http://www.microsoft.com/windowsazure/windowsazure/" rel="nofollow">Windows Azure</a>; the .NET optimized cloud computing initiative from Microsoft.</p>

<p>If you decide to go with Amazon EC2, then keep in mind that the server VM's may crash at any time, and (from reports on their forums) typically do disappear a handful of times over a year. IMHO that implies two things:</p>

<ol>
<li>You need proactive monitoring like <a href="http://aws.amazon.com/cloudwatch/" rel="nofollow">Cloudwatch</a> or <a href="https://www.scalr.net/login.php" rel="nofollow">SCALR</a> or similar.</li>
<li>While you <em>could</em> keep persistent data on a EBS volume, it's not exactly great. For example, after a VM crash, you may have to script re-attaching the EBS volume to your new VM, and running consistency checks on the DB files on the EBS from within your database engine. This could work, but EC2 is really more set up for keeping persistent data away from EC2, i.e. keeping persistent data inside Amazon SimpleDB or RDS exclusively.</li>
</ol>




---

All content is licensed under the [CC BY-SA 3.0 license](https://creativecommons.org/licenses/by-sa/3.0/).
