<template>
  <div class = "section3-contents">
    <div class ="section3-stackbox" v-for = "img in images" :key="img.id">
        <img :src ="img.url" />
    </div>
  </div>
</template>

<script>
export default {
  name: 'Contents',
  data: function () {
      return {
        images: [
          {url: `../../assets/HTML5logo.png`},
          {url: `../../assets/CSS3logo.png`}
        ]
      }
  }
}
</script>

<style scoped>
    .section3-contents {
        width: 1000px;
        display: flex;
        justify-content: center;
        align-items: center;
        flex-wrap: wrap;
        
    }

    .section3-stackbox {
        width: 220px;
        height: 220px;
        border: 2px solid black;
        border-radius: 100%;
        margin: 30px 50px 30px 50px;
    }
</style>
