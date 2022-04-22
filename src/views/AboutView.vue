<template>
  <div>
    <h1 class="title-about">About me</h1>
    <div class="about-main">
      <img src="../assets/imgs/image1.jpg" alt="" />
      <v-card
        class="about-card"
        elevation="5"
        shaped
        width="550px"
        height="400px"
        right
      >
        <h2 class="about-card__title">Profile</h2>
        <h3>Name : Arai Tomoya</h3>
        <h3>BirthYear : 1998</h3>
        <h3>From : Saitama</h3>
        <h3>Like : music, anime, comics</h3>
        <p class="about-comment">
          就職活動の際にプログラマーという職業に興味を持ち、2022年からフロントエンドエンジニアを目指し、
          本格的に学習を始めました。<br />音楽やアニメを見ることが好きで、高校時代からバンドを始め、現在でも楽器を弾いたりパソコンを使って作曲をすることなどが趣味です！
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

<style scoped>
@import url("https://fonts.googleapis.com/css2?family=Bitter:wght@400;700&family=PT+Serif:ital@1&display=swap");

.title-about {
  display: flex;
  height: 100px;
  font-size: 50px;
  color: aliceblue;
  justify-content: center;
  align-items: center;
  margin: 0 100px 0 100px;
  border-bottom: 1px solid #fff;
  font-family: "PT Serif", serif;
}

.about-main {
  display: flex;
  position: relative;
}

img {
  position: absolute;
  border-radius: 50%;
  height: 400px;
  width: 400px;
  top: 100px;
  left: 180px;
}

.about-card {
  position: absolute;
  top: 100px;
  left: 700px;
  font-family: "PT Serif", serif;
  color: rgb(118, 114, 114);
}

.about-card__title {
  width: 500px;
  margin: 0 auto;
  text-align: center;
  border-bottom: 1px solid rgb(104, 101, 101);
  color: rgb(118, 114, 114);
}

.v-application p {
  margin-bottom: 0px;
}

.about-card h3 {
  color: rgb(118, 114, 114);
  font-size: 20px;
  padding: 8px 0px 0px 25px;
  font-weight: 200;
}

.about-card p {
  width: 500px;
  margin: 0 auto;
  color: rgb(118, 114, 114);
  font-size: 17px;
  padding: 8px;
  border-top: 1px solid rgb(118, 114, 114);
}
</style>
