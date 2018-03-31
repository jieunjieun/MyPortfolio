// 자기소개 섹션 전체적인 내용 (사진 + 글)

<template>
  <div class = "section2-contents">
    <!-- 소개 -->
    <description/>
    <!-- 소개 사진 -->
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
