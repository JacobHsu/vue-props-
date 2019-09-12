# vue-props

vue create vue-props  
merge  


Vue CLI v3.6.2
┌────────────────────────────┐
│  Update available: 3.11.0  │
└────────────────────────────┘
? Please pick a preset: Manually select features
? Check the features needed for your project: Babel, Router, Vuex
? Use history mode for router? (Requires proper server setup for index fallback in production) Yes
? Where do you prefer placing config for Babel, PostCSS, ESLint, etc.? In dedicated config files
? Save this as a preset for future projects? Yes

`$ cd vue-props`  
`$ yarn serve`

## deploy  

[![NPM](https://nodei.co/npm/gh-pages.png?downloads=true&stars=true)](https://nodei.co/npm/gh-pages/)   
npm [gh-pages](https://www.npmjs.com/package/gh-pages)  
`npm install gh-pages --save-dev`  

package.json
```js
  "scripts": {
	...
    "deploy": "npm run build && gh-pages -d dist"
  },
```

vue.config.js 
```js
module.exports = {
    publicPath: 'vue-props'   
}
```
https://jacobhsu.github.io/vue-props  


# Note

父子元件溝通(Props down, Events up) 

![Props down, Events up](https://d1dwq032kyr03c.cloudfront.net/upload/images/20180105/20107673f0zb0ZxRz9.png)

# Debug

import Child from './Children.vue' fail
`npm install --save core-js`  

## Project setup
```
yarn install
```

### Compiles and hot-reloads for development
```
yarn run serve
```

### Compiles and minifies for production
```
yarn run build
```

### Run your tests
```
yarn run test
```

### Lints and fixes files
```
yarn run lint
```

### Customize configuration
See [Configuration Reference](https://cli.vuejs.org/config/).
