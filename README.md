# npm packages on GitHub

This goes over how to [install npm packages on GitHub](https://docs.npmjs.com/cli/install).

## Prerequisites

For an npm package to be valid, the `package.json` must:

- be parseable
- be located at the repository root
- contain the fields:
  - name
  - version

For example:

```json
{
  "name": "my-npm-package",
  "version": "1.2.3"
}
```

## Install package

### master

To install a package on GitHub at the latest (master) commit:

```sh
# npm install <git-user>/<repo-name>
$ npm install remarkablemark/npm-package-test
```

This is the same as:

```sh
# npm install <git-host>:<git-user>/<repo-name>
$ npm install github:remarkabelmark/npm-package-test
```

And this:

```sh
# npm install https://github.com/<git-user>/<repo-name>.git
$ npm install https://github.com/remarkablemark/npm-package-test.git
```
