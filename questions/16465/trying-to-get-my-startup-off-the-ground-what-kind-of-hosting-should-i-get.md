## Trying to get my startup off the ground, what kind of hosting should I get?

- posted by: [Community](https://stackexchange.com/users/-1/-1-community) on 2010-11-13
- tagged: `hosting`, `server`
- score: 0

I've just gotten off of HostGator (I love them, but they limit processes, which is bad for me now). I'm on a VPS (unmanaged, $15 a month, 1GB Ram, unlimited data transfer) but I don't really like them.

I want to keep the cost of the servers ~$20~$30/month as I'd like to keep initial costs down while I try to grow. The site uses Python cgi to fetch and parse remote pages to aggregate data, and mySQL to store some of the info (as opposed to fetching it).

I'm new to the hosting thing, but I feel I could handle a server on my own. I'm just wondering what kind of host I should be looking for (shared, semi-dedicated, vps, etc) and how much I should be willing to spend!

thanks!

The site is: http://BlueDevilBooks.com by the way


## Answer 16467

- posted by: [Matthew Dorian](https://stackexchange.com/users/-1/5382-matthew-dorian) on 2010-11-13
- score: 2

I love our provider... Linode.com. 


## Answer 16507

- posted by: [jtauber](https://stackexchange.com/users/-1/3994-jtauber) on 2010-11-15
- score: 1

At this stage, I would recommend staying with a VPS provider and would recommend Slicehost or Linode from personal experience.

You might want to consider separating the fetching / processing from the serving to users. That way any load on the former won't affect the latter.



---

All content is licensed under the [CC BY-SA 3.0 license](https://creativecommons.org/licenses/by-sa/3.0/).
