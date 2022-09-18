<template>

  <div class="whiteCircle"></div>

  <div class="topPart">
    
    <div class="leftPart">
      <h1>La Web App pensata per la ristorazione digitale</h1>
      <p>Per capire le potenzialità della nostra web app la cosa migliore è vedere una demo cliccando sul bottone sottostante.</p>
      <div class="buttonHeader">
        <button class="buttonOrdina">
           Guarda la demo
        <img class="arrowImg" src="../assets/arrow-red.png" alt="arrow-red">
        </button>
      </div>
    </div>

    <div class="rightPart">
      <img class="iphoneImg" src="../assets/iphone.png" alt="iphone">
    </div>   

  </div>

</template>

<script>

export default {
  name: 'TopPart',

  setup() {

    return { }
  }
}
</script>

<style scoped>

.whiteCircle {
  position: absolute;
  z-index: -1;
  top: -10%;
  left: -10%;
  width: 70%;
  height: 70%;
  width: 1500px;
  height: 1500px;
  background: #FFFFFF;
  border-radius: 0 0 1500px 0;
  -moz-border-radius: 0 0 1500px 0;
  -webkit-border-radius: 0 0 1500px 0;
}

.leftPart {
  display: grid;
  gap: 43px;
  max-width: 778px;
}

.topPart {
  padding: 20px 60px;
  max-width: 1100px;
  margin: 150px auto 0;
  display: grid;
  grid-template-columns: repeat(2, auto);
  align-items: start;
}

.leftPart > p {
  max-width: 526px;
}

.arrowImg {
  width: 30px;
}

.buttonHeader {
  position: relative;
}

.arrowImg {
  position: relative;
  top: 6.5px;
  right: -5px;
}

.buttonHeader {
  display: grid;
  justify-items: center;
  align-items: center;
  justify-content: start;
}

.buttonOrdina {
  border: none;
  background: #D7EFFF;
  font-style: normal;
  font-weight: 600;
  font-size: 18px;
  line-height: 28px;
  border-radius: 10px;
  padding: 5px 20px 10px 17px;
  color: #BE1622;
}

.buttonOrdina:hover {
  position: relative;
  top: 1.5px;
  background: #6c9cbc;
}

.leftPart > h1 {
  max-width: 550px;
  font-style: normal;
  font-weight: 500;
  font-size: 60px;
  line-height: 80px;
  color: #000000;
  mix-blend-mode: normal;
}

.leftPart > p {
  font-style: normal;
  font-weight: 400;
  font-size: 22px;
  line-height: 34px;
  color: #555555;
}

.iphoneImg {
  width: 375px;
  transition: .5s all ease-in-out;
}

.iphoneImg:hover {
  cursor: pointer;
  transform: scale(1.05);
  transition: .5s all ease-in-out;
}

@media screen and (max-width: 1073px) {

  .topPart {
    margin: 130px auto 0;
  }

}

@media screen and (max-width: 895px) {

  .topPart {
    margin: 120px auto 0;
    grid-template-columns: auto;
    gap: 40px;
    justify-items: start;
  }

}

@media screen and (max-width: 1200px) {

  .whiteCircle {
    display: none;
  }

}

@media screen and (max-width: 510px) {
  
  .topPart {
    padding: 20px;
    margin: 80px auto 0;
  }

  .leftPart h1 {
    font-size: 36px;
    line-height: 60px;
  }

  .iphoneImg {
    width: 80%;
  }
}

</style>
