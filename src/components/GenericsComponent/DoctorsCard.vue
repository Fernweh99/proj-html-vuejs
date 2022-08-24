<template>
  <div>
    <img :src="image" alt="">
    <h3>{{ name }}</h3>
    <h4>{{ role }}</h4>
    <p>{{ description }}</p>
  </div>
</template>

<script>
export default {
  name: 'DoctorsCard',
  props: {
    role: String,
    image: String,
    name: String,
    description: String,
  },
}
</script>

<style lang="scss" scoped>
  img {
    max-width: 100%;
  }
</style>