<template class="">
  <div class="container-fluid section1">
    <div class="row justify-content-around align-items-center">
      <div class="col-12 col-md-6 text-end">
        <img src="https://cdn.discordapp.com/attachments/1097757077029539850/1102856277501165578/CFR_Simple_Logo.png"
          alt="CFR Logo" class="CFRLogoMain">
      </div>
      <div class="col-6 delete-small">
        <h1 class="larger-font">Colonial First Responders</h1>
        <h3><i>In Blood We Trust.</i></h3>
      </div>
    </div>
  </div>




  <!-- <div class="container-fluid mt-5">
    <div class="row">
      <div class="col-12 text-center">
        <img src="https://cdn.discordapp.com/attachments/1097757077029539850/1102856277501165578/CFR_Simple_Logo.png"
          alt="CFR logo" class="CFRLogoMain">
      </div>
    </div>
    <div class="row text-center justify-content-center">
      <div class="col-2">
        <RouterLink :to="{ name: 'About' }" class="">
          <div class="button btn btn-primary">About</div>
        </RouterLink>
      </div>
    </div>
    <div class="row">
      <div class="col-2">
        <RouterLink :to="{ name: 'Members' }">
          <div class="button btn btn-primary">Members</div>
        </RouterLink>
      </div>

      <div>WUH</div>
      <div class="col-2">
        <RouterLink :to="{ name: 'Gallery' }">
          <div class="button btn btn-primary">Gallery</div>
        </RouterLink>
      </div>
    </div>
    <div class="row">
      <div class="col-2 text-center">
        <RouterLink :to="{ name: 'Account' }" class="btn btn-primary">
          <div class="button">Account</div>
        </RouterLink>
      </div>
    </div>
  </div> -->
</template>
<!-- TODO re-write the homepage to merge about into it  -->

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

@media screen and (max-width: 600px) {
  .delete-small {
    display: none;
  }
}

.CFRLogoMain {
  max-height: 50vh;
  max-width: 50vw;
}

.larger-font {
  font-size: 5em;
}

.section1 {
  background: url(https://media.discordapp.net/attachments/740165104686858252/1066491136891437056/IndustryOfWarPromo_NoLogo.jpg?width=1156&height=650);
  background-repeat: no-repeat;
  background-size: cover;
  background-attachment: fixed;
}
</style>
