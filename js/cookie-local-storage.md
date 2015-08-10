https://github.com/carhartl/jquery-cookie

Create session cookie:

$.cookie('name', 'value');

Create expiring cookie, 7 days from then:

$.cookie('name', 'value', { expires: 7 });

Create expiring cookie, valid across entire site:

$.cookie('name', 'value', { expires: 7, path: '/' });

Read cookie:

$.cookie('name'); // => "value"
$.cookie('nothing'); // => undefined

Read all available cookies:

$.cookie(); // => { "name": "value" }

Delete cookie:

// Returns true when cookie was successfully deleted, otherwise false
$.removeCookie('name'); // => true
$.removeCookie('nothing'); // => false

// Need to use the same attributes (path, domain) as what the cookie was written with
$.cookie('name', 'value', { path: '/' });
// This won't work!
$.removeCookie('name'); // => false
// This will work!
$.removeCookie('name', { path: '/' }); // => true
