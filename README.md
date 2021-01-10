# Install

```
npm i --save check-swear

```

# How to use

In your file put the following:

```
const check = require("check-swear");

// .............

check("whatever string you want!", "the type of thing that you put in") // returns false
```

# Additional Information

If your `check("blah blah blah")` doesn't work, thats because of the new update.
You need to put in the type of data that you have passed into the first argument.
This is due to the fact that I created this for a string array, and a different version of this npm package (has-swear | not made by me) can only do strings. I made this for both strings and string arrays.

Anyway, by now you are probably wodering how to fix this. Well, if the `text` element was a string, pass in `"string"` as the second parameter. if it's a string array, then you need to pass in `"String[]"`.

It'll look something like this...

```
`check("blah blah blah", "string")`
```

or

```
`check(["blah blah blah", "pog", "hallo", "some text"], "String[]")`
```

I hope this helps the problem that many of you are having!
