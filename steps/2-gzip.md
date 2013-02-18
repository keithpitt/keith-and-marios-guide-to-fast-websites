# Minifying Assets

```ruby
# config.ru
use Rack::Deflater

# config/initializers/asset_sync.rb
AssetSync.configure do |config|
  config.gzip_compression = true
end

```

## Test Result

Testing http://www.giftoppr.co/
At Mon Feb 18 23:00:17 2013
10 loops
                                   Fastest   Median    Slowest   Std Dev   
---------------------------------------------------------------------------

Server performance:
Total application time             35ms      55ms      99ms      21ms      

Host latency:
fonts.googleapis.com               158ms     159ms     162ms     1ms       
s3.amazonaws.com                   192ms     208ms     1209ms    334ms     
www.giftoppr.co                    272ms     274ms     276ms     1ms       

Browser performance:
Navigation Start:                  0ms       0ms       0ms       0ms       
Fetch Start:                       0ms       0ms       0ms       0ms       
Domain Lookup Start:               1ms       2ms       2ms       0ms       
Domain Lookup End:                 1ms       2ms       3ms       0ms       
Connect Start:                     10ms      11ms      13ms      0ms       
Connect End:                       236ms     245ms     250ms     4ms       
Request Start:                     236ms     245ms     250ms     4ms       
Response Start:                    528ms     628ms     19518ms   5661ms    
Response End:                      530ms     631ms     19521ms   5661ms    
DOM Loading:                       531ms     634ms     19522ms   5661ms    
DOM Interactive:                   1392ms    1620ms    20938ms   5916ms    
DOM Content Loaded Event Start:    1392ms    1620ms    20938ms   5916ms    
DOM Content Loaded Event End:      1441ms    1666ms    20984ms   5916ms    
Load Event End:                    6613ms    7390ms    27257ms   6122ms    
DOM Complete:                      6613ms    7390ms    27257ms   6122ms    
Load Event Start:                  6613ms    7390ms    27257ms   6122ms  

DOM Complete Median: 7390ms
