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
      <footer class="sticky-bottom text-end">
        <button class="contact-button m-4" title="Contact" data-bs-toggle="modal" data-bs-target="#contactModal"><span
            class="material-symbols-outlined text-retro fs-lg">
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
          <button type="button" title="Close" class="modal-close text-retro" data-bs-dismiss="modal"
            aria-label="Close">X</button>
        </div>
        <div class="modal-body modal-bg">
          <ContactMeModalComponent />
        </div>
      </div>
    </div>
  </div>
</template>

<style scoped>
footer {
  max-height: 12.5vh;
}

.contact-button {
  padding: .5rem;
  background: #00800000;
  border: none;
  background-color: #33ff005b;
  border-radius: 50%;
}

.contact-button:hover {
  transform: scale(1.2);
}

.modal-bg {
  background-color: #202020;
}

.modal-close {
  background-color: #2d2d2d;
}

@media (max-width: 768px) {}
</style>
