# metalsmith-register-helpers

A Metalsmith plugin for registering Handlebars helpers.

## CLI Usage

Install via npm and then add the `metalsmith-register-partials` key to your `metalsmith.json` plugins, like so:

```
{
  "plugins": {
    "metalsmith-register-helpers": {
      "directory": "path/to/helpers"
    }
  }
}
```

This will register all helpers in the specified directory, and use the first part of the filename as the helper name. For example, you could add a limit helper in the file `limit.js`:

```js
module.exports = function(collection, limit, start) {
  return collection.slice( start, limit + 1 );
}
```

And then access it in your templates:



## License

[The MIT License (MIT)](LICENSE.md)

Copyright © 2015 [Kenneth Ormandy](http://kennethormandy.com)
Copyright © 2015 Lin Clark
