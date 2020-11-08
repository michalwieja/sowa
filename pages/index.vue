<template>
  <div class="wrapper">
    <h2>Natalia Sowa-Stefańska</h2>
    <h1>Księgowa, której szukasz</h1>
    <button>WIĘCEJ</button>
  </div>
</template>

<script>
export default {};
</script>

<style scoped>
.wrapper {
  padding-top: 25vh;
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
h2 {
  font-size: 5vh;
}
h1 {
  font-size: 7vh;
}
@media (max-width: 800px) {
  h2 {
    font-size: 3vh;
  }
  h1 {
    font-size: 5vh;
  }
}
@media (max-width: 600px) {
  h2 {
    font-size: 3vh;
  }
  h1 {
    font-size: 3vh;
  }
}
button {
  width: 20%;
  border: none;
  background: var(--gold);
  height: 30px;
  border-radius: 10px;
  margin-top: 20px;
}
</style>
