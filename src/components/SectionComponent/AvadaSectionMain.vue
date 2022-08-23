<template>
  <section id="avada-section">
    <div class="container">
      <div class="row">
        <div class="col-10 offset-1">

          <div class="row text-center my-5">
            <div class="col-8 offset-2">
              <h2 class="_fw-200">Welcome to Avada Health</h2>
              <p class="_fw-200">
                Sed ut perspiciatis unde omnis iste natus error sit voluptatem accusantium 
                doloremque laudantium, totam rem aperiam, eaque ipsa quae ab illo
              </p>
            </div>
          </div>

          <div class="row">
            <div class="col" v-for="card in cards" :key="card.title">
              <BaseCard :image="card.source" :title="card.title" :text="card.text"/>
            </div>
          </div>
        </div>
      </div>
    </div>
  </section>
</template>

<script>
import BaseCard from '../GenericsComponent/BaseCard.vue'

export default {
  name: 'AvadaSectionMain',
  components: {
    BaseCard,
  },
  props: {
    cards: Array,
  }
}
</script>

<style lang="scss" scoped>
  #avada-section {
    padding: 80px 0;
    ._fw-200 {
      font-weight: 200;
    } p {
      font-size: 20px;
    }
  }
</style>