## using GREE mobile platform (aka openFeint)

- posted by: [socksocket](https://stackexchange.com/users/-1/19126-socksocket) on 2012-08-09
- tagged: `marketing`, `affiliate`, `mobile`, `android`, `traffic`
- score: 0

I uploaded two days ago my new game to the Andorid platform.  
so far, I don't have many downloads.  

I introduced with [GREE][1] which is kind of social network for mobile gamers  
I think it's something that can leverage the app's downloads.  

the problem is that GREE integration demands. you can see it in this [PDF][2]:  

    <uses-permission android:name="android.permission.WAKE_LOCK"/>
    <uses-permission android:name="android.permission.GET_TASKS"/>
    <uses-permission android:name="android.permission.ACCESS_WIFI_STATE"/>
    <uses-permission android:name="android.permission.READ_PHONE_STATE"/>
    <uses-permission android:name="android.permission.RECEIVE_SMS"/>
    <uses-permission android:name="android.permission.READ_SMS"/>
    <uses-permission android:name="android.permission.WRITE_EXTERNAL_STORAGE"/>
    <uses-permission android:name="net.gree.Sample.permission.C2D_MESSAGE"/>
    <uses-permission android:name="com.google.android.c2dm.permission.RECEIVE"/>
    <permission 
    android:name="net.gree.Sample.permission.C2D_MESSAGE" 
    android:protectionLevel="signature" >
    </ permission >

on the one hand I think it's something that can be very helpful to me, 
on the other hand, I think it can be intimidate users from downloading the game because of privacy issues.  

so, what do you think?  should I use the GREE platform?



  


  [1]: http://gree-corp.com/
  [2]: https://docs.developer.gree.net/en/assets/file/doc/en/GREEPlatformAndroidDeveloperGuide.pdf


## Answer 41185

- posted by: [Christian](https://stackexchange.com/users/-1/9952-christian) on 2012-08-09
- score: 0

Isn't it so you need to rewrite parts of your App to work with GREE? I don't know much about it and have no clue if it is worth the time you invest. After all your game is just two days online. It is like shaking an apple tree when the blossoms arrive. You should not be disappointed when nothing falls down. Before you integrate a tool like GREE I would suggest you to check if it is really bringing you benefit (not sure on that).

As to your question with privacy: if I want a game I want it to use the permissions I expect. Surely I would not expect it receives SMS or reads my SMS. Not sure what GET_TASKS is, but it make me not feel comfortable to be honest. I would be one of that guys who skip the game because of that. And I actually do things like that when some third party app wants to much information from my Facebook/Twitter account. 

Just my 2 cents. If I were you I would ask a lot of people. But again, before investing much time in this, I would even start to work on more traditional promotion ways, like Google AdWords, Viral campaigns and so on.



---

All content is licensed under the [CC BY-SA 3.0 license](https://creativecommons.org/licenses/by-sa/3.0/).
