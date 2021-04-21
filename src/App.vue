<template>
  <header>
    <Navbar />
  </header>
  <!-- NOTE router-view allows the router to determine the component that should be injected -->
  <main>
    <router-view />
    <CreateHouseModal />
  </main>
  <footer>
    <div class="bg-dark text-light text-center p-4">
      Made with 💖 by CodeWorks
    </div>
  </footer>
</template>

<script>
import CreateHouseModal from './components/CreateHouseModal.vue'
import Navbar from './components/Navbar'

export default {
  components: {
    Navbar,
    CreateHouseModal
  }
}
</script>

<style lang="scss">
@import "./assets/scss/main.scss";

</style>
