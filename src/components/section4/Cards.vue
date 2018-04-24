<template>
  <div class = "section4-cards">
      <div class = "section4-card" v-for = "box in card" :key="box.id">
          <div class = "section4-card-image"><img :src="box.imageurl"/></div>
          <div class = "section4-card-content">
            <div class = "section4-card-title">{{ box.title }}</div>
            <div class = "section4-card-info">
                <div class = "section4-card-info-info">기간: <div>{{ box.days }}</div></div>
                <br/>
                <div class = "section4-card-info-info">분야 : <div>{{ box.subject }}</div></div>   
                <br/>            
                <div class = "section4-card-info-info">스킬 : <div>{{ box.skill }}</div></div> 
                <div class = "section4-card-info-description"> <div>{{ box.description }}</div></div>
            </div>
            <a class = "section4-card-more" :href="box.url">MORE</a>
          </div>          
      </div>
  </div>
</template>

<script>
// import image1 from '../../assets/small.jpg';
import image1 from '../../assets/p1.png';
import image2 from '../../assets/p2.png';
import image3 from '../../assets/p3.png';

export default {
  name: 'Cards',
  data: function () {
      return {
          card: [
              // 카드 내용 (프로젝트 이름, 스킬, 분야, 기간 , 설명 등)
              {imageurl: image2, title: 'Dammunity',skill: 'HTML, CSS, JS(Vue.js)', subject: 'web UI development', days: '17.10 ~ 17.12' , url: 'https://github.com/DSM-Sinabro/DSM-Community', description: '대덕소프트웨어마이스터고등학교 학생들의 즐거운 커뮤니케이션을 위한 교내 커뮤니티 사이트 입니다. '},
              {imageurl: image3, title: 'Beautimage.js', skill: 'HTML, CSS, JS', subject: 'web UI development', days: '17.08 ~ 17.09',  url: 'https://github.com/jieunjieun/make-ImageFilter', description: 'Javascript를 활용한 간단한 이미지 필터 라이브러리 입니다.'},
              {imageurl: image1, title: 'infobank 사업부서 페이지', skill: 'HTML, CSS, JS(Vue.js, Node.js)', subject: 'web UI dev & Server dev', days: '18.01 ~ 18.02',  url: 'https://github.com/jieunjieun/business-department', description: '주식회사 인포뱅크의 사업부서 페이지를 개발하였습니다.'}
          ]
      }
  }
}
</script>

<style scoped>
.section4-cards {
    margin-top: 20px;
    width: 1100px;
    height: 550px;
    display: flex;
    justify-content: space-between;
    align-items: center;
    font-family: 'Nanum Gothic', sans-serif;

}

.section4-card {
    width: 330px;
    height: 550px;

    position: relative;

}

.section4-card-image {
    width: 100%;
    height: 200px;
}

.section4-card-image img {
    width: 100%;
    height: 100%;
    overflow: hidden;
}

.section4-card-title {
    font-size: 20px;
    margin-bottom: 40px; 
    margin-top: 10px;
}

.section4-card-content {
    display: flex;
    justify-content: center;
    align-items: center;
    flex-direction: column;
    
}

.section4-card-info {
    text-align: center;
    width: 300px;
    font-size: 13px;
    word-wrap: break-word;
}


.section4-card-info-info {
    display: inline-block;
    color: rgba(144, 144, 144, 0.5);    
}

.section4-card-info-info div {
    display: inline-block;
    color: black;
}

.section4-card-info-description {
    color: black;
    /* font-weight: 70; */
    margin-top: 30px;
}

.section4-card-more {
    width: 120px;
    height: 40px;
    position: absolute;
    border: 1px solid rgba(144, 144, 144, 0.5);
    border-radius: 4px; 
    bottom: 0;
    margin: 30px 0 30px 0;
    display: flex;
    justify-content: center;
    align-items: center;
    font-size: 14px; 
    font-family: 'Raleway', sans-serif;   
    text-decoration: none;
    color: black;

}

.section4-card-info-script {
    
}
</style>
