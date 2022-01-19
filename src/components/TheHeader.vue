<template>
  <header class="header bg-center bg-cover h-[50vw]">
    <TrafficLight/>
  </header>
</template>
<script setup lang="ts">
import TrafficLight from './TrafficLight.vue';
</script>
<style>
.header {
  background-image: url("./../assets/img/bg.svg");
}
</style>
