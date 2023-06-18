<script setup>
import { supabase } from '../supabase'

var aboutImg = ""

const fetchAboutImg = async () => {
  const { data: aboutImgData } = supabase
    .storage
    .from("images")
    .getPublicUrl("GJPortrait.jpg")

  aboutImg = aboutImgData.publicUrl
}

fetchAboutImg()
</script>

<template>
  <div class="container">
    <div class="heading">
      <h4>Hi everyone! My name is</h4>
      <h1>Genny Johnson</h1>
    </div>
    <div class="about">
      <p class="about-msg">
        I am mother to three beautiful girls and expecting our fourth (a boy!) in September. I've been married to
        my highschool sweetheart for thirteen years in October. I love being able to capture all of the special
        memories that come with living life. Thank you for taking the time to visit my website. I look forward to
        hearing from you!
      </p>
    </div>
    <div class="img-section">
      <img :src="aboutImg" class="about-img">
    </div>
  </div>
</template>

<style scoped>
.heading,
.about-msg {
  text-align: center;
}

h4,
h1 {
  font-size: 3em;
  text-shadow: 2px 2px 3px darkgray;
}

.about {
  width: 90%;
  margin: auto;
}

.about-msg {
  text-align: center;
  outline: solid 1px;
  border-radius: 2px;
  font-size: 2em;
  box-shadow: 0px 0px 5px 5px darkgray;
  animation: pop-out 3s;
}

.img-section {
  display: grid;
  align-items: center;
  width: 100%;
}

.about-img {
  margin: auto;
  object-fit: contain;
  margin-top: 0;
  width: 80%;
  height: 60%;
}

@keyframes fade-in {
  0% {
    opacity: 0;
  }

  100% {
    opacity: 1;
  }
}

@keyframes pop-out {
  0% {
    box-shadow: 0px 0px 0px 0px darkgray;
  }

  100% {
    box-shadow: 0px 0px 5px 5px darkgray;
  }
}

@media(max-width: 594px) {}

@media(max-width: 679px) {}
</style>