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
