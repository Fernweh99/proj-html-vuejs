<template>
  <div>
    <TheHeader :headerNavbar="headerNavbar"/>
    <TheMain/>
    <TheFooter/>
  </div>
</template>

<script>
import TheHeader from './components/TheHeader.vue';
import TheMain from './components/TheMain.vue';
import TheFooter from './components/TheFooter.vue';
import _headerNavbar from './assets/data/_headerNavbar';

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
    }
  }
}
</script>

<style lang="scss">
  @import "./assets/scss/style.scss";
</style>
