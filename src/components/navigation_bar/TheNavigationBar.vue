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
      <div class="account_menu">
        <img class="account_img" src="../../assets/icons/account_preset.png" />
        <div class="account_details">
          <div class="account_name">SampleAccout</div>
          <div class="account_id">@Sample1234</div>
        </div>
        <img class="" src="../../assets/icons/more.svg" />
      </div>
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
.navi_post {
  cursor: pointer;
  text-align: center;
  border-radius: 30px;
  background-color: rgb(29, 155, 240);
}
.account_menu {
  display: flex;
  flex-direction: row;
  align-items: center;
  justify-content: center;
}

.account_menu:hover {
  background-color: rgb(40, 40, 40);
  border-radius: 60px;
}
.account_details {
  margin: 5px 30px 0 10px;
  font-size: 15px;
}
.account_id {
  color: gray;
}
.account_img {
  width: 40px;
  height: 40px;
}
</style>
