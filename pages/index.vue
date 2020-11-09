<template>
  <div class="wrapper">
    <h2 class="hero">Natalia Sowa-Stefańska</h2>
    <h1 class="hero">Księgowa, której szukasz</h1>
    <button><NuxtLink class="link" to="/offer">WIĘCEJ</NuxtLink></button>
  </div>
</template>

<script>
export default {};
</script>

<style scoped>
.wrapper {
  padding-top: 55vh;
}
.wrapper::before {
  content: "";
  position: absolute;
  top: 0;
  left: 0;
  width: 100%;
  height: 100%;
  background-image: url("../assets/hero.jpg");
  background-size: cover;
  background-position: top;
  z-index: -1;
}
a.link {
  color: var(--gold);
  text-decoration: none;
}

h1.title {
  font-size: 5vh;
}
h2.title {
  font-size: 5vh;
}
</style>
