#cookie

## Cookie properties (source)




| type | name | Explanation |
| :----------- | :------: | ------------: |
| string | name | The name of the cookie |
| string | value | The value of the cookie. |
|string	|path	|The path of the cookie.|
|boolean| secure	|True if the cookie is marked as Secure (i.e. its scope is limited to secure channels, typically HTTPS).|
|boolean| httpOnly	|True if the cookie is marked as HttpOnly (i.e. the cookie is inaccessible to client-side scripts).|
|boolean | session| True if the cookie is a session cookie, as opposed to a persistent cookie with an expiration date.|
|double|	(optional) expirationDate | The expiration date of the cookie as the number of seconds since the UNIX epoch. Not provided for session cookies.|
|string|	storeId| The ID of the cookie store containing this cookie, as provided in getAllCookieStores().|
