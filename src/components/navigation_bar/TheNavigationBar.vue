<script setup>
import { ref } from 'vue';
import TheNavigation from './TheNavigation.vue';
</script>
<template>
  <div class="navi_wrapper">
    <img class="x_logo" src="../../assets/x_logo.svg" />
    <div class="navis">
      <TheNavigation icon="home">ホーム</TheNavigation>
      <TheNavigation icon="explore">話題を検索</TheNavigation>
      <TheNavigation icon="notifications">通知</TheNavigation>
      <TheNavigation icon="messages">メッセージ</TheNavigation>
      <TheNavigation icon="lists">リスト</TheNavigation>
      <TheNavigation icon="communities">コミュニティ</TheNavigation>
      <TheNavigation icon="../x_logo">プレミアム</TheNavigation>
      <TheNavigation icon="profile">プロフィール</TheNavigation>
      <TheNavigation icon="more">もっと見る</TheNavigation>
      <div class="navi_post">ポストする</div>
    </div>
  </div>
</template>
<style scoped>
.wrapper {
  flex-grow: 1;
}
.x_logo {
  width: 30px;
  height: 30px;
  margin: 10px 20px 10px 20px;
}
.navis {
  font-size: 1.3rem;
  margin: 0 30px 0;
}
.navis > div {
  padding: 12px;
}
@media (max-width: 600px) {
  .navis {
    display: none;
  }
}
</style>
