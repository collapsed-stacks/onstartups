## How are multi-lingual websites typically done?

- posted by: [TimJ](https://stackexchange.com/users/-1/1172-timj) on 2010-01-16
- tagged: `website`, `international`
- score: 1

A friend from Italy asked about setting up a website, and I am pretty sure she wants it in multiple languages.  How is that typically done?  Is there a framework in the CMSes that allows language content to be translated and then duplicated across multiple language domains?

The person who asked is multi-lingual and would be able to provide all the content. 

I think it will be a pretty simple site - and mostly static content.

NOTE

This is NOT a question about how to do translation - it is how to set up multiple languages and have the same navigation.  

Do you make multiple sites and duplicate effort, or do you have some sort of context parameter that is used to indicate the language resources that are used?

I'm not interested in speculation on how it could be done or your guess on how it is done - I would like to hear from people who KNOW.


## Answer 6630

- posted by: [Ross](https://stackexchange.com/users/-1/1390-ross) on 2010-01-16
- score: 2

Some CMS support multi lingual version of content. I can suggest to use WordPress with some appropriate plugin.
http://codex.wordpress.org/Multilingual_WordPress


## Answer 6639

- posted by: [Scott Drake](https://stackexchange.com/users/-1/2253-scott-drake) on 2010-01-16
- score: 1

If it's mostly static content, it might make sense to just do different versions. Just figure out how much time it will take to copy/paste/replace content to create the second version and how long it will take to maintain multiple versions and if that's less than how long it would take to create a programmatic solution, it might make sense. If the content is going to change a lot, this might get tedious.

Many of the modern programming environments provide some mechanisms for localization. .Net uses resource files which are basically XML docs that can be organized in different ways. You can pull the locale from the browser or set the locale you want to show, and based on that .Net will render the correct labels from the correct resource file.

So you might be able to do a simple site in one of the modern environments without a great deal of effort.

Can't speak much about CMS systems but I'm sure some out there have solved this problem. It's pretty common these days.

For an app we're building now we rolled our own solution storing localized strings in the database. This gives us a lot more control and it's easier to maintain data in the db than in resource or XML files.

My only advice is to get the site solid and polished before attempting to introduce localized versions. It's easy to make minor UI adjustments and label changes when you're just dealing with one language. Once you start dealing with multiple, adding new labels to a screen or changing them can go from a quick change to one that can take hours and involve multiple people who have to do the localization.

Also be aware that some languages are very long so the space you provide in your menus may be fine for English, but other languages can easily require much more width to communicate the same thing. You might experiment/keep that in mind as you begin working on the design.


## Answer 6618

- posted by: [Puk](https://stackexchange.com/users/-1/1859-puk) on 2010-01-16
- score: 0

If it is a purely static site then you could place all of the text content in an XML file and then call is the correct version when the page loads via java script. I had a web shop built like that a few years ago. Editing is a pain (down load language file from server, edit it, upload again) - but the text doesn't change often.

When repeating the process I opted for a multlingual CMS solution, its stil a shop so www.magenta.com proved a good solution. I can't tell you how the technical mechanism that calls the different language content into the page - but from a user perspective it is easy to use.

It sounds as though you are not building a shop, therefore multiligual CMS is probably the best route. If it were me then SiteCore (proprietary), Drupal (OS) would be on my list.



---

All content is licensed under the [CC BY-SA 3.0 license](https://creativecommons.org/licenses/by-sa/3.0/).
