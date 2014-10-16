##How To Check Your Browser
If you want to check that your browser changes have definitely removed SSLv3.0 support there are a couple of sites that you can use. If you visit [https://zmap.io/sslv3/](https://zmap.io/sslv3/) with SSLv3 enabled in your browser, you will see the warning message I'm getting here in Chrome where I haven't yet disabled SSLv3. To double check the site was working as expected, I disabled SSLv3 support in Internet Explorer and opened up the site there too. Here you can see the difference. 

![Chrome and IE SSLv3 test](/images/chrome-ie-sslv3-support.png)


There's also the [Qualys SSL Client Test](https://www.ssllabs.com/ssltest/viewMyClient.html) to see what your browser supports. Here is my result in Chrome with SSLv3 still enabled:

![Qualys Client Test Vulnerable](/images/qualys-client-test-vulnerable.png)


Here is the result in Internet Explorer with SSLv3 disabled:

![Qualys Client Test Not Vulnerable](/images/qualys-client-test-not-vulnerable.png)


You can also try [https://www.poodletest.com/](https://www.poodletest.com/) alongside Zmap and Qualys.
