<template>
  <div class = "section1-content">
      <span>Jieun Park</span>
      <span>Web UI Developer</span>
      
  </div>
</template>

<script>
export default {
  name: 'Contents'
}
</script>

<style scoped>
@import url('https://fonts.googleapis.com/css?family=Raleway');

    .section1-content {
        display: flex;
        justify-content: center;
        align-items: center;
        flex-direction: column;
        font-family: 'Raleway', sans-serif;        
        color: white;
    }

    .section1-content span:nth-child(1) {
        font-size: 55px;
        font-weight: bold;
    }

    .section1-content span:nth-child(2) {
        font-size: 20px;
    
    }

    
</style>
