## How do I create a service charge table

- posted by: [Jared](https://stackexchange.com/users/-1/21786-jared) on 2012-11-27
- tagged: `service`
- score: 2

I'm planning on changing the pricing model of my company from an hourly rate to a fixed rate. If that's not clear enough here's an example:

My current model is: customer asks us to install a power supply for an equipment, I'll charge 1 hour for that. If the customer asks us to install a power supply and a CPU for an equipment, I'll still charge 1 hour for that. But if it's a conveyor belt replacement, I'll charge 6 hours for that.

My gripe with my current model is, the man-hours for the job can be "different" from job to job. Instead of having a fixed charge per labor done.

New labor I want is similar to the way car dealers work when it comes to repair, for example: install power supply = $5. install CPU = $10, replace conveyor belt = $125.

So I guess what I'm saying is that, depending on the part to be installed/replaced/serviced, I'd like to have a fixed charge for that so all my engineers/sales has to do is add things up instead of having a man-hour estimate.

Now, what I don't know is how this is identified WITHOUT having a machine and doing multiple "time attacks" on servicing a certain part as this will involve tremendous investment of time and resources both on employees and the training equipment.

Hope this was a clear explanation and I hope you guys can help me out.




## Answer 44529

- posted by: [Frank](https://stackexchange.com/users/-1/4858-frank) on 2012-11-27
- score: 0

What are you creating the table in?  I think what you are missing is the minutes per task.  Change cpu = 15mins.  Change case = 90 mins.  Then you have an hourly rate, and calculate your figures that way.  You can have a minimum rate of 1 hour labor.  Or round up to the nearest 15 minute increment. 

When you charge based on time, and multiply against an hourly rate, you can adjust your hourly rate and have all prices update.  You can also get creative and have hourly rates based on the total hours.   So for jobs of 1 hour and less your rate is $100 per hour.  Jobs 2-8 hours its $75 per hour.  And jobs 9-100 hours its $50 per hour. 

The formula is simple.

Sum up all the tasks based on their minutes.  Determine rate bracket based on the total sum of minutes.  TotalMinutes x (HourlyRateThisBracket / 60)





## Answer 44535

- posted by: [Karlson](https://stackexchange.com/users/-1/15252-karlson) on 2012-11-27
- score: 0

You will need to do data collection and analysis of this and then you can come up with flat charges for certain tasks.  For example.

Replace CPU.  Performed 200 times.  Minimum time for task: 15 minutes.  Max: 2 hours, average: 30 minutes, median: 30 minutes.  Travel Time, min, max, average, median.

Based on this data you can calculate what it will cost you in man hours, equipment, etc and what can you charge so that you come out in black.  Same with conveyor belts, and power supplies.

After that simply come up with codes for your engineers if you haven't already and that's how you do your billing.



---

All content is licensed under the [CC BY-SA 3.0 license](https://creativecommons.org/licenses/by-sa/3.0/).
