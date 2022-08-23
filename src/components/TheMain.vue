<template>
  <main>
    <AvadaSectionMain :cards="avadaHealthCards"/>
  </main>
</template>

<script>
import AvadaSectionMain from './SectionComponent/AvadaSectionMain.vue'

export default {
  name: 'TheMain',
  components: {
    AvadaSectionMain,
  },
  props: {
    avadaHealthCards: Array
  }
}
</script>

<style>

</style>