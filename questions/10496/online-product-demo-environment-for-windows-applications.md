## Online product demo environment for Windows applications

- posted by: [Stefanos Tses](https://stackexchange.com/users/-1/3178-stefanos-tses) on 2010-04-22
- tagged: `demo`
- score: 1

I'm looking for a way to allow potential customers to try my application before they buy it.

The product is a windows forms application that requires an SQL Server database to operate.

Although I have a functional demo that the customer can install on their network, I want to make it easier for them by have them "play" with it at my environment.

I remember Microsoft had (has?) something similar. I was testing Visual Studio a few years ago in  a virtual environment where I was connecting to a server at Microsoft.

Any suggestions?

Thanks. 



## Answer 10935

- posted by: [Adam Perlow](https://stackexchange.com/users/-1/2612-adam-perlow) on 2010-05-07
- score: 1

Have you considered packaging SQL Server Express with your installer? You can give the customer the option of connecting an existing SQL Server or installing SQL Server Express (which is royalty free) during your setup process. If you go this route, I'd recommend a high level of automation during the setup process where your installer installs SQL Server Express, creates the database, grants permissions, etc. without requiring the user to understand the setup process.

This link might help http://msdn.microsoft.com/en-us/library/bb264562(SQL.90).aspx. 


## Answer 10522

- posted by: [SmartCompanySoftware](https://stackexchange.com/users/-1/1629-smartcompanysoftware) on 2010-04-23
- score: 0

I have a similar problem, but instead of installing the application, I am offering them to watch demos of the application. There are pros and cons of offering a demo or watching a demo. Getting them to watch it, I can show them the application features instead of them clicking aimlessly around.

I have played around with SCREEN2SWF and it is quite good.


## Answer 10932

- posted by: [Joe](https://stackexchange.com/users/-1/3307-joe) on 2010-05-07
- score: 0

Do you have a good demo video/walkthrough? If not you are getting ahead of yourself.  Have a video first.  Then if you are getting requests consider providing a virtual machine, which is what you are remembering from the VS demo.  You can also set up a machine that they can use remotely as part of the sales process once they are in contact with you.



---

All content is licensed under the [CC BY-SA 3.0 license](https://creativecommons.org/licenses/by-sa/3.0/).
