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
      <img src="../../images/GJPortrait.jpg" class="about-img">
    </div>
  </div>
</template>

<style scoped>
.heading,
.about-msg {
  text-align: center;
}

.about {
  width: 65%;
  margin: auto;
}

.about-msg {
  text-align: center;
  outline: solid 1px;
}

.img-section {
  display: grid;
  align-items: center;
}

.about-img {
  height: 300px;
  margin: auto;
  object-fit: contain;
}

@keyframes fade-in {
  0% {
    opacity: 0;
  }

  100% {
    opacity: 1;
  }
}

@media(max-width: 594px) {}

@media(max-width: 679px) {}
</style>