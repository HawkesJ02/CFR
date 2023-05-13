<template>
  <header>
    <Navbar />
  </header>
  <main class="background">
    <router-view />
  </main>
</template>

<script>
import { computed } from 'vue'
import { AppState } from './AppState'
import Navbar from './components/Navbar.vue'

export default {
  setup() {
    return {
      appState: computed(() => AppState)
    }
  },
  components: { Navbar }
}
</script>
<style lang="scss">
@import "./assets/scss/main.scss";

:root {
  --main-height: calc(100vh - 32px - 64px);
}


footer {
  display: grid;
  place-content: center;
  height: 32px;
}

// .background {
//   background: rgb(12, 66, 26);
//   background: linear-gradient(90deg, rgba(12, 66, 26, 1) 0%, rgba(41, 144, 68, 1) 100%);
// }

.background {
  background-color: #000000;
}
</style>
