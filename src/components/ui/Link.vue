<template>
  <a :href="to" >
    <button>
      {{ props.title }}
    </button>
  </a>
</template>

<script type="ts" setup>
const props = defineProps({
  title: String,
  to: String, // сюда передаем идентификатор
})
</script>


<style lang="sass" scoped>
  @import '@/components/style/FontVariables.sass'
  @import '@/components/style/MiscVariables.sass'


  button
    transition: $anim-default

    background: none
    color: white

    border: none
    cursor: pointer

    font-weight: $font-weight-medium
    font-size: 22px

    &:hover
      transform: scale(1.1)

    &:active
      transform: scale(.95)
</style>