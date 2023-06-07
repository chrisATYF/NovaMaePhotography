<template>
  <div class="top-bg-img">
    <div class="captionText">
      <div class="img-border">
        <p>Nova Mae Photography</p>
      </div>
    </div>
  </div>
  <section>
    <h2>My Work</h2>
    <p>Whether it's for seniors pictures, wedding photography, family portraits, or any other kind of picture taking,
      I got you covered
    </p>
  </section>
  <section>
    <div class="img-container">
      <div class="left-img">
        <img class="section-img" src="../../images/NMWebMel.jpg" />
      </div>
      <div class="center-content">
        <img class="section-img" src="../../images/NMWebHan.jpg" />
      </div>
      <div class="right-img">
        <img class="section-img" src="../../images/NMWebCan2.jpg" />
      </div>
    </div>
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

section {
  text-align: center;
  padding: 50px 80px;
}

.section-img {
  position: relative;
  height: 300px;
  width: 300px;
  object-fit: cover;
  border-radius: 100%;
  z-index: -2;
}

.img-container {
  display: flex;
  align-items: center;
  justify-content: space-between;
}

.left-img {
  left: 0;
  border-radius: 100%;
  box-shadow: inset 0px 0px 50px rgba(0, 0, 0, 0.9);
}

.center-content {
  border-radius: 100%;
  box-shadow: inset 0px 0px 10px rgba(0, 0, 0, 0.9);
}

.right-img {
  right: 0;
  border-radius: 100%;
  box-shadow: inset 0px 0px 10px rgba(0, 0, 0, 0.9);
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

@media(max-width:568px) {}
</style>