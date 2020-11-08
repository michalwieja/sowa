<template>
  <div>
    <div class="wrapper offer">
      <h1>Oferta</h1>

      <p>podatkowa księga przychodów i rozchodów</p>
      <p>ewidencja dla celów zryczałtowanego podatku dochodowego</p>
      <p>księgi handlowe</p>
      <p>obsługa kadrowo-płacowa</p>
      <p>rozliczenia roczne</p>
      <p>sprawozdania finansowe</p>

      <h1>Cennik</h1>
      <p>Ceny ustalane indywidualnie dla każdego klienta.</p>
      <p>
        Zależą min od: formy działalności, branży, ilości dokumentów, liczby
        pracowników i indywidualnych potrzeb klienta.
      </p>
      <p>Zapraszam bla bla do kontaktu jestem SUPER!!</p>
    </div>
  </div>
</template>

<script>
export default {};
</script>

<style scoped>
.wrapper::before {
  content: "";
  position: absolute;
  top: 0;
  left: 0;
  width: 100%;
  height: 100%;
  background: #000;
  z-index: -1;
}

.wrapper {
  padding-top: 10vh;
}

h1 {
  margin: 5vh;
}
p {
  margin: 5px;
}
@media (max-width: 800px) {
  .wrapper {
    width: 90%;
  }
}
</style>
