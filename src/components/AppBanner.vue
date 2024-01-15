<script setup>
    import BlurBg from '@/assets/bg_blur.png';
</script>
<template>
    <div :style="{ backgroundImage: `url(${BlurBg})`}" class="min-h-[325px] bg-cover bg-center bg-no-repeat flex flex-col justify-center px-[17px] lg:px-[100px] white-text">
        <div class="container mx-auto">
            <div class="flex flex-row flex-nowrap gap-x-3 mb-6">
            <img src="@/assets/Home.png" alt="">
            <span class="text-lg">/</span>
            <span class="text-lg">Contact</span>
        </div>
        <h1 class="text-[40px] mb-4">Contact</h1>
        <p class="text-base">Heb je nog vragen of wil je gewoon even kletsen over voetbal? Neem contact op via een van de onderstaande opties en we staan je graag te woord. Ook ben je tijdens kantooruren van harte welkom bij ons op kantoor in Maarssen!</p>
        </div>
    </div>
</template>