<template>
  <div class="top-bg-img">
    <div class="captionText">
      <div class="img-border">
        <h1>Nova Mae Photography</h1>
      </div>
    </div>
  </div>
  <section class="work-section">
    <h2>My Work</h2>
    <p>Whether it's for seniors pictures, wedding photography, family portraits, or any other kind of picture taking,
      I got you covered
    </p>
  </section>
</template>

<style scoped>
.top-bg-img {
  background-image: url('../../images/NMWebCan.jpg');
  min-height: 400px;
  position: relative;
  opacity: 0.70;
  background-position: center;
  background-size: cover;
  background-repeat: no-repeat;
  background-attachment: fixed;
}

.work-section {
  text-align: center;
  padding: 50px 80px;
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

@media(max-width: 679px) {
  .img-border {
    width: 100%;
  }
}
</style>