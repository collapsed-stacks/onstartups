## Selling app containing open source package

- posted by: [NurNE](https://stackexchange.com/users/-1/12335-nurne) on 2012-04-20
- tagged: `open-source`, `software-licensing`
- score: 1

I'm building an app that contains an open source package protected under EDL license

http://www.eclipse.org/org/documents/edl-v10.php

Can I sell it?
Do I need to specify something in *my* app's license?
Do I need to give it away as open source also?



## Answer 38400

- posted by: [Christian](https://stackexchange.com/users/-1/9952-christian) on 2012-04-20
- score: 4

You can sell it. It is a permissive license. 

If you sell it and use a binary format to distribute, you better read this:

"Redistributions in binary form must reproduce the above copyright notice, this list of conditions and the following disclaimer in the documentation and/or other materials provided with the distribution."

This means, you should add a NOTICE file and a LICENSE file (or something similar) to your distribution. THe Notice file says something like: "includes software by xxx licensed with yyy see LICENSE". And the LICENSE file should contain the actual license.

Please ask a lawyer for details. OS regulations are not easy and differs from country to country. But the direction should be fine.



---

All content is licensed under the [CC BY-SA 3.0 license](https://creativecommons.org/licenses/by-sa/3.0/).
