<template>
    <section class="p-12 mx-auto my-0 max-w-[1400px]">
        <div class="flex justify-between items-center">
            <h2>OUR CREATIONS</h2>
            <button>SEE ALL</button>
        </div>
        <div class="flex-gallery mt-8">
            <div class="bg-[url('../assets/images/desktop/image-deep-earth.jpg')]"><h2 class=" ">Deep Earth</h2></div>
            <div class="bg-[url('../assets/images/desktop/image-night-arcade.jpg')]"><h2 class=" ">Night Arcade</h2></div>
            <div class="bg-[url('../assets/images/desktop/image-soccer-team.jpg')]"><h2 class=" ">Soccer Team VR</h2></div>
            <div class="bg-[url('../assets/images/desktop/image-grid.jpg')]"><h2 class=" ">The Grid</h2></div>
            <div class="bg-[url('../assets/images/desktop/image-from-above.jpg')]"><h2 class=" ">From Up Above VR</h2></div>
            <div class="bg-[url('../assets/images/desktop/image-pocket-borealis.jpg')]"><h2 class=" ">Pocket Borealis</h2></div>
            <div class="bg-[url('../assets/images/desktop/image-curiosity.jpg')]"><h2 class=" ">The Curiosity</h2></div>
            <div class="bg-[url('../assets/images/desktop/image-fisheye.jpg')]"><h2 class=" ">Make it Fisheye</h2></div>
        </div>
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

.flex-gallery{
    display: grid;
    grid-template-columns: repeat(4, 1fr);
    grid-template-rows: repeat(2, 1fr);
    gap: 1rem;
    color: #fff;

    div{
        height: 480px;
        background-size: cover;
        background-position: center;
        position: relative;

        h2{
            font-size: 3rem;
            padding-left: 2rem;
            line-height: 1;
            font-weight: lighter;
            position: absolute;
            bottom: 2rem;
            text-transform: uppercase;
        }
    }
}

</style>