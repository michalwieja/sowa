<template>
  <div>
    <Header />
    <div class="wrapper">
      <div class="content">
        <h1>KONTAKT</h1>
        <div class="items">
          Pracuję stacjonarnie w swoim biurze W katowicach, ulica Dulęby 5, ale
          bez problemu możemy spotkać się w siedzibie Twojej firmy. Nie mam
          określonych ram czasowych pracy jeśli potrzebujesz tu i teraz wsparcia
          i porady - jestem dostępna
          <a
            href="mailto:kontakt@biurosowastefanska
"
            >mailowo</a
          >
          lub <a href="tel:512859845">telefonicznie</a>
        </div>
        <h1>Godziny pracy</h1>
        <div class="items">
          Elastyczne godziny pracy, możliwość spotkania w godzinach dogodnych
          dla klienta, dojazd do klienta, kontakt zdalny
        </div>
      </div>
      <div class="img">
        <iframe
          width="600"
          height="250"
          frameborder="0"
          src="https://www.google.com/maps/embed/v1/place?q=ul.%20Dul%C4%99by%205%2F601%2040-833%20Katowice&amp;key=AIzaSyDw1zhsW5hcgQrPmCp3XrvpkMRFuKj9R-o"
          allowfullscreen=""
          style="border: 0"
          data-v-9785e590=""
        ></iframe>
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
  padding-bottom: 30vh;
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
  top: -100px;
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
