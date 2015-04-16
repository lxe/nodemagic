# nodemagic

Run versions of `node` and `npm` specified in your `./package.json`.

### Features

 - Automatically reads [`package.json/engines`](https://docs.npmjs.com/files/package.json#engines) and uses those versions.
 - Automatically installs and caches npm and node versions for your specific platform
 - Probably works.

### Usage

 1. `npm install nodemagic -g` *or* [download](https://raw.githubusercontent.com/lxe/nodemagic/master/nodemagic) and place `nodemagic` in your path. Sorry, no copy-paste bash one-liner.
 2. `cd` into a project that has `package.json` with `engines` set up.
 3. Use:
   - `nodemagic npm install` isntead of `npm install`
   - `nodemagic node app.js` instead of `node app.js`, etc...

You can also alias `node` to `nodemagic node` and `npm` to `nodemagic npm`

### Bugs

Probably some semver issues. Please report issues and make PRs.

### FAQs

#### Why not `n` or `nvm?`

None of those allow decoupling of `node` and `npm` versions. Or read `engines`. I think.

#### Your bash is too hacky

Fix it and make a PR please!

### License

MIT
