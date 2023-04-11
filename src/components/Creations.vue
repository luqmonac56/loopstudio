<template>
    <section class="md:p-12 p-4 mx-auto my-0 max-w-[1400px]">
        <div class=" md:flex justify-between items-center">
            <h2 class="text-center text-4xl">OUR CREATIONS</h2>
            <button  class="md:block hidden">SEE ALL</button>
        </div>
        <div class="flex-gallery  grid-cols-1 md:grid-cols-2 lg:grid-cols-4 mt-8 mb-8">
            <div class=" bg-[url('../assets/images/mobile/image-deep-earth.jpg')] md:bg-[url('../assets/images/desktop/image-deep-earth.jpg')]"><h2 class=" md:text-[2rem] w-[50%] text-[2rem] lg:text-[2.5rem]">Deep Earth</h2></div>
            <div class="bg-[url('../assets/images/mobile/image-night-arcade.jpg')] md:bg-[url('../assets/images/desktop/image-night-arcade.jpg')]"><h2 class=" w-[55%] text-[2rem]  md:text-[2rem] lg:text-[2.5rem] ">Night Arcade</h2></div>
            <div class="bg-[url('../assets/images/mobile/image-soccer-team.jpg')] md:bg-[url('../assets/images/desktop/image-soccer-team.jpg')]"><h2 class=" w-[55%] text-[2rem] md:text-[2rem] lg:text-[2.5rem] ">Soccer Team VR</h2></div>
            <div class=" bg-[url('../assets/images/mobile/image-grid.jpg')] md:bg-[url('../assets/images/desktop/image-grid.jpg')]"><h2 class=" w-[40%] text-[2rem]  md:text-[2rem] lg:text-[2.5rem]">The Grid</h2></div>
            <div class=" bg-[url('../assets/images/mobile/image-from-above.jpg')] md:bg-[url('../assets/images/desktop/image-from-above.jpg')]"><h2 class=" w-[55%] text-[2rem]  md:text-[2rem] lg:text-[2.5rem]">From Up Above VR</h2></div>
            <div class=" bg-[url('../assets/images/mobile/image-pocket-borealis.jpg')] md:bg-[url('../assets/images/desktop/image-pocket-borealis.jpg')]"><h2 class=" w-[55%] text-[2rem]  md:text-[2rem] lg:text-[2.5rem]">Pocket Borealis</h2></div>
            <div class=" bg-[url('../assets/images/mobile/image-curiosity.jpg')] md:bg-[url('../assets/images/desktop/image-curiosity.jpg')]"><h2 class=" w-[55%] text-[2rem]  md:text-[2rem] lg:text-[2.5rem]">The Curiosity</h2></div>
            <div class=" bg-[url('../assets/images/mobile/image-fisheye.jpg')] md:bg-[url('../assets/images/desktop/image-fisheye.jpg')]"><h2 class=" w-[55%] text-[2rem]  md:text-[2rem] lg:text-[2.5rem]">Make it Fisheye</h2></div>
        </div>
        <button  class="block md:hidden my-0 mx-auto">SEE ALL</button>
    </section>
</template>

<script>
export default {
    setup () {
        

        return {}
    }
}
</script>

<style lang="scss" scoped>
button{
    border: 1px solid black;
    padding: .5rem 2.5rem;
    border-radius: 2px;

    &:hover{
        background: #000;
        color: #fff;
        transition: all .3s ease-in-out;

    }
}

.flex-gallery{
    display: grid;
    gap: 1rem;
    color: #fff;

    div{
        height: 150px;
        background-repeat: no-repeat;
        background-size: cover ;
        background-position: center;
        position: relative;

        h2{
            //font-size: 3rem;
            padding-left: 2rem;
            line-height: 1;
            font-weight: lighter;
            position: absolute;
            bottom: 1rem;
            text-transform: uppercase;
            text-shadow: 0px 0px 5px rgba(0, 0, 0, 0.6);
            
        }
    }
}

@media screen and (min-width: 768px) {


    .flex-gallery{
        div{
            height: 480px ;
    
            h2{
                bottom: 2rem;
                
            }
        }
    }
}

</style>