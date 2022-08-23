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
    padding: 7px 20px;
    &.general{
      background-color: #40bece;
      color: white;
      border-radius: 5px;
      border: 1px solid black;
    }&.base-black{
      background-color: transparent;
      border: 2px solid black;
      color: black;
    }&.base-white{
      background-color: transparent;
      border: 2px solid white;
      color: white;
    }
  }
</style>