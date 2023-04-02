<template>
    <div class="hero relative h-[80vh] text-white py-12 md:px-12 px-4">
        <nav class=" flex justify-between" >
            <img src="../assets/images/logo.svg" alt="Logo">
            <!-- <ul class="flex gap-6  ">
                <li>Home</li>
                <li>Home</li>
                <li>Home</li>
                <li>Home</li>
                <li>Home</li>
            </ul> -->
        </nav>
        <div class=" px-4 py-12 md:p-12 md:absolute relative top-[30%] md:top-[40%] w-full md:max-w-[50%] lg:max-w-[40%]">
            <h1 class=" text-[2.2rem] lg:text-5xl">IMMERSIVE EXPERIENCES THAT DELIVER</h1>
        </div>
    </div>
</template>

<script>
export default {
    setup () {
        

        return {}
    }
}
</script>

<style lang="scss" scoped>

.hero{
    background: #0000006b url(../assets/images/desktop/image-hero.jpg);
    background-size: cover;
    background-repeat: no-repeat;
    background-blend-mode: multiply;


    div{
        border: 1.5px solid #fff;
        width: fit-content;
        //padding: 2rem;
    }
}
</style>