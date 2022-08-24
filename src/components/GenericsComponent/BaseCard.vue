<template>
  <div class="text-center">
    <img :src="image" :alt="'img ' + title">
    <h4 class="h6 fw-lighter  my-3">{{ title }}</h4>
    <p>{{ text }}</p>
  </div>
</template>

<script>
export default {
  name: 'BaseCard',
  props: {
    image: String,
    title: String,
    text: String,
  },
}
</script>

<style lang="scss" scoped>
  h4, p{
    font-weight: 200;
  } p {
    font-size: 14px;
    line-height: 30px;
  }
</style>