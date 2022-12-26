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
    @apply lg:px-20 xl:px-40;
    background-color: white;

    .copy {
      font-weight: 400;

      strong {
        font-family: Sora, sans-serif;
        font-weight: 600;
        color: #282421;
      }
    }

    .logos {
      width: 40%;
      display: flex;
      justify-content: flex-end;
      gap: 12px;
      color: colors.$red;
      font-weight: 500;
    }
  }
</style>
