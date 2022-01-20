<template>
  <header
    class="header bg-center bg-cover relative overflow-hidden w-full aspect-[16/7.5]"
  >
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
    <TheRedCar
      leftPosition="-2vw"
      topPosition="20vw"
      heightSize="11vw"
      zIndex="0"
    />
    <TheOrangeCar
      leftPosition="54vw"
      topPosition="30vw"
      heightSize="18vw"
      zIndex="0"
    />
    <TheOldMan
      leftPosition="19vw"
      topPosition="23vw"
      heightSize="14vw"
      zIndex="0"
    />
    <ThePoliceman leftPosition="46.2vw" topPosition="8.2vw" heightSize="22vw" />
    <TheVan
      leftPosition="74vw"
      topPosition="10vw"
      heightSize="18vw"
      zIndex="0"
    />
    <TheGreenCar
      leftPosition="86vw"
      topPosition="19vw"
      heightSize="10vw"
      zIndex="0"
    />
  </header>
</template>
<script setup lang="ts">
import TrafficLight from "./TrafficLight.vue";
import TheRedCar from "./TheRedCar.vue";
import TheOrangeCar from "./TheOrangeCar.vue";
import TheOldMan from "./TheOldMan.vue";
import ThePoliceman from "./ThePolice.vue";
import TheVan from "./TheVan.vue";
import TheGreenCar from "./TheGreenCar.vue";
</script>
<style>
.header {
  background-image: url("./../assets/img/bg.svg");
}
</style>
