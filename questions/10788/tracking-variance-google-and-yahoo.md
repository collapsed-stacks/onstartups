## Tracking Variance - Google and Yahoo

- posted by: [Chris](https://stackexchange.com/users/-1/412-chris) on 2010-05-01
- tagged: `analytics`, `website`, `marketing`
- score: 1

We use Google Analytics to track metrics on our site. I'm doing search engine marketing with both Google and Yahoo. There is a HUGE difference in the visits we "see" on our site vs. what Google and Yahoo say they're sending us. I know there's going to be a difference always for many reasons. GA isn't perfect, bots and spiders, people bouncing before the full page loads, etc. But that shouldn't account for too much more than 10% from what I'm told. I'm seeing a difference of 2 to 3x. Both Yahoo and Google looked and said our tracking is set up properly, yes that's a way bigger variance than normal, we don't know why.

Has anyone else encountered this problem? Did you find a resolution or way to mitigate it?

Appreciate it,



## Answer 10798

- posted by: [Jesper Mortensen](https://stackexchange.com/users/-1/1261-jesper-mortensen) on 2010-05-02
- score: 2

I have not encountered a similar problem; but what has been done so far to track down possible root causes? Off the top of my head, I imagine the reason lies in "hits from clients capable of executing Javascript" (and hence be counted by GA etc) versus "HTTP hits on the server" based counting. Some thoughts:

 - Are the GA and Yahoo numbers consistent with each other (not identical, gut GA and Yahoo should follow each other, and server-side monitoring should be the outlier)? If not, this begins to look really weird.

 - Are you absolutely, 110% sure that your webserver side logging isn't counting a type of hit twice? I know, of course you are, yet I've seen this problem more than once.. Could there be some weird MIME type that's being counted as a page hit while it's just a supporting file, not a page (HTML)?

 - Are you getting many mobile users on your pages? Mobile (cell phones) generally don't execute Javascript, or have extremely limited JS support, so they're often not counted correctly by GA etc.

HTH,



---

All content is licensed under the [CC BY-SA 3.0 license](https://creativecommons.org/licenses/by-sa/3.0/).
