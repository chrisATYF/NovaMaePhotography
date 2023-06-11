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
      <img src="../../images/Hannah9.jpg" class="first-img">
      <img src="../../images/Hanna15.jpg" class="second-img">
      <img src="../../images/WM12.jpg" class="third-img">
    </div>
  </div>

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
  top: 0;
  background-image: url('../../images/Header.jpg');
  background-size: contain;
}

.top-bg-img,
.btm-bg-img {
  background-attachment: fixed;
  width: 100%;
  height: 1000px;
  background-position: center center;
  background-repeat: no-repeat;
  text-align: center;
  position: relative;
  margin: auto;
  padding: 0;
}

.offering-section {
  padding: 55px;
  background-color: rgb(74, 203, 209);
}

.btm-bg-img {
  background-image: url('../../images/NMWebMel.jpg');
  background-size: contain;
  bottom: 0;
}

.captionText {
  position: absolute;
  display: flex;
  align-items: center;
  justify-content: center;
  height: 100%;
  width: 100%;
  text-align: center;
  color: #000;
  font-size: 27px;
  letter-spacing: 8px;
}

.img-border {
  display: flex;
  align-items: center;
  justify-content: center;
  height: 65%;
  width: 60%;
  backdrop-filter: blur(2px);
}

.captionText .img-border {
  background-color: rgba(74, 202, 209, 0.623);
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
  height: 550px;
  border-radius: 25px;
  background-attachment: fixed;
  margin-left: 150px;
}

.third-img {
  margin-right: 150px;
}

.img-section {
  position: relative;
  display: flex;
  justify-content: center;
  width: 100%;
  padding: 50px;
}

@media(max-width: 1920px) {

  .top-bg-img,
  .btm-bg-img {
    height: 400px;
  }

  .first-img,
  .second-img,
  .third-img {
    height: 350px;
  }
}

@media(max-width: 679px) {
  .top-bg-img {
    background-size: 100%;
    background-attachment: scroll;
  }

  .first-img,
  .second-img,
  .third-img {
    object-fit: contain;
    width: 100%;
    padding-bottom: 10px;
    margin: 0px;
    justify-content: center;
  }

  .btm-bg-img {
    background-size: 100%;
    background-attachment: scroll;
  }

  .captionText .img-border {
    background-color: #11111100;
    color: #fff;
    padding: 70px;
    border-radius: 25px;
    backdrop-filter: none;
  }

  .img-section {
    display: flex;
    flex-direction: column;
    margin: 0px;
    padding: 25px;
  }

  .img-border {
    width: 75%;
    text-shadow: 2px 2px 4px black;
  }

  p {
    margin: 5px;
  }
}
</style>