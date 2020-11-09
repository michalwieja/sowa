<template>
  <div>
    <div class="wrapper">
      <h1>Godziny pracy</h1>

      <p>
        Elastyczne godziny pracy, możliwość spotkania w godzinach dogodnych dla
        klienta, dojazd do klienta, kontakt zdalny
      </p>
      <h1>Dane firmy</h1>
      <p>
        Biuro Rachunkowe Natalia Sowa-Stefańska ul. Dulęby 5/601 40-833 Katowice
        <!-- tel: 512859845 mail: nsowastefanska@gmail.com -->
      </p>
      <h1>Dojazd</h1>
      <iframe
        width="600"
        height="250"
        frameborder="0"
        style="border: 0"
        src="https://www.google.com/maps/embed/v1/place?q=ul.%20Dul%C4%99by%205%2F601%2040-833%20Katowice&key=AIzaSyDw1zhsW5hcgQrPmCp3XrvpkMRFuKj9R-o"
        allowfullscreen
      ></iframe>
    </div>
    <Footer />
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
@media (max-width: 800px) {
  iframe {
    width: 90%;
    height: 100px;
  }
}
</style>