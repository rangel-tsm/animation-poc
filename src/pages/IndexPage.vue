<template>
  <q-page class="flex row justify-around q-gutter-md">
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
        <p>Physics Launch</p>
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
    <q-card class="q-px-md" style="height: fit-content; overflow: hidden;">
      <q-card-section class="row q-gutter-md">
        <p>Reverse Explode</p>
        <q-btn flat fab icon="refresh" @click="playAgain(11)"/>
      </q-card-section>
      <q-card-section class="flex row justify-center">
        <h3 class="pre-A">A</h3><h3 class="pre-V">V</h3><h3 class="pre-O">Ō</h3><h3 class="pre-Q">Q</h3>
      </q-card-section>
    </q-card>
    <q-card class="q-px-md" style="height: fit-content; overflow: hidden;">
      <q-card-section class="row q-gutter-md">
        <p>All Bounce with Split Text</p>
        <q-btn flat fab icon="refresh" @click="playAgain(12)"/>
      </q-card-section>
      <q-card-section class="flex row justify-center">
        <h3 class="st-bounce">AVŌQ</h3>
      </q-card-section>
    </q-card>
    <q-card class="q-px-md" style="height: fit-content; overflow: hidden;">
      <q-card-section class="row q-gutter-md">
        <p>Text Scramble</p>
        <q-btn flat fab icon="refresh" @click="playAgain(13)"/>
      </q-card-section>
      <q-card-section class="flex row justify-center">
        <h3 class="ts-scramble"></h3>
      </q-card-section>
    </q-card>
    <q-card class="q-px-md" style="height: fit-content;">
      <q-card-section class="row q-gutter-md">
        <p>Fade and Wiggle</p>
        <q-btn flat fab icon="refresh" @click="playAgain(14)"/>
      </q-card-section>
      <q-card-section class="flex row">
        <h3 class="fw-fade">AV</h3><h3 class="fw-bounce">Ō</h3><h3 class="fw-fade">Q</h3>
      </q-card-section>
    </q-card>
    <q-card class="q-px-md" style="height: fit-content;">
      <q-card-section class="row q-gutter-md">
        <p>SVG Draw</p>
        <q-btn flat fab icon="refresh" @click="playAgain(15)"/>
      </q-card-section>
      <q-card-section class="flex row path">
        <svg width="109" height="47" viewBox="0 0 109 47" fill="none" xmlns="http://www.w3.org/2000/svg">
          <path id="path" class="black" d="M16.8567 8.66777L21.3089 22.6959H12.2667L16.8624 8.66777H16.8567ZM12.72 0.520569L0 36.1617H7.78574L10.2529 28.835H23.3859L25.6809 36.1617H33.7592L21.1368 0.520569H12.72Z" fill="#3A222C"/>
          <path id="path" class="black" d="M28.039 9.80377H35.7789L41.2639 29.248L46.8751 9.80377H54.2764L44.7695 36.1617H37.4944L28.039 9.80377Z" fill="#3A222C"/>
          <path id="path" class="black" d="M90.5314 27.7735C91.4322 29.9825 93.1076 31.0841 95.5632 31.0841C98.0188 31.0841 99.6196 30.0685 100.618 28.0375C101.261 26.7006 101.588 25.0081 101.588 22.9598C101.588 21.3476 101.312 19.9075 100.767 18.6338C99.786 16.3445 98.059 15.197 95.5919 15.197C93.8477 15.197 92.4535 15.8626 91.3978 17.2051C90.3421 18.5419 89.8143 20.573 89.8143 23.2983C89.8143 25.1228 90.0552 26.6088 90.5372 27.7735M101.398 46.6096V32.8971C100.882 33.9585 99.9983 34.9109 98.7475 35.7371C97.4967 36.5691 95.7927 36.9822 93.6354 36.9822C90.5888 36.9822 87.9898 35.7658 85.8497 33.3331C83.7039 30.9004 82.631 27.653 82.631 23.5852C82.631 19.2018 83.7096 15.6962 85.8611 13.0627C88.0127 10.4349 90.6691 9.12103 93.8305 9.12103C96.0222 9.12103 97.7951 9.66035 99.1491 10.739C99.9409 11.3529 100.744 12.357 101.565 13.7626V9.84395H108.214V46.6039H101.392L101.398 46.6096Z" fill="#3A222C"/>
          <path
            id="path"
            class="blue"
            d="M66.5067 30.3914C70.5451 30.3914 73.8189 27.1176 73.8189 23.0792C73.8189 19.0407 70.5451 15.7669 66.5067 15.7669C62.4682 15.7669 59.1944 19.0407 59.1944 23.0792C59.1944 27.1176 62.4682 30.3914 66.5067 30.3914ZM66.5067 37.3555C74.3912 37.3555 80.783 30.9637 80.783 23.0792C80.783 15.1946 74.3912 8.80286 66.5067 8.80286C58.6221 8.80286 52.2304 15.1946 52.2304 23.0792C52.2304 30.9637 58.6221 37.3555 66.5067 37.3555Z"
            fill-rule="evenodd"
            clip-rule="evenodd"
            fill="#57B9B0"
          />
          <path id="path" class="blue" d="M75.2117 1.8913H57.8016V6.76613H75.2117V1.8913Z" fill="#57B9B0"/>
        </svg>
      </q-card-section>
    </q-card>
  </q-page>
</template>

<script setup>
import { onMounted } from 'vue';
import { gsap } from 'gsap';
import { Physics2DPlugin } from "gsap/Physics2DPlugin";
import { SplitText } from "gsap/SplitText";
import { ScrambleTextPlugin } from "gsap/ScrambleTextPlugin";
import { DrawSVGPlugin } from "gsap/DrawSVGPlugin";

gsap.registerPlugin(DrawSVGPlugin, Physics2DPlugin, ScrambleTextPlugin, SplitText);

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
const tl11 = gsap.timeline();
const tl12 = gsap.timeline();
const tl13 = gsap.timeline();
const tl14 = gsap.timeline();
const tl15 = gsap.timeline();

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
timelines.push(tl11)
timelines.push(tl12)
timelines.push(tl13)
timelines.push(tl14)
timelines.push(tl15)

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

  tl9.to(".pd-O", {duration: 1, physics2D: {velocity: 400, angle: 270, gravity: 800}});

  tl10.fromTo(".pe-A", {duration: 1, opacity: 1}, {opacity: .3, physics2D: {velocity: 600, angle: 230, gravity: 200}}, "<");
  tl10.fromTo(".pe-V", {duration: 1, opacity: 1}, {opacity: .3, physics2D: {velocity: 600, angle: 240, gravity: 200}}, "<");
  tl10.fromTo(".pe-O", {duration: 1, opacity: 1}, {opacity: .3, physics2D: {velocity: 600, angle: 260, gravity: 200}}, "<");
  tl10.fromTo(".pe-Q", {duration: 1, opacity: 1}, {opacity: .3, physics2D: {velocity: 600, angle: 290, gravity: 200}}, "<");
  tl10.fromTo(".fade", {x: 0, y: 0, opacity: 0}, {x: 0, y: 0, opacity: 1, duration: 1}, ">+=.5")

  tl11.fromTo(".pre-A", {opacity: 0, x: -70, y: -150}, {opacity: 1, x: 0, y: 0, duration: 1, ease: "bounce"}, "<");
  tl11.fromTo(".pre-V", {opacity: 0, x: -30, y: -150}, {opacity: 1, x: 0, y: 0, duration: 1, ease: "bounce"}, "<");
  tl11.fromTo(".pre-O", {opacity: 0, x: 50, y: -150}, {opacity: 1, x: 0, y: 0, duration: 1, ease: "bounce"}, "<");
  tl11.fromTo(".pre-Q", {opacity: 0, x: 50, y: -150}, {opacity: 1, x: 0, y: 0, duration: 1, ease: "bounce"}, "<");

  const stBounce = new SplitText(".st-bounce")
  tl12.from(stBounce.chars, {y: -200, duration: 1, ease: "bounce", stagger: .25}, )

  tl13.to(".ts-scramble", {duration: 2, scrambleText: "AVŌQ"})

  tl14.from(".fw-bounce", {opacity: 0, duration: 1.5})
  tl14.to(".fw-bounce", {rotation: 45, duration: .5}, "<+=.25");
  tl14.fromTo(".fw-bounce", {rotation: 45}, {rotation: -45, duration: .5}, "<+=.25");
  tl14.fromTo(".fw-bounce", {rotation: -45}, {rotation: 30, duration: .5}, "<+=.25");
  tl14.to(".fw-bounce", {rotation: 0, duration: .5,}, "<+=.25");
  tl14.from(".fw-fade", {opacity: 0, duration: 1.5});

  tl15.fromTo("#path.blue", {drawSVG: "0", fill: "white"}, {duration: 1.5, drawSVG: "100%", ease: "power1.out"});
  tl15.fromTo("#path.black", {drawSVG: "0", fill: "white"}, {duration: 1.5, drawSVG: "100%", ease: "power1.out"}, "<+=.25");
  tl15.to("#path.blue", {duration: .5, fill: "#57B9B0"}, ">+=.25" );
  tl15.to("#path.black", {duration: .5, fill: "black"}, "<");

})

function playAgain(position) {
  timelines[position].restart();
}

</script>
<style>
#path {
  stroke: black;
  stroke-width: 1px;
  fill: none;
}
#path.blue {
  stroke: #57B9B0;
  stroke-width: 1px;
}
</style>
