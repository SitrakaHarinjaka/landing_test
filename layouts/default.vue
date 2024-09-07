<template>
  <div>
    <PartialsHeader :menu="menuItem"/>

    <slot />

    <footer>
      <h1>Footer</h1>
    </footer>
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
</script>

<style>

</style>