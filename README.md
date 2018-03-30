# esri-portal-maps

> A Vue.js project

## Installation

### CDN (Browser)

```html
<div id="app">
  <div is="EsriPortalMap" portal-id="b51fb4e76e154e1b93b630eac3ea94ae"></div>
</div>

<!-- include babel-polyfill for IE11 Promise support -->
<script src="https://cdnjs.cloudflare.com/ajax/libs/babel-polyfill/6.26.0/polyfill.min.js"></script>
<!-- include Vue -->
<script src="https://unpkg.com/vue/dist/vue.js"></script>
<!-- set HcAddressParcelForm Vue component -->
<script src="https://commbocc.github.io/hc-address-parcel-form/dist/build.var.js"></script>

<script type="text/javascript">
var app = new Vue({
  el: '#app',
  components: {
    EsriPortalMap: EsriPortalMap
  }
});
</script>
```

### NPM

`npm i --save https://github.com/Commbocc/esri-portal-map`

Example Single File Component

```html
<!-- App.vue -->
<template>
  <main>
    <div is="EsriPortalMap" portal-id="b51fb4e76e154e1b93b630eac3ea94ae"></div>
  </main>
</template>

<script>
import EsriPortalMap from 'esri-portal-map'

export default {
  // ...
  components: {
    EsriPortalMap
  }
  // ...
}
</script>
```

## Build Setup

``` bash
# install dependencies
npm install

# serve with hot reload at localhost:8080
npm run dev

# build for production with minification
npm run build
```

For detailed explanation on how things work, consult the [docs for vue-loader](http://vuejs.github.io/vue-loader).
