<template>
  <div class = "section5-background">
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
.section5-background {
    width: 100vw;
    height: 400px;
    background: transparent;
    display: flex;
    justify-content: center;
    align-items: center;
    position: relative;
    z-index: 2;
}
</style>
