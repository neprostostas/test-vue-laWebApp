<template>
  <div class="CustomHeader">
    <header>

      <div class="headerWrapperColor">

        <div class="headerWrapper">

          <div class="logoWrapper">
            <img class="logoImg" src="../assets/logo.png" alt="logo">
          </div>

          <nav class="customNav">

            <div class="navInfo">
              <a href="">Caratteristiche e funzionalità</a>
              <a href="">Prezzi</a>
              <a href="">Guarda la demo</a>
            </div>

            <div class="buttonHeader">
              <a href="#anker" class="buttonOrdina">
                Ordina Ora

              <img class="arrowImg" src="../assets/arrow.png" alt="arrow">
              </a>
            </div>

          </nav>

        </div>

      </div>



    </header>
  </div>
</template>

<script>

export default {
  name: 'CustomHeader',

  setup() {

    return { }
  }
}
</script>

<style scoped>

.headerWrapperColor {
  background: #f3f3f3;
  position: fixed;
  top: 0;
  left: 0;
  right: 0;
  z-index: 999;
}

.headerWrapper {
  z-index: 999;
  max-width: 1200px;
  margin: 0 auto;
  background: #f3f3f3;
  padding: 20px 60px;
  display: grid;
  gap: 40px;
  grid-template-columns: repeat(2, auto);
  justify-content: space-between;
}

.logoWrapper {
  display: grid;
  align-items: center;
}

.logoWrapper:hover {
  cursor: pointer;
}

.customNav {
  display: grid;
  grid-template-columns: repeat(2, auto);
  gap: 54px;
}

.navInfo {
  display: grid;
  grid-template-columns: repeat(3, auto);
  align-items: center;
  justify-content: center;
  gap: 49px;
}

.navInfo > a {
  text-decoration: none;
  font-style: normal;
  font-weight: 600;
  font-size: 18px;
  line-height: 28px;
  color: #000000;
}

.navInfo > a:hover {
  text-decoration: underline;
}

.logoImg {
  width: 180px;
  height: 92px;
}

.arrowImg {
  width: 30px;
}

.arrowImg {
  position: relative;
  top: 3px;
  right: -5px;
}

.buttonHeader {
  position: relative;
  display: grid;
  width: fit-content;
  align-items: center;
}

.buttonOrdina {
  text-decoration: none;
  border: none;
  background: #BE1622;
  font-style: normal;
  font-weight: 600;
  font-size: 18px;
  line-height: 28px;
  border-radius: 10px;
  padding: 10px 20px 10px 17px;
  color: #ffffff;
}

.buttonOrdina:hover {
  position: relative;
  top: 1.5px;
  background: #6c9cbc;
}

@media screen and (max-width: 1073px) {

  .navInfo {
    display: none;
  }

  .customNav {
    grid-template-columns: auto;
  }
}

@media screen and (max-width: 510px) {
  .headerWrapper {
    padding: 20px;
    gap: 20px;
  }

  .logoImg {
    width: 120px;
    height: unset;
  }
}

</style>