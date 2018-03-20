<template>
  <div class = "section2-description">
      <span class = "section2-title"><strong style = "color: #9B0007;">닭발</strong>을 좋아하는 <strong>박지은</strong>입니다.</span>
      <div class = "line"></div>
      <p class = "section2-detail"> 현재 대덕소프트웨어마이스터고 3학년에 재학중입니다.<br/>웹 프론트엔드 개발자를 꿈꾸고 있으며, 졸업 후 바로 취업을 희망하고 있습니다. <br/> 훌륭한 개발자가 되기 위해 로버트 H.슐러가 했던 말</p>
      <p class = "section2-moto">"성공에 대해서 서두르지 않고, 교만하지 않고, 쉬지않고, 포기하지 않는다."</p>
      <p class = "section2-detail">를 모토로 삼고, 하루하루를 배우는 자세로 공부하고 있습니다. <br/> 항상 노력하겠습니다. 감사합니다.</p>
  </div>
</template>

<script>
export default {
  name: 'Description',
}
</script>

<style scoped>
    .section2-description {
        width: 500px;
        height: 300px;
        margin-right: 50px;
    }

    .section2-title {
        font-family: 'Nanum Gothic', sans-serif;
        font-size: 30px;
        color: #555;
    }

    .line {
        width: 130px;
        height: 1px;
        background: linear-gradient(45deg, #ECB2B9,#A7D1EB );
        margin: 30px 0 30px 0
    }

    .section2-detail {
        font-size: 13px;
        line-height: 26px;
        font-family: 'Nanum Gothic', sans-serif;

    }

    .section2-moto {
        font-size: 13px;
        font-weight: bold;
        font-family: 'Nanum Gothic', sans-serif;
        text-indent: 5px;
        line-height: 28px;

    }

    
</style>
