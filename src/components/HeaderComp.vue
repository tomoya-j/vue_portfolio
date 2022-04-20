<template>
  <v-app>
    <v-app-bar color="#AED581">
      <v-app-bar-title class="header-title">MyProfileSite</v-app-bar-title>

      <v-spacer></v-spacer>

      <template>
        <v-tabs color="white" right>
          <v-tab to="/">HOME</v-tab>
          <v-tab to="/about">ABOUT</v-tab>
        </v-tabs>
      </template>
    </v-app-bar>
  </v-app>
</template>

<script>
export default {
  name: "HeaderComp",
};
</script>

<style scoped>
.header-title {
  color: aliceblue;
  font-size: 30px;
}
a:hover {
  opacity: 0.3;
}
</style>
