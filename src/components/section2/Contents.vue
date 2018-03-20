<template>
  <div class = "section2-contents">
    <description/>
    <images/>
  </div>
</template>

<script>
import Description from './Description'
import Images from './Images'
export default {
  name: 'Contents',
  components: {
    Description,
    Images
  }
}
</script>

<style scoped>
  .section2-contents {
    display: flex;
    justify-content: center;
    align-items: center;
  }
</style>
