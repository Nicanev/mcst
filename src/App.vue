<template>
  <div class="wrapper">
    <TheHeader />
    <router-view />
    <TheFooter />
  </div>
</template>

<script setup>
import TheFooter from "./components/TheFooter.vue";
import TheHeader from "./components/TheHeader.vue";
</script>

<style lang="scss"></style>
