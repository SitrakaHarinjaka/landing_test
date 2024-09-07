<template>
  <section id="baneer" class="min-h-screen bg-[url('/assets/img/baneer.png')] bg-cover bg-no-repeat bg-[50%_100%] flex flex-col items-center justify-between py-[45px] sm:min-h-[calc(100vh_-_97px)]">
    <div class="logo w-[186px] lg:mt-[70px] md:mt-0 md:ml-[15px] md:self-baseline">
       <Logo/>
    </div>
    <div class="title-baneer flex flex-col items-center max-w-[826px] mb-[185px] md:max-w-[90%] md:mx-auto">
       <h2 class="text-lightText text-[74px] leading-[84px] tracking-[0.2px] text-center font-bold mb-[27px] md:text-[30px] md:leading-[39px]">
         The best products<br> start with Figma</h2>
       <p class="text-lightText text-center text-[28px] leading-[40px] tracking-[0.2px] font-normal mb-[90px]">Most calendars are designed for teams. Slate is designed for freelancers</p>
       <a class="button-primary" href="#">Try for free</a>
    </div>
 </section>
</template>

<script lang="ts" setup>
  import Logo from '@/assets/img/logo.svg'
</script>

<style>

</style>