# Keith and Marios Guide to Fast Websites

## Things to do during the presentation
- Introduce ourselves.
- Let everyone know who we are (envato + desktoppr)
- List the things we ARE and aren't going to cover
- Not everything in this presentation is for everyone.
- Cost vs implementation benefit

### Why?

- Why should you care about a fast website?
- Slow websites are annoying.
- Imagine Github was super slow. Would you still use it? Probably not.
- Speed is a feature
- If you're building tools for businesses or developers, they don't have time to sit around waiting for your website to load. They have short attention spans.
- Conversions. More conversions == more money!
- It's easy to make a big difference
- Not just slow but completley inaccessible on mobiles
- **Show an example of a slow website vs a fast one (use a video)**

### Is it slow?

- Yes if it's above 100ms :D

### Latency

- How to measure it (ping!)
- Find our where your users are located and put your server there
- if your app is in the US, and you're in australia, then there you'll have latency cost to pay on every request. thats unavoidable (use cdn for assets)
- consider where your users are (show graph)
- if your customers are in Australia, why are you hosting in america? server prices are getting cheaper and cheaper in Australia

### DNS

- Pick a fast one!
- ** find a fast one to show **
- Matters for first time users, those are the ones you want to impress!

### Static Assets

- strip meta data
- compress
- cdn
- gzip
- minify
- cookieless host
- expiry headers
- Multple asset hosts
  - Example in rails
- avoid blocking on JavaScript
  * head.js
  * puts scripts last
- how ofter you change and splitting up assets and how to balance. most changed files vs least changed. ususally /app and /vendor will do fine.
- Avoid asset you don't need
  - jQuery is a good example, you don't _always_ need jquery.
- ** LOSSLESSLY COMPRESS IMAGES!!!!!!**
  - Try get an example site where we can save 100KB+	
- Consider sprites or icon font libraries
  - Compass can automatically sprite for you
- Resize images to what they're going to show at.
- Note that mobile can't cache files over x,so think about THAT!


### SSL

- Do you need it?
- Using it on parts of the app that require it (show amazon as an example) (hard) (using non secure and secure cookies)
- Using SPDY
  - Make sure enough of your users have support for it (chrome + firefox)
  - Use a single asset domain (as it streams and multiple will slow it down)
  - SSL protocols, 1024bit vs 2048 bit and why its good to be google (they can issue their own 1024bit ssl cert, but we cant get one) **show cert image**
  
### Cheating

- bootstrapping data on a page
- pages are page cached, ajax to grab the login bar (also local storage for speed, but dodgey)
- pjax and turbolinks
	- measuring is hard, but you can do it

### Caching in App server

- Hard to maintain, hard to test
- Easy to measure
- Hides real slowness
- Also Increases concurrency

### Other things to do

 - consider Remove social links
   - Show 3D Firefox of the buttons
   - Add the smashing magazine quote about removing social links.
 - Rails HTTP Streaming (difficult to serve in production, but can be useful)
 - Tune ruby on your server (may require a neck beard)