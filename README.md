<div align="center">
  <img src="https://github.com/cpatchane/create-cozy-app/raw/master/CreateCozyApp.png" alt="CCA illustration" />
</div>

<h1 align="center">Create Cozy App</h1>

<div align="center">
  <a href="https://github.com/CPatchane/create-cozy-app/blob/master/packages/create-cozy-app/LICENSE">
    <img src="https://img.shields.io/npm/l/create-cozy-app.svg" alt="license" />
  </a>
  <a href="https://travis-ci.org/CPatchane/create-cozy-app">
    <img src="https://img.shields.io/travis/CPatchane/create-cozy-app.svg" alt="travis" />
  </a>
  <a href="https://renovateapp.com/">
    <img src="https://img.shields.io/badge/renovate-enabled-brightgreen.svg" alt="renovate" />
  </a>
  <a href="https://github.com/facebook/jest">
    <img src="https://facebook.github.io/jest/img/jest-badge.svg" alt="tested with jest" />
  </a>
</div>

<p align="center">Start quickly your Cozy application</p>

### What's create-cozy-app?

`create-cozy-app` is a command line tool that create a skeleton of an application for Cozy, using Cozy libraries.

This tool can be run as an installed CLI or by using `yarn create`, see below for more information.

By default, `create-cozy-app` will use the [`cozy-scripts`](https://github.com/CPatchane/create-cozy-app/tree/master/packages/cozy-scripts) scripts bundle to build your app based on Preact (tested on React) and Redux frameworks.

#### Requirements

 - Node.js version 8 or higher;
 - [Yarn](https://yarnpkg.com). Yarn is a Node.js package manager, like `npm`;
 - a running [Cozy development environment](https://docs.cozy.io/en/dev/app/#install-the-development-environment) (optional if you just want to use standalone mode);


### Running it without installation via Yarn

You can use `create-cozy-app` without installing it globally by using the `yarn create cozy-app` command to bootstrap your application:

```
yarn create cozy-app mycozyapp
```

You can find more information about `yarn create` in the [yarnpkg documentation](https://yarnpkg.com/lang/en/docs/cli/create/).

### Install the CLI

Just use `yarn` to download and globally install the `create-cozy-app` CLI;

```
yarn global add create-cozy-app
```

#### CLI usage

If you installed the CLI as described before, use the `create-cozy-app` command to bootstrap your application:

```
create-cozy-app mycozyapp
```

### Ready to go

The script will download some dependencies (may take a while) and ask you a few questions, then create an application skeleton inside `mycozyapp`

That's all! You can start hacking:

```
cd mycozyapp
yarn watch:standalone
```

After the webpack build, your app should be available at http://localhost:8888


### Known limitations

For now, this project has only been tested on GNU/Linux and OS X.

### Options

##### `--scripts-source`

You can pass a custom scripts package using the optional `--scripts-source` option, it can be one of:

- a __relative local path__ to a tarball (`fileRel:` prefix): `fileRel:./a-folder/my-cozy-scripts.tar.gz`
- an __absolute local path__ to a tarball (`fileAbs:` prefix): `fileAbs:/root/my-cozy-scripts.tar.gz`
- an __URL__ to a tarball (`url:` prefix): `url:https://myurl.com/my-cozy-scripts.tar.gz`
- a specific __npm version__ (`version:` prefix): `version:0.1.5`
- a specific __git commit/branch__ with name provided after the '#' (`git:` prefix): `git://github.com/CPatchane/cozy-scripts.git#master`

##### `--vue`

Using this options, `create-cozy-app` will use the `cozy-scripts` package but with the `template-vue` template folder in order to build a Cozy application using the [VueJS 2+ framework](https://vuejs.org).

##### `--vanilla`

Using this options, `create-cozy-app` will use the `cozy-scripts-vanilla` package (instead of the default one: `cozy-scripts`) and build a Cozy application in VanillaJS without any npm dependencies.


## Community

### What's Cozy?

<div align="center">
  <a href="https://cozy.io">
    <img src="https://cdn.rawgit.com/cozy/cozy-site/master/src/images/cozy-logo-name-horizontal-blue.svg" alt="cozy" height="48" />
  </a>
 </div>
 </br>

[Cozy] is a platform that brings all your web services in the same private space.  With it, your webapps and your devices can share data easily, providing you with a new experience. You can install Cozy on your own hardware where no one's tracking you.

### Get in touch

You can reach the Cozy Community by:

- Chatting with us on IRC [#cozycloud on Freenode][freenode]
- Posting on our [Forum][forum]
- Posting issues on the [Github repos][github]
- Say Hi! on [Twitter][twitter]


## License

`create-cozy-app` is distributed under the MIT license.

CCA logo by [@CPatchane](https://github.com/CPatchane).


[cozy]: https://cozy.io "Cozy Cloud"
[freenode]: http://webchat.freenode.net/?randomnick=1&channels=%23cozycloud&uio=d4
[forum]: https://forum.cozy.io/
[github]: https://github.com/cozy/
[twitter]: https://twitter.com/cozycloud
