## Ramp Up Deployment for LAMP - Hosting recommendation?

- posted by: [ron M.](https://stackexchange.com/users/-1/2122-ron-m) on 2010-01-04
- tagged: `hosting`
- score: 2

As premature as it is right now, I'd still like to ask for your recommendation for a good scalable LAMP deployment. I will probably launch the beta with a single box, or a web server and a database on two boxes, but i'd like to know that the hosting service I choose can grow with me and my needs, without having me shut down in the middle of a growth boom and move elsewhere.

I'd appreciate advice from someone who's a few steps ahead of me and has launched a LAMP based web 2.0 application.

Thanks,
  Ron


## Answer 5891

- posted by: [Jason](https://stackexchange.com/users/-1/2-jason) on 2010-01-04
- score: 1

Start with Rackspace's Cloud.  Full LAMP stack out of the box and it scales like crazy, and it's pretty cheap.

Also if you ever wanted to move to a hosted situation, they will move your installation for you -- their customer service is legendary.


## Answer 5928

- posted by: [Joe](https://stackexchange.com/users/-1/1572-joe) on 2010-01-04
- score: 0

<p><a href="http://aws.amazon.com/ec2/" rel="nofollow">EC2</a> is popular, easy to scale, and there are numerous public AMIs (Amazon Machine Instances) that are LAMP-ready.  Many of my colleagues run their web businesses exclusively on EC2.  There is <a href="http://alestic.com" rel="nofollow">a directory of ubuntu AMIs at alestic.com</a>.</p>



## Answer 5934

- posted by: [Matthew Rankin](https://stackexchange.com/users/-1/1252-matthew-rankin) on 2010-01-04
- score: 0

<p>If you would prefer a non-cloud-based solution, such as Amazon's EC2 or Rackspace's Cloud, I would recommend <a href="http://www.slicehost.com/" rel="nofollow">Slicehost</a>. For $20/mo you get a Virtual Private Server (VPS) known as the 256 slice, which includes 256MB RAM, 10GB Storage, and 100GB bandwidth per month. Some of the things that I like about Slicehost, is that I know exactly what my costs are each month (they don't vary with usage as the cloud-based solutions do), and I get my choice of Lunix distribution (personally I prefer Ubuntu). All slices include a dedicated IP and RAID-10 disk storage.</p>

<p>I've used Slicehost for almost 3 years now to host both customer facing websites and to create internal company intranets using OpenVPN to limit access to employees. Their customer support is great.</p>

<p>Slicehost originally started in St. Louis as a small VPS, but they have since been bought by Rackspace. I view this as a plus, since if I ever need a cloud solution I can stay within the Rackspace family.</p>



## Answer 5940

- posted by: [Jesper Mortensen](https://stackexchange.com/users/-1/1261-jesper-mortensen) on 2010-01-04
- score: 0

<p>If possible, I would prefer not to deal with the operating system -- installation, performance tuning, and security patching. Therefore I'd personally prefer a provider who delivers a execution environment of my choice (.NET, PHP, Java) over one who delivers a bare-bones virtual PC. In other words, while Amazon EC2 is great, it is IMHO a better fit for larger, later-stage companies.</p>

<p>So my suggestions would <a href="http://www.rackspacecloud.com/" rel="nofollow">Rackspace Cloud</a> (already mentioned by Jason) be and <a href="http://www.joyent.com/" rel="nofollow">Joyent</a>. Joyent has been around for years, did cloud computing before it became fashionable, and has some very happy customers too -- worth looking at.</p>

<p>Windows Azure will actually work with PHP as well, and offers some very nice and highly scalable storage API's. I personally would never consider Microsoft's platform for PHP hosting, but maybe that's just a unfounded prejudice nowadays.</p>



## Answer 7959

- posted by: [jimg](https://stackexchange.com/users/-1/2380-jimg) on 2010-02-11
- score: 0

<p>If you want a VPS that has phone support, has a Parallels Virtuozzo panel to ease upgrades / administration, and good uptime, I would recommend <a href="http://eapps.com" rel="nofollow">eapps.com</a> It's a good step between shared hosting and unmanaged boxes, and the prices are good.</p>




---

All content is licensed under the [CC BY-SA 3.0 license](https://creativecommons.org/licenses/by-sa/3.0/).
