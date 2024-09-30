<script lang="ts" setup >
  const props = defineProps({
    title: String,
    placeholder: String,
  })
</script>

<template>
  <div class="inputHolder">
    <h3>{{ props.title }}</h3>
    <input type="text" :placeholder="props.placeholder" />
  </div>
</template>

<style lang="sass" scoped>
  @import '@/components/style/FontVariables.sass'
  @import '@/components/style/ColorsVariables.sass'

  *
    background: transparent

  input
    width: 100%

    background: #90C3FF
    color: $color-main

    outline: none
    border: solid 3px #0053B4
    border-radius: 15px

    font-weight: $font-weight-semi-bold
    font-size: 15px

    padding: 10px 15px

    &::placeholder
      color: #58A5FF

  h3
    color: #58A5FF

    font-weight: $font-weight-semi-bold
    font-size: 22px

    margin: 10px


</style>