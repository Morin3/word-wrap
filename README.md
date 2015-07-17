# word-wrap [![NPM version](https://badge.fury.io/js/word-wrap.svg)](http://badge.fury.io/js/word-wrap)  [![Build Status](https://travis-ci.org/jonschlinkert/word-wrap.svg)](https://travis-ci.org/jonschlinkert/word-wrap)

> Wrap words to a specified length.

Install with [npm](https://www.npmjs.com/)

```sh
$ npm i word-wrap --save
```

## Usage

```js
var wrap = require('word-wrap');

wrap('Lorem ipsum dolor sit amet, consectetur adipiscing elit, sed do eiusmod tempor incididunt ut labore et dolore magna aliqua. Ut enim ad minim veniam, quis nostrud exercitation ullamco laboris nisi ut aliquip ex ea commodo consequat.');
```

Results in:

```
  Lorem ipsum dolor sit amet, consectetur adipiscing
  elit, sed do eiusmod tempor incididunt ut labore
  et dolore magna aliqua. Ut enim ad minim veniam,
  quis nostrud exercitation ullamco laboris nisi ut
  aliquip ex ea commodo consequat.
```

## Options

[![image](https://cloud.githubusercontent.com/assets/383994/6543728/7a381c08-c4f6-11e4-8b7d-b6ba197569c9.png)](https://www.npmjs.com/)

### options.width

Type: `Number`

Default: `50`

The width of the text before wrapping to a new line.

**Example:**

```js
wrap(str, {width: 60});
```

### options.indent

Type: `String`

Default: `` (two spaces)

The string to use at the beginning of each line.

**Example:**

```js
wrap(str, {indent: '      '});
```

### options.newline

Type: `String`

Default: `\n`

The string to use at the end of each line.

**Example:**

```js
wrap(str, {newline: '\n\n'});
```

### options.trim

Type: `Boolean`

Default: `false`

Trim trailing whitespace from the returned string. This option is included since `.trim()` would also strip the leading indentation from the first line.

**Example:**

```js
wrap(str, {trim: true});
```

### options.cut

Type: `Boolean`

Default: `false`

Break a word between any two letters when the word is longer than the specified width.

**Example:**

```js
wrap(str, {cut: true});
```

## Related projects

* [common-words](https://github.com/jonschlinkert/common-words): Updated list (JSON) of the 100 most common words in the English language. Useful for… [more](https://github.com/jonschlinkert/common-words)
* [shuffle-words](https://github.com/jonschlinkert/shuffle-words): Shuffle the words in a string and optionally the letters in each word using the… [more](https://github.com/jonschlinkert/shuffle-words)
* [unique-words](https://github.com/jonschlinkert/unique-words): Return the unique words in a string or array.
* [wordcount](https://github.com/jonschlinkert/wordcount): Count the words in string. Has basic support for Cyrillic and CJK.

## Running tests

Install dev dependencies:

```sh
$ npm i -d && npm test
```

## Contributing

Pull requests and stars are always welcome. For bugs and feature requests, [please create an issue](https://github.com/jonschlinkert/word-wrap/issues/new)

## Author

**Jon Schlinkert**

+ [github/jonschlinkert](https://github.com/jonschlinkert)
+ [twitter/jonschlinkert](http://twitter.com/jonschlinkert)

## License

Copyright © 2015 Jon Schlinkert
Released under the MIT license.

***

_This file was generated by [verb-cli](https://github.com/assemble/verb-cli) on July 17, 2015._