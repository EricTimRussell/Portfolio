<template>
  <div class="container-fluid">
    <div class="row navbar-height">
      <div class="col-1">
        <img src="../assets/images/EricBnW (3).JPG" class="card-img-top profile-img" alt="profile image">
      </div>
      <div class="col-3">
        <h5 class="">Software Developer</h5>
        <p class="">Full-Stack Web Developer && JavaScript && Vue && C# || Aspiring Dungeon Master += World's Greatest Dad
        </p>
      </div>
      <div class="col-8 d-flex justify-content-center">
        <nav class="d-flex gap-5">
          <a>About</a>
          <a>Skills</a>
          <a>Works</a>
          <a>Contact</a>
        </nav>
      </div>
    </div>
  </div>
</template>

<script>
export default {
  setup() {


    return {}
  }
}
</script>

<style scoped>
.profile-img {
  border-radius: 50%;
  max-height: auto;
  max-width: 8rem;
}

.navbar-height {
  height: 12rem;
  padding: 1.5rem;
}
</style>