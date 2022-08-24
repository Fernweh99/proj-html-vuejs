<template>
  <div>
    <TheHeader :headerNavbar="headerNavbar"/>
    <TheMain 
    :avadaHealthCards="avadaHealthCards"
    :doctorsCards="doctorsCards"
    :healthServiceCards="healthServiceCards"
    :learnMoreCards="learnMoreCards"
    />
    <TheFooter/>
  </div>
</template>

<script>
//import Component
import TheHeader from './components/TheHeader.vue';
import TheMain from './components/TheMain.vue';
import TheFooter from './components/TheFooter.vue';

//import Data
import _headerNavbar from './assets/data/_headerNavbar';
import _avadaHealthCards from './assets/data/_avadaHealthCards';
import _doctorsCards from './assets/data/_doctorsCards';
import _healthServiceCards from './assets/data/_healthServiceCards';
import _learnMoreCards from './assets/data/_learnMoreCards';

export default {
  name: 'App',
  components: {
    TheHeader,
    TheMain,
    TheFooter,
  },
  data() {
    return {
      headerNavbar: _headerNavbar,
      avadaHealthCards: _avadaHealthCards,
      doctorsCards: _doctorsCards,
      healthServiceCards: _healthServiceCards,
      learnMoreCards: _learnMoreCards,
    }
  }
}
</script>

<style lang="scss">
  @import "./assets/scss/style.scss";
</style>
