<template>
  <div class = "section6-contents-info">
      <div class = "section6-contents-logo">
          <a href="https://www.facebook.com/jieun.jieunjieunjieun" class = "logo"></a>
          <a href="https://www.github.com/jieunjieun" class = "logo"></a>
          <a href="http://a-tothe-z.tistory.com/" class = "logo"></a>
      </div>
      <div class = "section6-contents-siteinfo">
          designed by HTML5UP.net | jieun park | kyn07077@gmail.com
      </div>
  </div>
</template>

<script>
export default {
  name: 'Contents'
}
</script>

<style scoped>

.section6-contents-info {
    width: 300px;
    height: 100px;
    display: flex;
    align-items: center;
    justify-content: space-between;
    flex-direction: column;
}

.section6-contents-logo {
    display: flex;
    justify-content: center;
    align-items: center;
    flex-direction: row;
}

.section6-contents-logo a {
    width: 40px;
    height: 40px;
    margin-right: 20px;
}

.section6-contents-logo a:nth-child(1) {
    background-image: url('../../assets/facebook.png');
    background-size: 100% auto;
}

.section6-contents-logo a:nth-child(2) {
    background-image: url('../../assets/github-logo.png');
    background-size: 100% auto;
}

.section6-contents-logo a:nth-child(3) {
    background-image: url('../../assets/tistory.png');
    background-size: 100% auto;
    margin-right: 0px;
}

.section6-contents-siteinfo {
    white-space: nowrap;
    color: rgba(144, 144, 144, 0.5);    
    font-size: 12px;


}







</style>
