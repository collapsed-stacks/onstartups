## Can GNU GPL licensed code not be used to develop proprietary software for commercial purposes?

- posted by: [morpheus](https://stackexchange.com/users/-1/9715-morpheus) on 2011-04-16
- tagged: `gpl`
- score: 2

my understanding of GPL is that its a viral license meaning any code that derives or builds upon GPL code must itself be licensed under GPL. However, does this mean I cannot develop proprietary software for commercial purposes using GPL licensed code w/o making any modifications whatsoever to the GPL code?


## Answer 23515

- posted by: [Community](https://stackexchange.com/users/-1/-1-community) on 2011-04-16
- score: 4

Yes, you can use GPL licensed software to develop proprietary, commercial code.  Many, many companies do this.  For example, you can use Linux and GCC to create your own proprietary, commercial code.

You have to be careful when you start modifying GPL licensed code or incorporating GPL licensed code into your own code (e.g., via a library).

If you don't distribute your code (e.g., your code runs a web site) then you can modify GPL code without any further obligations (but watch out for the Affero License, which presents a different situation).

If you do distribute your code, and it derives from GPL-licensed code, then the GPL applies and you need to provide the source of your own code.


## Answer 23539

- posted by: [Community](https://stackexchange.com/users/-1/-1-community) on 2011-04-17
- score: 1

The key point is you cannot **link** GPL'ed code with your proprietary code. If you link, its GPL.

The other important point is **distribution**. If you distribute your binary to 3rd party, you have to ship the source code in GPL terms. You can perfectly produce GPL code and not ship the sources, provided you don't ship the binaries.

Disclaimer: I am not a lawyer.



---

All content is licensed under the [CC BY-SA 3.0 license](https://creativecommons.org/licenses/by-sa/3.0/).
