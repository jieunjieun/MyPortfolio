<template>
  <div class = "section4-background">
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
    .section4-background {
        width: 100vw;
        height: 850px;
        display: flex;
        justify-content: center;
        align-items: center;
        background-color: white;
        position: relative;
        z-index: 2;
    }
</style>
