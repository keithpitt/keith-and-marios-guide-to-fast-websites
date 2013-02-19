# 6 - CDN

```
Testing http://www.giftoppr.co/
At Tue Feb 19 23:22:45 2013
10 loops
                                   Fastest   Median    Slowest   Std Dev   
---------------------------------------------------------------------------

Server performance:
Total application time             30ms      84ms      466ms     129ms     

Host latency:
a0.giftopprassets.com              16ms      17ms      21ms      1ms       
fonts.googleapis.com               156ms     160ms     161ms     1ms       
www.giftoppr.co                    233ms     243ms     586ms     110ms     

Browser performance:
Navigation Start:                  0ms       0ms       0ms       0ms       
Fetch Start:                       0ms       0ms       0ms       0ms       
Domain Lookup Start:               1ms       1ms       2ms       0ms       
Domain Lookup End:                 1ms       2ms       3ms       0ms       
Connect Start:                     10ms      11ms      12ms      0ms       
Connect End:                       235ms     245ms     246ms     4ms       
Request Start:                     235ms     245ms     246ms     4ms       
Response Start:                    524ms     629ms     1110ms    196ms     
Response End:                      527ms     634ms     1113ms    196ms     
DOM Loading:                       530ms     634ms     1116ms    196ms     
DOM Interactive:                   924ms     1028ms    1504ms    195ms     
DOM Content Loaded Event End:      924ms     1028ms    1504ms    195ms     
DOM Content Loaded Event Start:    924ms     1028ms    1504ms    195ms     
DOM Complete:                      1697ms    2079ms    2378ms    224ms     
Load Event Start:                  1697ms    2079ms    2378ms    224ms     
Load Event End:                    1726ms    2108ms    2406ms    223ms   
```

DOM Complete Median: 2079ms
