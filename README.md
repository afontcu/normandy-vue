# Vue CSS Objects

CSS Objects implementation in VueJS with Normandy CSS class naming.


## Features
---------------
+ Stateless Vue components
+ Import just the required components
+ Fully tested using [Jest](https://github.com/facebook/jest)
+ BEM-naming classes


## Installation
---------------
``` bash
npm install --save vue-objects
```

## Usage
---------------
``` javascript
import { Media } from 'vue-objects'
```

You can check out all the available components in `src/lib.js`.


This package provides the necessary CSS styles to render each object properly,
but it's not mandatory to import them: you can use whatever style provider
you want to use. Just make sure to map correctly all the classes generated by `vue-objects`.



## Contributing
---------------

Want to contribute?

``` bash
# install dependencies
npm install

# serve demo site with hot reload at localhost:8080
npm start

# unit tests
npm test (or npm run tdd)

# build for production with minification
npm run build

# build for production and view the bundle analyzer report
npm run build --report
```

For detailed explanation on how things work, checkout the
[guide](http://vuejs-templates.github.io/webpack/) and [docs for vue-loader](http://vuejs.github.io/vue-loader).


### How can I add more components to this library?
---------------

Fork the repo, and then:

1. Add your brand new component in `src/components/` folder. Develop and test it.

2. Make your component available by exporting it from `src/lib.js`.

3. Add it to the `demo/` app. Make sure to add import it in `demo/index.js` and add a new route in `demo/router/routes.js`.

4. Once registered and routed, develop a Showcase component and place it in `demo/showcase`. You're done!


### Why is /dist folder not gitignored?
---------------

The dist folder is removed from .gitignore so that it's available on npm and
user's who want the minified built distribution of this library can grab it
(located in /lib subfolder). Also  docs site built distribution is made
available in the same folder (located in /docs subfolder).


This package was created using [vue-template-library](https://github.com/prograhammer/vue-library-template)
package. For further clarifications refer to its README.
