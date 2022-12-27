<script setup>
  import { Bars3Icon } from '@heroicons/vue/24/outline'
</script>

<template>
  <header>
    <div class="controls">
      <img
        src="../assets/imgs/teslabank_logo.svg"
        alt="" />
      <nav>
        <ul>
          <li>
            TeslaBank
            <img src="../assets/imgs/chevron.svg" />
          </li>
          <li>
            Conta Digital
            <img src="../assets/imgs/chevron.svg" />
          </li>
          <li>
            Pra você
            <img src="../assets/imgs/chevron.svg" />
          </li>
        </ul>
      </nav>
    </div>
    <button>Login <img src="../assets/imgs/profile.svg" /></button>
    <Bars3Icon class="lg:hidden w-10 text-[#E51D37]" />
  </header>
</template>

<style scoped lang="scss">
  @use '../assets/css/colors';

  header {
    z-index: 10;
    position: absolute;
    top: 0;
    width: 100%;
    display: flex;
    justify-content: space-between;
    padding: 36px 0;
    @apply px-10 xl:px-40;

    .controls {
      display: flex;
      align-items: center;
      @apply lg:gap-8 xl:gap-11;

      nav ul {
        display: flex;
        @apply max-lg:hidden lg:gap-8 xl:gap-11;

        li {
          cursor: pointer;
          display: flex;
          align-items: center;
          gap: 12px;
          font-weight: 500;
          color: colors.$gray;
        }
      }
    }

    button {
      display: flex;
      align-items: center;
      gap: 12px;
      font-weight: 500;
      color: white;
      @apply max-lg:hidden;
    }
  }
</style>
