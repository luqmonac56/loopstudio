<template>
    <transition
        appear
        @before-enter="beforeEnter"
        @enter="enter"
    >
        <div class="relative mx-auto my-0 max-w-[1400px] md:flex-row flex flex-col gap-8 md:gap-0 mt-16 px-4 md:px-12 items-center">
            <div class="  md:w-[50%]">
                <img class=" vrImage w-full block" src="../assets/images/desktop/image-interactive.jpg" alt="">
            </div>
            <div class=" text-center  md:w-[50%] md:max-w-[600px] bg-white ">
                <h2 class="text-3xl md:text-4xl lg:text-[3rem] mb-4 tracking-widest">THE LEADER IN INTERACTIVE VR</h2>
                <P class=" leading-[1.8] text-[#696969]">Lorem ipsum dolor sit amet consectetur ci. Laborum consequuntur error, eveniet sunt mollitia accusantium similique saepe quia ipsa alias iusto totam! Unde.</P>
            </div>
        </div>
    </transition>
</template>

<script>
import gsap from 'gsap'
import ScrollTrigger from "gsap/ScrollTrigger";


gsap.registerPlugin(ScrollTrigger);

export default {
    setup () {

        const tl = gsap.timeline()

        const beforeEnter = (el) =>{
            el.style.transform = 'translateX(-1000px)'
            el.style.opacity = 0
        }

     
        const enter = (el, done)=>{

            tl.to(el, {
                duration:1,
                x:0,
                opacity:1,
                ease: "back.out(2)",
                delay: 2

            })

            tl.from(".vrImage", {
                scale:0,
                duration:1,
                ease: "back.out(2)",

            })

        }
        

        return {tl, enter,beforeEnter }
    }
}
</script>

<style lang="scss" scoped>

</style>