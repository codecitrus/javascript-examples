# Reading List For Promises
A compilation of good articles to read for dealing with Javascript promises

## Asynchronous Processing ##

### No, There Are No Race Conditions in Javascript
Javascript is a single threaded language and cannot have race conditions.
  - Javascript executes asynchronous tasks only AFTER the scope that fired them.
    For example, the async code in this example will never run:
    `function() { xmlhttp.send(); while(true){}; }`
  - In Javascript, there is no way to access *same* resource at same time
  - You can still ambiguous sequencing of callbacks however!




