## What are the best practices to protect sensitive user data from being misused by the engineers in a start up?

- posted by: [Sabya](https://stackexchange.com/users/-1/12738-sabya) on 2011-08-17
- tagged: `security`, `data-protection`
- score: 3

If a start up is storing sensitive user data in it's databases, how should the company protect it from it's engineers accessing it unnecessarily and misusing it?


## Answer 28911

- posted by: [NetTecture](https://stackexchange.com/users/-1/3350-nettecture) on 2011-08-17
- score: 2

Not at all, unless it makes financial sense. THen, by isolating operations from development - operations always has access - and using totally fake or randomized data (i.e. replace the same field in the table randomly... like customer names, names, surnames, cities, streets, zips all get randomized independently, the result is total garbage fo analysis).

It will cost, though - if not in tools, then significantly in time. MOST companies never bother. Protect yousrself legally. I work in a financial trading business at the moment and I have access to all the life deals although I am only dev lead of a techncial team for a data warehouse project. We work an develop of production copies.


## Answer 28926

- posted by: [JeffO](https://stackexchange.com/users/-1/1796-jeffo) on 2011-08-17
- score: 0

They should be doing most of their work on a test database. You can always mask/scramble the data during the copying and their access to the test database. You'll have to work closly with the dev that builds this part since they'll completely rely on you to verify the data before and after. This could be done with a few 'dummy' accounts. 

Most critical data shouldn't be that hard for them to work with an altered version. Your devs should be familiar with handling names, phone numbers, ssn's, account numbers, etc. Internal generated ID's and keys are meaningless anyway.




## Answer 28944

- posted by: [Shauna](https://stackexchange.com/users/-1/11273-shauna) on 2011-08-17
- score: 0

As the others have mentioned, use a test database with dummy information. You shouldn't be developing against a live database, anyway.

Other than that, though, put it in their terms of employment that you expect any access granted to them that involves any kind of sensitive information be treated as though it were officially considered Classified or Top Secret information, and that they would lose their job and there would be legal ramifications if they were to abuse the information entrusted to them. If you go this route, also make sure that all employees with access to sensitive information are educated on proper treatment of such information. It's astounding how much personal information gets stolen solely because the people handling it were uninformed.


## Answer 28959

- posted by: [cdkMoose](https://stackexchange.com/users/-1/12756-cdkmoose) on 2011-08-17
- score: 0

If you can't trust your employees, what are they doing there?  I learned many years ago that the first line of internal security is the front door.

Make sure that your employment contracts are clear regarding the requirements for client data confidentiality.  Developers should be developing against test databases with appropriate sample data, but inevitably, there will be a problem that needs to be checked against live data.



---

All content is licensed under the [CC BY-SA 3.0 license](https://creativecommons.org/licenses/by-sa/3.0/).
