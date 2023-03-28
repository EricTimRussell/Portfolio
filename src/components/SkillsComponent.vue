<template>
  <section id="skills" class="container-fluid">
    <div class="row">
      <div class="col-12 d-flex flex-column align-items-center">
        <h2 class="text-retro fs-xl d-flex letter-space skills-title anim-typewriter">PROFICIENT SKILLS</h2>
        <span class="divider"></span>
      </div>
      <div class="col-lg-3 col-md-6 col-sm-12 d-flex flex-column align-items-center p-3">
        <h3 class="text-retro fs-lg">Javascript</h3>
        <img title="Javascript" class="logo" src="../assets/images/Skills/javascript.png" alt="javascript logo">
      </div>
      <div class="col-lg-3 col-md-6 col-sm-12 d-flex flex-column align-items-center p-3">
        <h3 class="text-retro fs-lg">BootStrap 5</h3>
        <img title="Bootstrap" class="logo" src="../assets/images/Skills/bootstrap.png" alt="BootStrap logo">
      </div>
      <div class="col-lg-3 col-md-6 col-sm-12 d-flex flex-column align-items-center  p-3">
        <h3 class="text-retro fs-lg">Vuejs</h3>
        <img title="VueJs" class="logo" src="../assets/images/Skills/vue.png" alt="vue javascript logo">
      </div>
      <div class="col-lg-3 col-md-6 col-sm-12 d-flex flex-column align-items-center p-3">
        <h3 class="text-retro fs-lg">Nuxtjs</h3>
        <img title="Nuxtjs" class="logo" src="../assets/images/Skills/Nuxt3.png" alt="Nuxt logo">
      </div>
      <div class="col-lg-3 col-md-6 col-sm-12 d-flex flex-column align-items-center p-3">
        <h3 class="text-retro fs-lg">C Sharp</h3>
        <img title="CSharp" class="logo" src="../assets/images/Skills/c-sharp.png" alt="C sharp logo">
      </div>
      <div class="col-lg-3 col-md-6 col-sm-12 d-flex flex-column align-items-center p-3">
        <h3 class="text-retro fs-lg">DotNet</h3>
        <img title="DotNet" class="logo" src="../assets/images/Skills/dotnet.png" alt="dot net logo">
      </div>
      <div class="col-lg-3 col-md-6 col-sm-12 d-flex flex-column align-items-center p-3">
        <h3 class="text-retro fs-lg">MySQL</h3>
        <img title="MySQL" class="logo" src="../assets/images/Skills/mysql.png" alt="my SQL logo">
      </div>
      <div class="col-lg-3 col-md-6 col-sm-12 d-flex flex-column align-items-center p-3">
        <h3 class="text-retro fs-lg">Google Firebase</h3>
        <img title="Google Firebase" class="logo" src="../assets/images/Skills/firebase_logo.png" alt="firebase logo">
      </div>
    </div>
  </section>
</template>

<script>
export default {
  setup() {


    return {}
  }
}
</script>

<style scoped>
.skills-title {
  white-space: nowrap;
  overflow: hidden;
}

/* Animation */
.anim-typewriter {
  animation: typewriter .7s 1s 1 normal both,
    blinkTextCursor 500ms 6 normal;
}

@keyframes typewriter {
  from {
    width: 0;
  }

  to {
    width: 22.7rem;
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

.hidden {
  display: none;
}

.hidden:hover {
  display: block;
}

@media (max-width: 768px) {
  .logo {
    width: 16rem;
    height: 16rem;
    padding: 2rem;
  }
}
</style>