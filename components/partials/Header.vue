<template>
  <div>
    <header id="header" class="absolute top-0 left-0 right-0 m-auto w-full">
      <div class="container">
         <div class="menu-social flex items-center justify-between mt-[45px]">
            <nav class="menu">
               <ul>
                  <li v-for="(menuItem, key) in menu" :key="key"  class="inline-block mr-[40px]">
                     <a :href="menuItem.link">{{ menuItem.label }}</a>
                  </li>
               </ul>
            </nav>
            <div class="social mr-[30px]">
               <nav class="social">
                  <ul>
                     <li>
                        <a href="#">
                           <TwitterIcon/>
                        </a>
                     </li>
                     <li>
                        <a href="#">
                           <FacebookIcon/>
                        </a>
                     </li>
                     <li>
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
   <div id="show-menu-mobile" class="navigation-menu">
      <div class="bar"></div>
      <div class="bar"></div>
      <div class="bar"></div>
   </div>
  </div>
</template>

<script lang="ts" setup>
  import FacebookIcon from '@/assets/svg/FacebookIcon.svg'
  import TwitterIcon from '@/assets/svg/TwitterIcon.svg'
  import LinkedInIcon from '@/assets/svg/LinkedInIcon.svg'

  // import $ from 'jquery';

  defineProps({
    menu: Array
  });   
 
  onMounted(() => {
    console.log('called');
    /* $('#show-menu-mobile').on('click', function(){
        $(this).toggleClass('show'); 
        $('#header').toggleClass('show');
        if($(this).hasClass('show')){
          $('body').css('overflow','hidden')
        }else{
          $('body').css('overflow','auto')
        }
    }) */
  });
</script>
<style>

</style>