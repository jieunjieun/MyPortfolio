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
        border: 1px solid black;
        display: flex;
        justify-content: center;
        align-items: center;
        margin-bottom: 100px;
    }
</style>
