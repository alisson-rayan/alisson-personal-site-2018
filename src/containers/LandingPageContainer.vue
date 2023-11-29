<template>
    <div id="particles">
        <landing-page />
    </div>
</template>

<script>
import 'particles.js'
import LandingPage from '../components/landingPage'
import options from '../util/particlesConfig'

export default {
    components: {
        LandingPage
    },
    methods: {
        initParticles () {
            particlesJS('particles', options)
        }
    },
    mounted () {
        this.$nextTick(() => {
            this.initParticles()
        })
    }
}
</script>

<style lang="scss">
    #particles {
        display: flex;
        justify-content: center;
        align-items: center;
        background: #141619;
        width: 100%;
        height: 100%;
        position: fixed;
        z-index: -10;
        top: 0;
        left: 0;

        canvas {
            display: block;
            vertical-align: bottom;
            -webkit-transform: scale(1);
            -ms-transform: scale(1);
            transform: scale(1);
            opacity: 1;
            -webkit-transition: opacity .8s ease, -webkit-transform 1.4s ease;
            transition: opacity .8s ease, transform 1.4s ease
        }
    }
</style>
