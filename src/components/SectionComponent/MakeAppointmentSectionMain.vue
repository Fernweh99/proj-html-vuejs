<template>
  <section id="make-appointment">
    <div class="container">

      <MainCard
      title="Make An Appointment"
      text="Set ut perspiciatis unde omnis iste natus error
        sit voluptam accusantim doloremque laundatium, totam rem aperiam,
        eaque ipsa quae ab illo inventore veritatis et quasi architecto beatae."
      color="white"
      />
      <div class="row">
        <div class="col-3 offset-3">
          <input type="text" placeholder="Name*">
        </div>
        <div class="col-3">
          <input type="email" placeholder="Email*">
        </div>

        <div class="col-3 offset-3">
          <input type="phone" placeholder="Phone Number">
        </div> 
        <div class="col-3">
          <input type="date" placeholder="Appointment Date">
        </div>

        <div class="col-6 offset-3">
          <textarea name="" id="">How can we help you?*</textarea>
        </div> 

        <div class="col-6 offset-3 _button">
          <BaseButton 
          text="MAKE AN APPOINTMENT"
          type="general"
          width="max"
          />
        </div> 
      </div>
    </div>
  </section>
</template>

<script>
import MainCard from '../GenericsComponent/MainCard.vue';
import BaseButton from '../GenericsComponent/BaseButton.vue';

export default {
  name: 'MakeAppointmentMainSection',
  components: {
    MainCard,
    BaseButton,
  },
}
</script>

<style lang="scss" scoped>
  #make-appointment {
    padding: 150px 0;
    background-image: url(../../assets/img/make-an-appointment.jpg);
    background-position: center;
    input,textarea {
      width: 100%;
      margin-bottom: 20px;
      background-color: transparent;
      border: 1px solid rgb(203, 203, 203);
      color: gray;
      font-size: 12px;
      padding: 10px
    } textarea {
      height: 100px;
    }
  }
</style>