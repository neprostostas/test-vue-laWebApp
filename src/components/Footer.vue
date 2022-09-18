<template>
  <div class="CustomFooter">
    <footer class="footerWrapper">

     <div class="topPartWrapper">

      <div class="topPart">

        <div class="socialMedia">

          <div class="fbWrapper">

            <svg width="56" height="56" viewBox="0 0 56 56" fill="none" xmlns="http://www.w3.org/2000/svg">
              <path d="M28 55.9999C43.4639 55.9999 55.9999 43.4639 55.9999 28C55.9999 12.536 43.4639 0 28 0C12.536 0 0 12.536 0 28C0 43.4639 12.536 55.9999 28 55.9999Z" fill="#D1D1D6"/>
              <path d="M38.8991 36.0956L40.1395 28H32.3746V22.7472C32.3746 20.5343 33.4574 18.3726 36.9382 18.3726H40.4702V11.4819C40.4702 11.4819 37.2651 10.9346 34.2016 10.9346C27.8071 10.9346 23.6254 14.8091 23.6254 21.8298V28H16.5142V36.0956H23.6254V55.6613C25.0508 55.8857 26.5116 55.9999 28 55.9999C29.4884 55.9999 30.9492 55.8818 32.3746 55.6613V36.0956H38.8991Z" fill="#757575"/>
            </svg>

          </div>

          <div class="instWrapper">

            <svg width="36" height="36" viewBox="0 0 36 36" fill="#D1D1D6" xmlns="http://www.w3.org/2000/svg">
              <g clip-path="url(#clip0_737_1157)">
                <path d="M25.2757 0H10.7249C4.81106 0 0 4.81106 0 10.7249V25.2757C0 31.1896 4.81106 36.0006 10.7249 36.0006H25.2757C31.1896 36.0006 36.0006 31.1896 36.0006 25.2757V10.7249C36.0006 4.81106 31.1896 0 25.2757 0ZM32.3786 25.2757C32.3786 29.1983 29.1983 32.3786 25.2757 32.3786H10.7249C6.80239 32.3786 3.62202 29.1983 3.62202 25.2757V10.7249C3.62202 6.80173 6.80239 3.62202 10.7249 3.62202H25.2757C29.1983 3.62202 32.3786 6.80239 32.3786 10.7249V25.2757Z" fill="#757575"/>
                <path d="M18.0004 8.68896C12.8665 8.68896 8.68921 12.8657 8.68921 18.0001C8.68921 23.1346 12.8659 27.3113 18.0004 27.3113C23.1348 27.3113 27.3115 23.1346 27.3115 18.0001C27.3115 12.8657 23.1348 8.68896 18.0004 8.68896ZM18.0004 23.6892C14.8579 23.6892 12.3112 21.1419 12.3112 18.0001C12.3112 14.8583 14.8585 12.311 18.0004 12.311C21.1422 12.311 23.6895 14.8583 23.6895 18.0001C23.6895 21.1419 21.1422 23.6892 18.0004 23.6892Z" fill="#757575"/>
                <path d="M27.329 10.99C28.5612 10.99 29.5601 9.99113 29.5601 8.75893C29.5601 7.52673 28.5612 6.52783 27.329 6.52783C26.0968 6.52783 25.0979 7.52673 25.0979 8.75893C25.0979 9.99113 26.0968 10.99 27.329 10.99Z" fill="#757575"/>
              </g>
                <defs>
                  <clipPath id="clip0_737_1157">
                    <rect width="36" height="36"/>
                  </clipPath>
                </defs>
            </svg>
            
          </div>
         
        </div>


        <div class="centerWrapper">
          <img src="../assets/car.png" alt="car">
        </div>

        <div class="policies">

          <a href="#">Terminie condizioni</a>
          <a href="#">Privacy Policy</a>
          <a href="#">Cookie Policy</a>

        </div>

      </div>
      
      </div>

      <div class="bottomPartWrapper">
        <div class="bottomPart">
          <p class="desktop">© 2022 Scevoo è un prodotto di Consolidati sas - Tutti i diritti riservati  |  P.IVA 02634790733</p>
          <p class="desktop">Made with ❤️ by <a href="https://github.com/lytvynenkoy/">Yuriy Lytvynenko</a></p>
          <p class="mobile">© 2022 Scevoo è un</p>
          <p class="mobile">by <a href="https://github.com/lytvynenkoy/">Yuriy Lytvynenko</a></p>
        </div>
      </div>

    </footer>
  </div>
</template>

<script>

export default {
  name: 'CustomFooter',

  setup() {

    return { }
  }
}
</script>

<style scoped>

.policies a, .desktop a, .mobile a {
    color: #FFFFFF;
    text-decoration: none;
}

.policies a:hover, .desktop a:hover, .mobile a:hover {
  cursor: pointer;
  text-decoration: underline;
}

.policies a {
  font-style: normal;
  font-weight: 600;
  font-size: 18px;
  line-height: 30px;
  text-align: right;
  color: #FFFFFF;
}

.policies {
  display: grid;
}

.socialMedia {
  display: grid;
  grid-template-columns: repeat(2, auto);
  gap: 5px;
}

.instWrapper svg {
  background: #D1D1D6;
}

.fbWrapper svg {
  border-radius: 50%;
  width: 60px;
  height: 60px;
}

.instWrapper svg {
  padding: 5px;
  border-radius: 50%;
  width: 55px;
  height: 55px;
}

.topPartWrapper {
  background: #757575;
}

.topPart {
  max-width: 1200px;
  margin: 0 auto;
  padding: 20px 60px;
  display: grid;
  grid-template-columns: repeat(3, auto);
  justify-items: center;
  align-items: center;
  justify-content: space-between;
}

.bottomPartWrapper {
  background: #504d4d;
}

.bottomPart {
  max-width: 1200px;
  margin: 0 auto;
  padding: 20px 60px;
  display: grid;
  grid-template-columns: repeat(2, auto);
  justify-items: center;
  justify-content: space-between;
  align-items: center;
}

.bottomPart > p {
  font-style: normal;
  font-weight: 400;
  font-size: 16px;
  line-height: 48px;
  color: #FFFFFF;
}

  .fbWrapper svg,
  .instWrapper svg {
    cursor: pointer;
  }

.mobile {
  display: none;
}

@media screen and (max-width: 1035px) {

  .desktop {
    display: none;
  }

  .mobile {
    display: unset;
  }

}

@media screen and (max-width: 895px) {

  .fbWrapper svg {
    width: 30px;
    height: 30px;
  }

  .instWrapper svg {
    padding: 1px;
    width: 29px;
    height: 29px;
  }

  .centerWrapper img {
    width: 30px;
    height: unset;
  }

  .policies a {
    font-size: 14px;
  }
  
}

@media screen and (max-width: 510px) {

  .topPart,
  .bottomPart {
    padding: 10px 20px;
  }

}


</style>
