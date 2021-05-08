# auro-ms-conversion

This is a small milisecond conversion package, that converts miliseconds into human readable text.

The `relativeTime` function has two parameters:

`ms` which is the miliseconds you want to convert

`long` which is whether you want the string to be like: "10d" or "10 days" Defaults to false

Usage:

```js
// *the package name might be different*
const msConversion = require('auro-ms-conversion');

console.log(msConversion.relativeTime(8123751236));
// 94d, 35m, and 51s

console.log(msConversion.relativeTime(8123751236, true));
// 94 days, 35 minutes, and 51 seconds

console.log(msConversion.relativeTime(137236834));
// 14h, 7m, and 16s

console.log(msConversion.relativeTime(137236834, true));
// 1 day, 14 hours, 7 minutes, and 16 seconds
```
