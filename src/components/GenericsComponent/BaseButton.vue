<template>
  <div>
    <button
    :class="[{ 'general' : isGeneral },{ 'base-black' : isBaseBlack },{ 'base-white' : isBaseWhite}]">
      {{ text }}
    </button>
  </div>
</template>

<script>
export default {
  name: 'BaseButton',
  props: {
    text: {
      type: String,
      required: true,
      },
    type: {
      type: String,
    }
  },
  computed: {
    isGeneral() {
      return this.type === 'general';
    },
    isBaseBlack() {
      return this.type === 'base-black';
    },
    isBaseWhite() {
      return this.type === 'base-white';
    }
  }
}
</script>

<style lang="scss">
  button {
    padding: 10px 30px;
    &.general{
      text-transform: uppercase;
      background-color: #3cb0c0;
      color: white;
      border-radius: 2px;
      border: 1px solid rgb(116, 115, 115);
    }&.base-black{
      text-transform: uppercase;
      background-color: transparent;
      border: 2px solid black;
      color: black;
    }&.base-white{
      text-transform: uppercase;
      background-color: transparent;
      border: 2px solid white;
      color: white;
    }
  }
</style>