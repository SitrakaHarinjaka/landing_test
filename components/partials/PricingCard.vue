<template>
  <div :id="`${data.template}-template`" :class="`item ${data.name.toLowerCase()} p-[43px] px-[40px] box-border shadow-[0_13px_19px_rgba(0,0,0,0.07)] rounded-[10px] text-center w-[30%]`">
    <h4 class="text-[20px] leading-[28px] tracking-[0.1px] uppercase font-bold my-4">{{ data.name }}</h4>
    <p class="font-normal text-[16px] leading-[23px] text-center tracking-[0.1px] my-4">{{ data.desc }}</p>
    <div class="price flex items-center justify-center">
       <span class="font-bold text-[74px] leading-[84px] tracking-[0.2px]">{{ data.price }}</span>
       <div class="payment ml-[10px] text-left">
          <div class="curr text-[20px] leading-[28px] tracking-[0.1px] font-bold">$</div>
          <div class="recursive font-normal text-[16px] leading-[23px] tracking-[0.1px]">Per Month</div>
       </div>
    </div>
    <div class="feature mb-10">
        <p v-for="(feat, key) in data.feats" :key="key" class="my-4">{{ feat.desc }}</p>
    </div>
    <div class="cta">
       <a href="#" class="button-primary px-0 w-full">Order now</a>
    </div>
 </div>
</template>

<script lang="ts" setup>
defineProps({
  data: {
      name: String,
      desc: String,
      price: String,
      template: String,
      feats: Array
    }
})
</script>
  
<style>

</style>