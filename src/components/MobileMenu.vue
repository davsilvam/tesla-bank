<script setup>
  import { ref, watchEffect } from 'vue'
  import { XMarkIcon } from '@heroicons/vue/24/outline'

  const emits = defineEmits(['toogleMenu'])
  const props = defineProps({ menuStatus: Boolean })

  const toogleMenu = () => {
    emits('toogleMenu')
  }

  const menuStatus = ref(props.menuStatus)

  watchEffect(() => {
    menuStatus.value = props.menuStatus
  })
</script>

<template>
  <div
    class="menu transition-transform duration-500 ease-in-out"
    :class="[menuStatus ? 'translate-y-0' : '-translate-y-full']">
    <div>
      <header>
        <img src="../assets/imgs/teslabank_white_logo.svg" />
        <XMarkIcon
          class="w-8 text-white"
          @click="toogleMenu" />
      </header>
      <img
        src="../assets/imgs/cards.svg"
        alt="" />
      <nav>
        <ul>
          <div class="line"></div>
          <li>
            TeslaBank
            <img src="../assets/imgs/white-chevron.svg" />
          </li>
          <div class="line"></div>
          <li>
            Conta Digital
            <img src="../assets/imgs/white-chevron.svg" />
          </li>
          <div class="line"></div>
          <li>
            Pra você
            <img src="../assets/imgs/white-chevron.svg" />
          </li>
          <div class="line"></div>
        </ul>
      </nav>
    </div>
    <button>Login <img src="../assets/imgs/profile.svg" /></button>
  </div>
</template>

<style scoped lang="scss">
  @use '../assets/css/colors';

  .menu {
    z-index: 20;
    position: absolute;
    top: 0;
    width: 100%;
    height: 100vh;
    display: flex;
    flex-direction: column;
    align-items: center;
    justify-content: space-between;
    padding: 48px 32px;
    background-image: colors.$gradient;

    div {
      width: 100%;
      display: flex;
      flex-direction: column;
      align-items: center;
      gap: 32px;

      header {
        width: 100%;
        display: flex;
        align-items: center;
        justify-content: space-between;

        img {
          width: 40px;
        }
      }

      & > img {
        max-width: 320px;
        margin-top: 12px;
      }

      nav {
        width: 100%;

        ul {
          display: flex;
          flex-direction: column;
          align-items: stretch;
          gap: 24px;

          .line {
            opacity: 0.25;
            height: 0.5px;
            width: 100%;
            background: white;
          }

          li {
            display: flex;
            align-items: center;
            justify-content: space-between;
            gap: 12px;
            color: white;
          }
        }
      }
    }

    button {
      display: flex;
      align-items: center;
      gap: 12px;
      color: white;
    }
  }
</style>
