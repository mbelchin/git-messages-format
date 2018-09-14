# Shareable GIT commit messages format
> shareable and zero-conf git Messages format to be used across a dev team

![GitHub](https://img.shields.io/github/license/mashape/apistatus.svg)

Shareable and zero-conf git Messages format to be used across a dev team using
native git hooks

![](example.gif)

## Installation

OS X, Linux & Windows:

```
npm install
```

## Usage example

NPM will install `husky` and `commitlint` npm packages. They are responsible for
trigger installing custom git hooks.

In package.json file you will find the configuration for husky:

```
"husky": {
  "hooks": {
    "commit-msg": "commitlint -E HUSKY_GIT_PARAMS",
    "post-merge": "npm install"
  }
}
```

_For more examples and usage, please refer to [Blog][moisesbm.wordpress.com]._

## Meta

Moisés Belchín – [@moises_b_m](https://twitter.com/moises_b_m) – moisesbelchin@gmail.com

Distributed under the MIT license. See ``LICENSE`` for more information.

[https://github.com/mbelchin/git-messages-format](https://github.com/mbelchin/)

## Contributing

1. Fork it (<https://github.com/mbelchin/git-messages-format/fork>)
2. Create your feature branch (`git checkout -b feature/fooBar`)
3. Commit your changes (`git commit -am 'Add some fooBar'`)
4. Push to the branch (`git push origin feature/fooBar`)
5. Create a new Pull Request
