<template>
  <div>
    <PartialsHeader :state="state" :menu="menuItem"/>

    <slot/>

    <PartialsFooter/>
  </div>
</template>

<script lang="ts" setup>
  const menuItem = ref([
    { label: "Home", link: "#home" },
    { label: "Product", link: "#product" },
    { label: "Pricing", link: "#pricing" },
    { label: "About", link: "#about" },
    { label: "Contact", link: "#contact" },
  ]);
  let state  = ref(false);
</script>

<style>

</style>