<template>
  <div class="square"></div>
</template>

<script>
export default {
  name: 'Square',
  data() {
    return {
      marked: false
    }
  },

  mounted() {
    const box = document.getElementsByClassName('square')

    console.log('mamy box', box)
    const info = box[0].getBoundingClientRect()
    // getBoundingClientRect
    console.log('box info', info)
  }
}
</script>

<style lang="scss">
.square {
  background-color: cadetblue;
  border: 1px solid red;
  width: 15px;
  height: 15px;
}
</style>
