## Image uploading app - Terms of service

- posted by: [James](https://stackexchange.com/users/-1/17319-james) on 2012-04-05
- tagged: `legal`, `terms-and-conditions`, `tos`
- score: 1

I'm currently working on a simple image uploading app that lets you upload images to services like Flickr and Facebook. Do I need a **terms of service** or some other kind of *disclaimer* for an app like that? If so, what is a *must have* to include there?

Thank you.


## Answer 37892

- posted by: [JonnyBoats](https://stackexchange.com/users/-1/3100-jonnyboats) on 2012-04-05
- score: 1

Do I understand your question correctly that what you created is an application (like a word processor for example) that the user runs on his computer? In other words there is nothing running on a webserver that you control (other than being able to download the application) and that images are never uploaded or stored  on your webserver?

If so, then you are just like a FTP program that a user can run to transfer something from his computer to another computer. Just as a FTP program could be used to transfer copyrighted or illegal materials, so could your program. Just like an FTP program, you (and your program) have no control or awareness of what the user is transferring, to whom or when.

If all of the above is true then you would not need any more of a terms of service or disclaimer than a FTP program would. As for designating a DMCA agent (with associated costs), there is no point as you do not have any files on your server that could be removed. If a user uploads something inappropriate to Facebook using your app then that is between the user and Facebook. It is Facebook that should receive the DCMA takedown notice, not you. After all, you have no ability to remove something from Facebook's servers.

Perhaps you could use the verbiage that comes with Firefox as a model; after all the Firefox web browser is an application that a user runs that permits him to upload images to Facebook and other sites.



## Answer 37889

- posted by: [Justin C](https://stackexchange.com/users/-1/6947-justin-c) on 2012-04-05
- score: 0

You need two categories. The first is things that are there to protect you, such as

 - you're not liable if something happens to their images
 - You are not responsible for the users login credentials

and so forth. The second category are restrictions on what your users can do, such as

 - They may not post copyrighted material
 - They may not post computer virus/worms

You need to cover all your bases. I don't know what all of those bases are b/c I am not a lawyer and this is not legal advice. Those are the types of things you need to have.

Now, you can either pay a lawyer to put together something for you, even if it's simple and "boiler-plate", or you can spend a lot of time reviewing other similar terms of service and writing your own clauses, hoping to not miss something important.

I say budget $500-1,000 and see a lawyer, it may very well save you money in the long run.



---

All content is licensed under the [CC BY-SA 3.0 license](https://creativecommons.org/licenses/by-sa/3.0/).
