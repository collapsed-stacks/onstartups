## Why do big internet companies need thousands of "engineers"?

- posted by: [Jason Glib](https://stackexchange.com/users/-1/6582-jason-glib) on 2011-01-14
- tagged: `development`
- score: 2

I'm just starting to learn rails myself but I was wondering why companies like FaceBook need 3000+ coders? 


## Answer 18960

- posted by: [Community](https://stackexchange.com/users/-1/-1-community) on 2011-01-14
- score: 3

Because they have hundred of projects.


## Answer 18971

- posted by: [Giles Thomas](https://stackexchange.com/users/-1/1547-giles-thomas) on 2011-01-14
- score: 3

A product like Facebook simply requires a lot of people to build and maintain.  Obviously you could create something that did a lot of similar stuff pretty quickly in Rails just with a couple of people, but there would be a phenomenal number of details that you'd miss out -- and it's those details that take up all the programmer time. 

A recent example from my own experience -- we've built an online spreadsheet; it took us a month or so to put together something that calculates stuff.  It's now taken another month *just to get copy and paste working*.  Other seemingly-minor UI things will probably also take huge amounts of time.

And on top of all that, there's scalability.  A site with 500 million users, all of whom need to see roughly the same view of your datastore, is incredibly hard to get right.


## Answer 18954

- posted by: [Tekhne](https://stackexchange.com/users/-1/6507-tekhne) on 2011-01-14
- score: 2

I think it's for two reasons: (1) enterprise "drag", and (2) a small start-up application doesn't nearly cover the scope of operations of a large company. By #1, I mean things like bureaucracy, largely mediocre performance from people, supporting crappy "enterprisey" internal systems like time tracking, etc. By #2, I mean all the thousands of little details that go into making a business really work: financials, performance metrics, monitoring systems, HR systems, and on and on and on.


## Answer 18947

- posted by: [Henry the Hengineer](https://stackexchange.com/users/-1/1692-henry-the-hengineer) on 2011-01-14
- score: 0

<p>Because they have investment $ to burn on lots of different projects. Small startups typically focus on one project and as task volume and diversity increases, more engineers (and types of engineers) are required to handle them. FB has come a long way since 2004. Why wouldn't they need lots and lots of engineers?</p>

<p>Btw, if you want to have an idea as to how many employees Facebook actually attempts to hire from overseas, see <a href="http://www.seravia.com/records/world/--facebook" rel="nofollow">Here</a>. These are based on official government filings. Salary info. and title variations are also available.</p>

<p>You can also find out more about the current facebook employee clime <a href="http://www.glassdoor.com/Overview/Working-at-Facebook-EI_IE40772.11,19.htm" rel="nofollow">Here</a>. Best way to answer your question is to look at job posting descriptions, find out what they're actually working on based on employee gossip, how software eng/coder positions are titled, and whether they are separated into different departments.</p>



## Answer 18990

- posted by: [adrianh](https://stackexchange.com/users/-1/4599-adrianh) on 2011-01-14
- score: 0

<p>Because it takes lots of engineering to keep a site as large as Facebook up and running :-)</p>

<p>This <a href="http://www.quora.com/Twitter-Inc-company/Why-does-Twitter-need-300-employees" rel="nofollow">response to Twitter's head</a> count by Jane Huang gives you some idea of the kind of things that need doing.</p>

<p>Think about operations for example. Facebook has over <a href="http://www.datacenterknowledge.com/archives/2009/10/13/facebook-now-has-30000-servers/" rel="nofollow"><em>30,000</em> servers to manage</a>. Think about the issues involved in supporting that many machines...</p>




---

All content is licensed under the [CC BY-SA 3.0 license](https://creativecommons.org/licenses/by-sa/3.0/).
