<template>
  <section>
    <img
      class="wave"
      src="../assets/imgs/benefits_wave.svg" />
    <div class="headings">
      <h4>#INOVAÇÃO</h4>
      <h2>
        Quais as vantagens <br />
        de usar <span>TeslaBank</span>?
      </h2>
    </div>
    <div class="cards">
      <div class="card">
        <img src="../assets/imgs/credit-card.svg" />
        <div>
          <h3>Cartão TeslaBank</h3>
          <p>
            Lorem ipsum dolor sit amet, consectetur adipiscing elit. Aenean
            vitae leo lacinia, tempus odio hendrerit, ultricies diam.
          </p>
        </div>
        <a>VEJA AS OPÇÕES</a>
      </div>
      <div class="card">
        <img src="../assets/imgs/shopping-cart.svg" />
        <div>
          <h3>Investimentos</h3>
          <p>
            Lorem ipsum dolor sit amet, consectetur adipiscing elit. Aenean
            vitae leo lacinia, tempus odio hendrerit, ultricies diam.
          </p>
        </div>
        <a>VEJA AS OPÇÕES</a>
      </div>
      <div class="card">
        <img src="../assets/imgs/clock.svg" />
        <div>
          <h3>Atendimento 24h</h3>
          <p>
            Lorem ipsum dolor sit amet, consectetur adipiscing elit. Aenean
            vitae leo lacinia, tempus odio hendrerit, ultricies diam.
          </p>
        </div>
        <a>VEJA AS OPÇÕES</a>
      </div>

      <div class="lg:row-start-2 lg:col-start-2 card">
        <img src="../assets/imgs/shield.svg" />
        <div>
          <h3>Segurança</h3>
          <p>
            Lorem ipsum dolor sit amet, consectetur adipiscing elit. Aenean
            vitae leo lacinia, tempus odio hendrerit, ultricies diam.
          </p>
        </div>
        <a>VEJA AS OPÇÕES</a>
      </div>
      <div class="lg:row-start-2 lg:col-start-3 card">
        <img src="../assets/imgs/percent.svg" />
        <div>
          <h3>Sem taxas</h3>
          <p>
            Lorem ipsum dolor sit amet, consectetur adipiscing elit. Aenean
            vitae leo lacinia, tempus odio hendrerit, ultricies diam.
          </p>
        </div>
        <a>VEJA AS OPÇÕES</a>
      </div>
      <div class="lg:row-start-2 lg:col-start-4 card">
        <img src="../assets/imgs/gift.svg" />
        <div>
          <h3>Receba prêmios</h3>
          <p>
            Lorem ipsum dolor sit amet, consectetur adipiscing elit. Aenean
            vitae leo lacinia, tempus odio hendrerit, ultricies diam.
          </p>
        </div>
        <a>VEJA AS OPÇÕES</a>
      </div>
    </div>
  </section>
</template>

<style scoped lang="scss">
  @use '../assets/css/colors';

  section {
    position: relative;
    min-height: 110vh;
    display: flex;
    flex-direction: column;
    justify-content: center;
    gap: 52px;
    background-color: #f2f4fd;
    @apply py-32 px-10 xl:px-40;

    .wave {
      position: absolute;
      top: 30%;
      left: 0;
    }

    .headings {
      z-index: 10;
      display: flex;
      flex-direction: column;
      gap: 8px;

      h4 {
        font-size: 18px;
        font-weight: 500;
        color: colors.$red;
      }

      h2 {
        font-family: Sora, sans-serif;
        font-size: 32px;
        font-weight: 600;
        line-height: 45px;

        span {
          color: colors.$red;
        }
      }
    }

    .cards {
      z-index: 10;
      display: grid;
      grid-template-columns: repeat(4, 1fr);
      grid-template-rows: repeat(2, 1fr);
      @apply max-sm:grid-cols-1 max-lg:grid-cols-2 max-lg:grid-rows-3;
      gap: 32px;

      .card {
        display: flex;
        flex-direction: column;
        gap: 16px;
        padding: 16px;
        background-color: white;
        @apply shadow-md;

        img {
          width: 35px;
        }

        div {
          color: colors.$gray;

          h3 {
            font-family: Sora, sans-serif;
            font-size: 18px;
            font-weight: 500;
          }

          p {
            opacity: 0.75;
            text-align: justify;
            font-size: 14px;
          }
        }

        a {
          cursor: pointer;
          text-decoration: underline;
          font-size: 14px;
          font-weight: 600;
          color: colors.$red;
        }
      }
    }
  }
</style>
