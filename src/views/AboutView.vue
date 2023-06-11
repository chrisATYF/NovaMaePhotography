<template>
  <section class="about-section">
    <h2>About Me</h2>
    <div class="about">
      <p>
        Hi! My name is Genny Johnson. I'm a mother to three beautiful girls and am expecting our first boy in
        September. I've been married to my high school sweetheart for thirteen years this October. I love being
        able to capture all the special memories that come with living life. Thank you for taking the time to
        visit my website. I look forward to hearing from you!
      </p>
      <img src="../../images/GJPortrait.jpg" class="about-img">
    </div>
  </section>
</template>

<style scoped>
.about-section {
  text-align: center;
  padding: 50px 80px;
}

.about {
  display: flex;
  align-items: center;
  justify-content: space-between;
}

.about-img {
  height: 250px;
  width: 250px;
  object-fit: contain;
  border-radius: 50%;
}
</style>