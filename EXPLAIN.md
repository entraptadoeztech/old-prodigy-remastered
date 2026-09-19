# **Quick Overview**
In this project, we are pulling game assets from another Github repository(bpog's) **but** standard network requests to it will be **blocked**.
So a clever solution to this is to use *[jsDelivr](https://www.jsdelivr.com/)* because jsDelivr is a Content Delivery Network that is trusted by many, which it is likely not to be blocked.
## Network Side(skip if you want)
<img src="src/assets/prod.png" alt="pic of prodigy's network requests">
  
This shows the **[XHR](https://nhimg.org/glossary/xhr-requests/)** requests sent to Prodigy's CDN when we interact with the game.
## More About This
If a network admin were to block XHR requests to a website(*which they do lol*), the website assets will not load **but** since we used **[libcurl.js](https://github.com/ading2210/libcurl.js)** *it bypasses the network blocks.*

<img src="src/assets/lib.png" alt="libcurl's proxied XHR requests to prodigy's CDN">
This shows the XHR requests when libcurl.js is used.
