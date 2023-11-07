<script setup>
import { ref, watchEffect } from 'vue';
const props = defineProps({
  icon: String,
});
const logo = ref('');
watchEffect(async () => {
  logo.value = (
    await import(/* @vite-ignore */ '../../assets/icons/' + props.icon + '.svg')
  ).default;
});
</script>
<template>
  <div class="navi">
    <img class="icon" :src="logo" />
    <div class="navi_label"><slot></slot></div>
  </div>
</template>
<style scoped>
.navi {
  display: flex;
  flex-direction: row;
}
.icon {
  width: 30px;
  height: 30px;
}
.navi_label {
  margin: 0 40px 0 20px;
}
</style>
