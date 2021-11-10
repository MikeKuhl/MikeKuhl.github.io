# Local Storage! #

- Cookies are bad (less safe?) Cookies are included with every HTTP request, thereby slowing down your web application by needlessly transmitting the same data over and over
 - Cookies are included with every HTTP request, thereby sending data unencrypted over the internet (unless your entire web application is served over SSL)

 - Cookies are limited to about 4 KB of data — enough to slow down your application (see above), but not enough
 to be terribly useful


- HTML5 Storage/Local Storage is a spec called Web Storage, or DOM Storage or Local Storage.

- HTML5 Storage is a way for web pages to store key/value pairs locally within the browser.

- you’ll access HTML5 Storage through the localStorage object on the global window object.


- HTML5 Storage is based on named key/value pairs. You store data based on a named key, then you can retrieve that data with the same key. The named key is a string. The data can be any type supported by JavaScript, including strings, Booleans, integers, or floats. However, the data is actually stored as a string. If you are storing and retrieving anything other than strings, you will need to use functions like parseInt() or parseFloat() to coerce your retrieved data into the expected JavaScript datatype.


- Calling setItem() with a named key that already exists will silently overwrite the previous value. Calling getItem() with a non-existent key will return null rather than throw an exception.

- Like other JavaScript objects, you can treat the localStorage object as an associative array. Instead of using the getItem() and setItem() methods, you can simply use square brackets.

- If you want to keep track programmatically of when the storage area changes, you can trap the storage event. The storage event is fired on the window object whenever setItem(), removeItem(), or clear() is called and actually changes something. For example, if you set an item to its existing value or call clear() when there are no named keys, the storage event will not fire, because nothing actually changed in the storage area.