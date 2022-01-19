<template>
  <header class="header bg-center bg-cover h-[50vw] relative overflow-hidden">
    <TrafficLight
      :redStatus="true"
      :yellowStatus="false"
      :greenStatus="false"
      leftPosition="30vw"
      topPosition="5.4vw"
      heightSize="22vw"
    />
    <TrafficLight
      :redStatus="true"
      :yellowStatus="false"
      :greenStatus="false"
      leftPosition="71vw"
      topPosition="4vw"
      heightSize="32vw"
    />
  </header>
</template>
<script setup lang="ts">
import TrafficLight from "./TrafficLight.vue";
</script>
<style>
.header {
  background-image: url("./../assets/img/bg.svg");
}
</style>
