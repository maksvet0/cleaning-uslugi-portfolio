<script lang="ts" setup>
import Link from "@/components/ui/Link.vue";
</script>

<template>
  <div class="nav">
    <h2 class="logo">PortfolioClean</h2>
    <ul>
      <li><Link title="Home" to="#main" /></li>
      <li><Link title="About Us" to="#about-us" /></li>
      <li><Link title="Advantages" to="#pluses" /></li>
      <li><Link title="Reviews" to="#reviews" /></li>
      <li><Link title="Buy" to="#register" /></li>
      <li><Link title="Other Info" to="#basement" /></li>
    </ul>
  </div>
</template>

<style lang="sass" scoped>
*
  background-color: #0060BF

.nav
  position: fixed
  width: 100%
  padding: 0 20px
  display: flex
  align-items: center
  justify-content: space-between
  height: 50px

.logo
  font-size: 23px
  color: white
  font-weight: bold

ul
  display: flex
  list-style: none
  margin-right: 40px
  padding: 0

li
  margin-left: 20px
</style>
