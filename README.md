# Shareable GIT commit messages format
> shareable and zero-conf git Messages format to be used across a dev team

![GitHub](https://img.shields.io/github/license/mbelchin/git-messages-format.svg)
![GitHub release](https://img.shields.io/github/release/mbelchin/git-messages-format.svg)


[![Twitter](https://img.shields.io/twitter/url/https/shields.io.svg?style=social)](https://twitter.com/intent/tweet?text=Wow:&url=https%3A%2F%2Fgithub.com%2Fmbelchin%2Fgit-messages-format&hashtags=git,hooks,developers,commit,format)

*Read this in other languages: [English](README.md), [Español](README.es.md).*

Shareable and zero-conf git Messages format to be used across a dev team using
native GIT hooks

![](example.gif)

## Installation

OS X, Linux & Windows:

```
npm install
```

## Usage example

NPM will install `husky` and `commitlint` npm packages. They are responsible for
installing and triggering custom GIT hooks.

Inside the `package.json` file you will find the configuration for husky.
For this case we are using `commit-msg` and `post-merge` GIT hooks.

```
"husky": {
  "hooks": {
    "commit-msg": "commitlint -E HUSKY_GIT_PARAMS",
    "post-merge": "npm install"
  }
}
```

_For more examples and usage, please refer to [https://moisesbm.wordpress.com/2018/09/15/git-commit-messages-shareable-format/](https://moisesbm.wordpress.com/2018/09/15/git-commit-messages-shareable-format/)._

## Author

[Moisés Belchín](https://moisesbm.wordpress.com)
[@moises_b_m](https://twitter.com/moises_b_m)
[https://github.com/mbelchin/](https://github.com/mbelchin/)

Distributed under the MIT license. See ``LICENSE`` for more information.

## Documentation

For a detailed explanation, please refer to:
[https://moisesbm.wordpress.com/2018/09/15/git-commit-messages-shareable-format/](https://moisesbm.wordpress.com/2018/09/15/git-commit-messages-shareable-format/)

## Discussion

This project was created to find a simple way to share same GIT commit messages format across a whole developers team.

If you consider some things could be improved or you know another simpler, easier configurable tools, please open a discussion thread so all of us could benefit from those improvements.

## Contributing

1. Fork it (<https://github.com/mbelchin/git-messages-format/fork>)
2. Create your feature branch (`git checkout -b feature/fooBar`)
3. Commit your changes (`git commit -am '<type>(scope): add some fooBar'`)
4. Push to the branch (`git push origin feature/fooBar`)
5. Create a new Pull Request
