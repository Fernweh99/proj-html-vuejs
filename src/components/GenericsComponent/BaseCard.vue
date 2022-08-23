<template>
  <div class="text-center">
    <img :src="image" :alt="'img' + title">
    <h4>{{ title }}</h4>
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

<style lang="scss">
  h4, p{
    font-weight: 200;
  }h4 {
    font-size: 18px;
  } p {
    font-size: 14px;
  }
</style>