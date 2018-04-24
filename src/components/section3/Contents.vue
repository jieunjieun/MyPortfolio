// 스킬 섹션 로고를 위한 내용물
<template>
  <div class = "section3-contents">
    <div class ="section3-stackbox" v-for = "img in images" :key="img.id">
      <img :src="img.url"/>
    </div>
  </div>
</template>

<script>
import html5 from '../../assets/html5.png';
import jsLogo from '../../assets/js.png';
import css3 from '../../assets/css3.png';
import react from '../../assets/react.png';
import vueLogo from '../../assets/vue.png';
import node from '../../assets/node.png';
import mongo from '../../assets/mongo.png';
import npm from '../../assets/npm.png';
import webpack from '../../assets/webpack.png'

export default {
  name: 'Contents',
  data: function () {
      return {
        images: [
          {url: html5},
          {url: css3},
          {url: jsLogo},
          {url: react },
          {url: vueLogo},
          {url: node},
          {url: mongo},
          {url: npm},
          {url: webpack}
        ]
      }
  }
}
</script>

<style scoped>
    .section3-contents {
        display: flex;
        align-items: center;      
        padding: 30px;
        /* border: 2px dotted #535353;  */
        background: white;
    }

    .section3-stackbox {
        width: 100px;
        height: 100px;
        border-radius: 3px;
        margin-right: 20px;
    }

    .section3-stackbox:nth-last-child(1) {
      margin-right: 0;
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
