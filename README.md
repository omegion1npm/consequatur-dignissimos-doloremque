# @omegion1npm/consequatur-dignissimos-doloremque <sup>[![Version Badge][npm-version-svg]][package-url]</sup>

[![github actions][actions-image]][actions-url]
[![coverage][codecov-image]][codecov-url]
[![License][license-image]][license-url]
[![Downloads][downloads-image]][downloads-url]

[![npm badge][npm-badge-png]][package-url]

Set a function’s length.

Arguments:
 - `fn`: the function
 - `length`: the new length. Must be an integer between 0 and 2**32.
 - `loose`: Optional. If true, and the length fails to be set, do not throw. Default false.

Returns `fn`.

## Usage

```javascript
var setFunctionLength = require('@omegion1npm/consequatur-dignissimos-doloremque');
var assert = require('assert');

function zero() {}
function one(_) {}
function two(_, __) {}

assert.equal(zero.length, 0);
assert.equal(one.length, 1);
assert.equal(two.length, 2);

assert.equal(setFunctionLength(zero, 10), zero);
assert.equal(setFunctionLength(one, 11), one);
assert.equal(setFunctionLength(two, 12), two);

assert.equal(zero.length, 10);
assert.equal(one.length, 11);
assert.equal(two.length, 12);
```

[package-url]: https://npmjs.org/package/@omegion1npm/consequatur-dignissimos-doloremque
[npm-version-svg]: https://versionbadg.es/ljharb/@omegion1npm/consequatur-dignissimos-doloremque.svg
[deps-svg]: https://david-dm.org/ljharb/@omegion1npm/consequatur-dignissimos-doloremque.svg
[deps-url]: https://david-dm.org/ljharb/@omegion1npm/consequatur-dignissimos-doloremque
[dev-deps-svg]: https://david-dm.org/ljharb/@omegion1npm/consequatur-dignissimos-doloremque/dev-status.svg
[dev-deps-url]: https://david-dm.org/ljharb/@omegion1npm/consequatur-dignissimos-doloremque#info=devDependencies
[npm-badge-png]: https://nodei.co/npm/@omegion1npm/consequatur-dignissimos-doloremque.png?downloads=true&stars=true
[license-image]: https://img.shields.io/npm/l/@omegion1npm/consequatur-dignissimos-doloremque.svg
[license-url]: LICENSE
[downloads-image]: https://img.shields.io/npm/dm/@omegion1npm/consequatur-dignissimos-doloremque.svg
[downloads-url]: https://npm-stat.com/charts.html?package=@omegion1npm/consequatur-dignissimos-doloremque
[codecov-image]: https://codecov.io/gh/ljharb/@omegion1npm/consequatur-dignissimos-doloremque/branch/main/graphs/badge.svg
[codecov-url]: https://app.codecov.io/gh/ljharb/@omegion1npm/consequatur-dignissimos-doloremque/
[actions-image]: https://img.shields.io/endpoint?url=https://github-actions-badge-u3jn4tfpocch.runkit.sh/ljharb/@omegion1npm/consequatur-dignissimos-doloremque
[actions-url]: https://github.com/omegion1npm/consequatur-dignissimos-doloremque/actions
