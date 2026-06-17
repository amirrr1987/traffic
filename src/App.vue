<template>
  <div
    ref="headerRef"
    class="header bg-center bg-cover relative overflow-hidden w-full aspect-16/7.5 h-screen"
  >
    <TrafficLight
      :redStatus="redStatus"
      :yellowStatus="yellowStatus"
      :greenStatus="greenStatus"
      leftPosition="30.5vw"
      topPosition="3.8vw"
      heightSize="22vw"
      zIndex="0"
    />
    <TrafficLight
      :redStatus="redStatus"
      :yellowStatus="yellowStatus"
      :greenStatus="greenStatus"
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
      class="orange-car-anim"
    />
    <TheOldMan
      leftPosition="19vw"
      topPosition="23vw"
      heightSize="14vw"
      zIndex="6"
      class="old-man-anim"
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
  </div>
</template>
<script setup lang="ts">
import TrafficLight from "@/components/TrafficLight.vue";
import TheRedCar from "@/components/TheRedCar.vue";
import TheOrangeCar from "@/components/TheOrangeCar.vue";
import TheOldMan from "@/components/TheOldMan.vue";
import ThePoliceman from "@/components/ThePolice.vue";
import TheVan from "@/components/TheVan.vue";
import TheGreenCar from "@/components/TheGreenCar.vue";


import { onMounted, onUnmounted, ref } from "vue";
import { gsap } from "gsap";

const headerRef = ref<HTMLElement | null>(null);
let ctx: gsap.Context | undefined;

const redStatus = ref(false);
const yellowStatus = ref(false);
const greenStatus = ref(true);

const CYCLE_DURATION = 30;
const GREEN_END = 8;
const YELLOW_END = 9;
const RED_END = 22;
const ORANGE_CAR_START = 22;

function setLights(green: boolean, yellow: boolean, red: boolean) {
  greenStatus.value = green;
  yellowStatus.value = yellow;
  redStatus.value = red;
}

function initAnimations() {
  if (!headerRef.value) return;
  if (window.matchMedia("(prefers-reduced-motion: reduce)").matches) return;

  ctx = gsap.context(() => {
    gsap
      .timeline({ repeat: -1 })
      .set(".left-right", { left: "-20vw" })
      .to(".left-right", { left: "-2vw", duration: 6, ease: "none" })
      .to(".left-right", { left: "-2vw", duration: 3, ease: "none" })
      .to(".left-right", { left: "100vw", duration: 6, ease: "none" })
      .to(".left-right", { left: "100vw", duration: 15, ease: "none" });

    gsap
      .timeline({ repeat: -1 })
      .set(".right-left", { left: "100vw" })
      .to(".right-left", { left: "75vw", duration: 6, ease: "none" })
      .to(".right-left", { left: "75vw", duration: 3, ease: "none" })
      .to(".right-left", { left: "50vw", duration: 6, ease: "none" })
      .to(".right-left", { left: "-100vw", duration: 15, ease: "none" });

    gsap
      .timeline({ repeat: -1 })
      .set(".old-man-anim", { left: "-20vw" })
      .to(".old-man-anim", { left: "20vw", duration: 6, ease: "none" })
      .to(".old-man-anim", { left: "20vw", duration: 3, ease: "none" })
      .to(".old-man-anim", { left: "100vw", duration: 12, ease: "none" })
      .to(".old-man-anim", { left: "100vw", duration: 9, ease: "none" });

    const master = gsap.timeline({ repeat: -1, repeatDelay: 0 });

    master.set(".orange-car-anim", {
      scale: 1,
      top: "30vw",
      left: "54vw",
      opacity: 1,
      zIndex: 7,
    });

    master.call(() => setLights(true, false, false), undefined, 0);
    master.call(() => setLights(false, true, false), undefined, GREEN_END);
    master.call(() => setLights(false, false, true), undefined, YELLOW_END);
    master.call(() => setLights(true, false, false), undefined, RED_END);

    // پیرمرد تا ثانیه ۲۱ از عرض خیابان رد می‌شود؛ ماشین نارنجی با سبز شدن چراغ (۲۲) حرکت می‌کند
    master.to(".orange-car-anim", { zIndex: 0, duration: 2.4, ease: "none" }, ORANGE_CAR_START);
    master.to(
      ".orange-car-anim",
      {
        scale: 0.2,
        top: "3vw",
        left: "44vw",
        opacity: 0,
        zIndex: 0,
        duration: 3.6,
        ease: "none",
        keyframes: [
          { opacity: 0.9, duration: 2.22 },
          { opacity: 0, duration: 0.18 },
        ],
      },
      ORANGE_CAR_START + 2.4,
    );

    master.duration(CYCLE_DURATION);
  }, headerRef.value);
}

onMounted(() => {
  initAnimations();
});

onUnmounted(() => {
  ctx?.revert();
});



</script>
<style>
.header {
  background-image: url("@/assets/img/bg.svg");
}
</style>
