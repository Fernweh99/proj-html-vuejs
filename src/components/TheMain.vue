<template>
  <main>
    <AvadaSectionMain :cards="avadaHealthCards"/>
    <DoctorsSectionMain :cards="doctorsCards"/>
    <HealthSectionMain :cards="healthServiceCards"/>
  </main>
</template>

<script>
import AvadaSectionMain from './SectionComponent/AvadaSectionMain.vue'
import DoctorsSectionMain from './SectionComponent/DoctorsSectionMain.vue';
import HealthSectionMain from './SectionComponent/HealthSectionMain.vue';


export default {
  name: 'TheMain',
  components: {
    AvadaSectionMain,
    DoctorsSectionMain,
    HealthSectionMain,
  },
  props: {
    avadaHealthCards: Array,
    doctorsCards: Array,
    healthServiceCards: Array,
  }
}
</script>

<style>

</style>