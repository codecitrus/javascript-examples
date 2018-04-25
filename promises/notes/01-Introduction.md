# Javascript Promises - Introduction
The general syntax for creating a promise:
    var promise = new Promise(function(resolve,reject) {
      if(allgood) { resolve("success"); }
      else { reject(Error("fail")); }
    });

Javascript promises are a bit like event-listeners, except:
  1) A promise can only succeed/fail once. Once succeeded/failed, it cannot switch.
  1) If promise succeeded/failed before adding success/failure callback, the callback
     will still be called.
A promise is always in one of the following states:
  1) Pending - Not yet fulfilled/rejected
  1) Fulfilled - Action relating to promise succeeded
  1) Rejected - Action relating to promise failed
  1) Settled - Has fulfilled or rejected

