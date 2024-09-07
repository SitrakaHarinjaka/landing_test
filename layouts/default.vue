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
    { label: "product", link: "#home" },
    { label: "pricing", link: "#home" },
    { label: "About", link: "#home" },
    { label: "Contact", link: "#home" },
  ]);
</script>

<style>

</style>