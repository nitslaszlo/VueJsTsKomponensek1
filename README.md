# vuejs-ts-komponensek1
Forrás: Dósa Bálint: https://github.com/dosabalint/webfejleszto-vue-01-03<br>
Fejlesztői környezet beállítása: https://github.com/nitslaszlo/JedlikVueJsStarter
## Fejlesztői környezet beállítása 2
- npm install jquery --save
- npm install @types/jquery --save-dev
- npm install bootstrap --save
- npm install @types/bootstrap --save-dev
- npm install popper.js --save
- npm install @types/popper.js --save-dev
- npm install bootstrap-vue --save
- main.ts kiegészítése:
    > import Vue from "vue";<br>
    > **import BootstrapVue from "bootstrap-vue";**<br>
    > import App from "./App.vue";<br>
    > <br>
    > Vue.config.productionTip = false;<br>
    > <br>
    > **import "bootstrap/dist/css/bootstrap.css";**<br>
    > **import "bootstrap-vue/dist/bootstrap-vue.css";**<br>
    > <br>
    > **Vue.use(BootstrapVue);**<br>
    > <br>
    > new Vue({<br>
    >     render: h => h(App)<br>
    > }).$mount("#app");<br>
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
