<script setup>
import TheNavigationBar from './components/TheNavigationBar.vue';
import TheMain from './components/TheMain.vue';
import TheSuggestionBar from './components/TheSuggestionBar.vue';
</script>

<template>
  <div class="contents">
    <TheNavigationBar />
    <TheMain />
    <TheSuggestionBar />
  </div>
</template>

<style scoped>
.contents {
  display: flex;
  flex-direction: row;
  justify-content: space-evenly;
  gap: 0;
}
</style>
