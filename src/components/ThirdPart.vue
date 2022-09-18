<template>

  <div class="blueCircle">

    <div class="vase">
      <img src="../assets/vase.png" alt="vase">
    </div>

    <div class="cloud">
      <img src="../assets/cloud.png" alt="cloud">
    </div>

    <div class="cloud-xs">
      <img src="../assets/cloud.png" alt="cloud">
    </div>

    <div class="darkBlueCircle"></div>

    <div class="woman">
      <img src="../assets/woman.png" alt="woman">
    </div>

  </div>

  <div class="thirdPart">

    <h2 class="title">Guarda la demo 🚀</h2>
    <p class="text1">Scansiona il QR Code con lo smartphone</p>

    <img class="qr-code-img" src="../assets/qr-code.png" alt="qr-code">

    <p class="text2">e vedrai come appareil nostro menu digitale</p>

    <h2>Prezzi</h2>
    <p class="text3">Lorem Ipsum is simply dummy text of the printing and typesetting industry</p>

    <div class="card">
      <ul class="ul-card">
        <li><img src="../assets/done.svg" alt="done"></li>
        <li><img src="../assets/done.svg" alt="done"></li>
        <li><img src="../assets/done.svg" alt="done"></li>
        <li><img src="../assets/done.svg" alt="done"></li>
        <li><img src="../assets/done.svg" alt="done"></li>
        <li><img src="../assets/done.svg" alt="done"></li>
      </ul>
      <p class="text4"><span class="price">29,90€</span> /mese<span class="star">*</span></p>
      <p class="text5"><span class="star">*</span>Prezzi IVA esclusa. Paghi i primi 3 mesi ora e puoi annullare quando vuoi.</p>
    </div>

  </div>

</template>

<script>

export default {
  name: 'ThirdPart',

  setup() {


    return { 

    }
  }
}
</script>

<style scoped>

.qr-code-img:hover {
  cursor: pointer;
  transform: scale(1.005);
  transition: .5s all ease-in-out;
}

.cloud-xs img {
  width: 150px;
}

.cloud img {
  width: 220px;
}

.cloud-xs {
  position: relative;
  z-index: -4;
  top: 7%;
  left: 19%;
}

.cloud {
  position: relative;
  z-index: -3;
  top: 5%;
  left: 66%;
}

.woman img {
  width: 150px;
}

.woman {
  position: relative;
  z-index: -2;
  top: -74%;
  left: 65%;
}

.vase img {
  width: 150px;
}

.vase {
  position: relative;
  z-index: -2;
  top: 40%;
  left: 15%;
}

.darkBlueCircle {
  position: relative;
  z-index: -5;
  top: 20%;
  left: -8%;
  width: 600px;
  height: 600px;
  border-radius: 50%;
  background: #CCE3F1;
}

.blueCircle {
  position: absolute;
  z-index: -1;
  left: 50%;
  transform: translate(-50%, 0);
  width: 1000px;
  height: 1000px;
  border-radius: 50%;
  background: #D7EFFF;
}

.text1 {
  max-width: 190px;
  margin: 0 auto;
}

.text2 {
  max-width: 220px;
  margin: 0 auto;
  padding-bottom: 120px;
}

.text3 {
  padding: 20px 0;
  max-width: 330px;
  margin: 0 auto;
}

.text4 {
  font-weight: 400;
}

.text4 span {
  font-weight: 600;
}

.text5 {
  font-size: 12px;
}

.star {
  color: #BE1622!important;
}

.qr-code-img {
  width: 200px;
  padding: 40px 0;
  transition: .5s all ease-in-out;
}

.title {
  padding-bottom: 23px;
}

p {
  font-style: normal;
  font-weight: 300;
  font-size: 20px;
  line-height: 30px;
  text-align: center;
  color: #000000;
}

h2 {
  font-style: normal;
  font-weight: 500;
  font-size: 46px;
  line-height: 46px;
  text-align: center;
  color: #BE1622;
}

.ul-card li {
  padding-right: 60px;
  text-align: right;
}

.ul-card li img {
  padding: 10px 0;
  width: 20px;
}

.thirdPart {
  text-align: center;
  padding: 60px 60px 60px;
  margin: 0 auto;
  max-width: 1100px;
}

.card {
  margin: 20px 0;
  padding: 30px 20px;
  background: #F3F3F3;
  box-shadow: 0px 0px 40px rgba(0, 0, 0, 0.1);
  border-radius: 25px;
}

@media screen and (max-width: 1073px) {
  .blueCircle {
    display: none;
  }
}

</style>
