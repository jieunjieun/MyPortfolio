//자기 소개 섹션 배경

<template>
  <div class = "section2-background">
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
    .section2-background {
        width: 100vw;
        height: 500px;
        background-color: white;
        display: flex;
        justify-content: center;
        align-items: center;
        flex-direction: row;
        position: relative;
        z-index: 2;
    }
</style>
