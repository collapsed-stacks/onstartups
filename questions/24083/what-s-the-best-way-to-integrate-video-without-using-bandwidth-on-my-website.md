## What's the best way to integrate video without using bandwidth on my website?

- posted by: [Jodi W Von Oettingen](https://stackexchange.com/users/-1/10032-jodi-w-von-oettingen) on 2011-04-27
- tagged: `hosting`, `video`
- score: 1

 1. I have a Social Networking site for a niche market

 2. I need members to be able to view and upload content

 3. My members *content is copyrighted* therefore in no way can the content be available to the public

 4. Due to the copyright issues no member can copy and embed the content, to other online sources

 5. My bandwidth for my current website is a maximum of 250 gig and no way can my 12,000 members utilise my own bandwidth whithout crashing or slow loads etc.

I hope I can get some kind of response from anyone that can give me some information.
Hopefully some one has experience in do what I have in mind. And can direct me to the best alternatives I can consider.

Thanks


## Answer 24112

- posted by: [Yuri Gadow](https://stackexchange.com/users/-1/5083-yuri-gadow) on 2011-04-27
- score: 3

<p>S3 is probably the best bet for you because you'll want customers to <a href="http://doc.s3.amazonaws.com/proposals/post.html" rel="nofollow">upload directly to your storage service</a>, i.e., not to your servers within your bandwidth cap and then onto a CDN. And, you can run S3 with a CDN, theirs or any other with customer origin support. Just using a CDN would be problematic since it would require you to upload your content directly to them or source it from your origin, leading you to your bandwidth problems.</p>

<p>Once you've settled on storage: <a href="http://transloadit.com" rel="nofollow">transloadit.com</a> is a great way to get the files uploaded and <a href="http://sublimevideo.net" rel="nofollow">sublimevideo.net</a> for the other direction, i.e., playing. I use and really like both products. I also use a mixture of S3 and <a href="http://www.gogrid.com/cloud-hosting/content-delivery-network.php" rel="nofollow">EdgeCast via GoGrid</a> with customer uploads going to the former and served via EdgeCast's customer origin and company videos uploaded manually to EdgeCast's own storage and served from there.</p>



## Answer 24090

- posted by: [Yock](https://stackexchange.com/users/-1/9993-yock) on 2011-04-27
- score: 2

Have a look at [Amazon's S3 service](http://aws.amazon.com/s3/). Its the best non-public alternative to hosting content like video without burdening your current host with the bandwidth and requests.

With S3 you will have to alter whatever script you're currently using to upload/download the content into your S3 account. Once its there you pay for the bandwidth, space used and how often your users will request that specific content.

This will cost you more per month. You only pay for what you use. Its the smallest risk you can take vs buying a bigger server or possibly in your case a server farm.


## Answer 24086

- posted by: [Apollo Sinkevicius](https://stackexchange.com/users/-1/2119-apollo-sinkevicius) on 2011-04-27
- score: 1

Check out Wistia. We have used them as one of the platforms for our Pixability video marketing platform for years.


## Answer 24085

- posted by: [NetTecture](https://stackexchange.com/users/-1/3350-nettecture) on 2011-04-27
- score: 0

Ah - no way? I need a car that runs races but does not need any fuel.

You need editing and not  be public - no hosting side like youtube.

You dont want to invest into bandwidth and resources - no private hosting.

= no hosting at all.

= not possible.

Sorry, no magic wand here.



---

All content is licensed under the [CC BY-SA 3.0 license](https://creativecommons.org/licenses/by-sa/3.0/).
