<template>
  <div class="about-container">
    <h1 class="about-ttl">About me</h1>
    <div class="about-main">
      <img
        src="../assets/imgs/image1.jpg"
        class="about-img"
        alt="プロフィール写真"
      />
      <v-card class="about-card" elevation="5" shaped right>
        <h2 class="about-card_info">Profile</h2>
        <h3 class="about-card_info">Name : Arai Tomoya</h3>
        <h3 class="about-card_info">BirthYear : 1998</h3>
        <h3 class="about-card_info">From : Saitama</h3>
        <h3 class="about-card_info">Like : music, anime, comics</h3>
        <p class="about-card_comment">
          大学時代は経済学部に所属し、就職活動の際にプログラマーという職業に興味を持ち、2022年からフロントエンドエンジニアを目指し、本格的に学習を始めました。<br />音楽やアニメを見ることが好きで、高校時代からバンドを始め、現在でも楽器を弾いたりパソコンを使って作曲をすることなどが趣味です！
        </p>
      </v-card>
    </div>
  </div>
</template>

<script>
export default {
  name: "AboutView",
};
</script>

<style lang="scss" scoped>
@import url("https://fonts.googleapis.com/css2?family=Bitter:wght@400;700&family=PT+Serif:ital@1&display=swap");

.about-container {
  margin: 0 auto;
  width: 85%;

  .about-ttl {
    height: 20%;
    text-align: center;
    font-size: 50px;
    color: aliceblue;
    border-bottom: 1px solid #fff;
    font-family: "PT Serif", serif;
  }

  .about-main {
    display: flex;
    flex-wrap: wrap;

    .about-img {
      margin: 5%;
      border-radius: 50%;
      height: 35%;
      width: 35%;
      @media screen and(max-width:480px) {
        width: 90%;
        height: 90%;
      }
    }

    .about-card {
      margin: 5%;
      font-family: "PT Serif", serif;
      color: rgb(118, 114, 114);
      width: 40%;
      height: 60%;
      @media screen and(max-width:480px) {
        width: 100%;
        height: 30%;
      }

      .v-application p {
        margin-bottom: 0px;
      }

      &_info {
        color: rgb(118, 114, 114);
        font-size: 20px;
        padding: 8px 0px 0px 25px;
        font-weight: 200;
        @media screen and(max-width:480px) {
          width: 100%;
          height: 30%;
          font-size: 17px;
          font-weight: 150;
        }
      }

      &_comment {
        width: 85%;
        margin: 0 auto;
        color: rgb(118, 114, 114);
        font-size: 17px;
        padding: 8px;
        border-top: 1px solid rgb(118, 114, 114);
        @media screen and(max-width:480px) {
          width: 100%;
          height: 20%;
          font-size: 15px;
        }
      }
    }
  }
}
</style>
