## Slide Notes

#### Giftoppr Stats
- HTML:  16.80KB
- CSS:   64.54kB
- JS:    379.49KB
- Img:   442.02KB
- Total Page Size: 902.85KB

#### Before we talk about before we tweak
  - Convince your boss

#### Before we tweak
  - Latency is killer, position your servers closer
  - Bandwidth doesn't help overcome latency
  - Cookieless asset domains

#### Step 1 - Minify
  - Lots of gems available, sprockets, jammit
  - Asset pipeline
  - Saved: 291.10KB, total page size: 611.75K
  
#### Step 2 - gzip
  - on Platforms like heroku enable in rackup
  - Best to enable on web server (nginx, apache)
  - gzip static assets as well (asset_sync for asset pipeline)  
  - Saved: 115.6KB, total page size: 496.15KB
   
#### Step 3 - Compress Assets
  - ImageOptim for lossless compression
  - Strip user uploaded assets too, easy to do in carrierwave
  - Saved: 69.90KB, total page size: 426.25KB
  
#### Step 4 - Move Javascript to the bottom
  - JavaScript blocks
  - CSS also blocks but we don't want to see janky styling
  
#### Step 5 - Async Loader
  - You'll have issues with browser event (DOM ready), document.ready
  - Works best when there are multiple scripts to load in parallel
  - Does not block loading JavaScript
 
#### Step 6 - CDN
  - Clients using non local (googleDNS, openDNS) DNS servers may not get benefits.
  - Not very expensive, free ones available
  - Asset expiration, set expiry for 10 years, unique filenames (hash, digest)
  - Cookiless domains

#### Step 7 - Multiple asset subdomains
  - Browsers have a connection limit (6 per host)
  - 4x == 24 hosts
  - DNS lookup per subdomain initially, precache
  - Time was around ~3 seconds before we added precache
  - Raise DNS TTL unless you need to make changes

#### Step 8 - SPDY
  - TODO: What is spdy, be acurrate here! TODO: Write script.
  - Faster with single asset domain (uses streaming, no TCP rampup)
  - SSL for free
  - Doesn't require TLS, but usually runs over it; requires Next Pritocol Negotiation (NPN)

#### Afterwards
  - Diagram of the giftoppr setup 
  - Social media share buttons