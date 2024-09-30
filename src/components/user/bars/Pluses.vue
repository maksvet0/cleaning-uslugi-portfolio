<script setup>
import PersonIcon from "@/assets/image/PersonIcon.svg"
import PriceIcon from "@/assets/image/PriceIcon.svg"
import ProIcon from "@/assets/image/ProIcon.svg"
import PlusCard from "@/components/user/PlusCard.vue";
</script>

<template>
  <h1>You Get:</h1>

  <div class="pluses">
    <PlusCard
        :image-src="ProIcon"
        title="Professionalism"
        description="Our team consists of experienced specialists who have undergone training and possess skills in various types of cleaning, including post-renovation cleaning, deep cleaning, as well as specialized services such as window washing and carpet cleaning."
    />
    <PlusCard
        :image-src="PersonIcon"
        title="Individual Approach"
        description="We understand that every client has their own needs. Therefore, we are ready to offer you flexible terms of cooperation and adapt our services to your requirements."
    />
    <PlusCard
        :image-src="PriceIcon"
        title="Affordable Prices"
        description="We strive to offer high-quality services at reasonable prices. There are no hidden fees — you will always know exactly what you are paying for."
    />
  </div>

</template>

<style scoped lang="sass">
@import '@/components/style/FontVariables.sass'
@import '@/components/style/ColorsVariables.sass'

h1
  text-align: center
  padding: 50px 0 50px 0
  font-size: 44px
  font-weight: $font-weight-bold
  color: $color-main

*
  width: 100%
  margin-left: auto
  margin-right: auto

.pluses
  display: flex
  margin-top: 30px
  width: 70%
  margin-bottom: 110px

</style>
