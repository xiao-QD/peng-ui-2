<template>
  <h1></h1>
  <div class="demo">
    <div class="demo-component">
      <component :is="Tdemo" />
    </div>
    <div class="demo-actions">
      <Button @click="show1 = !show1">查看代码</Button>
    </div>
    <div class="demo-code" v-show="show1">
      <pre>{{ Tdemo.__sourceCode }}</pre>
    </div>
  </div>
</template>

<script lang="ts">
import Tdemo from "./Tdemo.vue";
import Button from "../lib/Button.vue";
import { ref } from "vue";

export default {
  components: {
    Button,
  },

  setup() {
    const show1 = ref(false);
    return {
      Tdemo,
      show1,
    };
  },
};
</script>

<style lang="scss" scoped>
$border-color: #d9d9d9;
.demo {
  border: 1px solid $border-color;
  margin: 16px 0 32px;
  > h2 {
    font-size: 20px;
    padding: 8px 16px;
    border-bottom: 1px solid $border-color;
  }
  &-component {
    padding: 16px;
  }
  &-actions {
    padding: 8px 16px;
    border-top: 1px dashed $border-color;
  }
  &-code {
    padding: 8px 16px;
    border-top: 1px dashed $border-color;
    > pre {
      line-height: 1.1;
      font-family: Consolas, "Courier New", Courier, monospace;
      margin: 0;
    }
  }
}
</style>
