# domnom.js
A simple dynamic browser fuzzer for the DOM inspired by [@lcamtuf's](https://twitter.com/lcamtuf) [ref_fuzz](http://lcamtuf.coredump.cx/ref_fuzz5.html) 

## usage
Simply open domnom.html in the browser, preferably on some sort of webserver as file:// seems to not work as well. 

## handling crashes
The issue with dynamic fuzzing completely in-browser is it may be difficult to reliably reproduce and debug crashes. Typically the most effective route is to make your desired tweaks to the fuzzer's settings, then open the browser attached to a debugger. Alternatively, a browser compiled with instrumentation can just be started and the crashes dealt with however you prefer. gdb and windbg work great for their respective platforms. 

If you are fuzzing Edge, I'd highly recommend using [skylined's EdgeDbg scripts](https://github.com/SkyLined/EdgeDbg) - you'll save a lot of time. 

## examples
Included are two of the many crashes already found using this fuzzer. In fact it has managed to produce crashes in all major browsers with the exception of Firefox(which I found odd). 
