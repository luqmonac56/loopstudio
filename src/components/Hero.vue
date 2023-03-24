<template>
    <div class="hero relative h-[80vh] text-white py-12 px-12 md">
        <nav class=" flex justify-between" >
            <img src="../assets/images/logo.svg" alt="Logo">
            <ul class="flex gap-6  ">
                <li>Home</li>
                <li>Home</li>
                <li>Home</li>
                <li>Home</li>
                <li>Home</li>
            </ul>
        </nav>
        <div class=" absolute top-[40%] md:max-w-[50%] lg:max-w-[40%]">
            <h1 class=" text-3xl lg:text-5xl">IMMERSIVE EXPERIENCES THAT DELIVER</h1>
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
    background: url(../assets/images/desktop/image-hero.jpg);
    background-size: cover;
    background-repeat: no-repeat;


    div{
        border: 1.5px solid #fff;
        width: fit-content;
        padding: 2rem;
    }
}
</style>