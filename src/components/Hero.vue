<template>
    <div class="hero relative md:h-[80vh] h-[100vh] text-white py-12 md:px-12 px-4">
        <nav class=" flex justify-between" >
            <img class="z-50 " src="../assets/images/logo.svg" alt="Logo">
            <ul class=" gap-6 hidden md:flex  ">
                <li>About</li>
                <li>Careers</li>
                <li>Events</li>
                <li>Products</li>
                <li>Support</li>
            </ul>
            <div @click="openMenu = !openMenu" class="  text-3xl md:hidden block z-50">
                <i v-if="openMenu" class="fa-solid fa-xmark"></i>
                <i v-else  class="fa-solid fa-bars  " ></i>

            </div>
            <div v-if="openMenu" class="dropdown-menu md:hidden block">
                <ul class=" text-3xl font-thin uppercase relative top-[40%] gap-6 flex flex-col  justify-center items-start pl-8 ">
                    <li>About</li>
                    <li>Careers</li>
                    <li>Events</li>
                    <li>Products</li>
                    <li>Support</li>
                </ul>
            </div>
        </nav>
        
        <div class="experience px-4 py-12 md:p-12 md:absolute  mt-[30%] md:mt-0 md:top-[40%] w-full md:max-w-[50%] lg:max-w-[40%]">
            <h1 class=" text-[2.2rem] lg:text-5xl">IMMERSIVE EXPERIENCES THAT DELIVER</h1>
        </div>
    </div>
</template>

<script>
import { ref } from 'vue'
// import gsap from 'gsap'

export default {
    setup () {
        const openMenu = ref(false)

        return {openMenu}
    }
}
</script>

<style lang="scss" scoped>

.hero{
    background: #0000006b url(../assets/images/desktop/image-hero.jpg);
    background-size: cover;
    background-repeat: no-repeat;
    background-blend-mode: multiply;


    .experience{
        border: 1.5px solid #fff;
        width: fit-content;
        //padding: 2rem;
    }

    .dropdown-menu{
        position: absolute;
        right: 0;
        top: 0px;
        height: 100%;
        background: #000000;
        width: 100%;

    }
}

li{

    &:hover{
        cursor: pointer;
    }
}
</style>