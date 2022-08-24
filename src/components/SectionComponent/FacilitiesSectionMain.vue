<template>
  <section id="tour-our-facilities">
    <div class="container">
      <MainCard
      :image="require('../../assets/img/icon-7.png')"
      title="TOUR OUR FACILITIES"
      text="Set ut perspiciatis unde omnis iste natus error
      sit voluptam accusantim doloremque laundatium, totam rem aperiam,
      eaque ipsa quae ab illo inventore veritatis et quasi architecto beatae."
      color="white"
      />
      <div class="row justify-content-center text-center">
        <div class="col-3">
          <a href="#">
            <img src="../../assets/img/play-icon.png" alt="">
          </a>
         </div>
      </div>
    </div>
  </section>
</template>

<script>
import MainCard from '../GenericsComponent/MainCard.vue';

export default {
  name: 'FacilitiesSectionMain',
  components: {
    MainCard,
  },
}
</script>

<style lang="scss">
  #tour-our-facilities {
    padding: 100px 0;
    background-image: url(../../assets/img/paralax-bg-tour-facilities.jpg);
    background-position: center;
  }
</style>