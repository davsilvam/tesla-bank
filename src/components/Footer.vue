<script setup>
  const year = new Date().getFullYear()
</script>

<template>
  <footer>
    <p class="copy">
      Copyright &copy; {{ year }}
      <a
        href="https://iuricode.com"
        target="_blank"
        >IuriCode</a
      >
      &
      <a
        href="https://portfolio-ds-one.vercel.app"
        target="_blank"
        >David Silva</a
      >.
      <span>Todos os direitos reservados.</span>
    </p>
    <p class="logos">
      Powered by <img src="../assets/imgs/iuri_logo.svg" /> and
      <img src="../assets/imgs/ds.png" />
    </p>
  </footer>
</template>

<style scoped lang="scss">
  @use '../assets/css/colors';

  footer {
    display: flex;
    justify-content: space-between;
    padding: 24px 0;
    @apply px-10 xl:px-40;
    background-color: white;

    .copy {
      @apply max-sm:hidden;
      font-weight: 400;

      a {
        font-family: Sora, sans-serif;
        font-weight: 600;
        color: #282421;
      }

      span {
        @apply max-lg:hidden;
      }
    }

    .logos {
      width: 40%;
      @apply max-sm:w-[100%];
      display: flex;
      align-items: center;
      justify-content: flex-end;
      gap: 12px;
      color: colors.$red;
      font-weight: 500;

      img {
        width: 20px;
      }
    }
  }
</style>
