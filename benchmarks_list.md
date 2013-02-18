# List of benchmarks - In Order

- Minify CSS and JS (Sprockets config)
- GZip HTML (Rack middleware on heroku), Gzip JS + CSS (Sprockets config)
- Lossily compress uploaded images (jpeg, 80%), strip metadata, compress asset images (imageOptim)
- Move JS to the bottom
- Load JS with head.js externally
- Load JS with head.js on the page (make sure to note that CSS goes on top)
- Add CDN
- Multiple asset domains
- Add SPDY
