# eslint-formatter-markdown [![Build Status](https://travis-ci.org/sven-piller/eslint-formatter-markdown.png?branch=master)](https://travis-ci.org/sven-piller/eslint-formatter-markdown)

Markdown ESLint formatter (reporter)

## Installation

Download node at [nodejs.org](http://nodejs.org) and install it, if you haven't already.

```sh
npm install eslint-formatter-markdown --save-dev
```

## Getting started

Use it with:

#### ESLint CLI

```bash
eslint --format node_modules/eslint-formatter-markdown/markdown.js file.js
```

#### [grunt-eslint](https://github.com/sindresorhus/grunt-eslint/)

```js
grunt.initConfig({
	eslint: {
		options: {
			format: require('eslint-formatter-markdown')
		},
		target: ['file.js']
	}
});

grunt.loadNpmTasks('grunt-eslint');
grunt.registerTask('default', ['eslint']);
```

## Tests

```sh
npm install
npm test
```

## Dependencies

None

## Dev Dependencies

- [chalk](https://github.com/chalk/chalk): Terminal string styling done right. Much color.
- [eslint](https://github.com/eslint/eslint): An AST-based pattern checker for JavaScript.
- [mocha](https://github.com/mochajs/mocha): simple, flexible, fun test framework

## Contributing

Feel free to contribute!

## Release History

* 0.9.1 Improvements in Documentation, [Issue #2](https://github.com/sven-piller/eslint-formatter-markdown/issues/2)
* 0.9.0 Initial release

## License

[MIT](http://opensource.org/licenses/MIT) © Sven Piller
