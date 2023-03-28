<template>
  <section class="container-fluid">
    <div class="row justify-content-center mt-5 text-retro">
      <div class="col-12 d-flex flex-column align-items-center">
        <h2 class="text-retro fs-xl d-flex letter-space">My Skills</h2>
        <span class="divider"></span>
      </div>
      <div class="col-lg-3 col-md-6 col-sm-12 skills-img p-5">
        <img title="Javascript" class="img-fluid" src="../assets/images/Skills/javascript.png" alt="javascript logo">
      </div>
      <div class="col-lg-3 col-md-6 col-sm-12 skills-img p-5">
        <img title="Bootstrap" class="img-fluid" src="../assets/images/Skills/bootstrap.png" alt="BootStrap logo">
      </div>
      <div class="col-lg-3 col-md-6 col-sm-12 skills-img p-5">
        <img title="VueJs" class="img-fluid" src="../assets/images/Skills/vue.png" alt="vue javascript logo">
      </div>
      <div class="col-lg-3 col-md-6 col-sm-12 skills-img p-5">
        <img title="Nuxtjs" class="nuxt" src="../assets/images/Skills/Nuxt3.png" alt="Nuxt logo">
      </div>
      <div class="col-lg-3 col-md-6 col-sm-12 skills-img p-5">
        <img title="CSharp" class="img-fluid" src="../assets/images/Skills/c-sharp.png" alt="C sharp logo">
      </div>
      <div
        class="col-lg-3 col-md-6 col-sm-12 skills-img text-center text-primary d-flex flex-column justify-content-center p-5">
        <img title="DotNet" class="img-fluid" src="../assets/images/Skills/dotnet.png" alt="dot net logo">
        <h3>DotNet</h3>
      </div>
      <div class="col-lg-3 col-md-6 col-sm-12 skills-img p-5">
        <img title="MySQL" class="img-fluid" src="../assets/images/Skills/mysql.png" alt="my SQL logo">
      </div>
      <div class="col-lg-3 col-md-6 col-sm-12 skills-img p-5">
        <img title="Google Firebase" class="img-fluid" src="../assets/images/Skills/firebase_logo.png"
          alt="firebase logo">
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
.skills-img {
  width: 20rem;
  max-height: 25rem;
  margin-bottom: 2rem;
}

.nuxt {
  height: 13rem;
  width: 15rem;
}
</style>