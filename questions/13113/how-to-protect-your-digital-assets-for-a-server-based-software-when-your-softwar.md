## How to protect your digital assets for a server based software when your software is installed within a third party Data centre

- posted by: [Shabda](https://stackexchange.com/users/-1/2973-shabda) on 2010-07-28
- tagged: `piracy`, `software`
- score: 2

We have developed a software which is server installable and is accessed by browser. We have just got our first large client which wants to use it, but wants to install it within their data center, for use by their employees.

Apart from the legal step we can take, what are the technical steps we can take to minimise chances of the code being pirated.

Our software stack is

Python + Django as the app backend.
Mysql DB

Frontend uses
Html, jquery + some flash and java for some pages.

Server: Linux based system, with Adobe FMS

We can give them complied pyc, swf and .jars but decompiling any of them is not particularly hard, and anway the complied assets can be used as they are.

In particular, can we use a hardware dongle to solve this problem?




## Answer 13115

- posted by: [Jesper Mortensen](https://stackexchange.com/users/-1/1261-jesper-mortensen) on 2010-07-28
- score: 1

If you're dealing with a large, well known company, then in general you shouldn't worry too much about them pirating your software. If they do, the potential PR problem for them is pretty big.

What you should worry more about is them exceeding the amount of users (seats) sold, because they don't know how many people are using it. And for that, the easiest thing to do is to give a site/company license, so that the software doesn't count users.

In general, for the first sales, you do whatever you have to do to make it work. You need the sales.

My worry with your setup is that Operations will hate it. Python is unusual in the corporate world, I don't even know what Adobe FMS is. Many large companies have standardized their technology stack, so f.x. the Ops team could refuse to install MySQL, because they support only Oracle and MSSQL for databases. Do what you can to make this smooth, possibly install the software yourself.

**As for your DRM question:**

 - In the world of Java and .NET one generally uses obfuscators to make decompiling the code harder. I don't know if Python even has a obfuscator, but that could be your first thing to look at.

 - You can make your code tied to the network card (which has a unique ID embedded in the hardware), or to a dongle. There are many old dongle protection systems available for purchase. Again Ops is not going to like this, it potentially messes up their options for moving the software to another server in case of an emergency. Without obfuscation, I question how useful a dongle or NIC lock will be against a determined cracker -- after all, he can easily edit the bytecode.

 - "Call home", making the code make a periodic call to your servers, with the license key of the installation. At least makes it easy to discover when a license key is being redistributed and used in many places, and to prohibit upgrading on the hacked license keys.

 - "Outrun the hackers". Don't bother with DRM protection on the first releases of your product, because you know these releases are somewhat weak on functionality, and later releases will be much much better. So you don't add DRM before your company is somewhat larger, and the software perhaps is in version 3.x or 4.x, under the assumption that the first versions won't really be worth pirating when compared to your latest versions.

Of the above, the "outrun the hackers" would be my personal choice.



---

All content is licensed under the [CC BY-SA 3.0 license](https://creativecommons.org/licenses/by-sa/3.0/).
