gitimg ![gitimg](http://dev.gitimg.com:8080/views/gitimg/1.png)
======


Tests


## These tests redirect to the http image on github http://raw.github.com/blak3r/yaai/master/SugarModules/modules/Asterisk/include/call_transfer-blue.png
### http:// blakerobertson.com/
![Test1](http://www.blakerobertson.com/http_test_301_to_github)

This test is interesting... because it works fine in a browser... but not when put into a SRC tag.  

This fails because github attempts to host any "http" image on a CDN.  
```
Request URL:https://a248.e.akamai.net/camo.github.com/a59fd20f6cd0dd641b9c0b59968ef99bf4cbe867/687474703a2f2f7777772e626c616b65726f62657274736f6e2e636f6d2f687474705f746573745f3330315f746f5f676974687562
Request Method:GET
Status Code:404 Not Found
```

And the code that retreives the image apparently doesn't follow the redirects to get the ultimate image.


### blake.squarespace 
![Test1](https://blake.squarespace.com/http_test_301_to_github)


## Now testing destination is SSL

### http --> 301 --> https on github
![Test1](http://www.blakerobertson.com/http_test_301_to_github)

### valid https --> 301 --> https    (blake.squarespace)
![Test1](https://blake.squarespace.com/https_test_301_to_github)





