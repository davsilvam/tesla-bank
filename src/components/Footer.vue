<script setup>
  const year = new Date().getFullYear()
</script>

<template>
  <footer>
    <p class="copy">
      Copyright &copy; {{ year }} <strong>IuriCode</strong> &
      <strong>David Silva</strong>. Todos os direitos reservados.
    </p>
    <p class="logos">Powered by <img src="../assets/imgs/iuri_logo.svg" /></p>
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
      @apply max-md:hidden;
      font-weight: 400;

      strong {
        font-family: Sora, sans-serif;
        font-weight: 600;
        color: #282421;
      }
    }

    .logos {
      width: 40%;
      @apply max-md:w-[100%];
      display: flex;
      align-items: center;
      justify-content: flex-end;
      gap: 12px;
      color: colors.$red;
      font-weight: 500;

      img {
        @apply max-lg:w-[20px];
      }
    }
  }
</style>
