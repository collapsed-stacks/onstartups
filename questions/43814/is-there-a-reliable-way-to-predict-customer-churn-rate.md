## Is there a reliable way to predict customer churn rate?

- posted by: [Mohammad Ali Akbari](https://stackexchange.com/users/-1/6717-mohammad-ali-akbari) on 2012-10-23
- tagged: `customers`, `statistics`, `forecast`
- score: 2

Recently, I heard about the concept of being able to predict customer churn as a way to avoid losing customers.

Is there a reliable way to predict customer churn rate?


## Answer 43825

- posted by: [Steve Jones](https://stackexchange.com/users/-1/12985-steve-jones) on 2012-10-24
- score: 3

It is possible to do this once you have a track record, or if you are in an established industry, but there is no way to do it otherwise.

If you need it for a business plan, then you'll have to take an educated guess, based upon your understanding of your market and your customers.


## Answer 45045

- posted by: [Jim Gray](https://stackexchange.com/users/-1/22047-jim-gray) on 2012-12-15
- score: 3

Modeling churn won't stop you losing customers, but it will give you more accurate information about what's happening, and it will help pinpoint when conditions improve or worsen. It will also give you a basis for doing experiments which try to improve your churn rate.

Here's a tiered approach to modeling churn.

0: For initial planning, assume 50%.<br />
1: Look at the monthly totals for signups vs. cancels vs. inactives (improvement: uses your data).<br />
2: Do regression analysis (improvement: better data + forecasting).<br />
3: Do cohort analysis (improvement: stop lumping together people with dissimilar behavior).

Regression analysis will attempt to model a generating function which underlies your data. Your customer data is assumed to follow the trend the function describes plus some noise. This gives you a clearer picture than looking at raw totals, plus you can do some forecasting by assuming that the trend will hold for some distance into the future.

Cohort analysis tries to break up your customer data into major clusters. This can be against any number of dimensions, e.g. join date, account type, customer demographic, tablet vs. smartphone vs. desktop, screen resolution - really, any dimension which provides a reasonably consistent segmentation result, and where the customer segments will have different responses to your products or marketing.


## Answer 45085

- posted by: [Varda Tirosh](https://stackexchange.com/users/-1/22134-varda-tirosh) on 2012-12-17
- score: 2

<p>You cannot avoid losing customers. There is a natural churn in every industry. However, churn prediction modeling can reliably indicate which individual customers are most likely to churn BEFORE they do – and thus take some action to try prevent it from happening. 
While most churn prediction approaches rely on static data and metrics, a more successful approach is based on dynamic micro-segmentation and monitoring of how customers migrate between micro-segments (based on changes in their behavior) before migrating to churn. This approach allows you to identify existing customers who are about to take the same route and thus churn. At this point, you can take action before they churn (e.g., send a particular offer or incentive that you know has worked in similar cases in the past for other customers). My startup’s founder has posted a detailed article on this approach – click <a href="http://www.optimove.com/churn-prediction-prevention.aspx" rel="nofollow">here</a> or search for Optimove churn prediction.</p>



## Answer 49806

- posted by: [Robert Graham](https://stackexchange.com/users/-1/26925-robert-graham) on 2013-07-07
- score: 0

<p><strong>Summary:</strong> You can predict churn rates and the most likely customers to churn on a month to month basis, but you need to collect data in order to make those predictions. Smaller customer bases and less mature businesses will experience larger swings in these numbers.</p>

<p>Predicting churn is distinct from predicting the churn rate of a business. The churn rate of your business is easier to track than predicting if a use will churn. You simply need historical data. The data will be more accurate if you are able to break the customers into meaningful segments or cohorts.</p>

<p>Early stage businesses with few customers or many new customers at once likely have higher churn and much higher variance in churn rates from month to month. At this stage, full churn prediction is likely over kill, but establishing a process for reaching out to churners and learning from them is critical.</p>

<p>Mature businesses with more established processes likely have very similar churn rates from month to month and know how customers churn from each cohort. This is a highly predictable stage and can benefit greatly from churn prediction.</p>

<p>I wrote a blog post that explains how <a href="http://whitetailsoftware.com/2013/03/how-to-predict-customer-churn-using-machine-learning/" rel="nofollow">predicting churners for next month</a> works at a high level. I would be happy to answer specific questions directly. I'm working on a <a href="http://keepify.com/announcements/2013/06/26/keepify/" rel="nofollow">startup</a> in this space myself.</p>




---

All content is licensed under the [CC BY-SA 3.0 license](https://creativecommons.org/licenses/by-sa/3.0/).
