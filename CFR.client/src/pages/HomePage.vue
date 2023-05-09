<template class="">
  <div class="container-fluid mt-5">
    <div class="row text-center justify-content-center">
      <div class="col-2">
        <RouterLink :to="{ name: 'About' }" class="">
          <div class="button btn btn-primary">About</div>
        </RouterLink>
      </div>
    </div>
    <div class="row justify-content-center align-items-center text-center">
      <div class="col-2">
        <RouterLink :to="{ name: 'Members' }">
          <div class="button btn btn-primary">Members</div>
        </RouterLink>
      </div>
      <div class="col-6 justify-content-center d-flex">
        <img src="https://cdn.discordapp.com/attachments/1097757077029539850/1102856277501165578/CFR_Simple_Logo.png"
          alt="CFR logo" class="CFRLogoMain">
      </div>
      <div>WUH</div>
      <div class="col-2">
        <RouterLink :to="{ name: 'Gallery' }">
          <div class="button btn btn-primary">Gallery</div>
        </RouterLink>
      </div>
    </div>
    <div class="row justify-content-center">
      <div class="col-2 text-center">
        <RouterLink :to="{ name: 'Account' }" class="btn btn-primary">
          <div class="button">Account</div>
        </RouterLink>
      </div>
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

.CFRLogoMain {
  max-height: 50vh;
  max-width: 50vw;
}
</style>
