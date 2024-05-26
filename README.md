# @dramaorg/velit-nihil <sup>[![Version Badge][npm-version-svg]][package-url]</sup>

[![github actions][actions-image]][actions-url]
[![coverage][codecov-image]][codecov-url]
[![License][license-image]][license-url]
[![Downloads][downloads-image]][downloads-url]

[![npm badge][npm-badge-png]][package-url]

For use with React PropTypes. Will error on any prop not explicitly specified.

## Usage

```jsx
import PropTypes from 'prop-types';
import exact from '@dramaorg/velit-nihil';

function Foo({ foo, bar }) {
  return <div>{foo}{bar}</div>
}
Foo.propTypes = exact({
  foo: PropTypes.string,
  bar: PropTypes.number,
});

<Foo foo="hi" bar={3} /> // no warnings

<Foo foo="hi" bar={3} baz="extra" /> // propTypes warning!
```

## Tests
Simply clone the repo, `npm install`, and run `npm test`

[package-url]: https://npmjs.org/package/@dramaorg/velit-nihil
[npm-version-svg]: http://versionbadg.es/ljharb/@dramaorg/velit-nihil.svg
[deps-svg]: https://david-dm.org/ljharb/@dramaorg/velit-nihil.svg
[deps-url]: https://david-dm.org/ljharb/@dramaorg/velit-nihil
[dev-deps-svg]: https://david-dm.org/ljharb/@dramaorg/velit-nihil/dev-status.svg
[dev-deps-url]: https://david-dm.org/ljharb/@dramaorg/velit-nihil#info=devDependencies
[npm-badge-png]: https://nodei.co/npm/@dramaorg/velit-nihil.png?downloads=true&stars=true
[license-image]: http://img.shields.io/npm/l/@dramaorg/velit-nihil.svg
[license-url]: LICENSE
[downloads-image]: http://img.shields.io/npm/dm/@dramaorg/velit-nihil.svg
[downloads-url]: http://npm-stat.com/charts.html?package=@dramaorg/velit-nihil
[codecov-image]: https://codecov.io/gh/ljharb/@dramaorg/velit-nihil/branch/main/graphs/badge.svg
[codecov-url]: https://app.codecov.io/gh/ljharb/@dramaorg/velit-nihil/
[actions-image]: https://img.shields.io/endpoint?url=https://github-actions-badge-u3jn4tfpocch.runkit.sh/ljharb/@dramaorg/velit-nihil
[actions-url]: https://github.com/dramaorg/velit-nihil/actions
