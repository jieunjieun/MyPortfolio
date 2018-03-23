<template>
  <div class = "section3-contents">
    <div class ="section3-stackbox" v-for = "img in images" :key="img.id">
      <img :src="img.url"/>
    </div>
  </div>
</template>

<script>
export default {
  name: 'Contents',
  data: function () {
      return {
        images: [
          {url: '../../../static/images/html5.png'},
          {url: '../../../static/images/css3.png'},
          {url: '../../../static/images/js.png'},
          {url: '../../../static/images/react.png'},
          {url: '../../../static/images/vue.png'},
          {url: '../../../static/images/node.png'},
          {url: '../../../static/images/mongo.png'},
          {url: '../../../static/images/npm.png'},
          {url: '../../../static/images/webpack.png'}
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
        width: 170px;
        height: 170px;
        border: 15px solid #461D0D;
        border-radius: 3px;
        margin: 30px 50px 30px 50px;

    }

    .section3-stackbox:hover {
      animation: scaleUp 1s alternate;      
      box-shadow: 0 0 2em gold;
    }

    @keyframes scaleUp {
      0% {
        transform: scale(1);
      }
      50% {
        transform: scale(1.2);
      }
      100% {
        transform: scale(1);
      }
    }

    /* .section3-stackbox:hover {
      border: 10px solid black;
      border-top: 10px solid pink;
      border-bottom: 10px solid pink;
      animation: hoverEvent 1s alternate;
    }

    @keyframes hoverEvent {
      0% {
        transform: rotate(0deg)
      }
      100% {
        transform: rotate(360deg)
      }
    } */

    .section3-stackbox img {
       width: 100%;
    }
</style>
