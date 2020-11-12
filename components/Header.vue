<template>
  <header>
    <div class="top">
      <div class="mail">
        <a href="mailto:mail@mail.mail">
          <font-awesome-icon :icon="['fas', 'envelope']" />
          <span class="desktop">kontakt@biurosowastefanska.pl</span>
        </a>
      </div>
      <div class="tel">
        <a href="tel:512859845">
          <font-awesome-icon :icon="['fas', 'mobile-alt']" />
          <span class="desktop">512 859 845</span>
        </a>
      </div>
    </div>
    <div class="bottom">
      <nav class="nav">
        <div class="logo">
          <NuxtLink class="borderNone" to="/">
            <img src="@/assets/logo-hor.svg" alt="logo" />
          </NuxtLink>
        </div>

        <ul class="nav__links">
          <li><NuxtLink class="nav__link" to="/">Start</NuxtLink></li>
          <li><NuxtLink class="nav__link" to="/oferta">Oferta</NuxtLink></li>
          <li><NuxtLink class="nav__link" to="/cennik">Cennik</NuxtLink></li>
          <li><NuxtLink class="nav__link" to="/omnie">O mnie</NuxtLink></li>
          <li><NuxtLink class="nav__link" to="/kontakt">Kontakt</NuxtLink></li>
        </ul>
        <div class="burger">
          <div class="burger__line"></div>
          <div class="burger__line"></div>
          <div class="burger__line"></div>
        </div>
      </nav>
    </div>
  </header>
</template>

<script>
export default {
  name: "Header",
  mounted() {
    const burger = document.querySelector(".burger");
    const nav = document.querySelector(".nav__links");
    const links = document.querySelectorAll(".nav__link");

    burger.addEventListener("click", () => {
      nav.classList.toggle("nav-active");
      burger.classList.toggle("toggle");
    });
    links.forEach((link, index) => {
      link.addEventListener("click", () => {
        nav.classList.remove("nav-active");
        burger.classList.toggle("toggle");
      });
    });
  },
};
</script>

<style lang='scss' scoped>
$break-small: 900px;
$break-large: 1200px;

.borderNone {
  border: none !important;
}
.nuxt-link-exact-active {
  border-bottom: 1px solid var(--gold);
}
header {
  width: 80%;
  height: 10vh;
  margin: 0 auto;
  .top {
    display: flex;
    align-items: center;
    justify-content: flex-end;
    margin-top: 2vh;
    a {
      color: var(--gold);
      text-decoration: none;
      margin-left: 20px;
    }
  }
}

.nav {
  display: flex;
  justify-content: space-between;
  align-items: center;

  .logo {
    img {
      position: relative;
      height: 8vh;
      z-index: 10000000;
    }
  }

  &__links {
    display: flex;
    width: 50%;
    justify-content: space-between;
    list-style: none;

    @media screen and (max-width: $break-small) {
      position: absolute;
      justify-content: space-evenly;

      background-color: black;
      right: 0;
      height: 88vh;
      top: 12vh;
      display: flex;
      flex-direction: column;
      align-items: center;
      width: 100%;
      transform: translateX(100%);
      transition: 0.3s;
      z-index: 2;
    }
  }

  &__link {
    text-decoration: none;
    text-transform: uppercase;
    letter-spacing: 2px;
    color: var(--gold);
    @media screen and (max-width: $break-small) {
      // opacity: 0;
    }
  }

  .burger {
    display: none;
    cursor: pointer;

    @media screen and (max-width: $break-small) {
      display: block;
    }

    &__line {
      background-color: var(--gold);
      width: 25px;
      height: 3px;
      margin: 5px;
      transition: 0.2s;
    }
  }
}

.toggle .burger__line:nth-child(1) {
  transform: rotate(-45deg) translate(-5px, 6px);
}

.toggle .burger__line:nth-child(2) {
  opacity: 0;
}

.toggle .burger__line:nth-child(3) {
  transform: rotate(45deg) translate(-5px, -6px);
}

.nav-active {
  transform: translateX(0);
}

@media screen and (max-width: $break-small) {
  .desktop {
    display: none;
  }
}
</style>