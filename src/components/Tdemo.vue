<demo>
    常规使用
</demo>
<template>
  <Tabs v-model:selected="x">
    <Tab title="导航1">内容1</Tab>
    <Tab title="导航222222">内容22222</Tab>
  </Tabs>
</template>

<script>
import Tabs from "../lib/Tabs.vue";
import Tab from "../lib/Tab.vue";
import { ref } from "vue";
export default {
  components: {
    Tabs,
    Tab,
  },

  setup() {
    const x = ref("导航222222");
    return { x };
  },
};
</script>

<style></style>
