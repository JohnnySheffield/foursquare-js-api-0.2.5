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
