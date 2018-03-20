<template>
    <div>
        <section1/>
        <section2/>
        <section3/>
    </div>
</template>

<script>
import Section1 from './containers/Section1'
import Section2 from './containers/Section2'
import Section3 from './containers/Section3'
export default {
    name: 'MainPage',
    components: {
        Section1,
        Section2,
        Section3
    }
}
</script>

<style scoped>

</style>
