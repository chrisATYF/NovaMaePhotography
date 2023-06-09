<template>
  <div class="top-bg-img"></div>
  <div class="offering-section">
    <div class="work">
      <h2 class="work-heading">Services Provided</h2>
      <p>
        I offer a range of sessions including: senior, prom, family, graduation, engagement, and wedding!
      </p>
    </div>
    <div class="img-section">
      <img src="../../images/Hannah 7.jpg" class="first-img">
      <img src="../../images/Hanna 15.jpg" class="second-img">
      <img src="../../images/WM 12.jpg" class="third-img">
    </div>
  </div>
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
  <div class="btm-bg-img">
    <div class="captionText">
      <div class="img-border">
        <h1>Contact me today</h1>
      </div>
    </div>
  </div>
</template>

<style scoped>
.top-bg-img {
  background-image: url('../../images/Header.jpg');
  background-attachment: fixed;
  width: 100%;
  height: 400px;
  background-size: auto 50%;
  background-position: center center;
  background-repeat: no-repeat;
  text-align: center;
  position: relative;
  margin: auto;
  padding: 0;
}

.about-section {
  text-align: center;
  padding: 50px 80px;
}

.about {
  display: flex;
  align-items: center;
  justify-content: space-between;
}

.captionText {
  position: absolute;
  display: flex;
  align-items: center;
  justify-content: center;
  top: 25%;
  width: 100%;
  text-align: center;
  color: #000;
  font-size: 27px;
  letter-spacing: 8px;
  text-transform: uppercase;
}

.img-border {
  width: 60%;
  backdrop-filter: blur(2px);
}

.captionText .img-border {
  background-color: #111111af;
  color: #fff;
  padding: 70px;
  border-radius: 25px;
}

.work {
  text-align: center;
}

.work-heading {
  padding: 25px;
}

.first-img,
.second-img,
.third-img {
  height: 250px;
  border-radius: 25px;
  background-attachment: fixed;
}

.img-section {
  position: relative;
  display: flex;
  justify-content: space-between;
  width: 100%;
  padding: 50px;
}

.about-img {
  height: 250px;
  width: 250px;
  object-fit: contain;
  border-radius: 50%;
}

.btm-bg-img {
  background-image: url('../../images/NMWebMel.jpg');
  background-attachment: fixed;
  width: 100%;
  height: 400px;
  background-size: auto 100%;
  background-position: center center;
  background-repeat: no-repeat;
  text-align: center;
  position: relative;
  margin: auto;
  padding: 0;
}

@media(max-width: 679px) {
  .top-bg-img {
    background-size: 100%;
  }

  .img-border {
    width: 75%;
  }

  p {
    margin: 5px;
  }
}

@media(max-width: 619px) {

  .first-img,
  .second-img,
  .third-img {
    object-fit: contain;
    width: 100%;
    padding-bottom: 10px;
  }

  .img-section {
    display: flex;
    flex-direction: column;
    margin: 0px;
    padding: 25px;
  }
}

@media(max-width: 594px) {
  .about {
    display: block;
  }
}
</style>