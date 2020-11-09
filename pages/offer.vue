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
.wrapper::after {
  content: "";
  position: absolute;
  top: 10%;
  left: 10%;
  width: 80%;
  height: 80%;
  background-image: url("../assets/logo.svg");
  background-size: contain;
  background-repeat: no-repeat;
  opacity: 0.05;
  z-index: -1;
}
</style>
