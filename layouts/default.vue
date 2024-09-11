<template>
  <div>
    <PartialsHeader :state="state" :menu="menuItem"/>

    <slot  @showMenu="showMenu"/>

    <PartialsFooter/>
  </div>
</template>

<script lang="ts" setup>
  const state  = ref(false);
  const showMenu = () =>{
    state.value = true
  }
  const menuItem = ref([
    { label: "Home", link: "#home" },
    { label: "Product", link: "#product" },
    { label: "Pricing", link: "#pricing" },
    { label: "About", link: "#about" },
    { label: "Contact", link: "#contact" },
  ]);
</script>

<style>

</style>