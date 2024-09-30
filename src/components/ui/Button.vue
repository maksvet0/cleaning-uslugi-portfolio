<script setup lang="ts">
  const props = defineProps({
    title: String,
    onClick: Function,
  })
</script>


<template>
  <button
      :onClick="onClick"
  >
    {{ props.title }}
  </button>
</template>

<style lang="sass" scoped>
  @import '@/components/style/FontVariables.sass'
  @import '@/components/style/MiscVariables.sass'
  @import '@/components/style/ColorsVariables.sass'


  button
    transition: $anim-default

    background: $color-main
    color: white

    border: none
    border-radius: 15px

    padding: 10pt 15pt
    cursor: pointer

    font-size: 25px
    font-weight: $font-weight-semi-bold


    &:hover
      background: #0070eb

    &:active
      background: #003772


</style>