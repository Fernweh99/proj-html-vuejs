<template>
  <main>
    <AvadaSectionMain :cards="avadaHealthCards"/>
    <DoctorsSectionMain :cards="doctorsCards"/>
    <HealthSectionMain :cards="healthServiceCards"/>
    <FacilitiesSectionMain/>
    <MoreCardsSectionMain :cards="learnMoreCards"/>
    <MakeAppointmentSectionMain/>
    <BannerGradientSectionMain/>
  </main>
</template>

<script>
import AvadaSectionMain from './SectionComponent/AvadaSectionMain.vue'
import DoctorsSectionMain from './SectionComponent/DoctorsSectionMain.vue';
import HealthSectionMain from './SectionComponent/HealthSectionMain.vue';
import FacilitiesSectionMain from './SectionComponent/FacilitiesSectionMain.vue';
import MoreCardsSectionMain from './SectionComponent/MoreCardsSectionMain.vue';
import MakeAppointmentSectionMain from './SectionComponent/MakeAppointmentSectionMain.vue';
import BannerGradientSectionMain from './SectionComponent/BannerGradientSectionMain.vue';

export default {
  name: 'TheMain',
  components: {
    AvadaSectionMain,
    DoctorsSectionMain,
    HealthSectionMain,
    FacilitiesSectionMain,
    MoreCardsSectionMain,
    MakeAppointmentSectionMain,
    BannerGradientSectionMain,
},
  props: {
    avadaHealthCards: Array,
    doctorsCards: Array,
    healthServiceCards: Array,
    learnMoreCards: Array,
  }
}
</script>

<style>

</style>