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
        <h2 class="mx-2 text-center">Current Project:</h2>
        <h3 class="text-center fs-lg text-decoration-underline">Riskier Fire</h3>
      </div>
      <div class="col-12 d-flex justify-content-center pt-3">
        <a target="_blank" href="https://github.com/EricTimRussell/riskierFire">
          <img class="riskier-2 my-3" src="../assets/images/More/Riskier-logo-bg.png" alt="riskier logo">
        </a>
      </div>
      <div class="col-10 text-retro text-center">
        <span class="fs-lg">Riskier</span>
        <p class="fs-md px-4 p-accessible"> Riskier Fire will be a more complete prettier version of my riskier app and
          board game. I have modelled and 3d printed most of my physical pieces. I am currently play testing and refining
          the riskier app and rules.</p>
      </div>
    </div>
    <div class="row">
      <div class="col-12 text-retro d-flex flex-column align-items-center pt-5">
        <span class="divider"></span>
        <h2 class="mx-2 text-center">Technologies I am currently learning or improving</h2>
      </div>
    </div>
    <div class="row justify-content-center py-4">
      <div class="col-12 eco-logo">
        <h3 class="text-light text-end">The Vue Ecosystem</h3>
      </div>
    </div>
    <div class="row pt-4 justify-content-center">
      <div class="col-lg-4 col-md-6 col-sm-12 d-flex flex-column align-items-center py-4">
        <h3 class="text-retro fs-lg">Python</h3>
        <img title="Python" class="logo" src="../assets/images/Skills/PythonLogo.png" alt="Python logo">
      </div>
      <div class="col-lg-4 col-md-6 col-sm-12 d-flex flex-column align-items-center py-4">
        <h3 class="text-retro fs-lg">Firebase</h3>
        <img title="Firebase" class="logo" src="../assets/images/Skills/firebase_logo.png" alt="Firebase logo">
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