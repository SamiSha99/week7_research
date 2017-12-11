# week7_research

## What are local storage and session storage and what is the difference between the two?

localStorage: Stores data with no expiration date, and gets cleared only through JavaScript, or clearing the Browser Cache / Locally Stored Data.

sessionStorage: Similar to localStorage but expires when the browser closed (not the tab).

## Why would you use cookies vs local/session storage?

Cookies stores data that has to be sent back to the server with subsequent requests. Its expiration varies based on the type and the expiration duration can be set from either server-side or client-side (normally from server-side).

Cookies are primarily for server-side reading (can also be read on client-side), localStorage and sessionStorage can only be read on client-side.

Despite that, the size must be less than 4KB, and can be secured by setting the HttpOnly flag as true for that cookie which will prevent client side access to it.

Local/session storage bring something different to the table like the storage limit is far bigger than cookies, Session has a limit 5MB, in some cases like Session storage which data is never transfered unlike Cookies.

 |Type           |Cookies     |localStorage  |  sessionStorage|
 |--------------:|-----------:|-------------:|---------------:|
 |Capacity       |         4kb|          10mb|           5mb|
 |Browser        | HTML 4/5   | HTML 5       |         HTML 5|
 |Expires        | Manually Set| Never| On tab close|
 |Storage        | Browser & Server| Browser Only| Browser Only|
 |Sent with request| Yes| No | No|
 
## localStorage and sessionStorage property and methods
* __length__ - property
* __clear()__ - method
* __key()__ - method
* __getItem()__ - method
* __setItem()__ - method
* __removeItem()__ - method

## Demo of a simple usage of localStorage and sessionStorage

To try a Demo of how the Local Storage and Session Storage work: 

1) Clone this repository

```git clone https://github.com/SamiSha99/week7_research.git```

2) Open each index.html one at the time and what is said in the each html.index.

3) Enjoy! (Optional)
