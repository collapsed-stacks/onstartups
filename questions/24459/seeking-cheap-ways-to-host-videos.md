## SEEKING CHEAP WAYS TO HOST VIDEOS

- posted by: [Jodi W Von Oettingen](https://stackexchange.com/users/-1/10032-jodi-w-von-oettingen) on 2011-05-05
- tagged: `video`
- score: -1

> **Possible Duplicate:**  
> [What&#39;s the best way to integrate video without using bandwidth on my website?](http://answers.onstartups.com/questions/24083/whats-the-best-way-to-integrate-video-without-using-bandwidth-on-my-website)  

<!-- End of automatically inserted text -->

Ok...I've posted a similiar question like this but there's a twist.

Who and/or what is the cheapest way to host video content within a current website ?

Please be considerate as I wish to gain information from ONLY those that *know* through their *own experience* (no geusstimating puhhlleeaaase)

1. If you host a website and use a 3rd party Host/Storage and/or a CDN then I'll assume you might just be able to answer my question.

2. Using non-professional *Hosts* (like youtube) is out of the question due to video content being extremely sensitive and copyright material.

3. So in a nut shell all video *can not* be viewed by the public

4. My current web service is members ONLY so no one is able to access member details or video content *outside* of my network

Thanks everyone, hope to get some seriously good information (pricing of the services would be good please, including links if able)

cheers again 

p.s. 3rd party Host needs to have the best uptime and bandwidth at a cheap budget. lol hey I might not get what Im asking but it doesnt pay to not ask !


## Answer 24465

- posted by: [Ankur Jain](https://stackexchange.com/users/-1/6146-ankur-jain) on 2011-05-05
- score: 0

<ul>
<li><p>We host one of our membership
websites on Hostgator VPS (we have zero
downtime with them till date and have
been with them since 6-7 months) and
all videos are on Amazon S3. With S3,
you will only pay for what you use.
Since it seems you have a membership
site you can configure the options
under Amazon S3 such that your video
links will auto expire after a
specified time period and people will
not be able to share the video links
with anyone else.</p></li>
<li><p>If you can spend some extra money and looking for out-of-the-box video analytics too, check <a href="http://wistia.com/" rel="nofollow">Wistia</a>. Wistia will be more or less plug-and-play solution while with S3 you may need to invest some time understanding, configuring various options. </p></li>
<li><p>You can also check my profile, where I have listed some resources for startups and the script we used to create our membership site.</p></li>
</ul>

<p>Hope that helps. All the best!</p>




---

All content is licensed under the [CC BY-SA 3.0 license](https://creativecommons.org/licenses/by-sa/3.0/).
