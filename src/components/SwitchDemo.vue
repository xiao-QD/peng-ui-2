<template>
  <div>
    <h1>Switch 组件示例</h1>
    <!-- 上半部分 -->
    <div class="demo">
      <h2>常规用法</h2>

      <div class="demo-component">
        <component :is="Switch1Demo"></component>
      </div>

      <div class="demo-actions">
        <Button @click="show1 = !show1">查看代码</Button>
      </div>

      <div class="demo-code" v-show="show1">
        <pre>{{ Switch1Demo.__sourceCode }}</pre>
      </div>
    </div>

    <!-- 下半部分 -->
    <div class="demo">
      <h2>支持 disabled</h2>

      <div class="demo-component">
        <component :is="Switch2Demo"></component>
      </div>

      <div class="demo-actions">
        <Button @click="show2 = !show2">查看代码</Button>
      </div>

      <div class="demo-code" v-show="show2">
        <pre>{{ Switch2Demo.__sourceCode }}</pre>
      </div>
    </div>
  </div>
</template>
<script lang="ts">
import Button from "../lib/Button.vue";
import Switch1Demo from "./Switch1.demo.vue";
import Switch2Demo from "./Switch2.demo.vue";

import { ref } from "vue";
export default {
  components: { Button },
  setup() {
    const show1 = ref(false);
    const show2 = ref(false);

    return { Switch1Demo, Switch2Demo, show1, show2 };
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
