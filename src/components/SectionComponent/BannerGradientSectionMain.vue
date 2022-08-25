<template>
  <section id="bn-gradient">
    <div class="container">
      <div class="row">
        <div class="col offset-1">
          <div class="row">
            <div v-for="n in 4" :key="n" class="col">
              <img :src="require(`../../assets/img/client-logos-${n}.png`)" alt="background gradient">
            </div>
          </div>
        </div>
      </div>
    </div>
  </section>
</template>

<script>
export default {
  name: 'BannerGradientSectionMain'
}
</script>

<style lang="scss" scoped>
  #bn-gradient {
    background-image: url(../../assets/img/rgb-gradient-bar-for-logo-carrasel.jpg);
    height: 260px;
  }
</style>