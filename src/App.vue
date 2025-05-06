<template>
<div class="app">
  <IntroSection />
  <CurrentProject />
  <PastProjects />
  <SubmitCraft />
  <FooterSection />
</div>
</template>

<script setup>
import IntroSection from './components/IntroSection.vue'
import CurrentProject from './components/CurrentProject.vue'
import PastProjects from './components/PastProjects.vue'
import SubmitCraft from './components/SubmitCraft.vue'
import FooterSection from './components/FooterSection.vue'
</script>

<style>
body {
margin: 0;
font-family: 'Comic Sans MS', cursive, sans-serif;
background-color: #fffdf6;
overflow-x: hidden;
}
.app section {
height: 100vh;
padding: 2rem;
display: flex;
flex-direction: column;
justify-content: center;
color: #333;
}
.parallax {
background-attachment: fixed;
background-size: cover;
background-repeat: no-repeat;
background-position: center;
}
</style>
