// 스킬 섹션 배경

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
        height: 300px;
        /* background: linear-gradient(-45deg, #090A0B, #BD1932, #FD6724, #FFCC74);
        background-size: 400% 400%;
        -webkit-animation: Gradient 8s ease infinite;
        -moz-animation: Gradient 8s ease infinite;
        animation: Gradient 8s ease infinite; */
        display: flex;
        justify-content: center;
        align-items: center;
        position: relative;
        z-index: 2;
    }

</style>
