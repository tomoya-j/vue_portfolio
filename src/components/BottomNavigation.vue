<template>
  <div>
    <v-bottom-navigation grow app>
      <v-btn
        v-for="item in items"
        :key="item.link"
        :to="item.link"
        color="#AED581"
      >
        <span class="white--text">{{ item.name }}</span>
      </v-btn>
    </v-bottom-navigation>
  </div>
</template>
<script>
export default {
  name: "BottomNav",

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
      ],
    };
  },
};
</script>
