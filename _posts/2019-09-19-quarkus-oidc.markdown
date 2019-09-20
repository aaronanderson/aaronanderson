---
title:  "Quarkus OIDC"
date:   2019-09-19 22:12:07 -0500
categories: quarkus
---
 
[Quarkus OIDC] is a Quarkus extension to enact OIDC authentication redirects on set web content. 

The extension can be enabled by adding the extension as a dependency to the Maven project and adding the following lines to the application.properties file:

{% highlight java %}
quarkus.oidc.security-constraints.1.roles=Everyone
quarkus.oidc.security-constraints.1.web-resources=/*

#External IDP 
quarkus.oidc.issuer=https://someorg.okta.com
quarkus.oidc.client-id=XXXXXXXXXXX 
quarkus.oidc.client-secret=XXXXXXXXXXXXXXXXXXXXXXXXXXXXXX
{% endhighlight %}

Check out the [Quarkus]  for more details on the microservices platform.

[Quarkus OIDC]: https://github.com/aaronanderson/quarkus-oidc
[Quarkus]: https://quarkus.io/
