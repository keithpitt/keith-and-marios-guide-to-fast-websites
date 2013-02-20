## Slide Notes

### Giftoppr Stats
- HTML:  16.80KB
- CSS:   64.54kB
- JS:    379.49KB
- Img:   442.02KB
- Total Page Size: 902.85KB

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
  - Easier to manage than loading at the bottom
  - Works best when there are multiple scripts to load in parallel