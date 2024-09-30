<script setup>
import Input from "@/components/ui/Input.vue";
import Button from "@/components/ui/Button.vue";
</script>

<template>
  <div class="registerHolder">
    <div class="oneMoreHolder">
      <h1 class="title">Clean your room!</h1>
      <Input
          title="Address"
          placeholder="Ufa, Lenina St. 3, apt. 5"
      />
      <Input
          title="Type of Cleaning"
          placeholder="Full cleaning"
      />
      <Input
          title="Phone"
          placeholder="+7 987 233 83 02"
      />
      <Input
          title="Time"
          placeholder="22.05 at 12:00"
      />
      <Button title="Order" />
    </div>
  </div>
</template>

<style scoped lang="sass">
@import "src/components/style/ColorsVariables"

$background-color: #E1F4FF

*
  background: $background-color
  box-sizing: border-box
  text-align: center
  color: $color-main

.oneMoreHolder
  width: 90%

.registerHolder
  padding: 30px
  display: flex
  flex-direction: column
  align-items: center
  background: $background-color

.title
  font-size: 35px
  font-weight: bold
  width: 100%
  text-align: center
  margin-bottom: 20px

Button
  margin: 30px
  width: 93%

</style>
