<template>
  <div class="site">
    <Header />
    <Nuxt />
  </div>
</template>
<script>
import Header from "../components/Header";

export default {
  components: {
    Header,
  },
};
</script>


<style>
:root {
  --gold: #c3a26f;
}
html {
  font-family: "Source Sans Pro", -apple-system, BlinkMacSystemFont, "Segoe UI",
    Roboto, "Helvetica Neue", Arial, sans-serif;
  font-size: 16px;
  word-spacing: 1px;
  -ms-text-size-adjust: 100%;
  -webkit-text-size-adjust: 100%;
  -moz-osx-font-smoothing: grayscale;
  -webkit-font-smoothing: antialiased;
  box-sizing: border-box;
  color: white;
}

*,
*::before,
*::after {
  box-sizing: border-box;
  margin: 0;
  padding: 0;
}

.wrapper {
  min-height: 100vh;
  max-width: 1000px;
  margin: 0 auto;
  color: var(--gold);
  display: flex;
  flex-direction: column;
  align-items: center;
  justify-content: center;
  text-align: center;
}
</style>



