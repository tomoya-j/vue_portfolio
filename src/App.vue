<template>
  <v-app>
    <v-main>
      <header-comp />
      <router-view />
    </v-main>
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
</style>
