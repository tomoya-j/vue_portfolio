<template>
  <div class="contact-container">
    <h1 class="contact-ttl">Contact</h1>
    <div class="contact-main">
      <v-card class="contact-card" elevation="4">
        <v-card-title class="contact-card_ttl">お問い合わせ</v-card-title>
        <p class="contact-card_comment">お気軽にお問い合わせください！</p>
        <p class="contact-card_adress">
          mail:
          <a href="mailto:tosn.mosd719@gmail.com">tosn.mosd719@gmail.com</a>
        </p>
        <p class="contact-card_adress">
          github:
          <a href="https://github.com/tomoya-j">https://github.com/tomoya-j</a>
        </p>
      </v-card>
    </div>
  </div>
</template>

<script>
export default {
  name: "ContactView",
};
</script>

<style lang="scss" scoped>
@import url("https://fonts.googleapis.com/css2?family=Bitter:wght@400;700&family=PT+Serif:ital@1&display=swap");

.contact-container {
  margin: 0 auto;
  width: 85%;

  .contact-ttl {
    height: 20%;
    text-align: center;
    font-size: 50px;
    color: aliceblue;
    border-bottom: 1px solid #fff;
    font-family: "PT Serif", serif;
  }

  .contact-main {
    display: flex;
    flex-wrap: wrap;
    justify-content: center;

    .contact-card {
      margin-top: 5%;
      width: 50%;
      height: 200px;

      @media screen and(max-width:480px) {
        width: 85%;
        height: 200px;
      }

      &_ttl {
        justify-content: center;
        margin: 0 5%;
        padding: 10px;
        border-bottom: 1px solid #000;
      }

      &_comment {
        width: 47%;
        margin: 0 auto;
        padding: 10px;

        @media screen and(max-width:480px) {
          width: 95%;
          height: 50px;
        }
      }
      &_adress {
        display: block;
        margin: 2% 25%;

        @media screen and(max-width:480px) {
          margin: 0 auto;
          width: 90%;
          height: 30px;
        }
      }
    }
  }
}
</style>
