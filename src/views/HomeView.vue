<template>
  <div class="h-full">
    <Hero/>
    <VrImage/>
    <Creations/>
  </div>

</template>

<script>
import Creations from '../components/Creations.vue';
import Hero from '../components/Hero.vue';
import VrImage from '../components/VrImage.vue';


export default {
    setup() {
        return {};
    },
    components: { Hero, VrImage, Creations }
}
</script>

<style lang="scss" scoped>


</style>