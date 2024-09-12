<template>
  <div>
    <PartialsHeader :state="state" :menu="menuItem"/>
    <SectionsBaneer @addClassMenu="showMenu"/>

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
  const state  = ref(false);
  const showMenu = () => state.value = true
</script>

<style>

</style>