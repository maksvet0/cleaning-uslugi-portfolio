<script setup>
import ReviewCard from "@/components/user/ReviewCard.vue";

const data = [
  { title: "Anna M.", description: "I used PortfolioClean services for a deep cleaning before my guests arrived and was absolutely thrilled! The team arrived on time, did everything quickly and efficiently. I especially liked how they treated my sofa — it looks like new! Now I plan to order cleaning regularly. Highly recommend!", starsCount: 5 },
  { title: "Svetlana K.", description: "I never thought cleaning could be so pleasant! I ordered apartment cleaning services after renovation. They arrived at the scheduled time, quickly finished the job, and there were no traces of construction debris left. I will happily recommend PortfolioClean to my friends!", starsCount: 5 },
  { title: "Igor P.", description: "I ordered office cleaning since we didn’t have time to do it ourselves. The team did a great job! They cleaned up all the trash, washed the windows, and even freshened up the plants. Now we work in a clean and pleasant environment. Thank you, PortfolioClean, for your speed and quality!", starsCount: 4 },
]
</script>

<template>
  <h1>Reviews</h1>
  <div class="reviews">
    <ReviewCard
        class="review"
        v-for="item in data"
        :title="item.title"
        :description="item.description"
        :star-count="item.starsCount"
    />
  </div>
</template>

<style scoped lang="sass">
@import '@/components/style/ColorsVariables.sass'

.review
  margin-left: auto
  margin-right: auto

*
  background: $color-main

h1
  color: white
  text-align: center
  padding-top: 50px
  padding-bottom: 30px

.reviews
  display: flex
  align-items: center
  padding-bottom: 50px
</style>
