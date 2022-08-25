<template>
  <footer>
    <div class="p-5">
      <div class="container-fluid">
        <div class="row g-5">
          <div class="col">
            <img src="../assets/img/medical_logo_1x_dark.png" alt="logo"/>
            <p class="py-3">
              Sed ut perspiciatis unde omnis iste natus error sit voluptatem accusantium dolemue launti
              totam aperiam, eaque ipsa quae ab illo. Invente veriatis et quasi architecto beatae luptatem
              accusantium, remaperiamsiat. Voluptatem accusest etsium loremque laudaien. Lorem ipsum sits dolores ets unser.
            </p>
            <hr>
            <h4 class="mb-4">LEARN MORE ABOUT US</h4>
            <a class="facebook" href="https://www.facebook.com/"><i class="fa-brands fa-square-facebook"></i></a>
            <a class="twitter" href="https://www.twitter.com"><i class="fa-brands fa-square-twitter"></i></a>
            <a class="youtube" href="https://www.youtube.com"><i class="fa-brands fa-square-youtube"></i></a>
            <a class="instagram" href="https://www.instagram.com"><i class="fa-brands fa-square-instagram"></i></a>
          </div>

          <div class="col">
            <h3>CONTACT INFORMATION</h3>
            <div class="_hr"></div>
            <p><i class="fa-solid fa-location-dot"></i>121 King Street, London United Kingdom</p>
            <p><i class="fa-solid fa-phone-flip"></i>1.800.458.566</p>
          </div>

          <div class="col">
            <h3>MEDICAL DEPARTMENTS</h3>
            <div class="_hr"></div>
            <div class="mb-5">
              <div class="cont-link-depart"><i class="fa-solid fa-circle-chevron-right"></i><span>Cardiology</span></div>
              <div class="cont-link-depart"><i class="fa-solid fa-circle-chevron-right"></i><span>Pediactrics</span></div>
              <div class="cont-link-depart"><i class="fa-solid fa-circle-chevron-right"></i><span>Diabetes Care</span></div>
              <div class="cont-link-depart"><i class="fa-solid fa-circle-chevron-right"></i><span>Pre-natel Care</span></div>
              <div class="cont-link-depart"><i class="fa-solid fa-circle-chevron-right"></i><span>Ultrasound EchoCardiogram</span></div>
            </div>
            <BaseButton text="VIEW OUR DEPARTMENTS" type="base-black"/>
          </div>
        </div>
      </div>
    </div>
    <div class="copyright">
      <span>©copyright 2012-2020 | Avada Theme by Theme Fusion | All Rights Reserved | Powered by WordPress</span>
    </div>
  </footer>
</template>

<script>
import BaseButton from './GenericsComponent/BaseButton.vue';

export default {
  name: 'TheFooter',
  components: {
    BaseButton,
}
}
</script>

<style lang="scss" scoped>
@import "../assets/scss/vars.scss";
  h4 {
    font-size: 15px;
    font-weight: 300;
  } h3 {
    font-size: 17px;
    font-weight: 400;
  } ._hr {
    margin: 20px 0;
    width: 30px;
    height: 2px;
    background-color: $primary-color;
  } p {
    font-size: 14px;
    line-height: 30px;
    font-weight: 300;
    i {
      color: $primary-color;
      margin-right: 10px;
    }
  }a {
      &.facebook {
        color: blue;
      } &.twitter {
        color: #54ACED;
      } &.instagram {
        color: #3E729A;
      } &.youtube {
        color: red;
      }i {
        font-size: 30px;
        margin-right: 10px;
      }
    } .cont-link-depart {
      display: flex;
      align-items: center;
      margin-bottom: 10px;
      cursor: pointer;
      i {
        margin-right: 10px;
        font-size: 22px;
        color: $primary-color;
      } span {
        font-size: 14px;
        font-weight: 300;
      }
    }
  .copyright {
    background-color: #F7F7F7;
    padding: 15px 3.7rem;
    span {
      font-size: 13px;
      font-weight: 200;
    }
  }
</style>