<script setup>
import { ref } from 'vue';
</script>
<template>
  <div class="wrapper">
    <span class="search_wrapper">
      <div class="search">
        <img class="search_icon" src="../assets/icons/explore.svg" />
        <form>
          <input
            name="search_input"
            class="search_input"
            type="text"
            placeholder="検索"
          />
        </form>
      </div>
    </span>
    <div class="sugestion_subscribe">
      <div class="sugestion_subscribe_title">プレミアムにサブスクライブ</div>
      <div class="sugestion_subscribe_text">
        サブスクライブして新機能を利用しましょう。
        資格を満たしている場合、広告収益分配を受け取れます。
      </div>
      <button class="button_subscribe">購入する</button>
    </div>
    <div class="sugestion_trend">
      <div class="sugestion_trend_title">いまどうしてる？</div>
      <div class="sugestion_trend_list">
        <div class="sugestion_trend_item">
          <div class="sugestion_trend_item_title">#パーフェクトスティック</div>
          <div class="sugestion_trend_item_text">
            アタックZEROパーフェクトスティックキャンペーン<br />
            花王アタック（お洗濯全般）によるプロモーション
          </div>
        </div>
        <div class="sugestion_trend_item">
          <div class="sugestion_trend_item_genre">日本のトレンド</div>
          <div class="sugestion_trend_item_title">三苫さん</div>
          <div class="sugestion_trend_item_post_count">1355 posts</div>
        </div>
        <div class="sugestion_trend_item">
          <div class="sugestion_trend_item_genre">音楽・トレンド</div>
          <div class="sugestion_trend_item_title">離婚危機</div>
          <div class="sugestion_trend_item_post_count">2663 posts</div>
        </div>
        <div class="sugestion_trend_item">
          <div class="sugestion_trend_item_genre">日本のトレンド</div>
          <div class="sugestion_trend_item_title">万博撤退の意向</div>
          <div class="sugestion_trend_item_post_count">2466 posts</div>
        </div>
        <div class="sugestion_trend_item">
          <div class="sugestion_trend_item_genre">音楽関係会社・トレンド</div>
          <div class="sugestion_trend_item_title">桜井美和</div>
          <div class="sugestion_trend_item_post_count">938 posts</div>
        </div>
        <div class="sugestion_trend_more">さらに表示</div>
      </div>
    </div>
    <div class="suggestion_account_list">
      <div class="suggestion_account_list_title">おすすめユーザー</div>
      <div class="account_menu">
        <img class="account_img" src="../assets/icons/account_preset.png" />
        <div class="account_details">
          <div class="account_name">SampleAccout</div>
          <div class="account_id">@Sample1234</div>
        </div>
        <button class="button_follow">フォロー</button>
      </div>
      <div class="account_menu">
        <img class="account_img" src="../assets/icons/account_preset.png" />
        <div class="account_details">
          <div class="account_name">SampleAccout</div>
          <div class="account_id">@Sample1234</div>
        </div>
        <button class="button_follow">フォロー</button>
      </div>
      <div class="account_menu">
        <img class="account_img" src="../assets/icons/account_preset.png" />
        <div class="account_details">
          <div class="account_name">SampleAccout</div>
          <div class="account_id">@Sample1234</div>
        </div>
        <button class="button_follow">フォロー</button>
      </div>
      <div class="account_menu">
        <img class="account_img" src="../assets/icons/account_preset.png" />
        <div class="account_details">
          <div class="account_name">SampleAccout</div>
          <div class="account_id">@Sample1234</div>
        </div>
        <button class="button_follow">フォロー</button>
      </div>
      <div class="account_more">さらに表示</div>
    </div>
    <footer class="footer">
      <span class="footer_content">利用規約</span>
      <span class="footer_content">プライバシーポリシー</span>
      <span class="footer_content">Cookieのポリシー</span>
      <span class="footer_content">アクセシビリティ</span>
      <span class="footer_content">広告情報</span>
      <span class="footer_content">もっと見る</span>
      <span class="footer_content">&copy; 2023 X Clone Project.</span>
    </footer>
  </div>
</template>
<style scoped>
.wrapper {
  margin-inline: 30px;
  width: 400px;
}
.search_wrapper {
  background-color: black;
  position: fixed;
  overflow: auto;
}
.search {
  width: 400px;
  height: 50px;
  display: flex;
  flex-direction: row;
  justify-content: center;
  background-color: rgb(32, 35, 39);
  border: 1px solid black;
  border-radius: 30px;
  align-items: center;
}
.search_icon {
  height: 15px;
  width: 15px;
}
.search_input {
  margin: 10px;
  width: 300px;
  font-size: 15px;
  background-color: rgb(32, 35, 39);
}
.sugestion_subscribe {
  margin-top: 70px;
  padding: 20px;
  background-color: rgb(32, 35, 39);
  border: 1px solid black;
  border-radius: 15px;
  font-weight: bold;
}
.sugestion_subscribe_title {
  font-size: 23px;
}
.sugestion_subscribe_text {
  margin-top: 5px;
  font-size: 16px;
}
.button_subscribe {
  padding: 5px 10px 5px 10px;
  cursor: pointer;
  text-align: center;
  border-radius: 30px;
  background-color: rgb(29, 155, 240);
}
.sugestion_trend {
  padding: 20px;
  margin-top: 20px;
  background-color: rgb(32, 35, 39);
  border: 1px solid black;
  border-radius: 15px;
  font-weight: bold;
}
.sugestion_trend_item {
  cursor: pointer;
  margin-top: 20px;
}
.sugestion_trend_item:hover {
  background-color: rgb(45, 41, 41);
}
.sugestion_trend_item_genre {
  font-size: 14px;
  color: gray;
}
.suggestion_option {
  margin-right: 100px;
  width: 14px;
  height: 14px;
  color: gray;
}
.sugestion_trend_title {
  font-size: 23px;
  font-weight: bold;
}
.sugestion_trend_item_text {
  font-size: 15px;
  color: gray;
}
.sugestion_trend_item_post_count {
  color: gray;
}
.sugestion_trend_more {
  margin-top: 16px;
  color: rgb(29, 155, 240);
}

.suggestion_account_list {
  width: 100%;
  margin-top: 20px;
  background-color: rgb(32, 35, 39);
  border: 1px solid black;
  border-radius: 15px;
  font-weight: bold;
}
.suggestion_account_list_title {
  padding: 12px 16px;
  font-size: 23px;
  font-weight: bold;
}

.account_menu {
  padding: 12px 16px;
  display: flex;
  flex-direction: row;
  align-items: center;
}

.account_details {
  margin-inline: 10px 50px;
  font-size: 15px;
  vertical-align: top;
}
.account_id {
  color: gray;
}
.account_img {
  width: 40px;
  height: 40px;
}

.button_follow {
  margin-left: auto;
  width: 100px;
  height: 30px;
  cursor: pointer;
  text-align: center;
  border-radius: 10px;
  background-color: white;
  color: black;
}
.account_more {
  padding: 16px;
  color: rgb(29, 155, 240);
}
.footer {
  margin-top: 20px;
  padding-inline: 16px;
}
.footer_content {
  display: inline-block;
  margin-inline-end: 12px;
}
</style>
