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
  background-color: #000;
}
.site {
  position: relative;
  overflow: hidden;
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
  text-align: center;
  padding-top: 10vh;
}

h1 {
  font-size: 7vh;

  margin: 5vh;
}
h2 {
  font-size: 5vh;
}
p {
  margin: 5px;
}
button {
  width: 25%;
  border: 2px solid var(--gold);
  background: transparent;
  color: var(--gold);
  height: 35px;
  font-size: 18px;
  border-radius: 10px;
  margin-top: 20px;
}
@media (max-width: 800px) {
  .wrapper {
    width: 90%;
  }
  h2 {
    font-size: 3vh;
  }
  h1 {
    font-size: 5vh;
  }
}

@keyframes navLinkFade {
  from {
    opacity: 0;
    transform: translateX(50px);
  }

  to {
    opacity: 1;
    transform: translateX(0);
  }
}
</style>



