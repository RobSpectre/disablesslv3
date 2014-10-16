##How To Check Your Server 
The easiest and probably the most widely used method to test anything to do with your SSL setup is the [Qualys SSL Test](https://www.ssllabs.com/ssltest/index.html). Simply navigate to the site, enter the domain for the website you want to test and hit submit to start the test. 

![Qualys insert domain](/images/qualys-domain-name.png)


Once the test has finished, you will get a nice summary of your results and a lot of detailed information further down the page. Specifically, you want to look in the Configuration section at your supported protocols. 

![Qualys protocols](/images/qualys-configuration.png)


What you want to see here is that you have *no* SSL protocols supported. You should have long since disabled SSLv2.0 and now we've just removed SSLv3.0 too. Supporting TLSv1.0 or better is good enough to support the absolute vast majority of internet users out there without exposing anyone to unecessary risk.
