<template>
  <section id="health-service">
    <div class="container">
      <MainCard 
      :image="require('../../assets/img/icon-6.png')"
      title="OUR HEALTH SERVICES"
      text="Set ut perspiciatis unde omnis iste natus error
      sit voluptam accusantim doloremque laundatium, totam rem aperiam,
      eaque ipsa quae ab illo inventore veritatis et quasi architecto beatae."
      />
      <div class="row">
        <div class="col-10 offset-1">
          <div class="row g-5">
            <div v-for="card in cards" :key="card.title" class="col-4">
              <BaseCard
              :image="card.source"
              :title="card.title"
              :text="card.text"
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
import BaseCard from '../GenericsComponent/BaseCard.vue';

export default {
  name: 'HealthSectionMain',
  components: {
    MainCard,
    BaseCard,
  },
  props: {
    cards: Array,
  },
}
</script>

<style lang="scss">
  #health-service {
    padding: 80px 0;
  }

</style>