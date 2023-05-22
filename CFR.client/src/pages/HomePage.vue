<template class="">
  <div class="container-fluid">
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

  <div class="container-fluid my-3 bg-black p-3">
    <div class="row justify-content-center">
      <div class="col-7">
        <div id="slideshow">
          <div class="slide-wrapper">
            <div class="slide">
              <img src="https://cdn.discordapp.com/attachments/1059340116168015882/1060997031813992588/MarbanSquad3.png"
                class="slideimg img-fluid" alt="">
            </div>
            <div class="slide">
              <img
                src="https://cdn.discordapp.com/attachments/1059340116168015882/1062152859153612871/20230110003158_1.jpg"
                class="slideimg img-fluid" alt="">
            </div>
            <div class="slide">
              <img
                src="https://cdn.discordapp.com/attachments/1059340116168015882/1105446026309029948/20230508182042_1.jpg"
                class="slideimg img-fluid" alt="">
            </div>
            <div class="slide">
              <img
                src="https://cdn.discordapp.com/attachments/1059340116168015882/1063516980163907686/20230113185601_1.jpg"
                alt="" class="slideimg img-fluid">
            </div>
          </div>
        </div>
      </div>
      <div class="col-md-5 col-12">

        <h1 class="bg-light rounded m-3 p-3 text-center"><i><b>What is CFR?</b></i></h1>
        <p class="bg-light rounded p-3 fs-5"><i>Founded on the 1st of January 2023 as a natural successor to the Colonial
            Medical
            Battalion, our regiment
            retains its focus on medical and support roles, while attempting to build a friendly and engaging community
            with
            the help of its experienced members and commanders. We consider ourselves to be a casual regiment: no playtime
            quotas, no strict command structure, no enforced medical duties. While all members are expected to attend
            medical duties to an extent, we mix it up with infantry, building, tanks and artillery from time to time,
            although these do not occur on a regular basis.</i><br>- Amp </p>
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
      height: 10vh;
      max-width: 50vw;
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

.bg-lightgrey {
  background-color: #999999;
}



/* Styling the area of the slides */
#slideshow {
  overflow: hidden;
  height: 50vh;
  width: 50vw;
  margin: 0 auto;
}

/* Style each of the sides
with a fixed width and height */
.slide {
  float: left;
  height: 50vw;
  width: 50vw;
}

.slideimg {
  min-height: 10vh;
}

/* Add animation to the slides */
.slide-wrapper {

  /* Calculate the total width on the
basis of number of slides */
  width: calc(50vw * 4);

  /* Specify the animation with the
duration and speed */
  animation: slide 45s ease infinite;
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
    margin-left: calc(-50vw * 1);
  }

  60% {
    margin-left: calc(-50vw * 2);
  }

  80% {
    margin-left: calc(-50vw * 3);
  }
}
</style>
