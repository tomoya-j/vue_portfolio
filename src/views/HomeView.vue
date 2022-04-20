<template>
  <div>
    <h1 class="fadeUp">Welcome to My Profile Site!</h1>
  </div>
</template>

<script>
export default {
  name: "HomeView",
};
</script>

<style scoped>
@import url("https://fonts.googleapis.com/css2?family=Bitter:wght@400;700&family=PT+Serif:ital@1&display=swap");

h1 {
  display: flex;
  color: aliceblue;
  justify-content: center;
  margin-top: 150px;
  font-family: "PT Serif", serif;
  font-size: 5rem;
}

.fadeUp {
  animation-name: fadeUpAnime;
  animation-duration: 2s;
  animation-fill-mode: forwards;
  opacity: 0;
}

@keyframes fadeUpAnime {
  from {
    opacity: 0;
    transform: translateY(150px);
  }

  to {
    opacity: 1;
    transform: translateY(0);
  }
}
</style>
