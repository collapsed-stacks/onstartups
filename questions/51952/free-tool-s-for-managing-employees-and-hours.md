## (Free) tool(s) for managing employees and hours

- posted by: [Joachim](https://stackexchange.com/users/-1/29858-joachim) on 2013-11-30
- tagged: `website`, `employees`, `management`, `tools`
- score: 0

<p>I am creating a service (PC maintenance) business and I need a tool for keeping track of which employees are available at what times. This data needs to be exported or otherwise accessible by a web application so clients on the website can schedule an appointment at a time where there is a staff member available.</p>

<p>It would serve as one system for me to manage the employees and the website to get relevant data. I consider this of pretty trivial nature yet I couldn't find any tools which provided this functionality without a major rewrite.</p>

<p>Do any of you have experience with such (preferably free) system?</p>



## Answer 51953

- posted by: [Liam Dolman](https://stackexchange.com/users/-1/27824-liam-dolman) on 2013-12-01
- score: 0

<p>I haven't seen anything with the functionality you are looking for, most erp/hr systems were built for fixing bugs rather than managing shifts, but I would tell you what I think would be the best way to approach this. </p>

<p>Firstly separate the front and back end of your service.</p>

<p>On the front end you would need to build a form that would gather the clients availability, basic details on the issue and contact details. Have that form email you a copy, simpler and faster to implement than integration which can be done at a later date.</p>

<p>On the back end have a shift management system, phpScheduleIt may be good but I have only used the demo, to match up client availability to staff availability.</p>

<p>Then contact the client to confirm booking.    </p>



## Answer 51966

- posted by: [Guido Leenders](https://stackexchange.com/users/-1/29864-guido-leenders) on 2013-12-01
- score: 0

<p>Not free, but very handy: let your employees use Outlook calendar to register time spent per job and to register future availability. Possibly backed by exchange or online exchange. Then use export of Outlook (or view as table, copy &amp; paste) to make it available elsewhere. For us, this was the basis for our ERP system Invantive for project and service organisations, but for this scenario you have sufficient with Outlook alone. Possibly you might want to code labor type using categories.
At my previous employer (Square Service Management Systems) we had a solution using what is now known as "optimize my day" (it is based on software of Geodan EDT which no longer exists). It is well suited for larger teams (up to 2000 service engineers) and also does distance-based planning (travelling sales men problem). See <a href="http://www.optimizemyday.com/home/en/" rel="nofollow">optimize my day site</a></p>




---

All content is licensed under the [CC BY-SA 3.0 license](https://creativecommons.org/licenses/by-sa/3.0/).
