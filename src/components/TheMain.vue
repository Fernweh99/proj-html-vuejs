<template>
  <main>
    <AvadaSectionMain :cards="avadaHealthCards"/>
    <DoctorsSectionMain :cards="doctorsCards"/>
  </main>
</template>

<script>
import AvadaSectionMain from './SectionComponent/AvadaSectionMain.vue'
import DoctorsSectionMain from './SectionComponent/DoctorsSectionMain.vue';

export default {
  name: 'TheMain',
  components: {
    AvadaSectionMain,
    DoctorsSectionMain,
  },
  props: {
    avadaHealthCards: Array,
    doctorsCards: Array,
  }
}
</script>

<style>

</style>