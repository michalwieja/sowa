<template>
  <div>
    <Header />
    <div class="wrapper">
      <div class="content">
        <h1>O MNIE</h1>
        <div class="items">
          <p>Nazywam się Natalia Sowa Stefańska.</p>
          <p>
            Jestem absolwentką Uniwersytetu Ekonomicznego w Katowicach na
            wydziale Finanse i Rachunkowość.
          </p>
          <p>
            <br />
            Pracę w księgowości rozpoczęłam w 2007r. Doświadczenie zdobywałam w
            biurze rachunkowym dzięki czemu mam szeroką i zróżnicowaną wiedzę w
            zakresie podatków, ubezpieczeń społecznych oraz spraw pracowniczych.
          </p>
          <p>
            Posiadam Certyfikat Księgowy Ministra Finansów nr 46638/2010
            Wychodzę z założenia, że za dobrą księgowością stoi profesjonalista:
            sumienny i pracowity człowiek, który jest otwarty na klienta i co
            więcej potrafi przeprowadzić go przez temat księgowości od A do Z.
            To ciągłe zwiększanie swoich kompetencji i pogłębianie wiedzy.
          </p>
          <p>
            <br />
            Prywatnie jestem żoną i mamą dwójki chłopców. Uwielbiam górskie
            wycieczki i dobrą literaturę.
          </p>
        </div>
      </div>
      <div class="img">
        <img src="@/assets/natalia.jpg" alt="logo" />
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
  padding-bottom: 20vh;
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
