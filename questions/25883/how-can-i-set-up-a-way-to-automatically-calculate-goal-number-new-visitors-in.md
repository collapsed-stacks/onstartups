## How can I set up a way to automatically calculate (goal number/new visitors) in Google Analytics

- posted by: [ben](https://stackexchange.com/users/-1/10974-ben) on 2011-06-04
- tagged: `analytics`, `conversion`, `metrics`
- score: 1

I have set up a goal which will count the amount of sign ups I get on my site. I need to divide this number by the amount of new visitors in order to get my conversation rate.

From what I can tell, the goal result is

    number of times goal is reached/unique visitors

Is there a way to change it to

    number of times goal is reached/visitors who have never been to the site before

Is there a way to set this up so it is calculated automatically?



## Answer 33267

- posted by: [Joel Friedlaender](https://stackexchange.com/users/-1/5543-joel-friedlaender) on 2011-12-03
- score: 1

<p>You can do this with the advanced segments feature in Google Analytics.  Google Analytics will already show your conversion rate, it just won't show it for new visitors only.</p>

<ol>
<li><p>Click advanced segments at the top of the conversions page (this page is under conversions > goals > overview)</p></li>
<li><p>Click "New Visitors" in the advanced segments section (this will restrict to people's first visit)</p></li>
<li><p>Click apply</p></li>
</ol>

<p>You will now see the conversion information for new visitors only.</p>

<p><img src="http://i.stack.imgur.com/FnUtr.png" alt="Advanced Segments"></p>



## Answer 25926

- posted by: [Rafferty Pendery](https://stackexchange.com/users/-1/11003-rafferty-pendery) on 2011-06-05
- score: 0

No, you are not able to do this within Google Analytics. Here is a video that discusses setting it up and how it works. 

http://www.youtube.com/watch?v=cGqq4bvrxPU


## Answer 27150

- posted by: [Nitrous Cloud](https://stackexchange.com/users/-1/11720-nitrous-cloud) on 2011-07-05
- score: 0

<p>You list</p>

<p><em>number of times goal is reached/unique visitors</em></p>

<p><em>number of times goal is reached/visitors who have never been to the site before</em></p>

<p>However, isn't aren't "visitors who have never been to the site before" the same thing as "unique visitors"?</p>

<p>Other than that, Google Analytics doesn't really allow you to customize your results that much. You could utilize their <a href="http://code.google.com/apis/analytics/docs/" rel="nofollow">API</a>, and configure the outputs yourself. </p>




---

All content is licensed under the [CC BY-SA 3.0 license](https://creativecommons.org/licenses/by-sa/3.0/).
