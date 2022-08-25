<template>
  <footer>
    <div class="p-5">
      <div class="container-fluid">
        <div class="row g-5">
          <div class="col">
            <img src="../assets/img/medical_logo_1x_dark.png" alt="logo"/>
            <p>
              Sed ut perspiciatis unde omnis iste natus error sit voluptatem accusantium dolemue launti
              totam aperiam, eaque ipsa quae ab illo. Invente veriatis et quasi architecto beatae luptatem
              accusantium, remaperiamsiat. Voluptatem accusest etsium loremque laudaien. Lorem ipsum sits dolores ets unser.
            </p>
            <hr>
            <h4>LEARN MORE ABOUT US</h4>
          </div>

          <div class="col">
            <h3>CONTACT INFORMATION</h3>
          </div>

          <div class="col">
            <h3>MEDICAL DEPARTMENTS</h3>
          </div>
        </div>
      </div>
    </div>
    <div class="copyright">
      <span>copyright</span>
    </div>
  </footer>
</template>

<script>
export default {
  name: 'TheFooter'
}
</script>

<style lang="scss" scoped>
  h4 {
    font-size: 15px;
    font-weight: 300;
  } h3 {
    font-size: 17px;
    font-weight: 400;
  } .copyright {
    background-color: #F7F7F7;
    padding: 15px 3.7rem;
  }
</style>