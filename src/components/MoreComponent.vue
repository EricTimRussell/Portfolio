<template>
  <header class="sticky-top">
    <NavbarComponent />
  </header>
  <section class="container-fluid blink">
    <div class="row pt-3">
      <div class="col-12 d-flex flex-column align-items-center">
        <h2 class="text-retro d-flex letter-space">WHAT I AM DOING</h2>
        <span class="divider"></span>
      </div>
    </div>
    <div class="row justify-content-center">
      <div class="col-12 text-retro pt-4">
        <h2 class="mx-2 text-center">Current Projects:</h2>
        <h3 class="text-center fs-lg">GregsList, Riskier Fire, & Get Outside Photography</h3>
      </div>
      <div class="col-12 d-flex justify-content-center">
        <a href="https://github.com/EricTimRussell/gregslist-laravel-vue/tree/main" target="_blank">
          <img class="gregslist my-4" src="../assets//images/WorksBG/GregsListUnderConstruction.png"
            alt="under construction road sign">
        </a>
      </div>
      <div class="col-10 text-retro text-center">
        <p class="fs-md px-4 p-accessible">Gregslist is a craigslist clone I am creating using Vuejs, Laravel, &
          InertiaJs. It will be my first full-stack application using Laravel and PHP.</p>
      </div>
      <div class="col-12 d-flex justify-content-center">
        <a target="_blank" href="https://github.com/EricTimRussell/riskierFire">
          <img class="riskier-2 my-4" src="../assets/images/More/Riskier-logo-bg.png" alt="riskier logo">
        </a>
      </div>
      <div class="col-10 text-retro text-center">
        <p class="fs-md px-4 p-accessible"> Riskier Fire will be a more complete prettier version of my riskier app and
          board game. I have modelled and 3d printed most of my physical pieces. I am currently play testing and refining
          the riskier app and rules.</p>
      </div>
      <div class="col-12">
        <a class="d-flex justify-content-center" target="_blank" href="https://github.com/EricTimRussell/pam-photo">
          <img class="photo-logo my-4" src="../assets/images/More/Get_Outside_Photography.png"
            alt="get outside photography logo">
        </a>
      </div>
      <div class="col-10 text-retro text-center">
        <p class="fs-md px-4 p-accessible">Get Outside Photography is a dynamic photography portfolio page that the owner
          can edit and change
          dynamically. It also will be connected to Shopify which enables the owner to add and
          modify
          their stores products. Get Outside Photography will be seperated into two parts. The first part is the gallery
          website where users can view and read about all the collections of photos. The second part will be the actual
          market website where customers can purchase photography prints on several different kinds of mediums.</p>
      </div>
    </div>
    <div class="row">
      <div class="col-12 text-retro d-flex flex-column align-items-center pt-5">
        <span class="divider"></span>
        <h2 class="mx-2 text-center">Currently Learning or Improving</h2>
      </div>
    </div>
    <div class="row justify-content-center py-4">
      <div class="col-12 eco-logo">
        <h3 class="text-light text-end">The Vue Ecosystem</h3>
      </div>
    </div>
    <div class="row pt-4">
      <div class="col-lg-4 col-md-6 col-sm-12 d-flex flex-column align-items-center py-4">
        <h3 class="text-retro fs-lg">Nuxtjs</h3>
        <img title="Nuxtjs" class="logo" src="../assets/images/Skills/Nuxt3.png" alt="Nuxt logo">
      </div>
      <div class="col-lg-4 col-md-6 col-sm-12 d-flex flex-column align-items-center py-4">
        <h3 class="text-retro fs-lg">PHP</h3>
        <img title="PHP" class="logo" src="../assets/images/More/php.png" alt="PHP logo">
      </div>
      <div class="col-lg-4 col-md-6 col-sm-12 d-flex flex-column align-items-center py-4">
        <h3 class="text-retro fs-lg">Shopify</h3>
        <img title="Shopify" class="logo" src="../assets/images/More/shopifyLogo.png" alt="Shopify logo">
      </div>
      <div class="col-lg-4 col-md-6 col-sm-12 d-flex flex-column align-items-center py-4">
        <h3 class="text-retro fs-lg">Laravel</h3>
        <img title="Laravel" class="logo" src="../assets/images/More/Laravel.png" alt="Laravel logo">
      </div>
    </div>
  </section>
</template>

<script>
import NavbarComponent from "./NavbarComponent.vue";

export default {
  setup() {
    return {
    };
  },
  components: { NavbarComponent }
}
</script>

<style scoped>
.blink {
  animation: blinker .1s step-start 2;
}

@keyframes blinker {
  50% {
    opacity: 0;
  }
}

.photo-logo {
  border: solid #33ff00 2px;
  width: 11.5rem;
  height: auto;
}

.photo-logo:hover {
  transform: translateY(-15px);
  box-shadow:#33ff00 0px 5px 5px 2px;
}

.gregslist{
  height: 22vh;
  width: 22vh;
  border-radius: 5px;
  border: solid #33ff00 2px;
}

.gregslist:hover{
  transform: translateY(-15px);
  box-shadow:#33ff00 0px 5px 5px 2px;
}

.riskier-2 {
  border: solid #33ff00 2px;
  height: 22vh;
  width: 44vh;
}

.riskier-2:hover {
  transform: translateY(-15px);
  box-shadow:#33ff00 0px 5px 5px 2px;
}

.logo {
  border: solid #33ff00 2px;
  background: linear-gradient(#33ff003e, #33ff003e);
  width: 30rem;
  height: 38rem;
  padding: 2rem;
}

.eco-logo {
  border: solid #33ff00 2px;
  background: linear-gradient(#33ff003e, #33ff003e);
  background-image: url(../assets/images/More/VueEcosystem.png);
  width: 75rem;
  height: 30rem;
  padding: 2rem;
}

.logo:hover {
  background: linear-gradient(#33ff0097, #33ff0097);
}

@media (max-width: 1600px) {
  .logo {
    width: 20rem;
    height: 30rem;
  }

  .eco-logo {
    width: 20rem;
    height: 30rem;
  }
}

@media (max-width: 1150px) {
  .logo {
    width: 18rem;
    height: 28rem;
  }
}

@media (max-width: 360px) {
  .logo {
    width: 15rem;
    height: 20rem;
  }

}


@media (max-width: 1200px) {
  .p-accessible {
    text-align: left;
  }
}
</style>