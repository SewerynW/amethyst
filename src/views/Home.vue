<template>
  <div class="playground">
    <Square />
    <p>Height: {{ windowOuterHeight }} - px</p>
    <p>Width: {{ windowOuterWidth }} - px</p>
  </div>
</template>

<script>
import Square from '@/components/Square.vue'

export default {
  name: 'Home',
  components: {
    Square
  },

  data() {
    return {
      // n: 10,
      windowOuterHeight: 0,
      windowOuterWidth: 0,
      x: 0,
      y: 0
    }
  },
  mounted() {
    this.windowOuterWidth = window.innerWidth
    this.windowOuterHeight = window.innerHeight

    console.log('OBject', this.Square)
  }
}
</script>

<style lang="scss">
.playground {
  height: 100vh;
  background-color: #4f4e32;
}
</style>
