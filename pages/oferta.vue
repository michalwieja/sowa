<template>
  <div>
    <Header />
    <div class="wrapper">
      <div class="content">
        <h1>Oferta</h1>
        <ul class="items">
          <li>podatkowa księga przychodów i rozchodów</li>
          <li>ewidencja dla celów zryczałtowanego podatku dochodowego</li>
          <li>księgi handlowe</li>
          <li>obsługa kadrowo-płacowa</li>
          <li>rozliczenia roczne</li>
          <li>sprawozdania finansowe</li>
        </ul>
        <small class="items">
          Dla Twojej wygody i bezpieczeństwa oferuję również księgowość
          zdalną(elektroniczne przekazywanie dokumentów, spotkania online).
          <br />
          Na stałe współpracuje z kancelarią adwokacką Tomasza Hartleba
          <a href=" www.kancelaria-th.pl" rel="noopener noreferrer ">
            www.kancelaria-th.pl</a
          >
        </small>

        <h1>DLA KOGO</h1>
        <div class="items">
          Współpracuję z osobami fizycznymi prowadzącymi działalność
          gospodarczą, spółkami osobowymi i kapitałowymi.
        </div>
        <ul class="items">
          <li>
            Otwierasz firmę i potrzebujesz profesjonalnego wsparcia? Możesz
            liczyć na moją pomoc na każdym etapie.
          </li>
          <li>
            Przekształcasz swoją działalność i potrzebujesz wsparcia? Mam
            doświadczenie w tym zakresie.
          </li>
          <li>Stawiam na księgowośc z indywidualnym podejściem do klienta.</li>
        </ul>
      </div>
      <div class="img desktop">
        <img src="@/assets/cofee.jpg" alt="logo" />
        <div class="block"></div>
      </div>
    </div>
    <Footer />
  </div>
</template>

<script>
</script>

<style scoped lang='scss'>
.content {
  padding-bottom: 10vh;
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

@media (max-width: 1200px) {
  .wrapper {
    height: auto;
    width: 100%;
  }
  .content {
    padding: 10vh 0;
    width: 100%;
  }
  h1 {
    font-size: 24px;
  }

  .items {
    width: 90%;
    text-align: left;
    margin: 25px;
  }

  .img {
    display: none;
  }
} ;
</style>
