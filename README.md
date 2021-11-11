# simple-cache-function

Saves the result of the function. With the same arguments, the function returns the stored result.

## Install

Install with [npm](https://www.npmjs.com/):

```sh
$ npm install --save simple-cache-function
```

## Usage

```js
const { memoize } = require('simple-cache-function');

function fibonacci(n) {
    if (n <= 1) {
        return 1
    }
    return fibonacci(n - 1) + fibonacci(n - 2);
}

const fibonacciMemo = memoize(fibonacci);

console.log(fibonacciMemo(6)); //=> 13

```

### Author

**Rostislav Kalyuzhny**

* [github/RostislavKalyuzhny](https://github.com/RostislavKalyuzhny)

