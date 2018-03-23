<template>
  <div class = "section3-background">
      <contents/>
  </div>
</template>

<script>
import Contents from './Contents'
export default {
  name: 'Background',
  components: {
      Contents
  }
}
</script>

<style scoped>
    .section3-background {
        width: 100vw;
        height: 900px;
        border: 1px solid black;
        background-color: white;
        display: flex;
        justify-content: center;
        align-items: center;
        position: relative;
        z-index: 2;
    }
</style>
