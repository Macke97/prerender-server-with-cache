# Prerender server with in-memory cache
A mini prerender server built with Prerender.io's Headless Chrome Node package. This one also utilizes their in-memory caching plugin.
Default port is 9000 but can be changed in `server.js`. 

See https://github.com/prerender/prerender for more configuration options and info.

## To start the server
Clone the repository:

`git clone https://github.com/Macke97/prerender-server-with-cache.git`

Then install dependencies with `npm install`

Run `npm start` to fire up the prerender server on the configured port!

Make sure you have Chrome/Chromium installed on your system!

## To use with Node.js + Express
First install the middleware:

`npm install prerender-node`

By default the prerender server will connect to the Prerender.io service. To use your local prerender server you can set the service url:

```javascript
app.use(require('prerender-node').set('prerenderServiceUrl', '<URL pointing to your prerender server>'));
```
