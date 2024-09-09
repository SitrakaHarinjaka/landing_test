<template>
  <section id="pricing" class="bg-titleSection py-[140px]">
    <div class="title-section text-center">
       <h3 class="text-lightText">Pricing</h3>
       <p class="text-lightText">Most calendars are designed for teams. Slate is designed for freelancers</p>
    </div>
    <div class="container">
       <div class="list-pricing flex items-center justify-between mt-20">
          <PartialsPricingCard v-for="(pricing, key) in pricings" :key="key" :data="pricing"/>
       </div>
    </div>
 </section>
</template>

<script lang="ts" setup>
  const pricings = [
    {
      name: 'Free',
      desc: 'Organize across all apps by hand',
      price: '0',
      template: 'white',
      feats: [
        { desc: 'Pricing Feature' },
        { desc: 'Pricing Feature' },
        { desc: 'Pricing Feature' },
        { desc: 'Pricing Feature' },
        { desc: 'Pricing Feature' },
      ]
    },
    {
      name: 'Standard',
      desc: 'Organize across all apps by hand',
      price: '10',
      template: 'blue',
      feats: [
        { desc: 'Pricing Feature' },
        { desc: 'Pricing Feature' },
        { desc: 'Pricing Feature' },
        { desc: 'Pricing Feature' },
        { desc: 'Pricing Feature' },
      ]
    },
    {
      name: 'Buisness',
      desc: 'Organize across all apps by hand',
      price: '99',
      template: 'white',
      feats: [
        { desc: 'Pricing Feature' },
        { desc: 'Pricing Feature' },
        { desc: 'Pricing Feature' },
        { desc: 'Pricing Feature' },
        { desc: 'Pricing Feature' },
      ]
    }
  ]
</script>

<style>

</style>