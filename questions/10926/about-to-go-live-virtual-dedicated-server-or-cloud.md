## About to go live: virtual dedicated server or cloud?

- posted by: [morpheous](https://stackexchange.com/users/-1/3365-morpheous) on 2010-05-07
- tagged: `hosting`
- score: 3

I am about to launch my startup company, and we will be going live in a few weeks time. We have really tight budgetary constraints, since we are bootstrapping - and would prefer not to raise external capital.

I cant use shared hosting because I need more control of the server machine (for technical reasons - e.g. using proprietary extensions to PHP, Apache and in the database layer as well) - but want to control costs and dont want to go fully private server route, until we have determined the market size etc. So the only real alternatives AFAIK is between virtual server and the cloud.

At the moment, cloud services seem a bit "vague" to me. My understanding is that they allow an entity to outsource its IT infrastructure, which in my mind (at least), is indistinguishable from what a hosting provider provides (at least from a functional point of view) - I would like to seek some clarification on exactly what the difference between the two is.

Back to my original question, my requirements are:

1. IT infrastructure that can scale with growth
2. Ability to have control of the machine (for e.g. to install our internally developed libraries etc)
3. Backup software that is flexible and comprehensive enough (yet simple to use), that allows a (secured) backup strategy to be implemented. On this issue, I have always wondered where the actual backed up data was stored (since the physical machines are remote, and one cant get access to any actual tapes etc backed onto). I would also like some advice and recommendations in this area. Regarding data size, I am expecting the dataset to be increasing by a few megabytes of data (originally, say 10Mb, in about a years time, possibly 50Mb) every day.

As an aside, I have decided to deploy on a Debian server (most of my additional libraries etc were compiled and built on a Debian machine).

Mindful of all of the above, I would like some advice (and reason) as to which route to take. I would also like some advice on which backup software to use, from people who have walked a similar path.


## Answer 10929

- posted by: [Jesper Mortensen](https://stackexchange.com/users/-1/1261-jesper-mortensen) on 2010-05-07
- score: 3

<p>and welcome to this site! :-)</p>

<blockquote>
  <p>cloud ... is indistinguishable from what a hosting provider provides (at least from a functional point of view)</p>
</blockquote>

<p>Not quite. A cloud provider sells you virtual machines to install you code on, just like a conventional hosting provider does. Beyond that, a cloud provider IMHO delivers:</p>

<ol>
<li>Assurances that you can instantiate 'any number' of virtual machines at any time, i.e. there is no upper ceiling on how much capacity you can get how quickly. This has a dramatic impact; it allows you to match your infrastructure to <em>observed current load</em>, not <em>expected near-future load</em>. And this saves you capital costs, and confers scaling agility.</li>
<li>Storage APIs that are highly scalable cf <a href="http://www.julianbrowne.com/article/viewer/brewers-cap-theorem" rel="nofollow">Brewer's CAP theorem</a>. Storage is stateful, and hence storage is always where scalability problems are the hardest, and a cloud computing provider should have something to ease that pain -- Amazon Simple DB, Simple Queue Service, etc.</li>
<li>Network level services &amp; system administration tools to help with horizontal scalability, such as load balancing.</li>
</ol>

<p><strong>My regular advice in this situation is to start small, and not start scaling before you have a proven need for scaling, i.e. you're getting many customers signing up.</strong> So I'd initially suggest a good Debian based VPS (fx Linode.com), and then migrating to a fast single server, and then cloud computing. This advice is based on the <strong>assumption</strong> that your organic growth will be really slow at first, that it takes many months for you to build up a sizable user base -- this is almost always true, but examine this assumption yourself.</p>



## Answer 15461

- posted by: [Ian Purton](https://stackexchange.com/users/-1/4942-ian-purton) on 2010-10-22
- score: 0

I would recommend you jump to cloud hosting. These days it is very cheap if you know where to look. The two providers I'm considering for my startup are vps.net and www.stormondemand.com

Why, well both offer the ability to add more processing and memory at very reasonable rates very quickly.

Debian is a good choice, but the one I thing I wish had done when I started to commission my server is to use Puppet http://www.debian-administration.org/articles/526. This allows you to configure your server via a script.

Hope this helps.





---

All content is licensed under the [CC BY-SA 3.0 license](https://creativecommons.org/licenses/by-sa/3.0/).
