<template>
  <section id="baneer" class="min-h-screen bg-[url('/assets/img/baneer.png')] bg-cover bg-no-repeat bg-[50%_100%] flex flex-col items-center justify-between py-[45px]">
    <div class="logo flex items-center justify-between w-full sm:justify-center">
       <Logo class="w-[186px]"/>
       <button @click="$emit('addClassMenu')" id="show-menu-mobile" class="navigation-menu sm:hidden">
          <svg width="28" height="16" viewBox="0 0 28 16" fill="none" xmlns="http://www.w3.org/2000/svg">
            <path d="M0.667969 0H14.0013H27.3346V2.66667H0.667969V0ZM7.33463 6.66667H27.3346V9.33333H7.33463V6.66667ZM15.668 13.3333H27.3346V16H15.668V13.3333Z" fill="white"/>
          </svg>
       </button>
    </div>
    <div class="title-baneer flex flex-col items-center max-w-[826px] mb-[185px]">
       <h2 class="text-lightText text-[74px] leading-[84px] tracking-[0.2px] text-center font-bold  mb-[27px] mt-16">
         The best products<br> start with Figma</h2>
       <p class="text-lightText text-center text-[28px] leading-[40px] tracking-[0.2px] font-normal mb-[90px]">Most calendars are designed for teams. Slate is designed for freelancers</p>
       <a class="button-primary" href="#">Try for free</a>
    </div>
 </section>
</template>

<script lang="ts" setup>
  import Logo from '@/assets/img/logo.svg';
</script>

<style>

</style>