<template>
  <v-app>
    <main class="app-main">
      <header-comp />
      <router-view />
    </main>
  </v-app>
</template>

<script>
import HeaderComp from "./components/HeaderComp.vue";

export default {
  name: "App",

  components: {
    HeaderComp,
  },

  data: () => ({
    //
  }),
};
</script>

<style>
.v-application--wrap {
  min-height: 0;
}

.app-main {
  height: 100vh;
  background: url("./assets/imgs/vinyl.jpg");
  background-size: cover;
}
</style>
