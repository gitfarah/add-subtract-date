# add-subtract-date [![Support this project][donate-now]][paypal-donations]

Add or subtract a specified time in a date object.

## Installation

```sh
$ npm i --save add-subtract-date
```

## Example

```js
const addSubtractDate = require("add-subtract-date");

var d = new Date(1989, 11, 20);

console.log(addSubtractDate.add(d, 2, "days"));
// => Fri Dec 22 1989 00:00:00 GMT+0200 (EET)

console.log(addSubtractDate.subtract(d, 1, "day"));
// => Thu Dec 21 1989 00:00:00 GMT+0200 (EET)

console.log(addSubtractDate.subtract(d, 1, "year"));
// => Wed Dec 21 1988 00:00:00 GMT+0200 (EET)

console.log(addSubtractDate.add(d, 10, "hours"));
// => Wed Dec 21 1988 10:00:00 GMT+0200 (EET)

console.log(addSubtractDate.add(d, 42, "minutes"));
// => Wed Dec 21 1988 10:42:00 GMT+0200 (EET)

console.log(addSubtractDate.add(d, 7, "seconds"));
// => Wed Dec 21 1988 10:42:07 GMT+0200 (EET)

console.log(addSubtractDate.add(d, 142, "milliseconds"));
// => Wed Dec 21 1988 10:42:07 GMT+0200 (EET)

console.log(addSubtractDate.subtract(d, 1, "week"));
// => Wed Dec 28 1988 10:42:07 GMT+0200 (EET)
```

## Documentation

The module exports an object containing two methods: `add`
(goes in the future) and `subtract` (goes in the past).
They require the following arguments:

 - `d` (Date): The date object.
 - `count` (Number): How many years/months/etc to add/subtract.
 - `what` (String): What to add/subtract. Supported values are:
    
     - `years`
     - `year`
     - `months`
     - `month`
     - `weeks`
     - `week`
     - `days`
     - `day`
     - `hours`
     - `hour`
     - `minutes`
     - `minute`
     - `seconds`
     - `second`
     - `milliseconds`
     - `millisecond`
    

## How to contribute
Have an idea? Found a bug? See [how to contribute][contributing].

## Where is this library used?
If you are using this library in one of your projects, add it in this list. :sparkles:

## License

[MIT][license] © [Ionică Bizău][website]

[paypal-donations]: https://www.paypal.com/cgi-bin/webscr?cmd=_s-xclick&hosted_button_id=RVXDDLKKLQRJW
[donate-now]: http://i.imgur.com/6cMbHOC.png

[license]: http://showalicense.com/?fullname=Ionic%C4%83%20Biz%C4%83u%20%3Cbizauionica%40gmail.com%3E%20(http%3A%2F%2Fionicabizau.net)&year=2015#license-mit
[website]: http://ionicabizau.net
[contributing]: /CONTRIBUTING.md
[docs]: /DOCUMENTATION.md