## What are some cloud based options for a file server?

- posted by: [AvgJoe007](https://stackexchange.com/users/-1/13518-avgjoe007) on 2011-09-25
- tagged: `server`
- score: 2

Have just joined a startup that has no infrastructure at all. At the moment we are only 3, expect to grow to 10 6 months from now, then possibly another 10 a few months thereafter.

I am the only technical person in the team, but I have other more important priorities. As such, I don't want to waste time maintaining infrastructure in the office. 

Our first need is a file server. I don't want to keep one in the office due to installation and maintenance. My other 2 colleagues will be travelling a lot too.

Are there good cloud based options? We don't want to sync gigs of data across all 3 user's laptops - just want to be able to centrally store docs somewhere (thats secure too). If the solution works from Windows Explorer, thats even better as we don't want to install loads of add ons

Documents are not likely to be huge, I imagine we'd use about 250mb to start with - going up to 1Gb

Any advice?

Thanks



## Answer 30624

- posted by: [Ryan Doom](https://stackexchange.com/users/-1/5655-ryan-doom) on 2011-09-25
- score: 2

<p>Options that come to mind</p>

<ul>
<li><a href="http://www.dropbox.com/" rel="nofollow">dropbox.com</a> (easiest initally: con as you mentioned is the syncing  / traffic between the cloud and the machines since copies are on your machines and server)</li>
<li>Virtual / Hosted VPN like <a href="http://www.infinitelyvirtual.com/categories/office-virtualization/virtual-vpn-server.html" rel="nofollow">infinitely virtual</a> that you all VPN to and can then browse the remote data through explorer. All data is on their drives so when editing files it needs to go across the network</li>
<li><a href="http://www.onthenetoffice.com/" rel="nofollow">Desktop Virtualization</a></li>
<li><a href="http://www.newegg.com/Store/SubCategory.aspx?SubCategory=124" rel="nofollow">Network Attached Storage</a> you could get a nice NAS that would have redundant hard drives, supports FTP for remote access and could appear 'mounted' in explorer or with a 3rd party app. Also some of these you can update the firmware and use Jungle Disk to backup to Amazon S3 or some cloud storage. </li>
</ul>



## Answer 30633

- posted by: [strongriley](https://stackexchange.com/users/-1/13514-strongriley) on 2011-09-25
- score: 0

<p>Initially, I'd start with <a href="http://www.dropbox.com" rel="nofollow">Dropbox</a> but as you grow, you'll want more control over file access, the ability to upload larger files and more.  For that, I'd recommend <a href="http://box.net" rel="nofollow">Box.net</a> as it's more geared towards businesses where Dropbox seems more personal.</p>




---

All content is licensed under the [CC BY-SA 3.0 license](https://creativecommons.org/licenses/by-sa/3.0/).
