## Video hosting provider for commercial content - who is the best

- posted by: [Ev.](https://stackexchange.com/users/-1/2511-ev) on 2010-02-11
- tagged: `video`, `hosting`
- score: 6

I am looking to host some video for our startup. We will be recording screencasts, interviews, and a range of things. We would therefore like to be able to host video at a decent resolution, and some of the videos will be up to an hour in length. 

I notice that Vimeo doesn't allow commercial content. Viddler looks ideal but we would prefer something cheaper if it exists. 

Does anybody know of a good solution?

Thanks in advance!


## Answer 7949

- posted by: [Community](https://stackexchange.com/users/-1/-1-community) on 2010-02-11
- score: 5

We had the same issue at my company and ended up selecting Wistia. They do everything Vimeo do, but also provide great data on who has watched your videos and for how long. Their prices are reasonable but their service has been great - they helped us out with some issues we had and were very hands on. 


## Answer 8041

- posted by: [Community](https://stackexchange.com/users/-1/-1-community) on 2010-02-13
- score: 5

I came across this post and had to take a moment to rave about Wistia. 

Our company ***was*** using Vimeo HD for a little while to support a few product videos embedded on our site. We quickly learned though that Vimeo has an aversion to any business-oriented content on their site. Even though we were actively paying for their service, one day they sent us an email and gave us 24hrs to move our videos before they deleted them! No joke.

In our mad dash to find another reliable solution we evaluated Wistia, Viddler and a handful of others. After a few quick trials we decided on Wistia and haven't looked back. Overall it's a great service and here's a few of the things that have kept us happy:

 - Wistia's user interface / user experience is really fantastic. You can tell that a lot of love has gone into the product.
 - Their "heatmaps" feature is very slick and it's an extremely useful way to quickly evaluate how individual viewers are interacting with the product videos on our site. For the cost, you absolutely can't beat it.
 - They have a pretty powerful multi-level permissioning system that allows us to easily control who can see and manage entire groups of videos. This way we can let our employees manage their own project-specific videos (web meetings, tutorials, etc.) and keep them completely separate from the product promo videos that are streamed on our site.
 - Wistia has also recently added the ability to let regular Wistia users (all our employees in our example) to access the "embed" code to embed a video externally. (This used to be available only for Wistia 'managers'.) This small change enabled us to start using Wistia as the central video repository for our entire internal corporate wiki (powered by Atlassian's Confluence). This was a HUGE deal for us because before the change, we were always uploading massive internal corporate videos within our wiki which took forever and added stress to our server. Now anyone on our team can just grab the embed code from one of their project videos in Wistia, embed it on an internal wiki page, and play it right in-line along with their other internal project documentation. It's great!






## Answer 7955

- posted by: [Chris Boesing](https://stackexchange.com/users/-1/1452-chris-boesing) on 2010-02-11
- score: 1

<p>I have the same problem right now.<br />
The solution the highest on my list is buying a commercial license from <a href="http://flowplayer.org" rel="nofollow">FlowPlayer</a> and then put my videos on Amazon CloudFront or S3.<br />
The cost for flowplayer for a one-domain license would be 95USD and 0.150 USD for one GB data transfer would go to Amazon.<br />
The great thing with this solution is, that you don't have tiered pricing, so you only pay for what you need.
A problem with this solution of course is, that you don't get analytics.</p>



## Answer 7956

- posted by: [jimg](https://stackexchange.com/users/-1/2380-jimg) on 2010-02-11
- score: 0

<p>If you're a bit technical, have a PHP server, and have enough bandwidth, you can host the videos yourself and save some cash.  <a href="http://stream.xmoov.com/" rel="nofollow">http://stream.xmoov.com/</a><a href="http://stream.xmoov.com/" rel="nofollow">link text</a> has a php "http streaming" solution (one can argue whether this is a technically correct term, but it does work) that allows you to support a variety of video formats, including flash videos (fla's).  </p>

<p>Fla's encoded with meta information can support progressive downloads - which gives two benefits:</p>

<ul>
<li>you don't download the entire file for every viewer request (saves bandwidth)</li>
<li>the viewer can move the player forward at will (helpful in long videos - can select 30 minutes into a 1 hour movie without problems)</li>
</ul>

<p>Downside is that you don't have the video in a video social network, so others cannot discover it.  </p>

<p>Good luck!</p>



## Answer 14074

- posted by: [Community](https://stackexchange.com/users/-1/-1-community) on 2010-09-14
- score: 0

YouTube is by far the most widely indexed video hosting solution, even more so now that is owned by Google. However many consumers may not think the layout and ads are as pleasing as a clean "pay for" plan. One problem I have run into with my company is that YouTube doesn't allow you to precisely choose a thumbnail picture for your video. You can only choose from three random pictures selected automatically from your video. These frames used to be at precisely 25%, 50%, and 75% of the way through your video but now they are random.







---

All content is licensed under the [CC BY-SA 3.0 license](https://creativecommons.org/licenses/by-sa/3.0/).
