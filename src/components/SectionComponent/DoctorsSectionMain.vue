<template>
  <section id="our-doctors">
    <div class="container">

      <MainCard 
      title="MEET OUR DOCTORS"
      :image='require("../../assets/img/icon-5.png")'
      text="Set ut perspiciatis unde omnis iste natus error
      sit voluptam accusantim doloremque laundatium, totam rem aperiam,
      eaque ipsa quae ab illo inventore veritatis et quasi architecto beatae."
      />

      <div class="row">
        <div class="col-10 offset-1">
          <div class="row">
            <div v-for="card in cards" :key="card.name" class="col">
              <DoctorsCard 
              :image="card.source"
              :name="card.name"
              :role="card.role"
              :description="card.description"
              />
            </div>
          </div>
        </div>
      </div>
    </div>
  </section>
</template>

<script>
import MainCard from '../GenericsComponent/MainCard.vue';
import DoctorsCard from '../GenericsComponent/DoctorsCard.vue';

export default {
  name: 'DoctorsSectionMain',
  components: {
    MainCard,
    DoctorsCard,
},
  props: {
    cards: Array,
  },
}
</script>

<style lang="scss">
  #our-doctors {
    background-color: #F7F7F7;
    padding: 80px 0;
  }
</style>