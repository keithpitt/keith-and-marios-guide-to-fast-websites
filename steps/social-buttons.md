# 8 - SPDY (Single asset domain HTTPS)

```
Testing http://www.giftoppr.co/
At Wed Feb 20 20:00:27 2013
10 loops
                                   Fastest   Median    Slowest   Std Dev   
---------------------------------------------------------------------------

Server performance:
Total application time             37ms      45ms      88ms      17ms      

Host latency:
apis.google.com                    16ms      89ms      128ms     39ms      
connect.facebook.net               4ms       108ms     663ms     245ms     
fonts.googleapis.com               156ms     207ms     266ms     39ms      
giftoppr.desktopprassets.com       19ms      60ms      600ms     164ms     
platform.twitter.com               6ms       113ms     677ms     220ms     
www.giftoppr.co                    239ms     273ms     1399ms    445ms     

Browser performance:
Navigation Start:                  0ms       0ms       0ms       0ms       
Fetch Start:                       0ms       0ms       0ms       0ms       
Domain Lookup Start:               1ms       1ms       3ms       0ms       
Domain Lookup End:                 1ms       2ms       911ms     272ms     
Connect Start:                     10ms      11ms      911ms     270ms     
Connect End:                       236ms     292ms     1163ms    264ms     
Request Start:                     237ms     292ms     1163ms    264ms     
Response Start:                    589ms     681ms     1763ms    404ms     
DOM Loading:                       593ms     685ms     1766ms    402ms     
Response End:                      596ms     685ms     1769ms    402ms     
DOM Interactive:                   1009ms    1208ms    2324ms    404ms     
DOM Content Loaded Event End:      1009ms    1208ms    2324ms    404ms     
DOM Content Loaded Event Start:    1009ms    1208ms    2324ms    404ms     
DOM Complete:                      3851ms    4716ms    6421ms    743ms     
Load Event Start:                  3851ms    4716ms    6421ms    743ms     
Load Event End:                    4213ms    5136ms    6780ms    729ms  
```

DOM Complete Median: 4716ms

