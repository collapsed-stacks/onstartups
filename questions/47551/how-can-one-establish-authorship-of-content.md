## How can one establish authorship of content?

- posted by: [jontyc](https://stackexchange.com/users/-1/15178-jontyc) on 2013-02-20
- tagged: `intellectual-property`
- score: 0

For a startup creating content for syndication, what is an effective way to establish that the content was indeed created by the startup and not those receiving it?

For example, one could print out or burn the content and mail it to oneself, storing the postmarked enveloped unopened. But with a constantly growing library of content, this becomes too impractical.

An wayback machine such as archive.org would work for public webpages, but this content is stored in a database and is not to be accessible publicly.







## Answer 47601

- posted by: [jimg](https://stackexchange.com/users/-1/2380-jimg) on 2013-02-21
- score: 1

<p>Why not use version control? Git, mercurial, subversion can be used.  Or you could go with a document repository model like what <a href="https://confluence.ucop.edu/display/Curation/Home" rel="nofollow">california digital library</a> uses. Or <a href="http://www.alfresco.com/" rel="nofollow">alfresco</a> or other document management systems. All can establish origin.  </p>



## Answer 47599

- posted by: [Tim Nash](https://stackexchange.com/users/-1/7035-tim-nash) on 2013-02-21
- score: 0

A very techie response would be to create a time sensitive salt ideally by a third party (so they hold the salt and the authenticity of the salt) which is then used to hash the entire content which is then stored on another third party. In effect you then have a system if their is any doubt you simply retrieve the salt from third party 1 and the hash from party 2 and then hash the disputed content and see if it matches. This obviously will only work for unmodified work.

Not sure the practicalities would be and you are reliant on multiple custodians, but would be more scalable and assuming the independence of the third parties possibly more reliable then mailing yourself.



---

All content is licensed under the [CC BY-SA 3.0 license](https://creativecommons.org/licenses/by-sa/3.0/).
