Safari 3rd party cookie in iframe workaround
=======================

The problem: site A (main site) loads site B (framed site) in iframe. Site B sets some cookies (e.g. store session data), to function properly.
These cookies are called 3rd party cookies, as they are not set by site A.

Safari browser on all platforms block 3rd party cookies by default.
![](https://f.cloud.github.com/assets/2770290/2116855/1142dd9c-90a3-11e3-90a6-864d9f9cdea0.png)

This is pure javascript solution to the problem. The main idea is to redirect a visitor from the main site to the framed site just for setting a cookie. After that Safari allows to set cookies in iframes for the framed site, as the site has become not a third party anymore.


This is very common problem for iframed Facebook applications. Sadly, if you don't have contorl over site B, you can't apply this solution.
