<template>
  <div class="wrapper">
    <h1>O mnie</h1>
    <p>
      Ukończony Uniwersytet Ekonomiczny na wydziale Finanse i Rachunkowość ze
      specjalnością Rachunkowość.
    </p>
    <p>
      12 lat doświadczenia w księgowości, prowadzenie księgowości w różnorodnych
      firmach(osoby fizyczne, spółki osobowe, spółki kapitałowe)
    </p>

    <p>Certyfikat Księgowy Ministra Finansów nr 46638/2010</p>
    <p>Obowiązkowe ubezpieczenie OC - odnawiane co roku.</p>
    <p>
      Zawsze na bieżąco: systematyczne uczestnictwo w szkoleniach i
      aktualizowanie wiedzy
    </p>
    <p>indywidualne podejście do każdego klienta</p>
    <p>profesjonalność i sumienność</p>
    <p>
      stała współpraca z Kancelarią adwokata Tomasza Hartleba :
      http://www.kancelaria-th.pl/
    </p>
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