<template>
  <div>
    <Header />
    <div class="wrapper">
      <div class="content">
        <h1 class="title">Księgowa, której szukasz</h1>
        <NuxtLink class="link" to="/oferta"> <button>WIĘCEJ</button></NuxtLink>
      </div>
    </div>
  </div>
</template>

<script>
export default {};
</script>

<style scoped lang='scss'>
.wrapper {
  height: 88vh;
}
.content {
  align-items: center;
  justify-content: center;
  padding-top: 20vh;
}
h1 {
  color: var(--gold);
  text-align: center;
  &::before {
    display: none;
  }
}
.wrapper::before {
  background-image: url("../assets/hero.jpg");
}
</style>
