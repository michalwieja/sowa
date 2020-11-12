<template>
  <div>
    <Header />
    <div class="wrapper">
      <div class="content">
        <h1>Oferta</h1>
        <div class="items">
          <p>podatkowa księga przychodów i rozchodów</p>
          <p>ewidencja dla celów zryczałtowanego podatku dochodowego</p>
          <p>księgi handlowe</p>
          <p>obsługa kadrowo-płacowa</p>
          <p>rozliczenia roczne</p>
          <p>sprawozdania finansowe</p>
        </div>

        <h1>Cennik</h1>
        <div class="items">
          <p>Ceny ustalane indywidualnie dla każdego klienta.</p>
          <p>
            Zależą min od: formy działalności, branży, ilości dokumentów, liczby
            pracowników i indywidualnych potrzeb klienta.
          </p>
          <p>Zapraszam bla bla do kontaktu jestem SUPER!!</p>
        </div>
      </div>
      <div class="img">
        <img src="@/assets/cofee.jpg" alt="logo" />
        <div class="block"></div>
      </div>
    </div>
    <Footer />
  </div>
</template>

<script>
</script>

<style scoped>
.wrapper {
  flex-direction: row;
  justify-content: space-evenly;
}
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
  text-align-last: left;
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
