## Is security a major concern with Enterprise grade cloud storage?

- posted by: [Joe](https://stackexchange.com/users/-1/1081-joe) on 2010-08-27
- tagged: `saas`, `data`
- score: 2

In your opinion or experience, is security the biggest concern when considering offsite cloud storage?  I am curious if vendors like box.net offer their cloud solutions with the intention that businesses are able to put sensitive data such as payroll and human resources on the cloud.  Is this even practical?  


## Answer 13741

- posted by: [Dror](https://stackexchange.com/users/-1/1057-dror) on 2010-08-27
- score: 3

There's security and there's privacy. The two aren't the same. Looks like you're asking about privacy.

The simple solution if you want to put sensitive data in the cloud is to encrypt it before it goes out. That way, you're not relying on the provider's good intentions or abilities. Here's an example of a solution that handles this correctly: https://spideroak.com/engineering_matters#true_privacy


## Answer 13733

- posted by: [JeffO](https://stackexchange.com/users/-1/1796-jeffo) on 2010-08-27
- score: 1

Data storage in the cloud is more likely to be attacked like @Prix mentioned, but I'm sure their system is much more secure than the office clerk that takes home the bonus spreadsheet on a thumb drive and works on it at home on a PC that has 50 infections from facebook, warcraft, and various porn sites (That I'm sure no one there ever visited.).


## Answer 13736

- posted by: [Mike](https://stackexchange.com/users/-1/3475-mike) on 2010-08-27
- score: 1

The CIA triad for data security is Confidentiality, Integrity, and Availability. 

**Confidentiality** is soluble: store the data in encrypted form and don't give the storage provider the key. 

**Integrity** = can we trust the storage provider to do their job and not lose or corrupt the data, get their disk drives seized by the government, or go out of business.

**Availability** is a far greater worry (for me): if something is somewhere in the cloud can I reliably get it when it is needed. The network is not under my control, nor under the control of the storage provider. If there are problems with the network, I'm really at the mercy of an unknown set of communication companies. 






## Answer 17458

- posted by: [Rory Alsop](https://stackexchange.com/users/-1/5784-rory-alsop) on 2010-12-06
- score: 0

I agree with Mike on the 'CIA' triad, but in addition, something you will need to look at if you are storing any personal data in the cloud is the location of your data.

If it is UK personal data you can use an EU wide cloud in most cases, but if the cloud is global you could be in trouble. Equally for the US, various regulationss will explicitly require you to know where your data is.

From a forensics perspective - e-Discovery can become tricky if you don't know explicitly where the data might be. Similarly when responding to a freedom of information request, you are under an obligation to provide the data you have.

From an audit perspective, segregation of duties becomes a much bigger issue - with data, services or applications hosted 'in the cloud' how can you be sure the support for front and back office infrastructure aren't the same team?

Now some enterprise grade clouds are selling premium services which do meet most of these requirements, but you typically pay extra for them.

Where there is a high degree of business risk, reputational risk, or regulatory pressure what I am seeing more commonly with Fortune 350 companies is the use of private clouds, with public clouds only used for lower risk services.



---

All content is licensed under the [CC BY-SA 3.0 license](https://creativecommons.org/licenses/by-sa/3.0/).
