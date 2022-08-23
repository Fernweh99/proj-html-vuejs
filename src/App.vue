<template>
  <div>
    <TheHeader :headerNavbar="headerNavbar"/>
    <TheMain 
    :avadaHealthCards="avadaHealthCards"
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
    }
  }
}
</script>

<style lang="scss">
  @import "./assets/scss/style.scss";
</style>
