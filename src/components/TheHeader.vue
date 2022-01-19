<template>
  <header class="header bg-center bg-cover relative overflow-hidden w-full aspect-[16/7.5]">
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
    <TheRedCar class="w-[23vw] absolute left-[-3vw] top-[22vw]" />
    <TheOrangeCar class="absolute w-[18vw] h-min left-[50vw] bottom-[0vw]" />
  </header>
</template>
<script setup lang="ts">
import TrafficLight from "./TrafficLight.vue";
import TheRedCar from "./TheRedCar.vue";
import TheOrangeCar from "./TheOrangeCar.vue";
</script>
<style>
.header {
  background-image: url("./../assets/img/bg.svg");
}
</style>
