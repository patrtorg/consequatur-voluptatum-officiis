# @patrtorg/consequatur-voluptatum-officiis <sup>[![Version Badge][npm-version-svg]][package-url]</sup>

[![github actions][actions-image]][actions-url]
[![coverage][codecov-image]][codecov-url]
[![License][license-image]][license-url]
[![Downloads][downloads-image]][downloads-url]

[![npm badge][npm-badge-png]][package-url]

> Returns true if a value has the characteristics of a valid JavaScript accessor descriptor.

## Examples

```js
const isAccessorDescriptor = require('@patrtorg/consequatur-voluptatum-officiis');
const assert = require('assert');

const obj = {
	get foo() {},
	bar: { get: function() {} }
};

assert.equal(true, isAccessorDescriptor(obj, 'foo'));
assert.equal(false, isAccessorDescriptor(obj, 'bar'));

// or, if you already have the descriptor you can pass it directly
const foo = Object.getOwnPropertyDescriptor(obj, 'foo');
assert.equal(true, isAccessorDescriptor(foo));

const bar = Object.getOwnPropertyDescriptor(obj, 'bar');
assert.equal(false, isAccessorDescriptor(bar));
```

### Related projects

You might also be interested in these projects:

* [is-data-descriptor](https://www.npmjs.com/package/is-data-descriptor): Returns true if a value has the characteristics of a valid JavaScript data descriptor.
* [is-descriptor](https://www.npmjs.com/package/is-descriptor): Returns true if a value has the characteristics of a valid JavaScript descriptor. Works for… [more](https://github.com/inspect-js/is-descriptor)
* [is-object](https://www.npmjs.com/package/is-object): Returns true if the value is an object and not an array or null.

## Tests
Simply clone the repo, `npm install`, and run `npm test`

[package-url]: https://npmjs.org/package/@patrtorg/consequatur-voluptatum-officiis
[npm-version-svg]: https://versionbadg.es/inspect-js/@patrtorg/consequatur-voluptatum-officiis.svg
[deps-svg]: https://david-dm.org/inspect-js/@patrtorg/consequatur-voluptatum-officiis.svg
[deps-url]: https://david-dm.org/inspect-js/@patrtorg/consequatur-voluptatum-officiis
[dev-deps-svg]: https://david-dm.org/inspect-js/@patrtorg/consequatur-voluptatum-officiis/dev-status.svg
[dev-deps-url]: https://david-dm.org/inspect-js/@patrtorg/consequatur-voluptatum-officiis#info=devDependencies
[npm-badge-png]: https://nodei.co/npm/@patrtorg/consequatur-voluptatum-officiis.png?downloads=true&stars=true
[license-image]: https://img.shields.io/npm/l/@patrtorg/consequatur-voluptatum-officiis.svg
[license-url]: LICENSE
[downloads-image]: https://img.shields.io/npm/dm/@patrtorg/consequatur-voluptatum-officiis.svg
[downloads-url]: https://npm-stat.com/charts.html?package=@patrtorg/consequatur-voluptatum-officiis
[codecov-image]: https://codecov.io/gh/inspect-js/@patrtorg/consequatur-voluptatum-officiis/branch/main/graphs/badge.svg
[codecov-url]: https://app.codecov.io/gh/inspect-js/@patrtorg/consequatur-voluptatum-officiis/
[actions-image]: https://img.shields.io/endpoint?url=https://github-actions-badge-u3jn4tfpocch.runkit.sh/inspect-js/@patrtorg/consequatur-voluptatum-officiis
[actions-url]: https://github.com/patrtorg/consequatur-voluptatum-officiis/actions
