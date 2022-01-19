<template>
  <header class="header bg-center bg-cover relative overflow-hidden w-full aspect-[16/7.5]">
    <TrafficLight
      :redStatus="true"
      :yellowStatus="false"
      :greenStatus="false"
      leftPosition="30.5vw"
      topPosition="3.8vw"
      heightSize="22vw"
    />
    <TrafficLight
      :redStatus="true"
      :yellowStatus="false"
      :greenStatus="false"
      leftPosition="71vw"
      topPosition="6vw"
      heightSize="28vw"
    />
    <TheRedCar class="w-[23vw] absolute left-[-2vw] top-[20vw]" />
    <TheOrangeCar class="absolute w-[18vw] h-min left-[50vw] bottom-[0vw]" />
    <TheOldMan class="w-[14vw] absolute left-[14vw] top-[21vw]" />
  </header>
</template>
<script setup lang="ts">
import TrafficLight from "./TrafficLight.vue";
import TheRedCar from "./TheRedCar.vue";
import TheOrangeCar from "./TheOrangeCar.vue";
import TheOldMan from "./TheOldMan.vue";
</script>
<style>
.header {
  background-image: url("./../assets/img/bg.svg");
}
</style>
