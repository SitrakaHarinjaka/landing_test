<template>
    <header id="header" class="absolute top-0 left-0 right-0 m-auto w-full">
      <div class="container">
         <div class="menu-social flex items-center justify-between mt-[45px]">
            <nav :class="{'menu': true, 'open': state}" class="md:w-1/3">
               <div class="close-btn w-10 fixed right-3 top-3" :class="{ 'hidden': !state }" @click="state = false">
                  <svg viewBox="0 0 24 24" fill="none" xmlns="http://www.w3.org/2000/svg" stroke="#2091f9"><g id="SVGRepo_bgCarrier" stroke-width="0"></g><g id="SVGRepo_tracerCarrier" stroke-linecap="round" stroke-linejoin="round"></g><g id="SVGRepo_iconCarrier"> <path d="M20.7457 3.32851C20.3552 2.93798 19.722 2.93798 19.3315 3.32851L12.0371 10.6229L4.74275 3.32851C4.35223 2.93798 3.71906 2.93798 3.32854 3.32851C2.93801 3.71903 2.93801 4.3522 3.32854 4.74272L10.6229 12.0371L3.32856 19.3314C2.93803 19.722 2.93803 20.3551 3.32856 20.7457C3.71908 21.1362 4.35225 21.1362 4.74277 20.7457L12.0371 13.4513L19.3315 20.7457C19.722 21.1362 20.3552 21.1362 20.7457 20.7457C21.1362 20.3551 21.1362 19.722 20.7457 19.3315L13.4513 12.0371L20.7457 4.74272C21.1362 4.3522 21.1362 3.71903 20.7457 3.32851Z" fill="#2091f9"></path> </g></svg>
               </div>
               <ul class="flex">
                  <li v-for="(menuItem, key) in menu" :key="key"  class="inline-block mr-[30px]">
                     <a :href="menuItem.link">{{ menuItem.label }}</a>
                  </li>
               </ul>
            </nav>
            <div class="logo flex items-center justify-between sm:justify-center md:w-1/3 w-full">
               <Logo class="w-[186px]"/>
               <button @click="state = true" id="show-menu-mobile" class="navigation-menu sm:hidden">
                  <svg width="28" height="16" viewBox="0 0 28 16" fill="none" xmlns="http://www.w3.org/2000/svg">
                    <path d="M0.667969 0H14.0013H27.3346V2.66667H0.667969V0ZM7.33463 6.66667H27.3346V9.33333H7.33463V6.66667ZM15.668 13.3333H27.3346V16H15.668V13.3333Z" fill="white"/>
                  </svg>
               </button>
            </div>
            <div class="social mr-[30px] md:w-1/3">
               <nav class="social" >
                  <ul class="flex justify-end">
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
  import Logo from '@/assets/img/logo.svg';
  

  let props = defineProps({
    menu: Array,
  });  

  let state = ref(false);

  watch(() => state.value, (newState: Boolean) => {
    if (newState) {
      document.body.classList.add('overflow-hidden');
    } else {
      document.body.classList.remove('overflow-hidden');
    }
  });
  
</script>
<style>

</style>