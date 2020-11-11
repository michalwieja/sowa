<template>
  <div>
    <Header />
    <div class="wrapper">
      <h2 class="">Natalia Sowa-Stefańska</h2>
      <h1 class="">Księgowa, której szukasz</h1>
      <button><NuxtLink class="link" to="/oferta">WIĘCEJ</NuxtLink></button>
    </div>
  </div>
</template>

<script>
export default {};
</script>

<style>
.wrapper::before {
  background-image: url("../assets/hero.jpg");
}
</style>
