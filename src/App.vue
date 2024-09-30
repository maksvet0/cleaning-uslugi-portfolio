<script setup lang="ts">
  import Navigation from "@/components/user/bars/Navigation.vue";
  import Main from "@/components/user/bars/Main.vue";
  import AboutUs from "@/components/user/bars/AboutUs.vue";
  import Pluses from "@/components/user/bars/Pluses.vue";
  import Reviews from "@/components/user/bars/Reviews.vue";
  import Register from "@/components/user/bars/Register.vue";
  import Basement from "@/components/user/bars/Basement.vue";
</script>


<template>
  <Navigation />
  <div id="main"><Main /></div>
  <div id="about-us"><AboutUs /></div>
  <div id="pluses"><Pluses /></div>
  <div id="reviews"><Reviews /></div>
  <div id="register"><Register /></div>
  <div id="basement"><Basement /></div>
</template>

<style lang="sass">
  @import url('https://fonts.googleapis.com/css2?family=Inter:ital,opsz,wght@0,14..32,100..900;1,14..32,100..900&display=swap')

  html
    scroll-behavior: smooth

  *
    margin: 0
    padding: 0
    font-family: "Inter", sans-serif
    background: white

</style>
