
js-format [![LICENSE](https://img.shields.io/github/license/tsu-complete/js-format.svg)](https://github.com/tsu-complete/js-format/blob/master/LICENSE)
===
[![Codacy Badge](https://www.codacy.com/project/badge/fe402d05a90245b2848a3fee4171f0e1)](https://www.codacy.com/app/tsu-complete/js-format)
[![Dependencies](https://david-dm.org/tsu-complete/js-format.svg)](https://david-dm.org/tsu-complete/js-format)
[![Dev Dependencies](https://david-dm.org/tsu-complete/js-format/dev-status.svg)](https://david-dm.org/tsu-complete/js-format#info=devDependencies)

> data formatting

Usage
---

```js
format("MM.YYYY", new Date());

format("(0.0a)", "-4.0e12", format.NUMBER);

format("({{status}}!)", { status: "Success" });

var currency_formatter = format.create("($0.00a)", Number, function ( value ) {
    return value.toUpperCase();
});

currency_formatter(-4000);
// => ($4.00K)
```

Vendor
---

### Numeric formatting

[Numeral](https://github.com/adamwdraper/Numeral-js)

### Date formatting

[datef](https://github.com/hogart/datef)

### String formatting

[Mustache](https://github.com/janl/mustache.js)

