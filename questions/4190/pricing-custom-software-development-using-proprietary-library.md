## Pricing Custom Software development using proprietary library

- posted by: [Community](https://stackexchange.com/users/-1/-1-community) on 2009-11-26
- tagged: `pricing`
- score: 0

One of our clients wants to hire us for writing a complex custome software.  We wants to build this on a proprietary library we wrote which abstracts lot of the complexity of the target platform. We are a startup and we agreed to put this library in an escrow so client can get access to it if we go down. We will be providig the source code for the custom software we are coding.  But the client who does not understand software licensing and pricing models is confused about all this. They want the source code for our propreitary library too we have spent ovew six months building and perfecting and that we have licensed to other clients. They know they are new to all this and are open to looking at publicly available case studies. Any advice on how to approach this?


## Answer 33004

- posted by: [Sergei Veinberg](https://stackexchange.com/users/-1/14491-sergei-veinberg) on 2011-11-25
- score: 2

The advice I received once for a similar situation was to put as much "legal" distance between your custom software development and the underlying product. If the library is a bona fide product, available to public, with its own website and client list, there is little argument that you shall not give the right to the software.

A good example of a company in this position is dhtmlx.com which makes, in my view, the best UI framework for web-based business systems. In addition to that, they do custom software development. However, the nature and the size of their product and the number of uses leaves little doubt that about code ownership for the custom systems.

As a last resort, you can agree to license the source code to them, ie:

 - they recognize that you retain the full ownership to the component library
 - grant them a non-exclusive, non-transferable, perpetual license to use and modify its source code.
 - they agree to treat the source code as confidential information and protect it as such
 - if they modify the source code, any warranties regarding system performance are void




## Answer 4191

- posted by: [Dane](https://stackexchange.com/users/-1/1441-dane) on 2009-11-27
- score: 1

You should explain to them that the software you are writing is based on a commercial component that you have developed and you are including only an object code license to it.  Then provide a price on acquiring the source code which is additional.  This allows them to make a business decision on whether they actually need the source code.

When we use libraries we often ask the vendor to add in a clause that gives us the option, for a price, to purchase the source code.  We do this because someday we might have to port it to a platform the vendor does not want to support.  This gives us a level of comfort.  This is another way to give the customer the secure feeling they need without having to come up with more money up front.

In general, understand there could be reasons they want the code you did not think of yet so just ask them, provide them options and you'll get through it.



---

All content is licensed under the [CC BY-SA 3.0 license](https://creativecommons.org/licenses/by-sa/3.0/).
