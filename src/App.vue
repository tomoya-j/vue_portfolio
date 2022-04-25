<template>
  <v-app>
    <main class="app-main">
      <header-comp class="hidden-md-and-down ma-0"></header-comp>
      <transition
        name="costom-transition"
        mode="out-in"
        :duration="transition.duration"
        :enter-active-class="transition.enter"
        :leave-active-class="transition.leave"
      >
        <router-view />
      </transition>
      <bottom-nav class="hidden-md-and-up ma-0 app-bottom-nav"></bottom-nav>
    </main>
  </v-app>
</template>

<script>
import HeaderComp from "./components/HeaderComp.vue";
import BottomNav from "./components/BottomNavigation.vue";

export default {
  name: "App",

  components: {
    HeaderComp,
    BottomNav,
  },
  watch: {
    $route(to, from) {
      if (to.meta.index > from.meta.index) {
        this.transition.enter =
          "animate__animated animate__fadeInRight animate__faster";
        this.transition.leave =
          "animate__animated animate__fadeOutLeft animate__faster";
        console.log("hoge");
      } else {
        this.transition.enter =
          "animate__animated animate__fadeInLeft animate__faster";
        this.transition.leave =
          "animate__animated animate__fadeOutRight animate__faster";
        console.log("fuga");
      }
    },
  },
  data() {
    return {
      transition: {
        enter: "",
        leave: "",
        duration: 700,
      },
    };
  },
};
</script>

<style>
.v-application--wrap {
  min-height: 0;
}

.app-main {
  height: 100vh;
  width: 100%;
  background-image: url("./assets/imgs/vinyl.jpg");
  background-size: cover;
  -webkit-backface-visibility: hidden;
  backface-visibility: hidden;
  overflow: hidden;
}

@media screen and(max-width:480px) {
  .app-main {
    background-position: 70% 30%;
  }
}

.app-bottom-nav {
  position: absolute;
  bottom: 0;
}
</style>
