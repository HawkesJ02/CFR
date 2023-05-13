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
  <!-- Slideshow container -->
  <div class="slideshow-container">

    <!-- Full-width images with number and caption text -->
    <div class="mySlides fade">
      <div class="numbertext">1 / 3</div>
      <img src="img1.jpg" style="width:100%">
      <div class="text">Caption Text</div>
    </div>

    <div class="mySlides fade">
      <div class="numbertext">2 / 3</div>
      <img src="img2.jpg" style="width:100%">
      <div class="text">Caption Two</div>
    </div>

    <div class="mySlides fade">
      <div class="numbertext">3 / 3</div>
      <img src="img3.jpg" style="width:100%">
      <div class="text">Caption Three</div>
    </div>

    <!-- Next and previous buttons -->
    <a class="prev" onclick="plusSlides(-1)">&#10094;</a>
    <a class="next" onclick="plusSlides(1)">&#10095;</a>
  </div>
  <br>

  <!-- The dots/circles -->
  <div style="text-align:center">
    <span class="dot" onclick="currentSlide(1)"></span>
    <span class="dot" onclick="currentSlide(2)"></span>
    <span class="dot" onclick="currentSlide(3)"></span>
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



* {
  box-sizing: border-box
}

/* Slideshow container */
.slideshow-container {
  max-width: 1000px;
  position: relative;
  margin: auto;
}

/* Hide the images by default */
.mySlides {
  display: none;
}

/* Next & previous buttons */
.prev,
.next {
  cursor: pointer;
  position: absolute;
  top: 50%;
  width: auto;
  margin-top: -22px;
  padding: 16px;
  color: white;
  font-weight: bold;
  font-size: 18px;
  transition: 0.6s ease;
  border-radius: 0 3px 3px 0;
  user-select: none;
}

/* Position the "next button" to the right */
.next {
  right: 0;
  border-radius: 3px 0 0 3px;
}

/* On hover, add a black background color with a little bit see-through */
.prev:hover,
.next:hover {
  background-color: rgba(0, 0, 0, 0.8);
}

/* Caption text */
.text {
  color: #f2f2f2;
  font-size: 15px;
  padding: 8px 12px;
  position: absolute;
  bottom: 8px;
  width: 100%;
  text-align: center;
}

/* Number text (1/3 etc) */
.numbertext {
  color: #f2f2f2;
  font-size: 12px;
  padding: 8px 12px;
  position: absolute;
  top: 0;
}

/* The dots/bullets/indicators */
.dot {
  cursor: pointer;
  height: 15px;
  width: 15px;
  margin: 0 2px;
  background-color: #bbb;
  border-radius: 50%;
  display: inline-block;
  transition: background-color 0.6s ease;
}

.active,
.dot:hover {
  background-color: #717171;
}

/* Fading animation */
.fade {
  animation-name: fade;
  animation-duration: 1.5s;
}

@keyframes fade {
  from {
    opacity: .4
  }

  to {
    opacity: 1
  }
}
</style>
