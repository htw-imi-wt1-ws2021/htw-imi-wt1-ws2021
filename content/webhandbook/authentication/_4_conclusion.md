---
title: 4. Conclusion
description : "Conclusion"
tags: ["conclusion", "authentication"]
---

As mentioned before, OWASP lists identification and authentication failures in its top 10 web security risks. This shows just how critical it is to implement proper authentication for a webapp to improve security. They also offer some advice on how prevent this security risk and possible attack scenarios on their website.

Simple password-based authentication is mostly used for webapps. It is easy to implement due to extensive documentation and code examples on the web. However, password have some drawback and there are a lot of possible attack strategies in addition to phishing and social engineering which make this a suboptimal authentication type. 2-factor/Multi-factor authentication or certificate authenticate thus offer additional security even though they themselves are not save from attack.

The authentication methods for webapps all have their advantages and disadvantages depending on the use case. Except for HTTP Basic and Digest all of them are valid methods to choose. What is important is to use existing, mature frameworks which provide the capabilities you need instead of trying to implement authentication on your own.