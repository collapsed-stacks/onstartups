## Violating US patents by having servers or domain name registered in the US

- posted by: [fobo](https://stackexchange.com/users/-1/14341-fobo) on 2011-11-10
- tagged: `patent`
- score: 2

Following this question:

http://answers.onstartups.com/questions/32442/what-to-do-before-offering-e-services-from-eu-to-us

I have another one:

A concern has been raised that if you have your servers in the US you may infringe a US patent. Is it really what it takes to just take the server out of the US to get clean?

What about having a domain name registered by a US registrar. Does this trigger the mechanism as well?


## Answer 32460

- posted by: [Kekito](https://stackexchange.com/users/-1/5898-kekito) on 2011-11-10
- score: 4

<p>Wikipedia explains the basic idea:</p>

<blockquote>
  <p>Patents are territorial, and infringement is only possible in a
  country where a patent is in force. For example, if a patent is filed
  in the United States, then anyone in the United States is prohibited
  from making, using, selling or importing the patented item, while
  people in other countries may be free to make the patented item in
  their country.</p>
</blockquote>

<p>And this is the relevant US law:</p>

<blockquote>
  <p>(a) Except as otherwise provided in this title, whoever without
  authority makes, uses, offers to sell, or sells any patented
  invention, within the United States, or imports into the United States
  any patented invention during the term of the patent therefor,
  infringes the patent.  35 USC 271.</p>
</blockquote>

<p>The place that the domain name is registered does not have any relevance to the issue of patent infringement.  What matters is the location of the infringing actions.</p>

<p>There are some complications though.</p>

<p><strong>1. What if the patent infringement takes place partly in the US (eg, by your customer)?</strong></p>

<p>It depends on the kind of patent claim.  </p>

<p>For a method claim, all of the steps of the method have to be performed in the US.  If just one step is performed outside the US, then there is no infringement of a US patent.  "A process cannot be used "within" the United States as required by section 271(a) unless each of the steps is performed within this country."  <a href="http://scholar.google.com/scholar_case?case=12741229581232708370" rel="nofollow">NTP v. RIM</a>.</p>

<p>For a system claim, there can only be infringement if the place of the system is in the US.  This is can be fuzzy when the system spans more than one country, and in this instance, the system is located at "the place at which the system as a whole is put into service, i.e., the place where control of the system is exercised and beneficial use of the system obtained."  See <a href="http://scholar.google.com/scholar_case?case=12741229581232708370" rel="nofollow">NTP v. RIM</a>.</p>

<p><strong>2. What if your actions outside the US cause someone else to infringe the patent inside the US?</strong></p>

<p>The above all covers direct infringement of a patent -- where you do the actual infringement.  There is also a notion of indirect infringement, more specifically induced infringement and contributory infringement.</p>

<p>Induced infringement is where you induce someone else to infringe a patent.  Contributory infringement is where you supply a (non staple) component of a patented invention to someone else who then builds the invention.  </p>

<p>Note that you can only be liable for indirect infringement of there is someone else who is liable for direct infringement. So if you can avoid direct infringement using the information in the previous section, then you probably avoid indirect infringement as well.</p>

<p>There is a lot of details to these, but hopefully this is enough to give you the general idea.</p>




---

All content is licensed under the [CC BY-SA 3.0 license](https://creativecommons.org/licenses/by-sa/3.0/).
