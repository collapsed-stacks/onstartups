## Where can I find a good online records management system?

- posted by: [Dave Feyereisen](https://stackexchange.com/users/-1/8565-dave-feyereisen) on 2011-03-23
- tagged: `database`
- score: 2

I'm looking for a web app that makes it easy to recreate paper forms (preferably drag and drop), and then save the information in a database, and generate custom reports (again, preferably drag and drop).  Anyone know of any small companies doing a good job with this, or any decent open source products?


## Answer 22145

- posted by: [Joseph Barisonzi](https://stackexchange.com/users/-1/8791-joseph-barisonzi) on 2011-03-23
- score: 2

<p>Both <a href="http://docs.google.com/support/bin/answer.py?hl=en&amp;answer=151187" rel="nofollow">Google</a> and <a href="http://www.zoho.com/creator/" rel="nofollow">Zoho</a> -- both open source and free -- have a simple WYSIWYG drag-n-drop form creator which you can then publish and receive results in a linked spreadsheet. </p>

<p>There are several web2email form management solutions on the market. Some that come to the top of mind are <a href="http://www.emailmeform.com/" rel="nofollow">emailmeform</a>, <a href="http://www.formsite.com/" rel="nofollow">formsite</a>, <a href="http://www.icebrrg.com/" rel="nofollow">icebrrg</a>, <a href="http://wufoo.com/" rel="nofollow">wufoo</a>, and <a href="http://www.jotform.com/" rel="nofollow">jotform</a>. A little simple programming would push tese into the a database of your choice. </p>

<p>If having it go into more than a spreadsheet-- but an actual database -- my recommendation is to deploy a CMS. Most of the good open source CMS -- <a href="http://www.joomla.org/" rel="nofollow">Joomla</a>, <a href="http://www.google.com/url?sa=t&amp;source=web&amp;cd=2&amp;ved=0CC8QFjAB&amp;url=http://drupal.org/&amp;ei=g1KKTba-GMqDtgfo4OXcDQ&amp;usg=AFQjCNFm9QShEHSv1oZ9NwNP_UHzLkKdqA&amp;sig2=hYiqfNvsJPAj21-ZG3lDRQ" rel="nofollow">Drupal</a>, <a href="http://goo.gl/9FVkc" rel="nofollow">Wordpress</a>(?) -- have form management extentions which caputre data, put it into the same mySQL database that drives the CMS. I use Joomla and we love <a href="http://www.chronoengine.com/" rel="nofollow">Chronoforms</a>. You could deploy a version with just the form onto a subdomain of your site.</p>

<p><a href="http://www.butterfat.net/wiki/Projects/phpESP/" rel="nofollow">LimeSurvey</a> is one of the base scripts/programs in Fantastico. Fantastico is a script library for easy one click program installation ont your server. It lives as an application on CPanel. Most web-hosting companies that provided shared hosting on Apache servers have CPanel and Fantastico availabile. LimeSurvey is an releatively easy open source survey tool -- which can make forms and drive them to a mySQL database. It has a farely good extraction options for reporting as well. For a non-techie it is a tad overwhelming to install on a server directly. Fantastic will make it easy. </p>

<p>Good luck! I hope you capture the information that you need!</p>




---

All content is licensed under the [CC BY-SA 3.0 license](https://creativecommons.org/licenses/by-sa/3.0/).
