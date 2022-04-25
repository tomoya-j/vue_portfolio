<template>
  <div class="work-container">
    <h1 class="work-ttl">My Work</h1>
    <div class="work-main">
      <v-card class="work-card" elevation="4">
        <img
          src="../assets/imgs/site_photo.png"
          class="work-card_img"
          alt="ポートフォリオサイトのスクリーンショット"
        />
        <v-card-title class="work-card_ttl">ポートフォリオサイト</v-card-title>
        <p class="work-card_comment">
          フロントエンドの学習のためvue.jsを使用して作成したポートフォリオサイトです。
          <br />手探りではありますが形にすることが出来て良い経験になりました。
        </p>
      </v-card>
      <v-card class="work-card" elevation="4">
        <v-card-title class="work-card_progress">on progress...</v-card-title>
      </v-card>
      <v-card class="work-card" elevation="4">
        <v-card-title class="work-card_progress">on progress...</v-card-title>
      </v-card>
    </div>
  </div>
</template>

<script>
export default {
  name: "WorkView",
};
</script>

<style lang="scss" scoped>
@import url("https://fonts.googleapis.com/css2?family=Bitter:wght@400;700&family=PT+Serif:ital@1&display=swap");

.work-container {
  margin: 0 auto;
  width: 85%;

  .work-ttl {
    height: 20%;
    text-align: center;
    font-size: 50px;
    color: aliceblue;
    border-bottom: 1px solid #fff;
    font-family: "PT Serif", serif;
  }

  .work-main {
    display: flex;
    flex-wrap: wrap;
    justify-content: center;

    .work-card {
      margin: 2.5%;
      font-family: "PT Serif", serif;
      color: rgb(66, 65, 65);
      width: 25%;
      height: 60%;

      &_ttl {
        justify-content: center;
        border-bottom: 1px solid rgb(118, 114, 114);
        margin: 2%;
        padding: 0px;
      }

      &_img {
        margin: 2%;
        width: 96%;
        height: 96%;
      }

      &_comment {
        margin: 0 5% 5% 5%;
        height: 130px;
      }

      &_progress {
        width: 155px;
        margin: 25%;
      }
    }
  }
}
</style>
