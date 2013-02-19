# 8 - SPDY (Single asset domain HTTPS)

```
Testing http://www.giftoppr.co/
At Wed Feb 20 00:32:12 2013
10 loops
                                   Fastest   Median    Slowest   Std Dev   
---------------------------------------------------------------------------

Server performance:
Total application time             30ms      44ms      448ms     122ms     

Host latency:
fonts.googleapis.com               158ms     161ms     162ms     1ms       
giftoppr.desktopprassets.com       16ms      18ms      19ms      1ms       
www.giftoppr.co                    236ms     397ms     449ms     82ms      

Browser performance:
Navigation Start:                  0ms       0ms       0ms       0ms       
Fetch Start:                       0ms       0ms       0ms       0ms       
Domain Lookup Start:               1ms       2ms       2ms       0ms       
Domain Lookup End:                 2ms       2ms       539ms     161ms     
Connect Start:                     10ms      12ms      539ms     158ms     
Connect End:                       236ms     246ms     803ms     167ms     
Request Start:                     237ms     246ms     803ms     167ms     
Response Start:                    524ms     627ms     1112ms    176ms     
Response End:                      529ms     662ms     1124ms    177ms     
DOM Loading:                       531ms     631ms     1125ms    178ms     
DOM Interactive:                   924ms     1023ms    1517ms    177ms     
DOM Content Loaded Event End:      924ms     1023ms    1517ms    177ms     
DOM Content Loaded Event Start:    924ms     1023ms    1517ms    177ms     
DOM Complete:                      1736ms    1856ms    2358ms    211ms     
Load Event Start:                  1736ms    1856ms    2358ms    211ms     
Load Event End:                    1766ms    1888ms    2389ms    211ms  
```

DOM Complete Median: 1856ms
