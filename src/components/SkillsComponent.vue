<template>
  <header class="sticky-top">
    <NavbarComponent />
  </header>
  <section class="container-fluid">
    <div class="row pt-3">
      <div class="col-12 d-flex flex-column align-items-center">
        <h2 class="text-retro fs-lg d-flex letter-space">PROFICIENCES</h2>
        <span class="divider"></span>
      </div>
    </div>
    <div class="row pb-5 anim-slide">
      <div class="col-xl-3 col-lg-4 col-md-6 col-sm-12 d-flex flex-column align-items-center py-3">
        <h3 class="text-retro fs-lg">Javascript</h3>
        <img title="Javascript" class="logo" src="../assets/images/Skills/javascript.png" alt="javascript logo">
      </div>
      <div class="col-xl-3 col-lg-4 col-md-6 col-sm-12 d-flex flex-column align-items-center py-3">
        <h3 class="text-retro fs-lg">BootStrap 5</h3>
        <img title="Bootstrap" class="logo" src="../assets/images/Skills/bootstrap.png" alt="BootStrap logo">
      </div>
      <div class="col-xl-3 col-lg-4 col-md-6 col-sm-12 d-flex flex-column align-items-center py-3">
        <h3 class="text-retro fs-lg">Vuejs</h3>
        <img title="VueJs" class="logo" src="../assets/images/Skills/vue.png" alt="vue javascript logo">
      </div>
      <div class="col-xl-3 col-lg-4 col-md-6 col-sm-12 d-flex flex-column align-items-center py-3">
        <h3 class="text-retro fs-lg">Nuxtjs</h3>
        <img title="Nuxtjs" class="logo" src="../assets/images/Skills/Nuxt3.png" alt="Nuxt logo">
      </div>
    </div>
    <div class="row anim-slide pb-5">
      <div class="col-xl-3 col-lg-4 col-md-6 col-sm-12 d-flex flex-column align-items-center py-3">
        <h3 class="text-retro fs-lg">C Sharp</h3>
        <img title="CSharp" class="logo" src="../assets/images/Skills/c-sharp.png" alt="C sharp logo">
      </div>
      <div class="col-xl-3 col-lg-4 col-md-6 col-sm-12 d-flex flex-column align-items-center py-3">
        <h3 class="text-retro fs-lg">DotNet</h3>
        <img title="DotNet" class="logo" src="../assets/images/Skills/dotnet.png" alt="dot net logo">
      </div>
      <div class="col-xl-3 col-lg-4 col-md-6 col-sm-12 d-flex flex-column align-items-center py-3">
        <h3 class="text-retro fs-lg">MySQL</h3>
        <img title="MySQL" class="logo" src="../assets/images/Skills/mysql.png" alt="my SQL logo">
      </div>
      <div class="col-xl-3 col-lg-4 col-md-6 col-sm-12 d-flex flex-column align-items-center py-3">
        <h3 class="text-retro fs-lg">Google Firebase</h3>
        <img title="Google Firebase" class="logo" src="../assets/images/Skills/firebase_logo.png" alt="firebase logo">
      </div>
    </div>
  </section>
</template>

<script>
import NavbarComponent from "./NavbarComponent.vue";

export default {
  setup() {
    return {};
  },
  components: { NavbarComponent }
}
</script>

<style scoped>
.logo {
  box-shadow: #33ff00 5px 5px 5px 0px, #33ff00 0px 0px 5px 5px;
  background: linear-gradient(#33ff003e, #33ff003e);
  width: 20rem;
  height: 22rem;
  padding: 2rem;
}

.logo:hover {
  background: linear-gradient(#33ff0097, #33ff0097);
}

.anim-slide {
  animation-name: skills-slide;
  animation-duration: 3s;
  animation-delay: .5s;
  animation-fill-mode: both;
  -moz-animation-name: skills-slide;
  -moz-animation-duration: 3s;
  -moz-animation-delay: .5s;
  -moz-animation-fill-mode: both;
  -webkit-animation-name: skills-slide;
  -webkit-animation-duration: 3s;
  -webkit-animation-delay: .5s;
  -webkit-animation-fill-mode: both;
  white-space: nowrap;
  overflow: hidden;
}

@keyframes skills-slide {
  from {
    width: 0;
  }

  to {
    width: 100%;
  }
}

@media (max-width: 1375px) {
  .logo {
    width: 18rem;
    height: 18rem;
    padding: 2rem;
  }
}

@media (max-width: 768px) {
  .logo {
    width: 16rem;
    height: 16rem;
    padding: 2rem;
  }
}
</style>