## Obfuscate or not reason?

- posted by: [jazar](https://stackexchange.com/users/-1/6750-jazar) on 2011-12-23
- tagged: `software`, `development`
- score: 0

I just wondering what is the reason for some companies to not obfuscate their product that written in Java/.NET ? 

I've worked with expensive enterprise software, and I helped since the software don't apply obfuscation on their web app client, so I can made understand how it work and write customization easily. Could this is one of the reason ?


## Answer 34083

- posted by: [JonnyBoats](https://stackexchange.com/users/-1/3100-jonnyboats) on 2011-12-23
- score: 2

For me the important things to consider are:

-What could the client do with my source code if they had it? Could they cost me money etc.?

-What kind of client am I dealing with, are they trustworthy?

I am in the USA. If I have a signed agreement with a major USA company and they agree not to reverse engineer or "steal" the software then I am generally not worried. If it turns out that they violate the agreement and it causes me to loose money I take them to court and collect big bucks in damages. Major companies just don't like to take such risks, and thus generally don't ripoff software on a major scale.

If on the other hand I had to send my software to some third-world country with no effective intellectual property protection and a track record of bootlegging like crazy it would behoove me to obfuscation as much as possible and understand that no matter what I do they are probably still going to steal it if they want to.

Now to the other point, what can they do with it to hurt me if they steal it? Most people think their software is worth far more than it probably is.  Think about the major companies; Microsoft Windows is pirated all the time, but Microsoft is still making lots of money.

Then there is the question of if the costs associated with obfuscation outweigh the benefits. Perhaps there is a parallel to copy protection; entertainment companies spend big dollars on copy protection and yet they get ripped off anyway while inconveniencing legitimate users. Consider how Apple decided to drop copy protection from the music they sell.

Finally there is some software that perhaps is so sensitive that it could affect national defense etc. In the USA there are laws and export controls on such things, but this is not your average software package.


## Answer 34077

- posted by: [Kort Pleco](https://stackexchange.com/users/-1/7876-kort-pleco) on 2011-12-23
- score: 0

If it's a webapp then the important part is on the server where you can't get to it.



---

All content is licensed under the [CC BY-SA 3.0 license](https://creativecommons.org/licenses/by-sa/3.0/).
