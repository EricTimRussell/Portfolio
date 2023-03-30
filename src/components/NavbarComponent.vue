<template>
  <main class="container-fluid">
    <div id="nav" class="row justify-content-evenly pt-3">
      <div class="col-1 nav-section"></div>
      <div class="col-1 d-flex justify-content-center">
        <span class="nav-line-y"></span>
        <span class="nav-line-x"></span>
        <RouterLink to="/" class="fs-lg nav-button">STATS</RouterLink>
        <span class="nav-line-x"></span>
        <span class="nav-line-y"></span>
      </div>
      <div class="col-1 nav-section mx-1"></div>
      <div class="col-1 d-flex justify-content-center">
        <span class="nav-line-y"></span>
        <span class="nav-line-x"></span>
        <RouterLink to="about" class="fs-lg nav-button">ABOUT</RouterLink>
        <span class="nav-line-x"></span>
        <span class="nav-line-y"></span>
      </div>
      <div class="col-1 nav-section mx-1"></div>
      <div class="col-1 d-flex justify-content-center">
        <span class="nav-line-y"></span>
        <span class="nav-line-x"></span>
        <RouterLink to="skills" class="fs-lg nav-button">SKILLS</RouterLink>
        <span class="nav-line-x"></span>
        <span class="nav-line-y"></span>
      </div>
      <div class="col-1 nav-section"></div>
      <div class="col-1 d-flex justify-content-center ml-1">
        <span class="nav-line-y"></span>
        <span class="nav-line-x"></span>
        <RouterLink to="works" class="fs-lg nav-button">WORKS</RouterLink>
        <span class="nav-line-x"></span>
        <span class="nav-line-y"></span>
      </div>
      <div class="col-1 nav-section ml-1"></div>
      <div class="col-1 d-flex justify-content-center">
        <span class="nav-line-y"></span>
        <span class="nav-line-x"></span>
        <RouterLink to="more" class="fs-lg nav-button">MORE</RouterLink>
        <span class="nav-line-x"></span>
        <span class="nav-line-y"></span>
      </div>
      <div class="col-1 nav-section"></div>
    </div>
  </main>
</template>

<script>
export default {
  setup() {


    return {}
  }
}
</script>

<style scoped>
#nav .active-router-link {
  transform: scale(1.2);
  transform: translateY(-.7rem);
  text-decoration: underline dotted 5px #33ff00;
}


a:hover {
  transform: scale(1.2);
  transform: translateY(-.7rem);
}

a:active {
  transform: scale(1.2);
  transform: translateY(-.7rem);
}

.nav-line-y {
  border: #33ff00 2px solid;
  height: 15px;
  position: relative;
  top: .5rem;
}

.nav-line-x {
  border: #33ff00 2px solid;
  height: 1px;
  width: 15px;
  position: relative;
  top: .5rem;
}

.nav-section {
  padding-top: .9rem;
  border-bottom: #33ff00 solid 5px;
  padding-left: 0%;
  padding-right: 0%;
}

@media (max-width: 1200px) {
  a {
    font-size: 16px;
  }

  .nav-line-y {
    border: #33ff00 2px solid;
    height: 12px;
    position: relative;
    top: .1rem;
  }

  .nav-line-x {
    border: #33ff00 2px solid;
    height: 1px;
    width: 15px;
    position: relative;
    top: .1rem;
  }

  a:hover {
    transform: translateY(-.5rem);
  }

  a:active {
    transform: translateY(-.5rem);
  }

  .nav-section {
    border-bottom: #33ff00 solid 2px;
  }
}

@media (max-width: 768px) {
  a {
    font-size: 16px;
  }

  .nav-line-y {
    border: #33ff00 2px solid;
    height: 12px;
    position: relative;
    top: .2rem;
  }

  .nav-line-x {
    border: #33ff00 2px solid;
    height: 1px;
    width: 15px;
    position: relative;
    top: .2rem;
  }

  a:hover {
    transform: translateY(-.4rem);
  }

  a:active {
    transform: translateY(-.4rem);
  }

  .nav-section {
    border-bottom: #33ff00 solid 2px;
  }

  .ml-1 {
    margin-left: .33rem;
  }
}
</style>