<!-- Please remove this file from your project -->
<template>
  <div class="circle"></div>
</template>

<style>
.circle {
  position: absolute;
  top: 25%;
  left: 52%;
  height: 50px;
  width: 50px;
  background-color: #555;
  border-radius: 50%;
}
</style>

<script>
export default {
  name: 'Ball',
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
  },
  mounted(){
    
  }
}
</script>