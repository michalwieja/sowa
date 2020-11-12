<template>
  <div>
    <Header />
    <div class="wrapper">
      <!-- <h2 class="">Natalia Sowa-Stefańska</h2> -->
      <h1 class="title">Księgowa, której szukasz</h1>
      <button><NuxtLink class="link" to="/oferta">WIĘCEJ</NuxtLink></button>
    </div>
  </div>
</template>

<script>
export default {};
</script>

<style scoped>
.wrapper {
  flex-direction: column;
  justify-content: center;
}
.title {
  margin: 30vh 0 5vh 0;
  font-size: 40px;
}
.wrapper::before {
  background-image: url("../assets/hero.jpg");
}
</style>
