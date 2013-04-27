#Foursquare-js-api-0.2.5


Foursquare-js-api is a standalone javascript wrapper for the Foursquare Api (v2). Using this api you can currently access all available endpoints.


##Questions, issues & feature requests

Questions are preferred to be posted in the google group set up for this project; http://groups.google.com/group/foursquare-js-api
Issues and feature requests can be posted as an issue.

##Version 0.2 released (Feb 01, 2012)

This version of the library alters all methods in such a manner that the applications build upon the older versions may not work anymore.

- Refactored methods - Added few examples
- Now using window.localStorage when available to store credentials.
- Fixed issue with DOM Exception 18 for mobile browsers.
- Updated venuesClient to have all the latest endpoints available.
- Added managed example for venues endpoint.

###Example

```javascript
var client = new FourSquareClient("<client_id>", "<client_secret>", "<redirect_uri>", "<remember_credentials>");

client.venuesClient.venues("<venue_id>", {
       onSuccess: function(data)
       {
            // do something with the response
            // actual object data is inside: data.response
       },
       onFailure: function(data)
       {
            // the request failed
       }
});
```

###Check here for more info

http://code.google.com/p/foursquare-js-api/

http://code.google.com/u/103190085207404134448/


###License


The MIT License

Copyright (c) 2011 M.F.A. ten Veldhuis

Permission is hereby granted, free of charge, to any person obtaining a copy
of this software and associated documentation files (the "Software"), to deal
in the Software without restriction, including without limitation the rights
to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
copies of the Software, and to permit persons to whom the Software is
furnished to do so, subject to the following conditions:

The above copyright notice and this permission notice shall be included in
all copies or substantial portions of the Software.

THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND, EXPRESS OR
IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY,
FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE
AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN
THE SOFTWARE.
