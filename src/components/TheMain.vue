<template>
  <main>
    <AvadaSectionMain :cards="avadaHealthCards"/>
    <DoctorsSectionMain :cards="doctorsCards"/>
    <HealthSectionMain :cards="healthServiceCards"/>
    <FacilitiesSectionMain/>
  </main>
</template>

<script>
import AvadaSectionMain from './SectionComponent/AvadaSectionMain.vue'
import DoctorsSectionMain from './SectionComponent/DoctorsSectionMain.vue';
import HealthSectionMain from './SectionComponent/HealthSectionMain.vue';
import FacilitiesSectionMain from './SectionComponent/FacilitiesSectionMain.vue';

export default {
  name: 'TheMain',
  components: {
    AvadaSectionMain,
    DoctorsSectionMain,
    HealthSectionMain,
    FacilitiesSectionMain,
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