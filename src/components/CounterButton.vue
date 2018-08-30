<template>
  <button :class="bindedClass" @click="Increase()">Számláló: {{ countPlusOffset }}</button>
</template>

<script lang="ts">
import { Component, Prop, Vue } from "vue-property-decorator";

@Component
export default class CounterButton extends Vue {
  @Prop() private theme!: string;
  @Prop() private offset!: number;
  private count: number = 0;

  private Increase(): void {
    this.count++;
  }

  get bindedClass(): string {
    let classes = "btn";

    if (this.theme) {
      classes += " btn-" + this.theme;
    }
    debugger;
    return classes;
  }

  get countPlusOffset(): number {
    return this.count + +this.offset;
  }
}
</script>

<!-- Add "scoped" attribute to limit CSS to this component only -->
<style scoped>
button {
  margin: 5px;
}
</style>
