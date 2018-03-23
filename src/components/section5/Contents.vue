<template>
  <div class = "section5-contents">
      <div class = "section5-contents-title">더 많은 정보를 원하세요?</div>
      <div class = "line"></div>
      <div class = "section5-contents-description">다운로드 버튼을 누르면 레주메를 다운받을 수 있습니다.</div>
      <div class = "section5-contents-download">레주메 다운로드</div>
  </div>
</template>

<script>
export default {
  name: 'Contents'  
}
</script>

<style scoped>
.section5-contents {
    display: flex;
    justify-content: center;
    align-items: center;
    flex-direction: column;
    font-family: 'Nanum Gothic', sans-serif;
    position: relative;
}

.section5-contents-title {
    font-size: 30px;
    color: white;
}

.line {
    width: 130px;
    height: 1px;
    background-color: white;
    margin: 30px 0 0px 0;
}

.section5-contents-description {
    font-size: 14px;
    line-height: 100px;
    color: white;
}

.section5-contents-download {
    width: 150px;
    height: 40px;
    border: 1px solid white;
    color: white;
    display: flex;
    justify-content: center;
    align-items: center;
    font-size: 13px;
    cursor: pointer;
}



</style>
