<template>
  <div class = "section4-top">
    <div class = "section4-contents-Top">진행한 프로젝트</div>
        <div class = "line"></div>
    <div class = "section4-contents-description">현재까지 진행한 프로젝트입니다.</div>
  </div>
</template>

<script>
export default {
  name: 'Top'  
}
</script>

<style scoped>

.section4-top {
    display: flex;
    justify-content: center;
    align-items: center;
    flex-direction: column;
    margin-bottom: 30px;
}

.section4-contents-Top {
    font-size: 30px;
    color: #555;
}

.line {
    width: 130px;
    height: 1px;
    background-color: rgba(144, 144, 144, 0.5);
    margin: 30px 0px 30px 0px;
}
</style>
