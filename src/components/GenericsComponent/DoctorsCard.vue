<template>
  <div class="cs_card">
    <img :src="image" :alt="'doctor-'+ name">
    <div class="p-5">
      <h3>{{ name }}</h3>
      <h4>{{ role }}</h4>
      <p class="py-3">{{ description }}</p>
      <a class="facebook" href="https://www.facebook.com"><i class="fa-brands fa-square-facebook"></i></a>
      <a class="twitter" href="https://www.twitter.com"><i class="fa-brands fa-square-twitter"></i></a>
      <a class="instagram" href="https://www.instagram.com"><i class="fa-brands fa-square-instagram"></i></a>
    </div>
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
  .cs_card {
    background-color: white;
    img {
      max-width: 100%;
    } h3,h4 {
      font-size: 17px;
      font-weight: 300;
    } h3 {
      text-transform: uppercase;
    } p {
      font-weight: 200;
    } a {
      &.facebook {
        color: blue;
      } &.twitter {
        color: #54ACED;
      } &.instagram {
        color: #3E729A;
      }
      i {
        font-size: 30px;
      margin-right: 10px;
      }
    }
  }
</style>