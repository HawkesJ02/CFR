<template>
  <div class="container">
    <div class="row">
      <RouterLink :to="{ name: 'About' }" class="btn btn-primary">
        <div class="button">About</div>
      </RouterLink>
      <RouterLink :to="{ name: 'Members' }">
        <div class="button btn btn-primary">Members</div>
      </RouterLink>
      <RouterLink :to="{ name: 'Gallery' }">
        <div class="button btn btn-primary">Gallery</div>
      </RouterLink>
      <RouterLink :to="{ name: 'Account' }" class="btn btn-primary">
        <div class="button">Account</div>
      </RouterLink>
    </div>
  </div>
</template>

<script>
import { RouterLink } from "vue-router";

export default {
  setup() {
    return {}
  }
}
</script>

<style scoped lang="scss">
.home {
  display: grid;
  height: 80vh;
  place-content: center;
  text-align: center;
  user-select: none;

  .home-card {
    width: 50vw;

    >img {
      height: 200px;
      max-width: 200px;
      width: 100%;
      object-fit: contain;
      object-position: center;
    }
  }
}
</style>
