<template>
  <div class="tdesign-demo-block">
    <t-button variant="outline" @click="visible = true">5000ms</t-button>
  </div>
  <t-message v-model="visible" content="5000ms后消失" :duration="5000" />
</template>

<script>
import { defineComponent, ref } from 'vue';

export default defineComponent({
  setup() {
    const visible = ref(false);
    return { visible };
  },
});
</script>
