<template>
<section style="background-color: #fff7e6;">
  <h2>📸 Wanna Share Yours?</h2>
  <form @submit.prevent="submit">
    <input type="text" placeholder="What’d you make?" v-model="title" />
    <textarea placeholder="Tell me how it went..." v-model="description"></textarea>
    <button type="submit">Send it my way</button>
  </form>
</section>
</template>

<script setup>
import { ref } from 'vue'
const title = ref('')
const description = ref('')
function submit() {
console.log("Craft submitted:", title.value, description.value)
}
</script>

<style scoped>
input, textarea {
display: block;
margin: 0.5rem 0;
width: 100%;
padding: 0.5rem;
}
button {
background-color: coral;
color: white;
padding: 0.5rem 1rem;
border: none;
}
</style>