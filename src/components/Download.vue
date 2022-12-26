<template>
  <section>
    <div>
      <h2>
        Uma nova experiência
        <br />
        em <strong>serviços financeiros</strong>.
        <br />
        Somos digital, somos TeslaBank.
      </h2>
      <p>
        Donec venenatis at turpis at ornare. Pellentesque a quam vel dui lacinia
        dapibus in sit amet dolor.
      </p>
      <div>
        <img src="../assets/imgs/apple-download.svg" />
        <img src="../assets/imgs/play-download.svg" />
      </div>
    </div>
    <img src="../assets/imgs/tesla_logo.svg" />
  </section>
</template>

<style scoped lang="scss">
  @use '../assets/css/colors';

  section {
    min-height: 60vh;
    display: flex;
    justify-content: space-between;
    gap: 160px;
    background-color: #f2f4fd;
    @apply py-32 lg:px-20 xl:px-40;

    div {
      display: flex;
      flex-direction: column;
      gap: 40px;

      h2 {
        font-family: Sora, sans-serif;
        font-size: 40px;
        font-weight: 600;
        color: #282421;

        strong {
          color: colors.$red;
        }
      }

      p {
        opacity: 0.75;
        font-size: 20px;
        color: colors.$gray;
      }

      div {
        display: flex;
        flex-direction: row;
        gap: 28px;

        img {
          cursor: pointer;
          width: 200px;
        }
      }
    }

    img {
      width: 320px;
    }
  }
</style>
