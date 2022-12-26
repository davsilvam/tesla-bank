<template>
  <section>
    <div class="headings">
      <h4>#DEPOIMENTOS</h4>
      <h2>
        <strong>TeslaBank fora das telinhas</strong>: Veja <br />
        o que falam sobre nosso serviço
      </h2>
    </div>
    <div class="depositions">
      <div class="deposition">
        <div>
          <div class="bar"></div>
          <h3>NIKOLA TESLA</h3>
        </div>
        <q
          >Lorem ipsum dolor sit amet, consectetur adipiscing elit. Vestibulum
          scelerisque nisl quis viverra tincidunt.</q
        >
      </div>
      <div class="deposition">
        <div>
          <div class="bar"></div>
          <h3>STEVE JOBS</h3>
        </div>
        <q
          >Lorem ipsum dolor sit amet, consectetur adipiscing elit. Vestibulum
          scelerisque nisl quis viverra tincidunt.</q
        >
      </div>
      <div class="deposition">
        <div>
          <div class="bar"></div>
          <h3>ALAN TURING</h3>
        </div>
        <q
          >Lorem ipsum dolor sit amet, consectetur adipiscing elit. Vestibulum
          scelerisque nisl quis viverra tincidunt.</q
        >
      </div>
    </div>
  </section>
</template>

<style scoped lang="scss">
  @use '../assets/css/colors';

  section {
    min-height: 60vh;
    display: flex;
    flex-direction: column;
    justify-content: center;
    gap: 80px;
    @apply py-32 px-10 xl:px-40;

    .headings {
      display: flex;
      flex-direction: column;
      gap: 8px;

      h4 {
        font-size: 18px;
        font-weight: 500;
        color: colors.$red;
      }

      h2 {
        font-size: 32px;
        line-height: 45px;

        strong {
          font-family: Sora, sans-serif;
          font-weight: 600;
        }
      }
    }

    .depositions {
      display: flex;
      @apply max-lg:flex-col;
      align-items: center;
      justify-content: space-between;
      gap: 52px;
      color: colors.$gray;

      .deposition {
        display: flex;
        flex-direction: column;
        gap: 20px;

        div {
          display: flex;
          align-items: center;
          gap: 8px;

          .bar {
            width: 3px;
            height: 30px;
            background-color: colors.$red;
          }

          h3 {
            font-family: Sora, sans-serif;
            font-size: 18px;
          }
        }

        q {
          font-style: italic;
        }
      }
    }
  }
</style>
