<template>
  <section id="partner" class="my-[180px]">
    <div class="title-section text-center">
       <h3>Partners</h3>
       <p class="mt-7">Most calendars are designed for teams. Slate is designed for freelancers</p>
    </div>
    <div class="container">
       <div class="partners-list flex flex-wrap mt-[80px]">
        <div class="item p-7 border border-[#d8d8d8] w-1/4 text-center flex flex-col" v-for="(partner, key) in partners" :key="key">
            <span class="text-base leading-6 tracking-[0.1px] text-[#374754] mb-4 inline-block font-normal">{{ partner.name }}</span>
            <div class="px-10 h-50px">
              <img :src="partner.img" alt="" class="w-full h-auto"/>
            </div>
        </div>
       </div>
       <div class="text-center mt-20">
          <a class="button-primary" href="#">Try For Free</a>
       </div>
    </div>
 </section>
</template>

<script lang="ts" setup>

const partners = [
  {
    name: 'Client Name',
    img: '/clients/google.png'
  },
  {
    name: 'Client Name',
    img: '/clients/amazon.png'
  },
  {
    name: 'Client Name',
    img: '/clients/microsoft.png'
  },
  {
    name: 'Client Name',
    img: '/clients/uber.png'
  },
  {
    name: 'Client Name',
    img: '/clients/dropbox.png'
  },
  {
    name: 'Client Name',
    img: '/clients/google.png'
  },
  {
    name: 'Client Name',
    img: '/clients/uber.png'
  },
  {
    name: 'Client Name',
    img: '/clients/amazon.png'
  },
]

</script>

<style>

</style>