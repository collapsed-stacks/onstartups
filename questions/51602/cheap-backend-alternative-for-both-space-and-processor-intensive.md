## Cheap backend alternative for both space and processor "intensive"?

- posted by: [fotanus](https://stackexchange.com/users/-1/28529-fotanus) on 2013-11-01
- tagged: `startup-costs`, `server`
- score: 0

<p>I have a start-up idea that is data-centric for users. This means that each user would have something like 5GB at least. But there is also a good amount of data processing, so I can't imagine have this thing up and running without 2GB ram.</p>

<p>Most cheap VPS plans (as always, needs to be cheap for start-ups) have very little disk space, like 50Gb, and this limits a lot the number of clients one can get.</p>

<p>I've been thinking of ways to have more space per less money without sacrificing the processing. One option is take a standard VPS and a storage VPS, and actually store the data on the storage.</p>

<p>Is this practical something normal, or to have a good disk space and processing it is mandatory to have a costly server? </p>

<p>Of course tips to avoid spending a lot on servers like this are welcome.</p>



## Answer 51604

- posted by: [Gavin Coates](https://stackexchange.com/users/-1/23633-gavin-coates) on 2013-11-01
- score: 1

<p>I would suggest speaking to some VPS hosts and see what they can do for you. VPS's are normally sold in packages - with each package designed to appeal to as wide an audience as possible. Typically storage is not one of the key features that clients demand, so the packages do not really focus on this.</p>

<p>To add extra storage to a VPS is easy - it's just a case of adjusting the slider when making the Virtual machine. Obviously this takes up more space on the physical machine, which may mean they can host fewer clients per machine (although typically processor/memory limits would restrict this before hard disk capacity).</p>

<p>Speak to them and I'm sure they can quote you a price for creating a machine tailored more to your needs.</p>

<p>However, from the sound of it you need to do a lot of processing on this data, and as such are going to need a lot of memory and CPU performance too. VPS's are not ideal for this - as you are sharing the load with multiple other clients on the same physical box, and often capacity is oversold as few clients use 100% of their allocation. If you are unfortunate enough to be on a heavily loaded box, with other clients using a large % of their allowance, then you will really struggle performance wise.</p>

<p>It might be worth getting a dedicated server, that way you have more control over the hard disk capacity, and have access to 100% of the memory and processing capacity of the server.</p>




---

All content is licensed under the [CC BY-SA 3.0 license](https://creativecommons.org/licenses/by-sa/3.0/).
