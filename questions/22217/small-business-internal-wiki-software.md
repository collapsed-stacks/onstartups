## Small Business Internal Wiki Software?

- posted by: [skaz](https://stackexchange.com/users/-1/7696-skaz) on 2011-03-24
- tagged: `software`
- score: 3

I am interested in running an internal wiki at my small business.  The content, to begin with, would list out major job functions/descriptions as well as policies for the company.  I imagine it would later branch into project specific information as well.  Can anyone recommend good wiki software that can accomplish this?  I am open to Windows or Linux solutions.

Thanks.


## Answer 22223

- posted by: [Joseph Barisonzi](https://stackexchange.com/users/-1/8791-joseph-barisonzi) on 2011-03-25
- score: 4

<p>Oh my lordy-- there are so many different "open-source" wiki programs on the market. It is overwhelming. There is even a <a href="http://www.wikimatrix.org/compare/DokuWiki+MediaWiki+PmWiki+Tiki-Wiki-CMS-Groupware" rel="nofollow">site dedicated</a> to allowing you to compare them -- or at least the 30 or so that they have. Go to the bottom left corner and there is a popup box where you can choose for those you want to compare with: </p>

<p><img src="http://i.stack.imgur.com/AgH4X.png" alt="enter image description here"></p>

<p>To their list I add: </p>

<p><strong>PHP Wiki's Easy Installation</strong>
<a href="http://phpwiki.sourceforge.net/" rel="nofollow">PhP Wiki</a> is free and open source. Description:</p>

<blockquote>
  <p>A WikiWikiWeb is a web site where
  anyone can edit the pages through an
  HTML form. Linking is done
  automatically on the server side; all
  pages are stored in a database.</p>
</blockquote>

<p>It can also be one click installed through Fantastico which a script installing program supplied through cpanel which is the most common software managing an Apache server account. Most places that you purchase share hosting or a managed hosting on an Apache/Linex server provide Cpanel, and thus support a one click installation of PhP Wiki. 
It is simple, clean, no frills and does just what I am hearing that you would like.</p>

<p><strong>The Wikipedia Engine</strong>
If you are attacted to Wiki's because of wikipedia -- why not use the same engine? <a href="http://www.mediawiki.org/wiki/MediaWiki" rel="nofollow">MediaWiki</a> is easily downloaded and installed onto an internal server. Or your server admin can install it on a remote server. There is far more support including videos and user guides for how to get going on their site. Very easy to use. And free. It API has a developer API if/wehn you grow and want to integrate it to other functions of the company.</p>

<p><strong>Google Docs as an option?</strong>
While technically not a wiki -- and all of the good wiki purest will be outraged at the thought of it being considered at the same time: Google Doc is another option to consider. A shared file system -- like Google Docs that tracks discussions and version control might also meet your business need. You can share docuement, set read/write permissions and now their new "Discussions" feature allows team members to discuss their ongoing development of the docuement. It also has a good built in version control allowing you to restore back to any point of the process. The benefit is the connection with your other services, low cost (free) and relativly low learning curve. </p>

<p><strong>Wiki + DropBox</strong>
And en additional interesting solution is deploying <a href="http://www.tiddlywiki.com/" rel="nofollow">TiddleyWiki</a> onto a shared drop box folder. No need for a server at all. It provides a basic wiki environment for your collaborative development of shared files -- without the need for a server -- or even a connection to the server to access. <a href="http://www.broowaha.com/articles/7671/a-personal-knowledgebase-solution-tiddlywiki-and-dropbox" rel="nofollow">Here's a guide on how to do it</a>.</p>

<p><strong>Your Website</strong>
If your website is built in one of the common open source CMS like Joomla, Drupal or Wordpress there is an integrated wiki extention which will allow for integration with your website structure. This allows you site to have an "intranet" component. Encouraging social media development, regular visiting your own website, accessiblity might be added value reasons you would want to host your wiki integrated with your site. Here is the example of the <a href="http://extensions.joomla.org/extensions/news-production/wiki-integration" rel="nofollow">Joomla wiki list</a>.  </p>

<p>Good Luck. I hope that is not too overwhelming. I had just done this research for a client and I am glad someone else will be able to take advantage of it! </p>



## Answer 22222

- posted by: [Doug Donohoe](https://stackexchange.com/users/-1/8906-doug-donohoe) on 2011-03-25
- score: 3

I highly recommend confluence by Atlassian (http://www.atlassian.com/software/confluence/).  You can get a hosted version of run it yourself.  It also has great integration with their issue tracking software (Jira) and software development tools (Fisheye/Crucible).


## Answer 22228

- posted by: [Robin Vessey](https://stackexchange.com/users/-1/984-robin-vessey) on 2011-03-25
- score: 2



**what are you going to do with it?**

 - Just local team of a few putting notes
 - Many spaces for many different projects 
 - Security levels required. No login, just login then see all, Down to the page level, per space security?
 - integration with other elements for Programming or Business
 - WebDAV / MS Word / Live Writer support
 - How skilled / techie are the people using it? Some have great features but are impossible to learn, others are lighter on the features but much eaiser for the average person. 

That should be a reasonable set of questions to start with.

**We have used** 

 1. Our own hand rolled one. Was great at the start but then we got really busy
 3. TWIKI which was good but suffered from "spotty nerd syndrome" ... they wouldn't provide autologin from a cookie "because its unsecure, if you want that use a different wiki".
 4. We currently use confluence which has some really good points if your using it with the rest of the atlassian suite but isn't as strong an offering on its own. Its also a bit pricy once you grow ... we had the issue where we wanted clients to be able to login and contribute to 'their areas" and the number of logins grew quickly which grew the price very quickly.

Microsoft have started offering Cloud based Sharepoint which includes Wikis and other document management solutions. It later allows you to integate with back end databases and work with .NET development environments. 

Its worth a look at as you go especially if your servicing larger corporates, the majority of whom use it.


**Host external VS internal**

We currently host our own but if we were starting again today I wouldn't bother. Too much pain and mucking around, get it hosted, pay the minor amounts and have done with it.


## Answer 22284

- posted by: [RJ Beri](https://stackexchange.com/users/-1/4960-rj-beri) on 2011-03-25
- score: 2

There are many open source wiki's out there in the wild. Make sure you list down all the features you are looking for and then start looking out for tools. My suggestion would be to use Google Sites - it's very simple and does meet the need for smaller organizations and on top of it Google hosts free for you - can't get better than that!



## Answer 22219

- posted by: [Justin C](https://stackexchange.com/users/-1/6947-justin-c) on 2011-03-25
- score: 1

<p>If you can pay a small monthly fee, take a look at the <a href="http://37signals.com/" rel="nofollow">37 signals</a> software packages. There are a few that can be paid for independently as your needs change.</p>

<p>If you want to look at the free market and you have enough tech skills to deploy it, take a look at <a href="http://www.redmine.org/" rel="nofollow">Redmine</a>. I use it for my consulting business for project management, file management, wikis, and time tracking.</p>



## Answer 22291

- posted by: [Nick ](https://stackexchange.com/users/-1/1502-nick) on 2011-03-25
- score: 1

My company uses Trac Wiki. 

I think it's free, or at least open source. It's got a bunch of other things it does as well. 

http://trac.edgewall.org/wiki/TracWiki





---

All content is licensed under the [CC BY-SA 3.0 license](https://creativecommons.org/licenses/by-sa/3.0/).
