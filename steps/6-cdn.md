# 6 - CDN

```
Testing http://www.giftoppr.co/
At Tue Feb 19 21:10:27 2013
10 loops
                                   Fastest   Median    Slowest   Std Dev   
---------------------------------------------------------------------------

Server performance:
Total application time             26ms      55ms      121ms     33ms      

Host latency:
a1.giftopprassets.com              16ms      17ms      474ms     137ms     
fonts.googleapis.com               158ms     159ms     161ms     0ms       
www.giftoppr.co                    235ms     249ms     538ms     100ms     

Browser performance:
Navigation Start:                  0ms       0ms       0ms       0ms       
Fetch Start:                       0ms       0ms       0ms       0ms       
Domain Lookup Start:               1ms       1ms       2ms       0ms       
Connect Start:                     10ms      11ms      23ms      3ms       
Domain Lookup End:                 1ms       2ms       23ms      6ms       
Connect End:                       237ms     238ms     257ms     6ms       
Request Start:                     237ms     238ms     257ms     6ms       
Response Start:                    513ms     546ms     756ms     73ms      
Response End:                      518ms     550ms     760ms     73ms      
DOM Loading:                       519ms     549ms     759ms     73ms      
DOM Interactive:                   917ms     939ms     1151ms    73ms      
DOM Content Loaded Event End:      917ms     939ms     1151ms    73ms      
DOM Content Loaded Event Start:    917ms     939ms     1151ms    73ms      
DOM Complete:                      1692ms    1796ms    1929ms    71ms      
Load Event Start:                  1692ms    1796ms    1929ms    71ms      
Load Event End:                    1721ms    1826ms    1959ms    71ms     
```

DOM Complete Median: 1796ms
