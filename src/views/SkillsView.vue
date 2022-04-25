<template>
  <div class="skills-container">
    <h1 class="skills-ttl">Skills</h1>
    <div class="skills-main">
      <v-card class="skills-card" elevation="4">
        <v-card-title class="skills-card_ttl">HTML/CSS</v-card-title>
        <img
          src="../assets/icons/html_icon.svg"
          class="skills-card_icon"
          alt="htmlのアイコン"
        />
        <p class="skills-card_comment">
          シンプルで参考文献も多く学習しやすいですが、特にCSSは奥が深くまだまだあいまいな部分もあるので、今後は設計思想も意識しつつ可読性の高いコードを書けるようになるのが目標です!
        </p>
      </v-card>

      <v-card class="skills-card" elevation="4">
        <v-card-title class="skills-card_ttl">JavaScript</v-card-title>
        <img
          src="../assets/icons/JavaScript_icon.svg"
          class="skills-card_icon"
          alt="javascriptのアイコン"
        />
        <p class="skills-card_comment">
          初めて学習したプログラミング言語です。今後は基礎を固め、より柔軟なプログラムを書けるようにな
          り、Vue.jsやReact.jsなどのフレームワークを使った開発にも挑戦したいと考えています!
        </p>
      </v-card>

      <v-card class="skills-card" elevation="4">
        <v-card-title class="skills-card_ttl">Guitar</v-card-title>
        <img
          src="../assets/icons/guitar_icon.svg"
          class="skills-card_icon"
          alt="guitarのアイコン"
        />
        <p class="skills-card_comment">
          中学時代からギターを始めました。ギターは不完全な楽器ですが、それ故に愛着がわきます！弾き始めると時間を忘れて練習してしまいます！
        </p>
      </v-card>

      <v-card class="skills-card" elevation="4">
        <v-card-title class="skills-card_ttl">Game</v-card-title>
        <img
          src="../assets/icons/game_icon.svg"
          class="skills-card_icon"
          alt="gameのアイコン"
        />
        <p class="skills-card_comment">
          FPSゲームやアクションゲームが得意です！もし機会があればオンラインで一緒にプレイしましょう！
        </p>
      </v-card>
    </div>
  </div>
</template>

<script>
export default {};
</script>

<style lang="scss" scoped>
.skills-container {
  margin: 0 auto;
  width: 85%;

  .skills-ttl {
    height: 20%;
    text-align: center;
    font-size: 50px;
    color: aliceblue;
    border-bottom: 1px solid #fff;
    font-family: "PT Serif", serif;
  }

  .skills-main {
    display: flex;
    flex-wrap: wrap;

    @media screen and(max-width:480px) {
      justify-content: center;
    }

    .skills-card {
      margin: 2.5%;
      font-family: "PT Serif", serif;
      color: rgb(66, 65, 65);
      width: 20%;
      height: 60%;

      @media screen and(max-width:480px) {
        width: 40%;
        height: 20%;
      }

      &_ttl {
        justify-content: center;
        border-bottom: 1px solid rgb(118, 114, 114);

        @media screen and(max-width:480px) {
          width: 100%;
          height: 30px;
          padding: 0;
        }
      }

      &_icon {
        margin: 5% 25%;
        width: 50%;
        height: 50%;
      }

      &_comment {
        margin: 0 5% 5% 5%;
        border-top: 1px solid rgb(118, 114, 114);
        height: 200px;

        @media screen and(max-width:480px) {
          width: 90%;
          height: 120px;
          font-size: 5px;
        }
      }
    }
  }
}
</style>
