<template>
  <section id="feature" class="mt-[115px]">
    <div class="container">
       <div class="title-section text-center">
          <h3 class="text-titleSection">Feature</h3>
          <p class="text-secondText">Most calendars are designed for teams. Slate is designed for freelancers</p>
       </div>
       <div class="feature-item flex justify-center mt-[80px] mb-[132px]">
          <div class="item text-center max-w-[255px] my-0 mx-[24px] flex flex-col items-center">
            <div class="w-[46px]">
              <FontIcon/>
            </div>
             <h4 class="text-[20px] leading-[28px] text-center tracking-[0.1px] text-titleSection font-bold mb-[20px] my-6">OpenType features Variable fonts</h4>
             <p class="text-[18px] leading-[25px] text-center tracking-[0.2px] font-normal my-4">Slate helps you see how many more days you need to work to reach your financial goal.</p>
          </div>
          <div class="item text-center max-w-[255px] my-0 mx-[24px] flex flex-col items-center">
              <div class="w-[46px]">
                <DesignIcon/>
              </div>
             <h4 class="text-[20px] leading-[28px] text-center tracking-[0.1px] text-titleSection font-bold mb-[20px] my-6">Design with real data</h4>
             <p class="text-[18px] leading-[25px] text-center tracking-[0.2px] font-normal my-4">Slate helps you see how many more days you need to work to reach your financial goal.</p>
          </div>
          <div class="item text-center max-w-[255px] my-0 mx-[24px] flex flex-col items-center">
            <div class="w-[46px]">
              <ActionIcon/>
            </div>
             <h4 class="text-[20px] leading-[28px] text-center tracking-[0.1px] text-titleSection font-bold mb-[20px] my-6">Fastest way to take action</h4>
             <p class="text-[18px] leading-[25px] text-center tracking-[0.2px] font-normal my-4">Slate helps you see how many more days you need to work to reach your financial goal.</p>
          </div>
       </div>
       <div class="video relative shadow-[0_8px_63px_rgba(0,_0,_0,_0.3)] rounded-[44.8123px] overflow-hidden">
          <div class="image-back w-full h-full absolute top-0 left-0" :style="{ opacity: isPlaying ? '0' : '1' }">
             <img src="~/assets/img/back-video.png" alt="" class="w-full h-full object-cover">
          </div>
          <div class="play-video absolute inset-0 h-max w-max m-auto z-[100]">
             <button id="play" class="bg-none border-none cursor-pointer" @click="playVideo" :style="{ opacity: isPlaying ? '0' : '1' }">
                <svg width="188" height="188" viewBox="0 0 188 188" fill="none" xmlns="http://www.w3.org/2000/svg">
                   <circle cx="93.8274" cy="94.0001" r="93.6985" fill="#2091F9" />
                   <g clip-path="url(#clip0_117_33)">
                      <path d="M79.4023 71.594L118.443 95.0186L79.4023 118.443V71.594Z" fill="white" />
                   </g>
                   <defs>
                      <clipPath id="clip0_117_33">
                         <rect width="46.8492" height="46.8492" fill="white" transform="translate(75.4961 71.594)" />
                      </clipPath>
                   </defs>
                </svg>                  
             </button>
          </div>
          <video class="video-play aspect-video	 w-full object-cover" ref="videoRef">
             <source src="/videos/video.mp4" type="video/mp4">
          </video>
       </div>
    </div>
 </section>
</template>

<script lang="ts" setup>
  import FontIcon from '@/assets/img/fonts.svg'
  import DesignIcon from '@/assets/img/design.svg'
  import ActionIcon from '@/assets/img/action.svg'

   const videoRef = ref(null);
   const isPlaying = ref(false);

  const playVideo = () => {
   const video = videoRef.value;
      if (video.paused) {
        isPlaying.value = true;
        video.play();
      } else {
        isPlaying.value = false;
        video.pause();
      }
  }
</script>

<style>

</style>