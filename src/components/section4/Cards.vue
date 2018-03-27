<template>
  <div class = "section4-cards">
      <div class = "section4-card" v-for="box in card" :key="box.id">
          <div class = "section4-card-image"><img :src="box.image"/></div>
          <div class = "section4-card-title">{{ box.title }}</div>
          <div class = "section4-card-description">{{ box.description }}</div>
          <div class = "section4-card-more">MORE</div>
      </div>
  </div>
</template>

<script>
export default {
  name: 'Cards',
  data: function () {
      return {
          card: [
              {image: '../../../static/images/project1.png', title: 'Beautimage.js', description: ''},
              {image: '../../../static/images/project2.png', title: 'Dammunity', description : '설명:'},
              {image: 'url3', title: '프로젝ㅌ트3', description : '프로젝트3 설명섦여 섦여서'}
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
    display: flex;
    justify-content: center;
    align-items: center;
    flex-direction: column;
    position: relative;

}

.section4-card-image {
    width: 100%;
    height: 200px;
    position: absolute;
    top: 0;
}

.section4-card-image img {
    width: 100%;
    height: 100%;
    overflow: hidden;
}

.section4-card-title {
    font-size: 20px;
    margin-bottom: 40px; 
}

.section4-card-description {
    text-align: center;
    width: 300px;
    font-size: 13px;
    word-wrap: break-word;
    color: rgba(144, 144, 144, 0.5);
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

}
</style>
