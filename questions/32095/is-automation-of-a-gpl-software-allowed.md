## is automation of a GPL software allowed

- posted by: [Ryan](https://stackexchange.com/users/-1/12068-ryan) on 2011-10-31
- tagged: `gpl`
- score: 1

if there is a batch software released under the GPL, can I create a services that calls that batch and uses it's output?I do not go into the source code of the program, I just call the batch file


## Answer 32103

- posted by: [Kekito](https://stackexchange.com/users/-1/5898-kekito) on 2011-10-31
- score: 2

Yes, it is allowed as long as you comply with the other provisions of the GPL license, and there are different GPL licenses so it would be helpful if you named the particular license.

For GPL2 and GPL3. the most significant limitation is that if you modify and distribute the GPL'ed software then you need to make your modifications available to others.  If you are not distributing then, you don't have to worry about this limitation.  For example, if you use GPL'ed software on the backend of your website and don't distribute the software, then you are ok.

Note that GPL3 also has patent implications that you should be aware of

Be careful of the Affero GPL license, as this one has obligations even if you don't distribute the GPL'ed software.



---

All content is licensed under the [CC BY-SA 3.0 license](https://creativecommons.org/licenses/by-sa/3.0/).
