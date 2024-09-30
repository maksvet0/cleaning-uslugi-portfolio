<script lang="ts" setup>
// Определяем входные параметры компонента
const props = defineProps({
  title: String,
  description: String,
  starCount: Number,
})
</script>

<template>
  <div class="review">
    <!-- Заголовок -->
    <h3>{{ title }}</h3>

    <!-- Описание -->
    <p>{{ description }}</p>

    <!-- Рейтинг в виде звезд -->
    <div class="stars">
      <!-- Цикл по количеству звезд -->
      <img v-for="n in starCount" :key="n" class="star" src="@/assets/image/StarIcon.svg" alt="star" />
    </div>
  </div>
</template>

<style scoped lang="sass">
@import '@/components/style/FontVariables.sass'


*
  background-color: #CAE2FF

.review
  background-color: #CAE2FF
  border-radius: 20px
  padding: 20px
  max-width: 400px

  h3
    color: #1976d2
    margin-bottom: 10px
    font-size: 25px

  p
    color: #4299FF
    font-weight: $font-weight-bold
    font-size: 20px
    margin-bottom: 20px

  .stars
    display: flex
    gap: 5px


  .star
    width: 35px
    height: 35px

</style>
