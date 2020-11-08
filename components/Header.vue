<template>
  <header>
    <!-- <div class="logo">
      <img src="@/assets/logo.svg" alt="logo" />
    </div> -->
    <nav>
      <ul>
        <li><NuxtLink to="/">Start</NuxtLink></li>
        <li><NuxtLink to="/offer">Oferta</NuxtLink></li>
        <li><NuxtLink to="/about">O nas</NuxtLink></li>
      </ul>
    </nav>
  </header>
</template>

<script>
export default {
  name: "Header",
};
</script>

<style scoped>
header {
  position: absolute;
  width: 100%;
}
.nuxt-link-exact-active {
  border-bottom: 1px solid var(--gold);
}
nav {
  width: 50%;
  margin: 0 auto;
  height: 10vh;
  display: flex;
  align-items: center;
  justify-content: space-between;
}
ul {
  width: 100%;
  display: flex;
  align-items: center;
  justify-content: space-between;
  list-style: none;
}
li a {
  color: var(--gold);
  text-decoration: none;
  text-transform: uppercase;
}
</style>