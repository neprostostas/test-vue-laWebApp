<template>


  <div class="fourthPart">

    <h2 class="title">Contattaci</h2>
    <p class="text">Compila il form sottostante e richiedi subito il tuo Scevoo</p>

    <form class="customForm" action="" id="form1">
      <input type="text" placeholder="Nome e cognome">
      <input type="email" placeholder="E-mail" required>
      <input type="tel" placeholder="Telefono">
      <input type="text" placeholder="Nome dell’attività" required>
      <select name="select" required>
        <option value="" selected disabled hidden>Tipo di attività</option>
        <option value="value1">Value 1</option>
        <option value="value2">Value 2</option>
        <option value="value3">Value 3</option>
      </select>
      <input type="text" placeholder="Città">

      <div class="checkWrapper">
        <input class="checkboxCustom" type="checkbox" name="privacy" required>
        <label for="privacy">Accetto <a href="#">Termini e condizioni</a> e <a href="#">Privacy</a></label>
      </div>

    </form>
    
    <div class="buttonHeader">
      <button id="anker" type="submit" form="form1" value="Submit" class="buttonOrdina">
        Ordina Ora
      <img class="arrowImg" src="../assets/arrow.png" alt="arrow">
      </button>
    </div>

    <p class="textLast">I campi contrassegnati con * sono obbligatori</p>

  </div>

  <div class="greyCircle"></div>

</template>

<script>

export default {
  name: 'FourthPart',

  setup() {


    return { 

    }
  }
}
</script>

<style scoped>

.greyCircle {
  position: absolute;
  z-index: -1;
  background: #D9D9D9;
  transform: translate(0, -86%);
  height: 1000px;
  width: 100%;
  border-radius: 40% 40% 0 0;
}

input, select {
  width: 400px;
  background: rgba(255, 255, 255, 0.7);
  border-radius: 15px;
  border: none;
  padding: 15px 35px;

  font-family: 'Outfit';
  font-style: normal;
  font-weight: 400;
  font-size: 16px;
  line-height: 22px;
  color: #AAAAAA;
}

select {
  -webkit-appearance: none;
  -moz-appearance: none;
  appearance: none;
  /* Some browsers will not display the caret when using calc, so we put the fallback first */ 
  background: url("http://cdn1.iconfinder.com/data/icons/cc_mono_icon_set/blacks/16x16/br_down.png") white no-repeat 98.5% !important; /* !important used for overriding all other customisations */
  background: url("http://cdn1.iconfinder.com/data/icons/cc_mono_icon_set/blacks/16x16/br_down.png") white no-repeat calc(100% - 20px) !important; /* Better placement regardless of input width */
}
/*For IE*/
select::-ms-expand { display: none; }

select {
  padding: 15px 35px 15px 35px;
  width: 470px;
}

input:focus, select:focus { 
  outline: none!important;
  border-color: #BE1622;
  box-shadow: 0 0 10px #BE1622;
}

input[type='checkbox'] {
  accent-color: #BE1622;
}

.checkboxCustom:focus {
  outline: none!important;
  border-color: none;
  box-shadow: none;
}

.checkWrapper {
  padding: 10px 0 20px;
  display: grid;
  grid-template-columns: 10px auto;
  gap: 7px;
  justify-items: center;
  align-items: center;
  justify-content: center;
}

.title {
  padding-bottom: 19px;
  font-style: normal;
  font-weight: 500;
  font-size: 46px;
  line-height: 46px;
  text-align: center;
  color: #BE1622;
}

label {
  font-style: normal;
  font-weight: 300;
  font-size: 12px;
  line-height: 20px;
  text-align: center;
  color: #000000;
}

label a:hover {
  text-decoration: underline;
}

label a {
  font-style: normal;
  font-weight: 500;
  font-size: 12px;
  line-height: 14px;
  text-align: center;
  color: #BE1622;
  text-decoration: none;
}

.text {
  margin: 0 auto;
  max-width: 250px;
  font-style: normal;
  font-weight: 300;
  font-size: 20px;
  line-height: 22px;
  text-align: center;
  color: #000000;
  padding-bottom: 47px;
}

.textLast {
  font-style: normal;
  font-weight: 300;
  font-size: 12px;
  line-height: 12px;
  text-align: center;
  color: #777777;
}

.customForm {
  display: grid;
  gap: 20px;
  align-items: center;
  justify-items: center;
  justify-content: center;
}

.fourthPart {
  text-align: center;
  padding: 60px 60px 90px;
  margin: 0 auto;
  max-width: 1100px;
}

.arrowImg {
  width: 30px;
}

.buttonHeader {
  position: relative;
  display: grid;
  width: fit-content;
  align-items: center;
  margin: 0 auto;
}

.arrowImg {
  position: relative;
  top: 3px;
  right: -5px;
}

.buttonOrdina {
  border: none;
  background: #BE1622;
  font-style: normal;
  font-weight: 600;
  font-size: 18px;
  line-height: 28px;
  border-radius: 10px;
  padding: 10px 20px 10px 17px;
  color: #ffffff;
  margin-bottom: 20px;
}

.buttonOrdina:hover {
  position: relative;
  top: 1.5px;
  background: #6c9cbc;
}

@media screen and (max-width: 1073px) {
  .greyCircle, .greySquare {
    display: none;
  }
}

@media screen and (max-width: 555px) {
  input {
    width: 300px;
  }

  select {
    width: 370px;
  }
}

@media screen and (max-width: 435px) {
  input {
    width: 250px;
  }

  select {
    width: 320px;
  }
}

</style>
