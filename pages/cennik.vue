<template>
  <div>
    <Header />
    <div class="wrapper">
      <div class="content">
        <h1>Cennik</h1>
        <div class="items">
          Współpraca z zróżnorodnymi firmi pokazała mi jak ważne jest
          indywidualne podejście do każdego klienta. Każde przedsiębiorstwo jest
          inne pod względem potrzeb i oczekiwań w zakresie księgowości. Dlatego
          zapraszam do niezobowiązującego kontaktu. Przygotuję dla Ciebie
          indywidualną wycenę na podstawie informacji takich jak:
        </div>
        <ul class="items">
          <li>forma działalności jaką prowadzisz</li>
          <li>branża jaką się zajmujesz</li>
          <li>w przybliżeniu ilość dokumentów miesięcznie</li>
          <li>liczba zatrudnionych pracowników</li>
          <li>liczba umów cywilnoprawnych</li>
        </ul>
      </div>
      <div class="img">
        <img src="@/assets/glasses.jpg" alt="logo" />
        <div class="block"></div>
      </div>
    </div>
    <Footer />
  </div>
</template>

<script>
</script>

<style scoped>
.content {
  display: flex;
  flex-direction: column;
  align-items: flex-start;
  justify-content: space-evenly;
  height: 100%;
  width: 40%;
}
h1 {
  width: 100%;
  color: #000;
  position: relative;
  font-family: "Montserrat", sans-serif;
  font-weight: 400;
  text-transform: uppercase;
}
h1::before {
  content: "";
  position: absolute;
  top: 0;
  left: -25%;
  height: 100%;
  width: 100%;
  background-color: var(--gold);
  z-index: -1;
}
.items {
  width: 75%;
  text-align: left;
}
p {
  font-size: 18px;
}
.wrapper::before {
  background: #000;
}
.img {
  position: relative;
}
.img::before {
  content: "";
  position: absolute;

  top: 5%;
  left: 5%;
  height: 100%;
  width: 100%;
  background-color: var(--gold);
  z-index: -1;
}
</style>
