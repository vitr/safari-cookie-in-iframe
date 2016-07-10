## Safari 3rd party cookie in iframe workaround

The demo: http://vitr.github.io/safari-cookie-in-iframe/demo.html


The problem: site A (main site) loads site B (framed site) in iframe. Site B sets some cookies (e.g. store session data), to function properly.
These cookies are called 3rd party cookies, as they are not set by site A.

Safari browser on all platforms block 3rd party cookies by default.
![](https://f.cloud.github.com/assets/2770290/2116855/1142dd9c-90a3-11e3-90a6-864d9f9cdea0.png)

This is pure javascript solution to the problem. The main idea is to redirect a visitor from the main site to the framed site just for setting a cookie. After that Safari allows to set cookies in iframes for the framed site, as the site has become not a third party any more.


This is very common problem for iframed Facebook applications. Sadly, if you don't have control over site B, you can't apply this solution.

#### 2016 Update
The fix works well with recent Safari 9.1.1
![](https://camo.githubusercontent.com/f6e6a28460cc3539fc4ac1a2480a99fe981b016a/687474703a2f2f696d6167652e70726e747363722e636f6d2f696d6167652f34303063626435393834656634363931626632616539653933636231356232622e706e67)
