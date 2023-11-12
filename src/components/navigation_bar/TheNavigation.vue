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
  cursor: pointer;
  display: flex;
  flex-direction: row;
  margin: 5px 5px 5px 5px;
  border-radius: 30px;
  text-align: center;
}
.navi:hover {
  background-color: rgb(40, 40, 40);
  border-radius: 30px;
}
.icon {
  width: 30px;
  height: 30px;
}
.navi_label {
  padding-inline-start: 24px;
  padding-inline-end: auto;
  display: inline-block;
}
</style>
