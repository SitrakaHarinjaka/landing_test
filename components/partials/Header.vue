<template>
    <header id="header" class="absolute top-0 left-0 right-0 m-auto w-full">
      <div class="container">
         <div class="menu-social flex items-center justify-between mt-[45px]">
            <nav :class="{'menu': true, 'open': state}">
               <ul>
                  <li v-for="(menuItem, key) in menu" :key="key"  class="inline-block mr-[40px]">
                     <a :href="menuItem.link">{{ menuItem.label }}</a>
                  </li>
               </ul>
            </nav>
            <div class="social mr-[30px]">
               <nav class="social" >
                  <ul>
                     <li class="inline-block mr-[30px]">
                        <a href="#">
                           <TwitterIcon/>
                        </a>
                     </li>
                     <li class="inline-block mr-[30px]">
                        <a href="#">
                           <FacebookIcon/>
                        </a>
                     </li>
                     <li class="inline-block mr-[30px]">
                        <a href="#">
                           <LinkedInIcon/>
                        </a>
                     </li>
                  </ul>
               </nav>
            </div>
         </div>
      </div>
   </header>
</template>

<script lang="ts" setup>
  import FacebookIcon from '@/assets/svg/FacebookIcon.svg'
  import TwitterIcon from '@/assets/svg/TwitterIcon.svg'
  import LinkedInIcon from '@/assets/svg/LinkedInIcon.svg'

  defineProps({
    menu: Array,
    state: Boolean
  });   
  
  onMounted(() => {
    console.log('called');
   
  });
  
</script>
<style>

</style>