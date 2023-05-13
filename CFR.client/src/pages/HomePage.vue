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
    <div id="slideshow">
      <div class="slide-wrapper">

        <!-- Define each of the slides
         and write the content -->

        <div class="slide">
          <img
            src="https://media.discordapp.net/attachments/1097757077029539850/1106970069151535235/MedicSwarm.png?width=911&height=512"
            class="slideimg" alt="">
        </div>
        <div class="slide">
          <img
            src="https://media.discordapp.net/attachments/1059340116168015882/1094828091265781820/image.png?width=706&height=513"
            class="slideimg" alt="">
        </div>
        <div class="slide">
          <img src="https://cdn.discordapp.com/attachments/1059340116168015882/1105446026309029948/20230508182042_1.jpg"
            class="slideimg" alt="">
        </div>
        <div class="slide">
        </div>
      </div>
    </div>
  </div>
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

body {
  font-family: Helvetica, sans-serif;
  padding: 5%;
  text-align: center;
  font-size: 50;
}

/* Styling the area of the slides */
#slideshow {
  overflow: hidden;
  height: 1080px;
  width: 1080px;
  margin: 0 auto;
}

/* Style each of the sides
with a fixed width and height */
.slide {
  float: left;
  height: 1080px;
  width: 1080px;
}

.slideimg {
  max-height: 1080px;
}

/* Add animation to the slides */
.slide-wrapper {

  /* Calculate the total width on the
basis of number of slides */
  width: calc(1080px * 4);

  /* Specify the animation with the
duration and speed */
  animation: slide 15s ease infinite;
}

/* Define the animation
for the slideshow */
@keyframes slide {

  /* Calculate the margin-left for
each of the slides */
  20% {
    margin-left: 0px;
  }

  40% {
    margin-left: calc(-1080px * 1);
  }

  60% {
    margin-left: calc(-1080px * 2);
  }

  80% {
    margin-left: calc(-1080px * 3);
  }
}
</style>
