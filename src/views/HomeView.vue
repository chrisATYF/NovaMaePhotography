<script setup>
import { supabase } from '../supabase'

var bannerImg = ""
var leftImg = ""
var rightImg = ""
var centerImg = ""
var btmImg = ""

const fetchImgs = async () => {
  const { data: bannerImgData } = supabase
    .storage
    .from('images')
    .getPublicUrl('Header.jpg')

  bannerImg = bannerImgData.publicUrl

  const { data: leftImgData } = supabase
    .storage
    .from('images')
    .getPublicUrl('Hannah9.jpg')

  leftImg = leftImgData.publicUrl

  const { data: centerImgData } = supabase
    .storage
    .from('images')
    .getPublicUrl('Hanna15.jpg')

  centerImg = centerImgData.publicUrl

  const { data: rightImgData } = supabase
    .storage
    .from('images')
    .getPublicUrl('WM12.jpg')

  rightImg = rightImgData.publicUrl

  const { data: BtmImgData } = supabase
    .storage
    .from('images')
    .getPublicUrl('NMWebMel.jpg')

  btmImg = BtmImgData.publicUrl
}

fetchImgs()
</script>

<template>
  <div class="top-bg-img" v-bind:style="{ 'background-image': 'url(' + bannerImg + ')' }"></div>
  <div class="offering-section">
    <div class="work">
      <h2 class="work-heading">Services Provided</h2>
      <p>
        I offer a range of sessions including: senior, prom, family, graduation, engagement, and wedding!
      </p>
    </div>
    <div class="img-section">
      <img :src="leftImg" class="first-img">
      <img :src="centerImg" class="second-img">
      <img :src="rightImg" class="third-img">
    </div>
  </div>

  <div class="btm-bg-img" v-bind:style="{ 'background-image': 'url(' + btmImg + ')' }">
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
}

.third-img {}

.img-section {
  position: relative;
  display: flex;
  justify-content: space-around;
  width: 100%;
  padding: 50px 0px;
}

@media(max-width: 1920px) {

  .top-bg-img,
  .btm-bg-img {
    height: 500px;
  }

  .first-img,
  .second-img,
  .third-img {
    height: 350px;
  }
}

@media(max-width: 768px) {
  .top-bg-img {
    background-size: 100%;
    background-attachment: none;
  }

  .first-img,
  .second-img,
  .third-img {
    width: 100%;
    padding-bottom: 10px;
    margin: 0px;
  }

  .btm-bg-img {
    background-size: 100%;
    background-attachment: none;
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