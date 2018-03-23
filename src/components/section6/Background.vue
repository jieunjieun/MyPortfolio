<template>
  <div class = "section6-background">
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
.section6-background {
    width: 100vw; 
    height: 250px;
    background-color: white;
    position: relative;
    z-index: 2;
    display: flex;
    justify-content: center;
    align-items: center;
}
</style>
