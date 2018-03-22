<template>
    <div class = "section4-contents">
        <top/>
        <cards/>
    </div>
</template>

<script>
import Top from './Top'
import Cards from './Cards'
export default {
  name: 'Contents',
  components: {
      Top,
      Cards
  }
}
</script>

<style scoped>

.section4-contents {
    display: flex;
    justify-content: center;
    align-items: center;
    font-family: 'Nanum Gothic', sans-serif;
    flex-direction: column;
}


</style>
