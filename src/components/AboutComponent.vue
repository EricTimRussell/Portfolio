<template>
  <section id="about" class="container-fluid">
    <div class="row mobile justify-content-center">
      <div class="col-12 d-flex flex-column align-items-center">
        <h2 class="text-retro fs-xl d-flex letter-space about-title anim-typewriter">ABOUT ME</h2>
        <span class="divider"></span>
      </div>
      <div class="col-md-4 col-sm-12 d-flex flex-column align-items-center pt-5 fade-in">
        <img class="px-5 code-works-logo mobile"
          src="https://codeworks.blob.core.windows.net/public/assets/img/cw-logo-circle.png" alt="Boise CodeWorks Logo">
        <span class="text-retro fs-lg">Class of Fall 2022 <span class="material-symbols-outlined text-retro fs-lg">
            school
          </span></span>
      </div>
      <div class="col-md-6 col-sm-12 text-retro fs-md my-3 letter-space fade-in">
        <p class="paragraph text-shadow pt-4"> &nbsp&nbsp My career life began when I graduated from Boise State
          University
          with a BS in
          criminal
          justice. Shortly
          after graduating I learned that the world of law enforcement was not for me. I found myself working in the
          logistics industry for 5 years, but it was not a fulfilling career path. I discoverd software development
          from
          a simple Udemy course on javascript and after that I knew it was what I wanted to pursue. After a grueling
          13-week software development bootcamp with CodeWorks Boise, I have gained the confidence and skills needed
          to pursue my developer goals.</p>
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
.about-title {
  white-space: nowrap;
  overflow: hidden;
}

/* Animation */
.anim-typewriter {
  animation: typewriter 1.5s 1 normal both,
    blinkTextCursor 500ms infinite normal;
}

@keyframes typewriter {
  from {
    width: 0;
  }

  to {
    width: 12.5rem;
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

.code-works-logo {
  box-shadow: #33ff00 5px 5px 5px 0px, #33ff00 0px 0px 5px 5px;
  background: linear-gradient(#33ff003e, #33ff003e);
}

.mobile {
  margin-bottom: 2rem;
}

@media (max-width: 768px) {
  .code-works-logo {
    max-width: 17rem;
    margin-bottom: .25rem;
  }

  .paragraph {
    font-size: 18px;
  }

  .mobile {
    margin-bottom: .25rem;
  }
}
</style>