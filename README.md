# Install

```
npm i --save check-swear
```

# How to use

In your file put the following:

```
const check = require("check-swear");

// .............

check("whatever string you want!", (String, Array)) // returns false
```

# Additional Information

If your `check("blah blah blah")` doesn't work, thats because of the new update.
You need to put in the type of data that you have passed into the first argument.
This is due to the fact that I created this for a string array, and a different version of this npm package (has-swear | not made by me) can only do strings. I made this for both strings and arrays.

Anyway, by now you are probably wodering how to fix this. Well, if the `text` element was a string, pass in `String` as the second parameter. if it's a string array, then you need to pass in `Array`.

It'll look something like this...

```
`check("blah blah blah", String)`
```

or

```
`check(["blah blah blah", "pog", "hallo", "some text"], Array)`
```

I hope this helps the problem that many of you are having!

# Notes

If you use an array, inside of the Array must not be empty, or have anything else besides a string, otherwise it will throw an error.
English only. You may fork this and create a pull request if you would like another language.