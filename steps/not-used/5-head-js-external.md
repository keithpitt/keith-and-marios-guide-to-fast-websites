# 5 - HEAD JS Externally (CDN)

## Test Result

```
Testing http://www.giftoppr.co/
At Tue Feb 19 00:07:52 2013
10 loops
                                   Fastest   Median    Slowest   Std Dev   
---------------------------------------------------------------------------

Server performance:
Total application time             25ms      35ms      86ms      21ms      

Host latency:
cdnjs.cloudflare.com               18ms      18ms      19ms      0ms       
fonts.googleapis.com               158ms     160ms     161ms     1ms       
s3.amazonaws.com                   191ms     200ms     1158ms    297ms     
www.giftoppr.co                    251ms     274ms     395ms     38ms      

Browser performance:
Navigation Start:                  0ms       0ms       0ms       0ms       
Fetch Start:                       0ms       0ms       1ms       0ms       
Domain Lookup Start:               1ms       1ms       2ms       0ms       
Domain Lookup End:                 1ms       2ms       3ms       0ms       
Connect Start:                     11ms      11ms      12ms      0ms       
Connect End:                       236ms     245ms     246ms     3ms       
Request Start:                     236ms     245ms     246ms     3ms       
Response Start:                    557ms     573ms     956ms     115ms     
Response End:                      560ms     576ms     958ms     114ms     
DOM Loading:                       561ms     578ms     960ms     114ms     
DOM Interactive:                   959ms     974ms     1358ms    114ms     
DOM Content Loaded Event Start:    959ms     974ms     1358ms    114ms     
DOM Content Loaded Event End:      960ms     974ms     1359ms    115ms     
DOM Complete:                      5915ms    6075ms    6446ms    143ms     
Load Event Start:                  5915ms    6075ms    6446ms    143ms     
Load Event End:                    5945ms    6105ms    6475ms    143ms    
```

DOM Complete Median: 6075ms
