<template>
  <v-app>
    <v-app-bar color="#AED581">
      <v-app-bar-title class="header-title">MyProfileSite</v-app-bar-title>

      <v-spacer></v-spacer>

      <v-tabs color="white" right>
        <v-tab v-for="item in items" :key="item.link" :to="item.link">
          <span class="white--text">{{ item.name }}</span>
        </v-tab>
      </v-tabs>
    </v-app-bar>
  </v-app>
</template>

<script>
export default {
  name: "HeaderComp",

  data() {
    return {
      items: [
        {
          name: "HOME",
          link: "/",
        },
        {
          name: "ABOUT",
          link: "/about",
        },
        {
          name: "SKILLS",
          link: "/skills",
        },
        {
          name: "WORK",
          link: "/work",
        },
        {
          name: "CONTACT",
          link: "/contact",
        },
      ],
    };
  },
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
