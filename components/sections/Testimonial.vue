<template>
  <section id="testimonials" class="mb-[100px] flex flex-col items-center">
    <div class="title-section">
        <h3 class="text-titleSection">Testimonials</h3>         
    </div>
    <div class="testimonial-content  flex flex-col items-center">
        <div class="w-[150px] h-auto mb-[60px]">
          <IbmLogo/>
        </div>
        <p class="text-[28px] leading-[40px] tracking-[0.2px] font-graphik-regular text-secondText max-w-[987px] mx-auto text-center">Most calendars are designed for teams. Slate is designed for freelancers 
          who want a simple way to plan their schedule.</p>
        <div class="author flex items-center justify-center mt-16">
          <div class="auth-img overflow-hidden w-[50px] h-[50px] rounded-full">
              <img src="~/assets/img/profil.jpeg" alt="" class="w-[50px] h-auto">
          </div>
          <div class="role ml-3 text-left">
              <div class="org text-secondText text-[16px] leading-[23px] font-graphik-bold">Organize accross</div>
              <div class="post text-secondText text-[15px] leading-[28px] font-graphik-regular">UI designer</div>
          </div>
        </div>
        <div class="cta mt-20">
          <a href="#" class="button-primary">More testimonials</a>
        </div>
    </div>
  </section>
</template>

<script lang="ts" setup>
import IbmLogo from '~/assets/img/ibm.svg'
</script>

<style>

</style>