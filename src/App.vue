<script setup>
import TheNavigationBar from './components/navigation_bar/TheNavigationBar.vue';
import TheMain from './components/TheMain.vue';
import TheSuggestionBar from './components/TheSuggestionBar.vue';
</script>

<template>
  <div class="wrapper">
    <div class="contents">
      <TheNavigationBar />
      <TheMain />
      <TheSuggestionBar />
    </div>
  </div>
</template>

<style scoped>
.wrapper {
  display: flex;
  flex-direction: column;
  align-items: center;
}
.contents {
  display: flex;
  flex-direction: row;
}
</style>
