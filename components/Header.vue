<template>
  <header>
    <nav class="nav">
      <div class="logo">
        <NuxtLink class="nav__link borderNone" to="/">
          <svg
            width="33"
            height="47"
            viewBox="0 0 131 188"
            fill="none"
            xmlns="http://www.w3.org/2000/svg"
          >
            <path
              fill-rule="evenodd"
              clip-rule="evenodd"
              d="M21.8326 85.4067L35.318 134.211L95.6808 168.887L83.4798 123.294L66.7837 78.343L21.8326 85.4067ZM24.1509 86.9014L36.8871 132.994L92.7647 165.094L81.7282 123.852L65.5851 80.3904L24.1509 86.9014Z"
              fill="#84673B"
            />
            <path
              d="M91.8291 122.652L75.133 78.9854L109.167 86.0491V187.51L91.8291 122.652Z"
              fill="url(#paint0_linear)"
            />
            <path
              d="M131 54.3944L111.735 77.0587L66.7843 70.6372L19.2647 77.0587L0 54.3944V22.6643L19.2647 0L66.7843 9.06573L111.735 0L131 22.6643V54.3944Z"
              fill="url(#paint1_linear)"
            />
            <path
              d="M24.4023 43.1529V39.0431L27.4846 35.9608H31.5944L34.6768 39.0431V43.1529L31.5944 46.2353H27.4846L24.4023 43.1529Z"
              fill="black"
            />
            <path
              fill-rule="evenodd"
              clip-rule="evenodd"
              d="M27.1043 35.0425H31.9748L35.595 38.6628V43.5333L31.9748 47.1535H27.1043L23.4841 43.5333V38.6628L27.1043 35.0425ZM27.865 36.879L25.3205 39.4235V42.7726L27.865 45.317H31.2141L33.7586 42.7726V39.4235L31.2141 36.879H27.865Z"
              fill="black"
            />
            <path
              d="M96.3233 43.1529V39.0431L99.4056 35.9608H103.515L106.598 39.0431V43.1529L103.515 46.2353H99.4056L96.3233 43.1529Z"
              fill="black"
            />
            <path
              fill-rule="evenodd"
              clip-rule="evenodd"
              d="M99.0253 35.0425H103.896L107.516 38.6628V43.5333L103.896 47.1535H99.0253L95.4051 43.5333V38.6628L99.0253 35.0425ZM99.786 36.879L97.2415 39.4235V42.7726L99.786 45.317H103.135L105.68 42.7726V39.4235L103.135 36.879H99.786Z"
              fill="black"
            />
            <path
              fill-rule="evenodd"
              clip-rule="evenodd"
              d="M23.4627 24.6851L48.7649 30.0118L67.5904 64.4168L65.9793 65.2983L47.5596 31.6348L24.0578 26.6871L15.0461 35.6987V47.139L24.1406 56.2335H38.1495L47.513 46.8701L48.8115 48.1686L38.9102 58.0699H23.3799L13.2096 47.8997V34.9381L23.4627 24.6851Z"
              fill="black"
            />
            <path
              fill-rule="evenodd"
              clip-rule="evenodd"
              d="M110.104 23.4031L84.8094 28.6409L65.9824 62.4847L67.5872 63.3775L86.0054 30.2687L109.515 25.4004L118.524 34.261V45.4923L109.434 54.4334H95.4157L86.0513 45.2225L84.7635 46.5318L94.6639 56.2698H110.185L120.36 46.2619V33.4914L110.104 23.4031Z"
              fill="black"
            />
            <defs>
              <linearGradient
                id="paint0_linear"
                x1="82.8389"
                y1="128.431"
                x2="111.736"
                y2="129.074"
                gradientUnits="userSpaceOnUse"
              >
                <stop stop-color="#84673B" />
                <stop offset="1" stop-color="#C4A26F" />
              </linearGradient>
              <linearGradient
                id="paint1_linear"
                x1="209.343"
                y1="38.5294"
                x2="2.9292e-07"
                y2="38.5294"
                gradientUnits="userSpaceOnUse"
              >
                <stop offset="0.381386" stop-color="#C4A26F" />
                <stop offset="0.736685" stop-color="#A88859" />
                <stop offset="1" stop-color="#84673B" />
              </linearGradient>
            </defs></svg
        ></NuxtLink>
      </div>
      <div class="contact">
        <div class="mail">
          <a href="mailto:mail@mail.mail">
            <font-awesome-icon :icon="['fas', 'envelope']"
          /></a>
        </div>
        <div class="tel">
          <a href="tel:512859845">
            <font-awesome-icon :icon="['fas', 'mobile-alt']" />
          </a>
        </div>
      </div>
      <ul class="nav__links">
        <li><NuxtLink class="nav__link" to="/">Start</NuxtLink></li>
        <li><NuxtLink class="nav__link" to="/oferta">Oferta</NuxtLink></li>
        <li><NuxtLink class="nav__link" to="/omnie">O mnie</NuxtLink></li>
        <li><NuxtLink class="nav__link" to="/kontakt">Kontakt</NuxtLink></li>
      </ul>
      <div class="burger">
        <div class="burger__line"></div>
        <div class="burger__line"></div>
        <div class="burger__line"></div>
      </div>
    </nav>
  </header>
</template>

<script>
export default {
  name: "Header",
  mounted() {
    const navSlide = () => {
      const burger = document.querySelector(".burger");
      const nav = document.querySelector(".nav__links");
      const links = document.querySelectorAll(".nav__link");

      links.forEach((link, index) => {
        link.addEventListener("click", () => {
          nav.classList.remove("nav-active");
        });
        if (link.style.animation) {
          link.style.animation = "";
        } else {
          link.style.animation = `navLinkFade 1.5s ease forwards ${index / 5}s`;
        }
      });

      burger.addEventListener("click", () => {
        nav.classList.toggle("nav-active");
        burger.classList.toggle("toggle");
      });
    };

    navSlide();
  },
};
</script>

<style lang='scss' scoped>
.borderNone {
  border: none !important;
}
header {
  position: absolute;
  width: 100%;
}
.nuxt-link-exact-active {
  border-bottom: 1px solid var(--gold);
}
$break-small: 900px;
$break-large: 1200px;

.nav {
  display: flex;
  justify-content: space-around;
  align-items: center;
  height: 8vh;

  .logo {
    margin-top: 2vh;
  }
  .contact {
    display: flex;
    align-items: center;
    justify-content: space-between;
    svg {
      margin-right: 20px;
      color: var(--gold);
      font-size: 3vh;
    }
  }

  &__links {
    display: flex;
    width: 30%;
    justify-content: space-evenly;
    list-style: none;

    @media screen and (max-width: $break-small) {
      position: absolute;
      background-color: black;
      right: 0;
      height: 92vh;
      top: 8vh;
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
      opacity: 0;
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
</style>