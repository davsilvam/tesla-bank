<script setup>
  import { ref } from 'vue'
  import TheHeader from './components/Header.vue'
  import Hero from './components/Hero.vue'
  import Overview from './components/Overview.vue'
  import Benefits from './components/Benefits.vue'
  import Depositions from './components/Depositions.vue'
  import Download from './components/Download.vue'
  import Help from './components/Help.vue'
  import TheFooter from './components/Footer.vue'
  import MobileMenu from './components/MobileMenu.vue'

  const menuStatus = ref(false)

  const onToogleMenu = () => {
    menuStatus.value = !menuStatus.value
  }
</script>

<template>
  <div>
    <MobileMenu
      :menuStatus="menuStatus"
      @toogleMenu="onToogleMenu" />
    <TheHeader @toogleMenu="onToogleMenu" />
    <Hero />
    <Overview />
    <Benefits />
    <Depositions />
    <Download />
    <Help />
    <TheFooter />
  </div>
</template>

<style scoped lang="scss">
  div {
    position: relative;
    background-color: #f8f9ff;
  }
</style>
