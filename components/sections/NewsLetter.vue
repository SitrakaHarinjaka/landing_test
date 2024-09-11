<template>
  <section id="newsletter">
    <div class="container">
       <div class="newsletter-content flex justify-between">
          <div class="image">
            <LightDrawIcon/>
          </div>
          <div class="description">
             <h4 class="mb-[17px] font-bold">At your fingertips</h4>
             <h3 class="text-[48px] tracking-[0.1px] leading-[55px] text-titleSection mb-9 mt-0">Lightning fast <br>
                prototyping </h3>
             <div class="action-content">
                <h4 class="subscribe tracking-[1px] font-bold mb-0 leading-7 text-titleSection text-[20px]">Subscribe to our Newsletter</h4>
                <p class="font-sans text-[18px] leading-[25px] tracking-[0.2px] text-secondText mt-0 mb-9">Available exclusivery on Figmaland</p>
                <form class="form">
                   <input type="text" class="input-text mr-[12px]" placeholder="Your Email"/>
                   <button class="button-primary" type="submit">Subscribe</button>
                </form>
             </div>
          </div>
       </div>
    </div>
 </section>
</template>

<script lang="ts" setup>
  import LightDrawIcon from '@/assets/img/light-draw.svg'

</script>

<style>

</style>