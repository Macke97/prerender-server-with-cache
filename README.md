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

# Copyright

The MIT License (MIT)

Copyright (c) 2013 Todd Hooper <todd@prerender.io>

Permission is hereby granted, free of charge, to any person obtaining a copy of this software and associated documentation files (the "Software"), to deal in the Software without restriction, including without limitation the rights to use, copy, modify, merge, publish, distribute, sublicense, and/or sell copies of the Software, and to permit persons to whom the Software is furnished to do so, subject to the following conditions:

The above copyright notice and this permission notice shall be included in all copies or substantial portions of the Software.

THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND, EXPRESS OR IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY, FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM, OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE SOFTWARE.
