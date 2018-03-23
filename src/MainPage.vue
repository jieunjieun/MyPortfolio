<template>
    <div class = "mainpage">
        <section1/>
        <section2/>
        <section3/>
        <section4/>
        <section5/>
        <section6/>
    </div>
</template>

<script>
import Section1 from './containers/Section1'
import Section2 from './containers/Section2'
import Section3 from './containers/Section3'
import Section4 from './containers/Section4'
import Section5 from './containers/Section5'
import Section6 from './containers/Section6'
export default {
    name: 'MainPage',
    components: {
        Section1,
        Section2,
        Section3,
        Section4,
        Section5,
        Section6
    }
}
</script>

<style scoped>

.mainpage {
    position: relative;
}

.mainpage::after {
    position: fixed;
    top: 0;
    left: 0;
    content: "";
    width: 100vw;
    height: 100vh;
    background-image: url('./assets/travel.jpg');
    background-size: 100% auto;
    background-position: center;
    z-index: 1;
}


</style>
