# Minifying Assets

CSS: 64.54kB  => 18.48KB  ( Saved 46.06KB)
JS:  379.49KB => 134.45KB ( Saved 245.04KB)
==========================
Total Saving: 291.10KB
Total Page Size: 611.75K


```ruby
# config/environments/production.rb
config.assets.compress = true
```

## Test Result

Testing http://www.giftoppr.co/
At Mon Feb 18 22:50:54 2013
10 loops
                                   Fastest   Median    Slowest   Std Dev   
---------------------------------------------------------------------------

Server performance:
Total application time             36ms      38ms      104ms     25ms      

Host latency:
fonts.googleapis.com               158ms     161ms     501ms     102ms     
s3.amazonaws.com                   190ms     193ms     542ms     139ms     
www.giftoppr.co                    234ms     274ms     343ms     34ms      

Browser performance:
Navigation Start:                  0ms       0ms       0ms       0ms       
Fetch Start:                       0ms       0ms       0ms       0ms       
Domain Lookup Start:               1ms       2ms       2ms       0ms       
Domain Lookup End:                 2ms       2ms       3ms       0ms       
Connect Start:                     11ms      11ms      12ms      0ms       
Connect End:                       235ms     246ms     255ms     6ms       
Request Start:                     235ms     246ms     255ms     6ms       
Response Start:                    553ms     606ms     912ms     98ms      
DOM Loading:                       559ms     610ms     915ms     97ms      
Response End:                      814ms     866ms     1164ms    96ms      
DOM Content Loaded Event Start:    1911ms    2491ms    3054ms    328ms     
DOM Interactive:                   1911ms    2491ms    3054ms    328ms     
DOM Content Loaded Event End:      1957ms    2536ms    3102ms    328ms     
DOM Complete:                      7281ms    8061ms    9638ms    710ms     
Load Event End:                    7281ms    8062ms    9638ms    710ms     
Load Event Start:                  7281ms    8061ms    9638ms    710ms   

DOM Complete Mean: 8061ms
