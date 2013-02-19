# 5 - JavaScript async loader

```
Testing http://www.giftoppr.co/
At Tue Feb 19 00:36:45 2013
10 loops
                                   Fastest   Median    Slowest   Std Dev   
---------------------------------------------------------------------------

Server performance:
Total application time             31ms      48ms      386ms     105ms     

Host latency:
fonts.googleapis.com               159ms     161ms     646ms     145ms     
s3.amazonaws.com                   191ms     206ms     813ms     195ms     
www.giftoppr.co                    252ms     269ms     411ms     43ms      

Browser performance:
Navigation Start:                  0ms       0ms       0ms       0ms       
Fetch Start:                       0ms       0ms       0ms       0ms       
Domain Lookup Start:               1ms       2ms       2ms       0ms       
Domain Lookup End:                 2ms       2ms       3ms       0ms       
Connect Start:                     11ms      11ms      12ms      0ms       
Connect End:                       238ms     246ms     252ms     3ms       
Request Start:                     239ms     246ms     253ms     3ms       
Response Start:                    547ms     611ms     1733ms    341ms     
Response End:                      569ms     613ms     1738ms    341ms     
DOM Loading:                       569ms     614ms     1737ms    340ms     
DOM Interactive:                   964ms     1008ms    2131ms    362ms     
DOM Content Loaded Event End:      964ms     1008ms    2131ms    362ms     
DOM Content Loaded Event Start:    964ms     1008ms    2131ms    362ms     
DOM Complete:                      5850ms    6133ms    7350ms    431ms     
Load Event Start:                  5850ms    6133ms    7350ms    431ms     
Load Event End:                    5880ms    6163ms    7380ms    431ms  
```

DOM Complete Median: 6133ms
