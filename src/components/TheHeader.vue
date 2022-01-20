<template>
  <header
    class="header bg-center bg-cover relative overflow-hidden w-full aspect-[16/7.5]"
  >
    <TrafficLight
      :redStatus="true"
      :yellowStatus="true"
      :greenStatus="true"
      leftPosition="30.5vw"
      topPosition="3.8vw"
      heightSize="22vw"
      zIndex="0"
    />
    <TrafficLight
      :redStatus="true"
      :yellowStatus="true"
      :greenStatus="true"
      leftPosition="71vw"
      topPosition="6vw"
      heightSize="28vw"
      zIndex="5"
    />
    <TheRedCar
      leftPosition="-2vw"
      topPosition="20vw"
      heightSize="11vw"
      zIndex="4"
      class="left-right"
    />
    <TheOrangeCar
      leftPosition="54vw"
      topPosition="30vw"
      heightSize="18vw"
      zIndex="7"
      class="scale-out-top"
    />
    <TheOldMan
      leftPosition="19vw"
      topPosition="23vw"
      heightSize="14vw"
      zIndex="6"
      class="left-rightf"
    />
    <ThePoliceman
      leftPosition="46.2vw"
      topPosition="8.2vw"
      heightSize="22vw"
      zIndex="3"
    />
    <TheVan
      leftPosition="74vw"
      topPosition="10vw"
      heightSize="18vw"
      zIndex="1"
      class="right-left"
    />
    <TheGreenCar
      leftPosition="86vw"
      topPosition="19vw"
      heightSize="10vw"
      zIndex="2"
      class="right-left"
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
.left-right {
  animation: left-keyframes 16s linear infinite both;
}
@keyframes left-keyframes {
  0% {
    left: -100vw;
  }
  100% {
    left: 100vw;
  }
}
.right-left {
  animation: right-keyframes 16s linear infinite both;
}
@keyframes right-keyframes {
  0% {
    left: 100vw;
  }
  100% {
    left: -100vw;
  }
}

.scale-out-top {
  animation: scale-out-top 6s linear infinite both;
}
@keyframes scale-out-top {
  0% {
    transform: scale(1);
    top: 33vw;
    left: 54vw;
    opacity: 1;
  }
  40%{
    z-index: 0;
  }
  87% {
    opacity: 0.9;
  }
  90% {
    opacity: 0;
  }
  100% {
    transform: scale(0.2);
    top: 3vw;
    left: 44vw;
    opacity: 0;
    z-index: 0;
  }
}
</style>
