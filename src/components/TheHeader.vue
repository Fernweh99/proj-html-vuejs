<template>
  <header>
    <div class="container h-100">
      <nav class="row">
        <div class="col">
          <img src="../assets/img/medical_logo_1x_light.png" alt="main logo">
        </div>

        <div class="col">
          <div class="d-flex justify-content-end align-items-center">
            <a :href="link.href" v-for="(link, i) in headerNavbar" 
            :key="link.name">
              <span v-if="link.type==='link'" 
              :class="[{'active' : (link.active==='true')}]"
              @click="changeActive(i)"
              >
                {{link.name}}
              </span>
              <BaseButton v-else :text="link.name" type="general"/>
            </a>
          </div>
        </div>
      </nav>
      <div class="row h-100 align-items-center">
        <div class="col-6 offset-1 content text-white">
          <h2 class="display-2">Caring <span>For Life</span></h2>
          <p>
            Kind words can be short and easy to speak, but their echoes are truly endless.
            Avada Health Focuses on you as if it was our own family.
          </p>
          <BaseButton text="Learn more" type="general"/>
        </div>
      </div>
    </div>
  </header>
</template>

<script>
import BaseButton from './GenericsComponent/BaseButton.vue';

export default {
  name: 'TheHeader',
  components: {
    BaseButton,
  },
  props: {
    headerNavbar: Array,
  },
  methods: {
    changeActive(i) {
      this.headerNavbar.forEach((link) => {
        link.active = false;
      })
      // eslint-disable-next-line
      this.headerNavbar[i].active = 'true';
    }
  },
}
</script>

<style lang="scss" scoped>
  @import "../assets/scss/vars.scss";

  header {
    height: 850px;
    background-image: url(../assets/img/header-image-homepage.jpg);
    nav {
      position: fixed;
      background-color: #0000004f;
      top: 0;
      left: 0;
      width: 100%;
      padding: 25px 40px;
      a {
        text-decoration: none;
        color: white;
        margin: 0 15px;
        font-weight: 300;
        text-transform: uppercase;
        .active {
          color: $primary-color;
          font-weight: 600;
        }
      }
    }.content {
      color: white;
      font-weight: 200;
      h2{
        font-weight: 200;
        span{
          color: $primary-color;
        }
      }p {
        margin: 25px 0;
        font-size: 22px;
      }
    }
  }
</style>