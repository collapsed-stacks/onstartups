## How to get permission/integrate with ERP legally?

- posted by: [katit](https://stackexchange.com/users/-1/11093-katit) on 2011-07-01
- tagged: `legal`, `recommendations`, `competition`, `proposal`
- score: 2

I created my own product(P) which is pretty much standalone but would benefit a LOT if it integrates with existing ERP package(ERP). Integration can be done 2 ways:

 - read only where I pull data from ERP
 - two way where I will write back to
   ERP but that is not necessary

My first client already uses P and likes it a lot. Especially that he had P that was built-in into ERP :) If I integrated my P into same ERP that would make it lot more valualbe.

Here is facts. There is a lot of similar P modules. Some of them integate with ERP. Some of them integrate with multiple ERP's. ERP legal note says that nobody can pull data from their DB without written permission...

Technically, I don't see why company that owns ERP will not allow me to integrate but I have "small guy" fear. I'm 1 person company right now and not sure how and who I need to talk to. My client is a big account with ERP and they going to drop their P subscription soon.

Questions:

 - What the best approach to get permission from ERP to allow me to
   integrate? 
 - Who should I contact?
 - What should I say? Should I ask for
   permission or make proposal?
 - When should I do it? Before or after
   my client cancels?
 - Should ERP company know I already
   took their client? Any other advice
   on this matter?

Product is ready. Now I just need to get it out.

EDIT:

This is in US. ERP is client-server installed on clients hardware.
Here is legal excerpt(s):

Software may be used only by the User for internal business purposes. Unless
specifically authorized by COMPANY in writing, Software may not be used by
subsidiaries or affiliates of the User, and may not be used by a third party or by
User for any third party. User is not authorized to sub-license Software in whole or
part. **User agrees not to resell or otherwise transfer to a third party any data
extracted from the database portion of the Software**.

Software is the valuable exclusive property of COMPANY and is protected by
applicable U.S. copyright law and international treaty provisions. Software may
not be copied, decompiled, reverse assembled or disassembled without the express
written authorization of COMPANY. **User agrees not to use a software program
other than those provided by COMPANY to extract data from the database portion of
the Software unless otherwise authorized by COMPANY in writing**.


## Answer 27004

- posted by: [Robin Vessey](https://stackexchange.com/users/-1/984-robin-vessey) on 2011-07-01
- score: 1

Ouch, well that is an unusal clause in the contract ... in theroy the data should be owned by your client, and they should be free to use it however they see fit.

If your approaching the ERP company themselves I would target the technical staff VIA your mutual client. If the request is coming from your client the ERP company are far more likely to listen becuase its their client they are keepning happy. I would target either sales or technical staff, sales will want to keep a good rapore and technical generally will want to help or at least point you in the right direction.

If you can ask your client to ask if there is an API or method of extracting data so they can integrate their surronding processes to the ERP system. You need to make the ERP company focus on the fact that this will bind them into the clients processes closer ... thus they will continue to get the service fees for many years to come because they won't be replaced ... this is most likely you key leverage point with the ERP company.

Your one **maybe** way around it is to ask your client to write a view layer in a 3rd database, managed by them, (you could provide a very close template for them to work off). You then hook to views provided by your client to data they own. BUT becareful (I'm not a lawyer) and it is a last resort measure. 




---

All content is licensed under the [CC BY-SA 3.0 license](https://creativecommons.org/licenses/by-sa/3.0/).
