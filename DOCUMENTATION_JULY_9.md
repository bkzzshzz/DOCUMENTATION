##### July 9

### Today I made the login and signup pages work(~~logically~~aesthetically). The thing I did was again what I did yesterday: making every mentioned link in all the python codes and html, css and scss files relative to the root folder. That helped a lot. Then there was this issue of `.woff?v=2.2.0` and `.tff?v=2.2.0`.  First I checked if removing the texts `?v=2.2.0` made any error in the template I downloaded. But, it didn't. 

### So, I moved some files to the root folder, added `/static/` in places of `../` and removed `?v=2.2.0` from all the links within all the html, css and scss files. Then I ran the server and
```
Voila!
```
### It works! 