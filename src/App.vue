<template>
  <v-app>
    <main class="app-main">
      <header-comp class="hidden-md-and-down ma-0"></header-comp>
      <router-view />
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
