<script setup>
import { RouterView } from 'vue-router'
import ContactMeModalComponent from "./components/ContactMeModalComponent.vue";
import NavbarComponent from "./components/NavbarComponent.vue";
</script>

<template>
  <body>
    <header class="sticky-top">
      <NavbarComponent />
    </header>
    <main>
      <RouterView />
      <footer class="sticky-bottom">
        <button class="contact-button p-3" data-bs-toggle="modal" data-bs-target="#contactModal"><span
            class="material-symbols-outlined text-retro fs-xl">
            smartphone
          </span></button>
      </footer>
    </main>
  </body>

  <!-- Contact Modal -->
  <div class="modal fade" id="contactModal" tabindex="-1" aria-labelledby="contactModalLabel" aria-hidden="true">
    <div class="modal-dialog modal-dialog-centered">
      <div class="modal-content modal-bg">
        <div class="modal-header">
          <h1 class="modal-title fs-lg text-retro" id="contactModalLabel">Contact Me</h1>
          <button type="button" class="btn-close" data-bs-dismiss="modal" aria-label="Close"></button>
        </div>
        <div class="modal-body modal-bg">
          <ContactMeModalComponent />
        </div>
      </div>
    </div>
  </div>
</template>

<style scoped>
.contact-button {
  background: #00800000;
  border: none;
}

.contact-button:hover {
  transform: scale(1.2);
}

.modal-bg {
  background-color: #202020;
}
</style>
