## Adwords - Understanding Modified Broad Match Keywords

- posted by: [bcWeb](https://stackexchange.com/users/-1/21361-bcweb) on 2012-11-21
- tagged: `marketing`, `advertising`, `google`, `adwords`, `keywords`
- score: 1

I'm not completely new to Adwords optimization, but I guess the learning process never really ends...

My company is focused tightly on a specific niche.  All of my keywords (across several ad groups) are set using the modified broad match.  So for example, I'm entering all keywords like this:

+baseball +training +kids

I understand this means any query containing "baseball" AND "training" AND "kids" (in any order) will trigger my ad, which is good.

A few questions:

1.  Is there any clear benefit to using Phrase match ("baseball training for kids") or Exact match ([baseball training for kids]) over my modified broad match approach?  My thinking is I'll get more impressions using modified broad match.  

2.  What if I include BOTH Modified broad match and Phrase match keywords (using the same keywords) in the same group?  Will the Phrase match override the Modified Broad match?  For example... If I have both "baseball training for kids" and +baseball +training +kids, will my ad NOT trigger for the query: 'kids training in baseball' ?

3.  Does using Modified broad match have any impact on Quality Score?  I'm noticing my quality scores are quite low on my MBM keywords, despite having a tightly focused ad text matched with a highly relevant landing page containing those keywords.

I hope these questions aren't too far "in the weeds" for this forum... Just haven't found a reliable Q/A site for Adwords.


## Answer 44487

- posted by: [Mark](https://stackexchange.com/users/-1/21761-mark) on 2012-11-26
- score: 1

I think you are correct, you will surely get more impressions using modified broad match. It's good that you are not using exact match terms, as it will be hard to get impressions by it. Well, it might be possible that your quality score decreases, but it shouldn't bother you much after seeing the advantages. You may also try this link for knowing Adwords concept in a better way. http://www.dpfoc.com/blog/does-adwords-really-work


## Answer 44407

- posted by: [JonDiPietro](https://stackexchange.com/users/-1/11642-jondipietro) on 2012-11-21
- score: 0

You will definitely get more impressions with broad match than phrase or exact. However, the question is quality vs. quantity. If you're using the "right" phrase and exact match keywords, your overall cost per conversion will be lower (theoretically) because you won't have as many low quality impressions.

However, the way I approach this is not an either/or situation but a staged process:

 1. For a new campaign, I will start out with broad search and see what happens. You need to watch carefully and see what searches are generating impressions, click-throughs and conversions.
 2. As I'm watching the campaign, I will quickly look for dirty searches (ones that are obviously unrelated to my offer) and keep adding negative keywords. This will reduce impressions but increase click-trhough rate (and consequently, the quality score).
 3. Over time, I'll grab search phrases that are performing well and use them as phrase and/or exact match keywords for a completely separate ad campaign that is optimized for the phrase.

Here's how it would work using your example. I start out with +baseball +training +kids. As I watch the clicks roll in, I notice a bunch of searches for "potty training kids" so I add -potty as a negative keyword. I'll keep doing this for a while and maybe I see that the most common search is "baseball training camps for kids." So I'll create a whole new campaign with that exact match phrase with ads that use those words specifically.

If you run broad and exact/phrase at the same time in the same campaign, you won't really learn anything because the exact/phrase matches are a subset of the broad. In other words, a search for "baseball training for kids" will show up for +baseball +training +kids and [baseball training for kids] and "baseball training for kids". I use the broad match for research and the phrase/exact for optimization. Eventually, the broad searches tend to get shut off over time once you find phrases that work.



---

All content is licensed under the [CC BY-SA 3.0 license](https://creativecommons.org/licenses/by-sa/3.0/).
