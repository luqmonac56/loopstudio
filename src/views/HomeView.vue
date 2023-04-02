<template>
  <div class="h-full">
    <Hero/>
    <VrImage/>
    <Creations/>
    <Footer/>
  </div>

</template>

<script>
import Creations from '../components/Creations.vue';
import Hero from '../components/Hero.vue';
import VrImage from '../components/VrImage.vue';
import Footer from '../components/Footer.vue';


export default {
    setup() {
        return {};
    },
    components: { Hero, VrImage, Creations, Footer }
}
</script>

<style lang="scss" scoped>


</style>