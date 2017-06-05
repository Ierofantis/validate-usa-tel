## validate-usa-tel

String validate-usa-tel

Time complexity: **O(log(n))**



## Install

```bash
$ npm install validate-usa-tel
```

## Usage

```js
const Validate = require('validate-usa-tel')

Validate("555-555-5555") should return a boolean.
Validate("1 555-555-5555") should return true.
Validate("1 (555) 555-5555") should return true.
Validate("5555555555") should return true.
Validate("555-555-5555") should return true.
Validate("(555)555-5555") should return true.
Validate("1(555)555-5555") should return true.
Validate("555-5555") should return false.
Validate("5555555") should return false.
Validate("1 555)555-5555") should return false.
Validate("1 555 555 5555") should return true.
Validate("1 456 789 4444") should return true.
Validate("123**&!!asdf#") should return false.
Validate("55555555") should return false.
Validate("(6505552368)") should return false
Validate("2 (757) 622-7382") should return false.
Validate("0 (757) 622-7382") should return false.
Validate("-1 (757) 622-7382") should return false
Validate("2 757 622-7382") should return false.
Validate("10 (757) 622-7382") should return false.
Validate("27576227382") should return false.
Validate("(275)76227382") should return false.
Validate("2(757)6227382") should return false.
Validate("2(757)622-7382") should return false.
Validate("555)-555-5555") should return false.
Validate("(555-555-5555") should return false.
Validate("(555)5(55?)-5555") should return false.

```
