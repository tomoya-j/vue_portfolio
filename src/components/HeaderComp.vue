<template>
  <v-app>
    <v-app-bar>
      <v-toolbar-title>MyPortfolio</v-toolbar-title>

      <v-spacer></v-spacer>

      <v-tabs right>
        <v-tab to="/">HOME</v-tab>
        <v-tab to="/about">ABOUT</v-tab>
      </v-tabs>
    </v-app-bar>
  </v-app>
</template>

<script>
export default {
  name: "HeaderComp",
};
</script>
