<template>
    <div class = "section1-background">
        <contents/>
    </div>
</template>

<script>
import Contents from './Contents'

export default {
    name: 'Background',
    components : {
        Contents
    }
}
</script>

<style scoped>
    .section1-background {
        width: 100vw; 
        height: 600px;
        background: linear-gradient(-45deg, #96D7AC, #A7D1EB, #ECB2B9, #FFCC74);
        background-size: 400% 400%;
        -webkit-animation: Gradient 8s ease infinite;
        -moz-animation: Gradient 8s ease infinite;
        animation: Gradient 8s ease infinite;
        position: relative;
        display: flex;
        justify-content: center;
        align-items: center;
        flex-direction: column;
        z-index: 2;
    }

   @-webkit-keyframes Gradient {
	0% {
		background-position: 0% 50%
	}
	50% {
		background-position: 100% 50%
	}
	100% {
		background-position: 0% 50%
	}
}

    @-moz-keyframes Gradient {
        0% {
            background-position: 0% 50%
        }
        50% {
            background-position: 100% 50%
        }
        100% {
            background-position: 0% 50%
        }
    }

    @keyframes Gradient {
        0% {
            background-position: 0% 50%
        }
        50% {
            background-position: 100% 50%
        }
        100% {
            background-position: 0% 50%
        }
    }
</style>
