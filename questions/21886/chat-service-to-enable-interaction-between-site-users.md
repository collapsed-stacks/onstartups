## Chat service to enable interaction between site users

- posted by: [tucson](https://stackexchange.com/users/-1/2407-tucson) on 2011-03-19
- tagged: `chat`
- score: 1

I would like to enable my website users to chat with specific listed service providers. Ideally the chat service would not require any kind of login, and would be usable directly.

Scenario: user on site looks for a plumber, my site presents a list of plumbers that are currently online on the chat service, and clicks on one of them to directly chat.

Is there such service out there?
Has anyone a recommendation?

Perhaps an API to Skype would be the solution..., but Skype requires being registered I think. Or an API to other chat service.


## Answer 21915

- posted by: [Tim Nash](https://stackexchange.com/users/-1/7035-tim-nash) on 2011-03-20
- score: 1

<p>We spent a lot of time looking for suitable chat system and while we haven't found anything perfect the one we settled for is <a href="http://www.olark.com" rel="nofollow">olark</a> which has a javascript front end you put on your site, and you connect to it via Jabber on the backend (gtalk also uses jabber).</p>

<p>Ultimately we went with it because we could customise it (a lot) and it had a nice javascript API allowing us to identify and notify the operators when people hit certain points in the site: i.e 4 pages and the pricing page or 10 pages in total meaning not only could people talk to us but we could be proactive in engaging them.</p>

<p>Their are similar services to Olark (i.e using jabber backends) and most cost (as does Olark on the plan we are using) also while I know they are working on it, their is no way to remotely access the transcripts (except via their web site) </p>

<p>We are only in month 2 of a 3 month trial while we evaluate and it paid for itself in under a couple of hours, it's a lovely feeling to be able to actually engage with our customers and without over selling it, having a chat system has increased sales, and especially increased higher value sales and reduced support costs (though the flip side is people do use it as a support channel even when they are told its just a sales channel)</p>




---

All content is licensed under the [CC BY-SA 3.0 license](https://creativecommons.org/licenses/by-sa/3.0/).
