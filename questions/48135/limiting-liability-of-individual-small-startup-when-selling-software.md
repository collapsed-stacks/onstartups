## Limiting liability of individual/small startup when selling software

- posted by: [SnakeDoc](https://stackexchange.com/users/-1/25569-snakedoc) on 2013-03-21
- tagged: `legal`, `sales`, `licensing`, `liability`
- score: 5

If I make and sell some software (online if that matters), and say that software ends up causing some unexpected behavior (let's go extreme and say it deletes all data on the hard drive!). Am I liable for damages even if I license my software with Apache 2.0?

http://www.apache.org/licenses/LICENSE-2.0.html

Excerpt from Apache 2.0:

> 7) Disclaimer of Warranty. Unless required by applicable law or agreed to in writing, Licensor provides the Work (and each Contributor provides its Contributions) on an "AS IS" BASIS, WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied, including, without limitation, any warranties or conditions of TITLE, NON-INFRINGEMENT, MERCHANTABILITY, or FITNESS FOR A PARTICULAR PURPOSE. You are solely responsible for determining the appropriateness of using or redistributing the Work and assume any risks associated with Your exercise of permissions under this License.

> 8) Limitation of Liability. In no event and under no legal theory, whether in tort (including negligence), contract, or otherwise, unless required by applicable law (such as deliberate and grossly negligent acts) or agreed to in writing, shall any Contributor be liable to You for damages, including any direct, indirect, special, incidental, or consequential damages of any character arising as a result of this License or out of the use or inability to use the Work (including but not limited to damages for loss of goodwill, work stoppage, computer failure or malfunction, or any and all other commercial damages or losses), even if such Contributor has been advised of the possibility of such damages.

I live in California if this matters, but the global nature of the internet implies I might be subject to international law of some kind? Does Apache 2.0 protect in this instance? A license may state whatever it wants, this does not mean it is legal nor will hold up in a lawsuit.

PS: for those people who would reply with "yes Apache 2.0 clearly states you are not liable", be aware that most countries and states have laws that over-ride bad or invalid contractual agreements. As in, no contract nor agreement may violate or supersede a state or federal law (or international law presumably).

TO FURTHER EXPAND: It is common practice to found an LLC. or incorporate as a business and "shield" yourself from legal liability. This way your business can be sued, but you as an individual cannot (usually). This is great practice for anyone selling anything or providing any service. But for the sake of this question, I'd like to avoid any possibility of lawsuit to either myself or my startup.


## Answer 48138

- posted by: [Joel Spolsky](https://stackexchange.com/users/-1/4335-joel-spolsky) on 2013-03-21
- score: 5

Software is licensed, and the terms of the license are usually written by the software creator (you), and as long as the recipient has done something positive to accept those terms, courts generally uphold them.

Realistically, you're pretty safe. You're not planning to be insanely negligent, are you? I didn't think so. So stop worrying about this and write some code.


## Answer 48199

- posted by: [Gary E](https://stackexchange.com/users/-1/2587-gary-e) on 2013-03-25
- score: 3

<p>I am not a lawyer, but I do sell software and have been doing so for 35+ years.</p>

<p>If you are in the United states and the people buying your software are in the United States, <strong>you can not disclaim all warranties</strong> in your license. Many states follow the <a href="http://en.wikipedia.org/wiki/Uniform_Commercial_Code" rel="nofollow">Uniform Commercial Code (UCC)</a> and if your state follows that law or you sell to someone in that state that follows it, your disclaimer of all warranties is at least partially invalid.</p>

<p>In particular, under the UCC "<strong>Implied warranty of fitness</strong>—Implied warranty of fitness arises when the seller knows the buyer is relying upon the seller's expertise in choosing goods. Implied warranty of merchantability: every sale of goods fit for ordinary purposes. Express warranties: arise from any statement of fact of promise."</p>

<p>Every good software license includes the following text:</p>

<p>COMPANY DISCLAIMS ANY AND ALL OTHER WARRANTIES, WHETHER EXPRESS, IMPLIED, OR STATUTORY, INCLUDING, BUT WITHOUT LIMITATION, (i) THE IMPLIED WARRANTIES OF NONINFRINGEMENT OF THIRD PARTY RIGHTS, MERCHANTABILITY OR FITNESS FOR A PARTICULAR PURPOSE; OR (ii) THAT ANY INFORMATION ACCESSED BY THE SOFTWARE WILL BE ACCURATE OR COMPLETE. THIS WARRANTY DISCLAIMER AFFECTS YOUR LEGAL RIGHTS, AND YOU MAY ALSO HAVE OTHER RIGHTS WHICH VARY FROM JURISDICTION TO JURISDICTION. <strong>SOME JURISDICTIONS DO NOT ALLOW EXCLUSIONS OF IMPLIED WARRANTIES OR LIMITATIONS ON HOW LONG AN IMPLIED WARRANTY LASTS, SO THE ABOVE EXCLUSION MAY NOT APPLY TO YOU.</strong></p>

<p><strong>Note the last sentence.</strong> Then you come to your question about liability. The answer here depends on negligence. No LLC or corporation is likely to protect you from neligence.</p>

<p>So:</p>

<p>1) You can not disclaim all warranties everywhere. </p>

<p>2) An LLC will not protect you from outright negligence on your part.</p>

<p>For more detailed answers, check with a lawyer.</p>




---

All content is licensed under the [CC BY-SA 3.0 license](https://creativecommons.org/licenses/by-sa/3.0/).
