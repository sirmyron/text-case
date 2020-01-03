# Change Case

[![NPM version][npm-image]][npm-url]
[![NPM downloads][downloads-image]][downloads-url]
[![Bundle size][bundlephobia-image]][bundlephobia-url]

> Convert text between
> [`camelCase`](https://github.com/idimetrix/text-case/tree/master/packages/camel-case),
> [`PascalCase`](https://github.com/idimetrix/text-case/tree/master/packages/pascal-case),
> [`Capital Case`](https://github.com/idimetrix/text-case/tree/master/packages/capital-case),
> [`Header-Case`](https://github.com/idimetrix/text-case/tree/master/packages/header-case),
> [`Title Case`](https://github.com/idimetrix/text-case/tree/master/packages/title-case),
> [`path/case`](https://github.com/idimetrix/text-case/tree/master/packages/path-case),
> [`snake_case`](https://github.com/idimetrix/text-case/tree/master/packages/snake-case),
> [`param-case`](https://github.com/idimetrix/text-case/tree/master/packages/param-case),
> [`dot.case`](https://github.com/idimetrix/text-case/tree/master/packages/dot-case),
> [`CONSTANT_CASE`](https://github.com/idimetrix/text-case/tree/master/packages/constant-case),
> [`lower case`](https://github.com/idimetrix/text-case/tree/master/packages/lower-case),
> [`lOWER CASE FIRST`](https://github.com/idimetrix/text-case/tree/master/packages/lower-case-first),
> [`UPPER CASE`](https://github.com/idimetrix/text-case/tree/master/packages/upper-case),
> [`Upper case first`](https://github.com/idimetrix/text-case/tree/master/packages/upper-case-first),
> and other

## Installation

```
npm install text-case --save
```

## Usage

```js
import {
  camelCase, // `camelCase`
  pascalCase, // `PascalCase`
  capitalCase, // `Capital Case`
  headerCase, // `Header-Case`
  titleCase, // `Title Case`
  pathCase, // `path/case`
  snakeCase, // `snake_case`
  paramCase, // `param-case`
  dotCase, // `dot.case`
  constantCase, // `CONSTANT_CASE`
  lowerCase, // `lower case`
  lowerCaseFirst, // `lOWER CASE FIRST`
  upperCase, // `UPPER CASE`
  upperCaseFirst, // `Upper case first`
  sentenceCase,
  isLowerCase,
  isUpperCase
} from "text-case";
```

Methods can also be installed [independently](https://github.com/idimetrix/text-case). All functions also accept [`options`](https://github.com/idimetrix/text-case#options) as the second argument.

### Options

- **`splitRegexp`** RegExp used to split into word segments (see [example](#split-example)).
- **`stripRegexp`** RegExp used to remove extraneous characters (default: `/[^A-Z0-9]/gi`).
- **`delimiter`** Value used between words (e.g. `" "`).
- **`transform`** Used to transform each word segment (e.g. `lowerCase`).

#### Split Example

If you find the default split hard to use, you can provide a different one. The example below will change the behavior to `expo2020 -> expo 2019` and `WorldExpo -> world expo`:

```js
const options = {
  splitRegexp: /([a-z])([A-Z0-9])/g
};
```

## Related

- [Meteor](https://github.com/Konecty/change-case)
- [Atom](https://github.com/robhurring/atom-change-case)
- [VSCode](https://github.com/wmaurer/vscode-change-case)

## License

MIT

[npm-image]: https://img.shields.io/npm/v/text-case.svg?style=flat
[npm-url]: https://npmjs.org/package/text-case
[downloads-image]: https://img.shields.io/npm/dm/text-case.svg?style=flat
[downloads-url]: https://npmjs.org/package/text-case
[bundlephobia-image]: https://img.shields.io/bundlephobia/minzip/text-case.svg
[bundlephobia-url]: https://bundlephobia.com/result?p=text-case
