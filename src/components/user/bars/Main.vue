<template>
  <div class="container">
    <h1>Cleaning Services</h1>
    <p>We always clean quickly, efficiently, and affordably</p>
    <Button title="Purchase Cleaning" :on-click="onClickPurchase" />
  </div>
</template>

<script setup lang="ts">
  import Button from "@/components/ui/Button.vue";

  function onClickPurchase() {
    window.location.href = "#register"
  }
</script>

<style scoped lang="sass">
.container
  background: url("@/assets/image/MainImg.png") center no-repeat

*
  box-sizing: border-box
  text-align: center
  color: white
  height: 750px
  display: flex
  flex-direction: column
  justify-content: center
  align-items: center

h1
  background: none
  padding-top: 110px
  font-size: 50px
  margin: 10px

p
  font-size: 25px
  background: none
  margin-bottom: 10px
  padding: 0

button
  margin-bottom: 50px
  height: 150px

</style>
