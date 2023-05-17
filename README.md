[![DevOps By Rultor.com](https://www.rultor.com/b/h1alexbel/serialize)](https://www.rultor.com/p/h1alexbel/serialize)
[![We recommend IntelliJ IDEA](https://www.elegantobjects.org/intellij-idea.svg)](https://www.jetbrains.com/idea/)
<br>

[![node](https://github.com/h1alexbel/serialize/actions/workflows/node.yml/badge.svg)](https://github.com/h1alexbel/serialize/actions/workflows/node.yml)
[![Hits-of-Code](https://hitsofcode.com/github/h1alexbel/serialize)](https://hitsofcode.com/view/github/h1alexbel/serialize)
[![Lines-of-Code](https://tokei.rs/b1/github/h1alexbel/serialize)](https://github.com/h1alexbel/serialize)
[![PDD status](http://www.0pdd.com/svg?name=h1alexbel/serialize)](http://www.0pdd.com/p?name=h1alexbel/serialize)
[![License](https://img.shields.io/badge/license-MIT-green.svg)](https://github.com/h1alexbel/serialize/blob/master/LICENSE)

Project architect: [@h1alexbel](https://github.com/h1alexbel)

Simple Serialization Interceptor and it Decorator for [NestJS](https://nestjs.com/).

**Motivation**.
We are not happy with duplicating code each time we are working with serialization in NestJs.

**How to use**.
First install package from [npm.js](https://www.npmjs.com/package/serialize-nest):
```shell
npm install serialize-nest
```

```typescript
@Serialize(ResponseUser)
function user() {
  return new User();
}
```
It will serialize your User object returned by method `user` into ResponseUser.

## How to Contribute

Fork repository, make changes, send us a [pull request](https://www.yegor256.com/2014/04/15/github-guidelines.html).
We will review your changes and apply them to the `master` branch shortly,
provided they don't violate our quality standards. To avoid frustration,
before sending us your pull request please run full NPM build:

```bash
$ npm run ci
```

You will need NPM 9+ and Node.js 18.16.0+.

Our [rultor image](https://github.com/yegor256/rultor-image) for CI/CD.