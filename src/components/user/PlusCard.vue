<script lang="ts" setup>
  const props = defineProps({
    imageSrc: String,
    title: String,
    description: String
  })
</script>

<template>
  <div class="card">
    <img :src="props.imageSrc">
    <h3>{{ props.title }}</h3>
    <p>{{ props.description }}</p>
  </div>
</template>

<style scoped lang="sass">
  @import '@/components/style/FontVariables.sass'
  @import '@/components/style/ColorsVariables.sass'

  img, h3, p
    text-align: center
    align-self: center

    margin-left: auto
    margin-right: auto

  p
    color: #5E96D3

  h3
    color: $color-main

    font-weight: $font-weight-bold
    font-size: 24px

  img
    width: 90%
    height: 150px

  *
    background: #E1F4FF

    border-radius: 33px

    padding: 10pt

  .card
    width: 290px

    align-items: center
    align-content: center

</style>