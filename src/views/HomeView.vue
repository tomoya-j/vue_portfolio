<template>
  <div>
    <h1 class="title-home fadeUp">
      Welcome <br class="br_sp" />to My <br class="br_sp" />
      Profile <br class="br_sp" />Site!
    </h1>
  </div>
</template>

<script>
export default {
  name: "HomeView",
};
</script>

<style lang="scss" scoped>
@import url("https://fonts.googleapis.com/css2?family=Bitter:wght@400;700&family=PT+Serif:ital@1&display=swap");

.title-home {
  color: aliceblue;
  text-align: center;
  margin-top: 11%;
  font-family: "PT Serif", serif;
  font-size: 5rem;

  @media screen and(min-width:768px) {
    .br_sp {
      display: none;
    }
  }
}
</style>
