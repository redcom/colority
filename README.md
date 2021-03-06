# colority

![travis](https://api.travis-ci.org/JustClear/colority.svg?branch=master)
[![dependencies](https://david-dm.org/justclear/colority.svg)](https://david-dm.org/justclear/colority#info=dependencies&view=table)
[![devDependencies](https://david-dm.org/justclear/colority/dev-status.svg)](https://david-dm.org/justclear/colority#info=devDependencies&view=table)

extracting colors from pictures.

[DEMO](https://justclear.github.io/colority/demo/?image=https://user-gold-cdn.xitu.io/2017/8/8/c5267eadfded82a98cd3cad7a16d5a48?imageView2/1/w/1200/h/700/q/85/interlace/1)

## Installation

```sh
$ yarn add colority
```

## Usage

```js
import colority from 'colority';

colority(imageURL, colors => {
    // do something here...
});

// or skip pixels

colority(imageURL, {
    skip: 1000,
}, colors => {
    // do something here...
});
```

## APIs

- `colority(imageURL[, options], colors => {})`
    - `imageURL`: picture url.
    - `options.skip`: skip pixels(Optional, default to `10`).
    - `colors`: the extracted `rgb` colors(Sort by quantity).

## License

Licensed under the [MIT License](https://github.com/JustClear/just-sketch/blob/master/LICENSE)
