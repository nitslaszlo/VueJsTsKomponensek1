# vuejs-ts-komponensek1

## Project setup
- npm install jquery --save
- npm install @types/jquery --save-dev
- npm install bootstrap --save
- npm install @types/bootstrap --save-dev
- npm install popper.js --save
- npm install @types/popper.js --save-dev
- npm install bootstrap-vue --save
- main.ts kiegészítése:
    > import Vue from "vue";
    > import BootstrapVue from "bootstrap-vue";
    > import App from "./App.vue";
    > 
    > Vue.config.productionTip = false;
    > 
    > import "bootstrap/dist/css/bootstrap.css";
    > import "bootstrap-vue/dist/bootstrap-vue.css";
    > 
    > Vue.use(BootstrapVue);
    > 
    > new Vue({
    >     render: h => h(App)
    > }).$mount("#app");
```
npm install
```

### Compiles and hot-reloads for development
```
npm run serve
```

### Compiles and minifies for production
```
npm run build
```

### Lints and fixes files
```
npm run lint
```
