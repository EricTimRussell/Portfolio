<template>
  <section class="container-fluid">
    <div class="row pt-5">
      <div class="col-12 d-flex flex-column align-items-center">
        <h2 class="text-retro fs-xl d-flex letter-space more-title anim-typewriter">WHAT AM I UP TO?</h2>
        <span class="divider"></span>
      </div>
      <div class="col-12 text-center" v-if="isLoading">
        <span class="text-retro fs-xl">Loading<i class="spinner-grow text-retro" role="status"></i><i
            class="spinner-grow text-retro" role="status"></i><i class="spinner-grow text-retro" role="status"></i></span>
      </div>
    </div>
    <div class="row justify-content-center" v-if="!isLoading">
      <div class="col-12 text-retro pt-4">
        <h2 class="mx-2 text-center">Current Project</h2>
        <a class=" d-flex justify-content-center" target="_blank" href="https://github.com/EricTimRussell/riskierFire">
          <img class="riskier-2 my-4" src="../assets/images/More/addressBarImage.jpg" alt="riskier version 2">
        </a>
        <h3 class="text-center fs-lg">Riskier Fire</h3>
      </div>
      <div class="col-12 text-retro text-center">
        <p class="fs-md mx-1 p-accessible"> Riskier Fire will be a more complete prettier version of my riskier app and
          board
          game.
          It will also utilize Google Firebase for my backend and database.</p>
      </div>
    </div>
    <div class="row" v-if="!isLoading">
      <div class="row pt-5">
        <div class="col-12 text-retro d-flex flex-column align-items-center pt-5">
          <span class="divider"></span>
          <h2 class="mx-2 text-center">Currently Learning or Improving</h2>
        </div>
        <div class="col-lg-4 col-md-6 col-sm-12 d-flex flex-column align-items-center py-5">
          <h3 class="text-retro fs-lg">Nuxtjs</h3>
          <img title="Nuxtjs" class="logo" src="../assets/images/Skills/Nuxt3.png" alt="Nuxt logo">
        </div>
        <div class="col-lg-4 col-md-6 col-sm-12 d-flex flex-column align-items-center py-5">
          <h3 class="text-retro text-center">Pinia State Management</h3>
          <img title="Pinia" class="logo" src="../assets/images/More/piniaJPG.png" alt="Pinia logo">
        </div>
        <div class="col-lg-4 col-md-6 col-sm-12 d-flex flex-column align-items-center py-5">
          <h3 class="text-retro fs-lg">TypeScript</h3>
          <img title="Typescript" class="logo" src="../assets/images/More/typescript.png" alt="Typescript logo">
        </div>
        <div class="col-lg-4 col-md-6 col-sm-12 d-flex flex-column align-items-center py-5">
          <h3 class="text-retro fs-lg">Vitest Unit Testing</h3>
          <img title="Vitest" class="logo" src="../assets/images/More/vitest.png" alt="Vitest logo">
        </div>
      </div>
    </div>
  </section>
</template>

<script>
import { ref, onMounted } from "vue";

export default {
  setup() {
    const isLoading = ref(false)
    function pageLoading() {
      isLoading.value = true
      setTimeout(() => {
        isLoading.value = false
      }, 2500)
    }

    onMounted(() => {
      pageLoading()
    })
    return {
      isLoading
    }
  }
}
</script>

<style scoped>
.more-title {
  white-space: nowrap;
  overflow: hidden;
}

/* Animation */
.anim-typewriter {
  animation: typewriter 2.5s 1 normal both,
    blinkTextCursor 500ms infinite normal;
}

@keyframes typewriter {
  from {
    width: 0;
  }

  to {
    width: 22rem;
  }
}

@keyframes blinkTextCursor {
  from {
    border-right: #33ff00 10px solid;
  }

  to {
    border-right: transparent;
  }
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
    height: 25rem;
  }
}


@media (max-width: 1200px) {
  .p-accessible {
    text-align: left;
  }
}
</style>