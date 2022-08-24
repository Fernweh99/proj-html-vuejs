<template>
  <section id="moreCards">
    <div class="_row text-center text-white">
      <div v-for="card in cards" 
      :key="card.title" 
      class="column"
      :class="[{'bg-aqua' : (card.bgcolor === 'aqua')},{'bg-cyan' : (card.bgcolor === 'cyan')},{'bg-blue' : (card.bgcolor === 'blue')}]"
      >
        <h3 class="h5">{{card.title}}</h3>
        <img class="my-2" :src="card.source" alt="">
        <p>{{ card.text }}</p>
        <BaseButton 
        text="Learn More"
        type="base-white"
        />
      </div>
    </div>
  </section>
</template>

<script>
import BaseButton from '../GenericsComponent/BaseButton.vue';

export default {
  name: 'MoreCardsSectionMain',
  components: {
    BaseButton,
  },
  props: {
    cards: Array,
  },
}
</script>

<style lang="scss" scoped>
  ._row {
    display: flex;
    width: 100%;
    .column {
      width: calc(100% / 3);
      padding: 50px 10px;
      &.bg-aqua {
        background-color: #3AAFBF;
      } &.bg-cyan {
        background-color: #3597C3;
      } &.bg-blue {
        background-color: #327DC6;
      } p {
        line-height: 30px;
      }
    } 
  }
</style>