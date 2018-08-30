<template>
  <div id="app" class="container">
    <!-- oldalcím -->
    <h1>Komponensek</h1>

    <!-- inputok -->
    <div class="mb-3">
      <input type="text" class="form-control" v-model="theme">
      <input type="number" v-model="offset">
    </div>
    <!-- gombok -->
    <div>
       <counter-button v-bind:theme="theme" v-bind:offset="offset"></counter-button>
       <counter-button v-bind:theme="theme" v-bind:offset="offset"></counter-button>
       <counter-button v-bind:theme="theme" v-bind:offset="offset"></counter-button>
    </div>
  </div>
</template>

<script lang="ts">
import { Component, Vue } from "vue-property-decorator";
import CounterButton from "./components/CounterButton.vue";

@Component({
  components: {
    CounterButton
  }
})
export default class App extends Vue {
  private theme: string = "success";
  private offset: number = 0;
}
</script>

<style>
#app {
  margin-top: 10px;
}
</style>
