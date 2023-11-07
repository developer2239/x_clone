<script setup>
import TheNavigationBar from './components/navigation_bar/TheNavigationBar.vue';
import TheMain from './components/TheMain.vue';
import TheSuggestionBar from './components/TheSuggestionBar.vue';
</script>

<template>
  <div class="contents">
    <i class="bi bi-search"></i>
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
