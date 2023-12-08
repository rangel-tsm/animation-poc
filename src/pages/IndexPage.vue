<template>
  <q-page class="flex row justify-around">
    <q-card class="q-px-md" style="height: fit-content;">
      <q-card-section class="row q-gutter-md">
        <p>Bounce and slide</p>
        <q-btn flat fab icon="refresh" @click="playAgain(0)"/>
      </q-card-section>
      <q-card-section class="flex row">
        <h3 class="test">AV</h3><h3 class="test-o">Ō</h3><h3 class="test">Q</h3>
      </q-card-section>
    </q-card>
    <q-card class="q-px-md" style="height: fit-content;">
      <q-card-section class="row q-gutter-md">
        <p>All Bounce</p>
        <q-btn flat fab icon="refresh"  @click="playAgain(1)"/>
      </q-card-section>
      <q-card-section class="flex row">
        <h3 class="bounce">AV</h3><h3 class="bounce1">Ō</h3><h3 class="bounce2">Q</h3>
      </q-card-section>
    </q-card>
    <q-card class="q-px-md" style="height: fit-content;">
      <q-card-section class="row q-gutter-md">
        <p>Bounce and Fade</p>
        <q-btn flat fab icon="refresh"  @click="playAgain(2)"/>
      </q-card-section>
      <q-card-section class="flex row">
        <h3 class="bf-fade">AV</h3><h3 class="bf-bounce">Ō</h3><h3 class="bf-fade">Q</h3>
      </q-card-section>
    </q-card>
    <q-card class="q-px-md" style="height: fit-content;">
      <q-card-section class="row q-gutter-md">
        <p>Bounce, Wiggle, and Fade</p>
        <q-btn flat fab icon="refresh" @click="playAgain(3)"/>
      </q-card-section>
      <q-card-section class="flex row">
        <h3 class="bwf-fade">AV</h3><h3 class="bwf-bounce">Ō</h3><h3 class="bwf-fade">Q</h3>
      </q-card-section>
    </q-card>
    <q-card class="q-px-md" style="height: fit-content;">

      <q-card-section class="row q-gutter-md">
        <p>Roll in and Fade</p>
        <q-btn flat fab icon="refresh" @click="playAgain(4)"/>
      </q-card-section>
      <q-card-section class="flex row">
        <h3 class="rif-fade">AV</h3><h3 class="rif-bounce">Ō</h3><h3 class="rif-fade">Q</h3>
      </q-card-section>
    </q-card>
    <q-card class="q-px-md" style="height: fit-content;">

      <q-card-section class="row q-gutter-md">
        <p>Staggered Roll In</p>
        <q-btn flat fab icon="refresh" @click="playAgain(5)"/>
      </q-card-section>
      <q-card-section class="flex row">
        <h3 class="sr-roll1">A</h3><h3 class="sr-roll2">V</h3><h3 class="sr-roll4">Ō</h3><h3 class="sr-roll3">Q</h3>
      </q-card-section>
    </q-card>
    <q-card class="q-px-md" style="height: fit-content;">

      <q-card-section class="row q-gutter-md">
        <p>O first Stagger</p>
        <q-btn flat fab icon="refresh" @click="playAgain(6)"/>
      </q-card-section>
      <q-card-section class="flex row">
        <h3 class="ofs-roll1">A</h3><h3 class="ofs-roll2">V</h3><h3 class="ofs-roll4">Ō</h3><h3 class="ofs-roll3">Q</h3>
      </q-card-section>
    </q-card>
    <q-card class="q-px-md" style="height: fit-content;">

      <q-card-section class="row q-gutter-md">
        <p>Off the wall bounce</p>
        <q-btn flat fab icon="refresh" @click="playAgain(7)"/>
      </q-card-section>
      <q-card-section class="flex row">
        <h3>A</h3><h3>V</h3><h3 class="otw-bounce">Ō</h3><h3>Q</h3>
      </q-card-section>
    </q-card>
    <q-card class="q-px-md" style="height: fit-content;">

      <q-card-section class="row q-gutter-md">
        <p>Roll down stairs</p>
        <q-btn flat fab icon="refresh" @click="playAgain(8)"/>
      </q-card-section>
      <q-card-section class="flex row">
        <h3>A</h3><h3>V</h3><h3 class="rds-roll">Ō</h3><h3>Q</h3>
      </q-card-section>
    </q-card>
    <q-card class="q-px-md" style="height: fit-content;">

      <q-card-section class="row q-gutter-md">
        <p>Physics Drop</p>
        <q-btn flat fab icon="refresh" @click="playAgain(9)"/>
      </q-card-section>
      <q-card-section class="flex row">
        <h3 class="pd-A">A</h3><h3 class="pd-V">V</h3><h3 class="pd-O">Ō</h3><h3 class="pd-Q">Q</h3>
      </q-card-section>
    </q-card>
    <q-card class="q-px-md" style="height: fit-content; overflow: hidden;">
      <q-card-section class="row q-gutter-md">
        <p>Physics Explode and Fade</p>
        <q-btn flat fab icon="refresh" @click="playAgain(10)"/>
      </q-card-section>
      <q-card-section class="flex row justify-center">
        <h3 class="pe-A fade">A</h3><h3 class="pe-V fade">V</h3><h3 class="pe-O fade">Ō</h3><h3 class="pe-Q fade">Q</h3>
      </q-card-section>
    </q-card>
  </q-page>
</template>

<script setup>
import { onMounted } from 'vue';
import { gsap } from 'gsap';
import { Physics2DPlugin } from "gsap/Physics2DPlugin";

gsap.registerPlugin(Physics2DPlugin);

const tl0 = gsap.timeline();
const tl1 = gsap.timeline();
const tl2 = gsap.timeline();
const tl3 = gsap.timeline();
const tl4 = gsap.timeline();
const tl5 = gsap.timeline();
const tl6 = gsap.timeline();
const tl7 = gsap.timeline();
const tl8 = gsap.timeline();
const tl9 = gsap.timeline();
const tl10 = gsap.timeline();

const timelines = []
timelines.push(tl0)
timelines.push(tl1)
timelines.push(tl2)
timelines.push(tl3)
timelines.push(tl4)
timelines.push(tl5)
timelines.push(tl6)
timelines.push(tl7)
timelines.push(tl8)
timelines.push(tl9)
timelines.push(tl10)

onMounted(() => {
  tl0.from(".test-o", {y: -200, opacity: 0, duration: 1, ease: "bounce"});
  tl0.from(".test", {opacity: 0, x: -100, duration: 1});

  tl1.fromTo(".bounce1", {y: -200}, {y: 0, duration: 1, ease: "bounce"});
  tl1.fromTo(".bounce", {y: -200}, {y: 0, duration: 1, ease: "bounce"}, "<+=.25");
  tl1.fromTo(".bounce2", {y: -200}, {y: 0, duration: 1, ease: "bounce"}, "<+=.25");

  tl2.fromTo(".bf-bounce", {y: -200}, {y: 0, duration: 1, ease: "bounce"});
  tl2.fromTo(".bf-fade", {opacity: 0}, {opacity: 1, duration: 1.5});

  tl3.from(".bwf-bounce", {y: -200, duration: .5, ease: "bounce"})
  tl3.to(".bwf-bounce", {rotation: 45, duration: .5});
  tl3.fromTo(".bwf-bounce", {rotation: 45}, {rotation: -45, duration: .5});
  tl3.fromTo(".bwf-bounce", {rotation: -45}, {rotation: 30, duration: .5});
  tl3.to(".bwf-bounce", {rotation: 0, duration: .5, ease: "bounce"});
  tl3.from(".bwf-fade", {opacity: 0, duration: 1.5});

  tl4.fromTo(".rif-bounce", {rotation: 0, x: -100, opacity: 0}, {rotation: 360, x: 0, opacity: 1, duration: 2, ease: "power1.inOut"})
  tl4.fromTo(".rif-fade", {opacity: 0}, {opacity: 1, duration: 1.5});

  tl5.fromTo(".sr-roll1", {rotation: 0, x: -100, opacity: 0}, {rotation: 360, x: 0, opacity: 1, duration: 1.5, ease: "power1.inOut"}, "<+=.25")
  tl5.fromTo(".sr-roll2", {rotation: 0, x: -100, opacity: 0}, {rotation: 360, x: 0, opacity: 1, duration: 1.5, ease: "power1.inOut"}, "<+=.25")
  tl5.fromTo(".sr-roll3", {rotation: 0, x: -100, opacity: 0}, {rotation: 360, x: 0, opacity: 1, duration: 1.5, ease: "power1.inOut"}, "<+=.25")
  tl5.fromTo(".sr-roll4", {rotation: 0, x: -100, opacity: 0}, {rotation: 360, x: 0, opacity: 1, duration: 1.5, ease: "power1.inOut"}, "<+=.25")

  tl6.fromTo(".ofs-roll4", {rotation: 0, x: -100, opacity: 0}, {rotation: 360, x: 0, opacity: 1, duration: 1.5, ease: "power1.inOut"})
  tl6.fromTo(".ofs-roll1", {rotation: 0, x: -100, opacity: 0}, {rotation: 360, x: 0, opacity: 1, duration: 1.5, ease: "power1.inOut"})
  tl6.fromTo(".ofs-roll2", {rotation: 0, x: -100, opacity: 0}, {rotation: 360, x: 0, opacity: 1, duration: 1.5, ease: "power1.inOut"}, "<+=.25")
  tl6.fromTo(".ofs-roll3", {rotation: 0, x: -100, opacity: 0}, {rotation: 360, x: 0, opacity: 1, duration: 1.5, ease: "power1.inOut"}, "<+=.25")

  tl7.fromTo(".otw-bounce", {x: -100, y: -100}, {x: -10, y: 0, duration: .5, ease: "none"})
  tl7.fromTo(".otw-bounce", {x: -10, y: 0}, {x: 90, y: -50, duration: .5, ease: "none"})
  tl7.fromTo(".otw-bounce", {x: 90, y: -50}, {x: 60, y: -100, duration: .5, ease: "none"})
  tl7.fromTo(".otw-bounce", {x: 60, y: -100}, {x: 0, y: 0, duration: 1, ease: "bounce"})

  tl8.fromTo(".rds-roll", {x: 100, y:-100, rotation: 360}, {x: 60, y: -100, rotation: 300, duration: .5, ease: "none"})
  tl8.fromTo(".rds-roll", {x: 60, y: -100, rotation: 300}, {x: 55, y: -66, rotation: 240, duration: .25, ease: "bounce"})
  tl8.fromTo(".rds-roll", {x: 55, y: -66, rotation: 240}, {x: 30, y: -66, rotation: 180, duration: .5, ease: "none"})
  tl8.fromTo(".rds-roll", {x: 30, y: -66, rotation: 180}, {x: 30, y: -33, rotation: 120, duration: .25, ease: "bounce"})
  tl8.fromTo(".rds-roll", {x: 30, y: -33, rotation: 120}, {x: 0, y: -33, rotation: 60, duration: .5, ease: "none"})
  tl8.fromTo(".rds-roll", {x: 0, y: -33, rotation: 60}, {x: 0, y: 0, rotation: 0, duration: .25, ease: "bounce"})

  tl9.fromTo(".pd-O", {y: -100}, {duration: 1, physics2D: {angle: 270, gravity: 200}, ease: "bounce"});

  tl10.fromTo(".pe-A", {duration: 1, opacity: 1}, {opacity: .3, physics2D: {velocity: 400, angle: 230, gravity: 200}}, "<");
  tl10.fromTo(".pe-V", {duration: 1, opacity: 1}, {opacity: .3, physics2D: {velocity: 400, angle: 240, gravity: 200}}, "<");
  tl10.fromTo(".pe-O", {duration: 1, opacity: 1}, {opacity: .3, physics2D: {velocity: 400, angle: 260, gravity: 200}}, "<");
  tl10.fromTo(".pe-Q", {duration: 1, opacity: 1}, {opacity: .3, physics2D: {velocity: 400, angle: 290, gravity: 200}}, "<");
  tl10.fromTo(".fade", {x: 0, y: 0, opacity: 0}, {x: 0, y: 0, opacity: 1, duration: 1}, ">+=.5")

})

function playAgain(position) {
  timelines[position].restart();
}

</script>
