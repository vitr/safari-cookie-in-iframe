Safari 3rd party cookie in iframe workaround
=======================

Safari browser on all platforms block 3rd party cookies by default.
![](https://f.cloud.github.com/assets/2770290/2116855/1142dd9c-90a3-11e3-90a6-864d9f9cdea0.png)

This is pure javascript solution to the problem. The main idea is to redirect a visitor from the main site to the framed site just for setting a cookie. After that Safari allows to set cookies in frames for the framed site, as the site has become not a third party site anymore.


