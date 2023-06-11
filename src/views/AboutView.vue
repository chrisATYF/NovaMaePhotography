<template>
  <section class="about-section">
    <h2>About Me</h2>
    <img src="../../images/AboutMe.png" class="aboutme-img">
    <!-- <div class="about">
      <p>
        Hi! My name is Genny Johnson. I'm a mother to three beautiful girls and am expecting our first boy in
        September. I've been married to my high school sweetheart for thirteen years this October. I love being
        able to capture all the special memories that come with living life. Thank you for taking the time to
        visit my website. I look forward to hearing from you!
      </p>
      <img src="../../images/GJPortrait.jpg" class="about-img">
    </div> -->
  </section>
</template>

<style scoped>
.about-section {
  text-align: center;
  padding: 0px 40px;
}

.aboutme-img {
  width: 100%;
  height: 100%;
  animation: fade-in 2.5s;
}

.about {
  display: flex;
  align-items: center;
  justify-content: space-between;
  animation: fade-in 2.5s;
}

.about-img {
  height: 250px;
  width: 250px;
  object-fit: contain;
  border-radius: 50%;
}

@keyframes fade-in {
  0% {
    opacity: 0;
  }

  100% {
    opacity: 1;
  }
}

@media(max-width: 594px) {
  .about {
    display: block;
  }
}

@media(max-width: 679px) {
  p {
    margin: 5px;
  }
}
</style>