<template>
  <header class="sticky-top">
    <NavbarComponent />
  </header>
  <section class="container-fluid">
    <div class="row pt-3">
      <div class="col-12 d-flex flex-column align-items-center">
        <h2 class="text-retro fs-md d-flex letter-space">WHAT I AM DOING</h2>
        <span class="divider"></span>
      </div>
    </div>
    <div class="row justify-content-center">
      <div class="col-12 text-retro pt-4">
        <h2 class="mx-2 text-center">Current Projects:</h2>
        <h3 class="text-center fs-lg">Riskier Fire & Get Outside Photography</h3>
      </div>
      <div class="col-2">
        <a class="d-flex justify-content-center" target="_blank" href="https://github.com/EricTimRussell/riskierFire">
          <img class="riskier-2 my-4" src="../assets/images/More/addressBarImage.jpg" alt="riskier logo">
        </a>
      </div>
      <div class="col-2">
        <a class="d-flex justify-content-center" target="_blank" href="https://github.com/EricTimRussell/pam-photo">
          <img class="photo-logo my-4" src="../assets/images/More/Get Outside Photography-1.png"
            alt="get outside photography logo">
        </a>
      </div>
      <div class="col-12 text-retro text-center">
        <p class="fs-md mx-1 p-accessible"> Riskier Fire will be a more complete prettier version of my riskier app and
          board
          game. Get Outside Photography is a dynamic photography portfolio page that the owner can edit and change
          dynamically.</p>
      </div>
    </div>
    <div class="row">
      <div class="row pt-5">
        <div class="col-12 text-retro d-flex flex-column align-items-center pt-5">
          <span class="divider"></span>
          <h2 class="mx-2 text-center">Currently Learning or Improving</h2>
        </div>
        <div class="col-lg-4 col-md-6 col-sm-12 d-flex flex-column align-items-center py-4">
          <h3 class="text-retro fs-lg">Nuxtjs</h3>
          <img title="Nuxtjs" class="logo" src="../assets/images/Skills/Nuxt3.png" alt="Nuxt logo">
        </div>
        <div class="col-lg-4 col-md-6 col-sm-12 d-flex flex-column align-items-center py-4">
          <h3 class="text-retro text-center">Pinia State Management</h3>
          <img title="Pinia" class="logo" src="../assets/images/More/piniaJPG.png" alt="Pinia logo">
        </div>
        <div class="col-lg-4 col-md-6 col-sm-12 d-flex flex-column align-items-center py-4">
          <h3 class="text-retro fs-lg">TypeScript</h3>
          <img title="Typescript" class="logo" src="../assets/images/More/typescript.png" alt="Typescript logo">
        </div>
        <div class="col-lg-4 col-md-6 col-sm-12 d-flex flex-column align-items-center py-4">
          <h3 class="text-retro fs-lg">Vitest Unit Testing</h3>
          <img title="Vitest" class="logo" src="../assets/images/More/vitest.png" alt="Vitest logo">
        </div>
      </div>
    </div>
  </section>
</template>

<script>
import { ref, onMounted } from "vue";
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
.photo-logo {
  box-shadow: #33ff00 5px 5px 5px 0px, #33ff00 0px 0px 5px 5px;
  width: 11.5rem;
  height: auto;
}

.photo-logo:hover {
  transform: scale(1.1);

}

.riskier-2 {
  box-shadow: #33ff00 5px 5px 5px 0px, #33ff00 0px 0px 5px 5px;
}

.riskier-2:hover {
  transform: scale(1.1);
}

.logo {
  box-shadow: #33ff00 5px 5px 5px 0px, #33ff00 0px 0px 5px 5px;
  background: linear-gradient(#33ff003e, #33ff003e);
  width: 30rem;
  height: 38rem;
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