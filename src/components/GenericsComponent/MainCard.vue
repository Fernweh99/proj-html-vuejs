<template>
  <div class="row">
    <div class="col-10 offset-1">

      <div class="row text-center my-5">
        <div class="col-8 offset-2">
          <div class="text-center" :class="{'text-white': (color === 'white')}">
            <img v-if="image" :src="image" :alt="'img ' + title">
            <h4 class="h1 fw-lighter  my-3">{{ title }}</h4>
            <div class="hr"></div>
            <p>{{ text }}</p>
          </div>
        </div>
      </div>
    </div>
  </div>
</template>

<script>
export default {
  name: 'MainCard',
  props: {
    image: String,
    title: String,
    text: String,
    color: String,
  },
}
</script>

<style lang="scss" scoped>
  p {
    font-weight: 200;
    font-size: 21px;
  } .hr {
    margin: 20px auto;
    width: 270px;
    height: 1px;
    background-color: rgb(210, 210, 210);
  }
</style>