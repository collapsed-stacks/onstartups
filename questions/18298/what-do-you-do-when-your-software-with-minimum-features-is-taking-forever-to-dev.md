## What do you do when your software with minimum features is taking forever to develop?

- posted by: [Kim Jong Woo](https://stackexchange.com/users/-1/3650-kim-jong-woo) on 2010-12-29
- tagged: `development`, `lean`
- score: 5

This will be tough to explain but....

What do you do when you are developing a software that needs to deal with large amount of variations of semi structured data from the web ? 

I told myself it was finished but today feeding it more random sample, it's failing however progress is being shown as more bugs are being fixed. 

I feel like I'm so close yet it also feels like every step forward results in two steps backward due to more bugs being discovered. I'm not trying to be a perfectionist but I feel that it needs to be able to deal with most variations in semi structured data to be useful to my future users.

I have gained strong interest from my past clients I worked for in this software but I feel that once they realize, they are having poor rate of success, I will lose them.

Mentors say that I should be releasing early and often in small increments. However, I feel that currently, my software is not able to even perform very well.

My patience is running out and I am being burnt out. I have been working on this software and researching for the past 2 years. My release date is late January but with the amount of bugs (caused by large variations in sample size) makes things difficult.

I'm not sure if I am expressing myself correctly but this software is not a typical CRM or simple game with clear cut features. This software function at it's minimum is to deal with large variations across semi structured data found on the web but to reach this goal seems to require much more testing and fixing.

Every bug I fix, does bring progress, but it just seems endless.

**UPDATE: Happy New Year ! Hi everyone, I realized why I was keep getting the same bugs. Problem is my algorithm overlooked a very simple parameter (one of the answers here gave me an idea). Thank you James. It makes perfect sense why I keep seeing the similar bugs over and over !
I wish there was a way to select more than one answer ! All of the answers here are equally great ! 


## Answer 18301

- posted by: [Susan Jones](https://stackexchange.com/users/-1/2737-susan-jones) on 2010-12-29
- score: 10

The lean startup model is fantastic and I support it wholeheartedly, but the truth is, it doesn't work for every type of business.

There are some business models where it is absolutely critical to your market to release a product that has a full feature set and a high accuracy.

It sounds like you need to take some time to get your head out of the coding and think about your software as a business. Is it critical to release with the degree of accuracy your gut is telling you? If so why? What will the impact on your customers be if the software isn't as accurate as you would like?

If a high degree of accuracy is imperative, maybe you need to look for angel funding to get to the point you need to before release. Not the lean startup model, but still a relevant one depending on what your business model is. 


## Answer 18300

- posted by: [Virtuosi Media](https://stackexchange.com/users/-1/3825-virtuosi-media) on 2010-12-29
- score: 7

Take a deep breath and hang in there. Every piece of software has bugs, so don't let them get you too frustrated. I'd recommend doing something like the following:

 - Prioritize your bugs in order of
   severity and importance to the main
   features of your software.
 - Fix the most mission critical bugs so
   that your main features are more or
   less stable.
 - As you fix each bug, write a unit
   test for it. It'll take a few extra
   minutes now, but it will save time
   and provide more stability for the
   future.
 - Don't necessarily worry too much
   about non-mission-critical bugs. If
   it doesn't affect your main features,
   you can update it in a future
   release.
 - Slap a beta tag on your software.
   Generally, people will be more
   forgiving of bugs in a beta version. They may even expect them.
 - Acknowledge known bugs for each release. Transparency helps and your clients and community will be more understanding if they know you're working on it.
 - Don't develop new features until you
   take care of the majority or all of
   the existing bugs.
 - Iterate quickly.

If you don't feel like your **main** features are stable enough by your release date, push back the release. Delays happen in software all the time and it will be easier to overcome a delay by a few weeks or even months than the initial bad reputation that would result from your main features not working. 



## Answer 18308

- posted by: [Nir](https://stackexchange.com/users/-1/4237-nir) on 2010-12-29
- score: 6

Cut scope.

Your basic problem is that there is a lot of data on the internet, you can't possibly support every type of data - it's just not going to work, by the time you add support for all types of data that exists today new types will pop up - you will never finish.

Think about your first client (it can be an imaginary client), think about the smallest subset of data they absolutely need - that is the smallest subset where using your software provide any value what so ever not the smallest subset you think is acceptable.

Release this initial version and continue to prioritize new data types by the frequency your customers are failing to process them.

(I don't know exactly what data you are trying to process, so I may be wrong but from your question I get the feeling that it is one of those endlessly dynamic types of data where you can't possibly support everything).


## Answer 18309

- posted by: [james](https://stackexchange.com/users/-1/5800-james) on 2010-12-29
- score: 2

Without knowing the specifics of your product I can't offer any fixes. But, if you have been working on this for 2 years and you are still discovering major problems, it sounds like you have a fundamental problem with your parser/algorithm/methodology. 

Are you just collecting more and more dataset/samples then 'bug fixing' to handle each 'exception'? did you start off with a clear concept how you were going to solve the problem, or are you guessing your way through each new data sample?

To be the bearer of bad news - you might need to stop, take a deep breath then re-visit your core code and decide if it is properly designed to handle the job.  Do you need a module approach? e.g if you are parsing web logs you might need a apache module, iis module etc where you can add specific features instead of a monolithic one-thing-does-it-all-and-will-rule-the-world. It might give you a better marketing/sales approach too. When a customer has a new/different data set you can sell/publish a new module


## Answer 18306

- posted by: [Community](https://stackexchange.com/users/-1/-1-community) on 2010-12-29
- score: 1

<p><strong>Seth Godin</strong> talk about the ultimate technique <a href="http://the99percent.com/videos/5822/Seth-Godin-Quieting-the-Lizard-Brain" rel="nofollow">in this video</a>.</p>

<blockquote>
  <p>There is one secret to shipping on time and on budget. The secret is: when you run out of time or you run out of money, you ship. The you are on time and on budget.</p>
</blockquote>

<p>Time to market is important for technology products.</p>

<p>I suggest you to use <a href="http://www.scrum.org" rel="nofollow">Scrum</a> to achieve that goal.</p>




---

All content is licensed under the [CC BY-SA 3.0 license](https://creativecommons.org/licenses/by-sa/3.0/).
