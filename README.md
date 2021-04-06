# ie11-vuetify-symbol-error

This repository is a reproduction of the ie11 issue with vuetify ripple directive and core-js symbol polyfill.

The issue is documented as [known caveat of core-js symbol polyfill](https://github.com/zloirock/core-js#caveats-when-using-symbol-polyfill).

## Steps

1. Install dependencies
2. Start the project with `dev` or `build + start` (treeShake is enabled in `nuxt.config.js` to be able to use `dev` in ie11)
3. Open ie11 and go to app url
4. Open devtools/console
5. Click at any button of the view
6. Check console. You will see `SCRIPT28 error` in console

## Build Setup

```bash
# install dependencies
$ yarn install

# serve with hot reload at localhost:3000
$ yarn dev

# build for production and launch server
$ yarn build
$ yarn start

# generate static project
$ yarn generate
```

For detailed explanation on how things work, check out [Nuxt.js docs](https://nuxtjs.org).
