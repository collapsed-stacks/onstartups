## Does code-signing a software app improve the conversion rate?

- posted by: [jitbit](https://stackexchange.com/users/-1/4407-jitbit) on 2011-02-10
- tagged: `software`, `conversion`
- score: 10

My [small software company][1] ships both SaaS and downloadable versions of software. I was wondering if signing the "downloadable" apps with a code-signing certificate will improve conversions?

Well, I know it **will** (at least by removing the Windows' warning messages), but the question is - how much? Is that improvement worth chasing?


  [1]: http://www.jitbit.com/


## Answer 20077

- posted by: [Gary E](https://stackexchange.com/users/-1/2587-gary-e) on 2011-02-10
- score: 11

We have been code signing all of our executables for **years**. Windows warnings on non-signed executables grow more dire with each new release. Windows 7 warns you **every** time you start an installed program (that isn't signed)!

Comodo lets resellers handle their code signing certificates and you can find great bargins out there. We paid under $200 for a 3 year certificate. And when you code sign an executable you always time stamp it, so the signing stays valid even after your certificate has expired.

Finally, code signed programs have a hidden advantage. Once you code sign a file, if that file gets modified, the code signing for that file is invalid. So if your customer claims he installed your program and it gave his computer a virus, trojan, or another related problem- you ask them to right click on the file and check the code sign status. If the file is not code signed- their computer modified your program. If it is still code signed, you can easily scan it for a problem.

Note you need to code sign **all** executables in your package. You code sign the program itself, the installer, and if you deilver it on a CD with a menu system- that program too.

Note added Oct 1, 2011- Windows 8 will have a new feature (that also requires new hardware). Basically in Windows 8 a user will have the option to have the computer **hardware** check the digital certificates of every module, dll, and exe that loads at boot time. No signature means no boot.


## Answer 20105

- posted by: [ShaneG](https://stackexchange.com/users/-1/3074-shaneg) on 2011-02-11
- score: 0

Code signing is a great idea and should be done wherever possible (including enforcing SSL for access to your website - certainly any parts that can be accessed after login). It limits the opportunity for your application to be used as an infection vector for a start. Even if you self sign (not using a known and registered CA) the benefit is great.

If you have an application that may be included in an SOE it may not be acceptable unless it is signed.

Regards,
ShaneG



---

All content is licensed under the [CC BY-SA 3.0 license](https://creativecommons.org/licenses/by-sa/3.0/).
