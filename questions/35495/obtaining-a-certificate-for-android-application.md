## Obtaining a certificate for Android Application

- posted by: [Hank](https://stackexchange.com/users/-1/16098-hank) on 2012-01-31
- tagged: `android`
- score: 1

As a potential start up that is releasing an Android application, I need to sign the application with a certificate. I'm wondering if I should use a self-signed certificate or should I use a certificate signed by a certificate authority?

If I should use the latter, what is process for obtaining a certificate and getting it signed by a certificate authority?


## Answer 35497

- posted by: [Zuly Gonzalez](https://stackexchange.com/users/-1/2692-zuly-gonzalez) on 2012-01-31
- score: 3

<p>According to the <a href="http://developer.android.com/guide/publishing/app-signing.html" rel="nofollow">Android developer site</a>, you can use self-signed certificates to sign your applications. No certificate authority is needed. To quote the site:</p>

<blockquote>
  <p>The certificate does not need to be signed by a certificate authority: it is perfectly allowable, and typical, for Android applications to use self-signed certificates.</p>
</blockquote>

<p>As far as the process for signing your application, take a look at the link I provided. That page has a ton of information regarding signing your application. Here's an excerpt:</p>

<blockquote>
  <p>When you build in release mode you use your own private key to sign your application. If you don't have a private key, you can use the Keytool utility to create one for you. When you compile your application in release mode, the build tools use your private key along with the Jarsigner utility to sign your application's .apk file. Because the certificate and private key you use are your own, you will have to provide the password for the keystore and key alias.</p>
</blockquote>

<p>If you were developing a Windows application I would say that using a certificate authority is a must, since the end user receives a terrible warning without it. However, Android doesn't warn end users in that way.</p>

<p>Here's a <a href="https://groups.google.com/a/googleproductforums.com/forum/#!category-topic/android-market/technical-help/lIWTntG8hXs" rel="nofollow">Google Groups thread</a>, which mentions the same thing.</p>

<p>If you still want to pursue purchasing a code-signing certificate from a trusted source, the process is fairly straightforward. </p>

<ol>
<li>Find a vendor that can supply you with an Android compatible certificate.</li>
<li>Purchase the certificate.</li>
<li>Supply the vendor with the requested documentation to prove you are who you say you are.</li>
<li>Read the Android documentation to learn how to properly sign your application with your purchased certificate.</li>
</ol>



## Answer 35540

- posted by: [Casandra](https://stackexchange.com/users/-1/16125-casandra) on 2012-02-01
- score: 0

The Android Application should have the certificate's like SSL certificate's because these day's The Android Apps are causing major security problem in mobile industry.So it has to build with more security options.



---

All content is licensed under the [CC BY-SA 3.0 license](https://creativecommons.org/licenses/by-sa/3.0/).
