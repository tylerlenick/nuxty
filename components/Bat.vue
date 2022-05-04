<!-- Please remove this file from your project -->
<template>
  <div v-bind:style="{transform: `rotate(${deg}deg)`}" @click="swingBat" class="square"></div>
</template>

<style>
.square {
  position: absolute;
  top: 80%;
  left: 50%;
  height: 50px;
  width: 200px;
  background-color: #555;
  transition: transform 0.1s ease-in-out;
}
</style>

<script>
export default {
  name: 'Bat',
  data() {
    return {
      deg: 0,
    }
  },
  methods: {
    swingBat() {
      this.deg += 90;

      setTimeout(() => {
        this.deg = 0
      }, 500)
    }
  }
}
</script>