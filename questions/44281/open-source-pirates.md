## Open-source pirates

- posted by: [ted.strauss](https://stackexchange.com/users/-1/16513-ted-strauss) on 2012-11-16
- tagged: `open-source`
- score: 0

Are there any well-known cases of open source piracy?

By that I mean cases where a developer releases their project with an open source license and someone else takes their product and markets it successfully, to the detriment of the original developer. It seems like raiding [GitHub][1] for code and pumping out cheap software is a possible business model; I'm wondering if there are well known cases of people doing that.

**Note after answer 1**

An example of the kind of scenario I'm thinking of: Company A develops their amazing open-source software (for example, [WordPress][2]) and publishes code on GitHub during development. During the alpha release of the software company B takes the code, makes a couple superficial changes, re-brands it, and then commercializes the software. Company A then has to compete with company B, and this seriously affects their bottom line.

Are there any known examples of this happening?

  [1]: http://en.wikipedia.org/wiki/GitHub
  [2]: http://en.wikipedia.org/wiki/WordPress



## Answer 44284

- posted by: [shaunhusain](https://stackexchange.com/users/-1/21651-shaunhusain) on 2012-11-17
- score: 3

<p>It depends on the licensing included in the open source project if this is legally possible or not. Some licenses leave open the possibility of taking the source and packaging it as a binary and distributing it for money without really providing any extra value.</p>

<blockquote>
  <p>4.5 How does the BSD license differ from the GNU Public license? Linux is available under the GNU General Public License (GPL), which is
  designed to eliminate closed source software. In particular, any
  derivative work of a product released under the GPL must also be
  supplied with source code if requested. By contrast, the BSD license
  is less restrictive: binary-only distributions are allowed. This is
  particularly attractive for embedded applications.</p>
</blockquote>

<p>Taken from <a href="http://www.freebsd.org/doc/en/articles/explaining-bsd/comparing-bsd-and-linux.html" rel="nofollow">http://www.freebsd.org/doc/en/articles/explaining-bsd/comparing-bsd-and-linux.html</a></p>

<p>I can't really think of any cases of software that has an open source license that does not permit redistribution as a binary without source like <a href="http://www.gnu.org/licenses/gpl.html" rel="nofollow">GPL licensed</a> software being stolen. If that were to happen the thief could be prosecuted though assuming the license is deemed valid by whatever body enforces rules where they live.</p>

<p>Also a developer who is attempting to protect their work doesn't need to post it to GitHub (or can pay for a private account).  It's fairly cheap to setup a <a href="http://en.wikipedia.org/wiki/Git_%28software%29" rel="nofollow">Git</a> server (or other <a href="http://en.wikipedia.org/wiki/Apache_Subversion" rel="nofollow">Subversion</a> system) at home with <a href="http://en.wikipedia.org/wiki/RAID" rel="nofollow">RAID</a> (mirroring the data for backup) and have a secure solution for code that you want to keep private. If someone is using GitHub, they are generally okay with people taking the code, and those who want to try and take legal recourse if someone else benefits from their work and gives them no credit then a license just needs to be included.</p>




---

All content is licensed under the [CC BY-SA 3.0 license](https://creativecommons.org/licenses/by-sa/3.0/).
